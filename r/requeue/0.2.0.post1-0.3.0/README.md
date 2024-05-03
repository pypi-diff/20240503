# Comparing `tmp/requeue-0.2.0.post1.tar.gz` & `tmp/requeue-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requeue-0.2.0.post1.tar", max compression
+gzip compressed data, was "requeue-0.3.0.tar", max compression
```

## Comparing `requeue-0.2.0.post1.tar` & `requeue-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2024-03-10 22:34:57.217631 requeue-0.2.0.post1/LICENSE
--rw-r--r--   0        0        0     1318 2024-04-22 03:53:47.024295 requeue-0.2.0.post1/README.md
--rw-r--r--   0        0        0      397 2024-04-22 03:59:50.554434 requeue-0.2.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2714 2024-03-16 19:58:57.882205 requeue-0.2.0.post1/requeue/__init__.py
--rw-r--r--   0        0        0     1927 1970-01-01 00:00:00.000000 requeue-0.2.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-10 22:34:57.217631 requeue-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1318 2024-05-03 12:10:34.112347 requeue-0.3.0/README.md
+-rw-r--r--   0        0        0      391 2024-05-03 11:50:51.082351 requeue-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3087 2024-05-03 12:15:51.593431 requeue-0.3.0/requeue/__init__.py
+-rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 requeue-0.3.0/PKG-INFO
```

### Comparing `requeue-0.2.0.post1/LICENSE` & `requeue-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requeue-0.2.0.post1/README.md` & `requeue-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `requeue-0.2.0.post1/requeue/__init__.py` & `requeue-0.3.0/requeue/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 import asyncio
+import inspect
 import traceback
 
 from typing import Any, Union, Optional, Callable, Awaitable
 from dataclasses import dataclass, field
 
 
+CheckCallable = Union[Callable[..., bool], Callable[..., Awaitable[bool]]]
+
+
 @dataclass
 class _Request:
     lock: asyncio.Lock = field(default_factory=asyncio.Lock)
     completed: asyncio.Event = field(default_factory=asyncio.Event)
-    check: Optional[Callable[..., bool]] = field(default=None)
+    check: Optional[CheckCallable] = field(default=None)
     result: Union[Any, tuple[Any]] = field(default=None)
 
+    async def validate(self, *contents) -> Awaitable[bool]:
+        """
+        Validate contents against check.
+        """
+
+        if self.check is None:
+            return True
+
+        valid = self.check(*contents)
+
+        if inspect.isawaitable(valid):
+            return await valid
+        return valid
+
 
 class Requeue:
     """
     An asynchronous queue for requesting data
     """
 
     def __init__(self) -> None:
         self._requests: list[_Request] = []
         self._lock = asyncio.Lock()
 
     async def wait_for(self,
-        check: Optional[Callable[..., bool]] = None,
+        check: Optional[CheckCallable] = None,
         timeout: Optional[float] = None,
     ) -> Union[Any, tuple[Any]]:
         """
         Make a request for data and wait for it.
         
         Optionally, apply a check to only permit data matching certain criteria.
         `check` should return a boolean of whether it is a match or not.
@@ -67,16 +85,17 @@
 
         for request in requests:
             # Skip timed out requests.
             if request.completed.is_set():
                 continue
 
             try:
-                if request.check is not None and not request.check(*contents):
+                if not await request.validate(*contents):
                     continue
+
             except Exception:
                 # Ignore any exception raised with the calling of the check.
                 # If the check or data is faulty, that should not affect
                 # or interrupt the completion of other requests.
                 traceback.print_exc()
                 continue
```

### Comparing `requeue-0.2.0.post1/PKG-INFO` & `requeue-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requeue
-Version: 0.2.0.post1
+Version: 0.3.0
 Summary: An asynchronous queue for requesting data
 Home-page: https://gitlab.com/deepadmax/requeue
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

