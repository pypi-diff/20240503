# Comparing `tmp/viur-toolkit-0.1.0.dev5.tar.gz` & `tmp/viur_toolkit-0.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur-toolkit-0.1.0.dev5.tar", last modified: Tue Apr  2 15:53:20 2024, max compression
+gzip compressed data, was "viur_toolkit-0.1.0.dev6.tar", last modified: Fri Apr 19 21:40:22 2024, max compression
```

## Comparing `viur-toolkit-0.1.0.dev5.tar` & `viur_toolkit-0.1.0.dev6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.503153 viur-toolkit-0.1.0.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.503153 viur-toolkit-0.1.0.dev5/src/viur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.503153 viur-toolkit-0.1.0.dev5/src/viur/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/viur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:40:22.972419 viur_toolkit-0.1.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-19 21:40:22.972419 viur_toolkit-0.1.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-19 21:40:22.972419 viur_toolkit-0.1.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:40:22.968419 viur_toolkit-0.1.0.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:40:22.964419 viur_toolkit-0.1.0.dev6/src/viur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:40:22.968419 viur_toolkit-0.1.0.dev6/src/viur/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-19 21:40:19.000000 viur_toolkit-0.1.0.dev6/src/viur/toolkit/viur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:40:22.972419 viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-19 21:40:22.000000 viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 21:40:22.000000 viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:40:22.000000 viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 21:40:22.000000 viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 21:40:22.000000 viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/top_level.txt
```

### Comparing `viur-toolkit-0.1.0.dev5/LICENSE` & `viur_toolkit-0.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev5/PKG-INFO` & `viur_toolkit-0.1.0.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev5 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev6 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `viur-toolkit-0.1.0.dev5/setup.cfg` & `viur_toolkit-0.1.0.dev6/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/checks.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/checks.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/context.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/context.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/db.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/db.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/decorators.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/decorators.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/memcache.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/memcache.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/property.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/property.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,48 @@
-import datetime
+import typing as t  # noqa
+from datetime import datetime as dt, timedelta as td, timezone as tz  # noqa
+
+from viur.core import utils
 
 __all__ = ["CachedProperty"]
 
+Seconds: t.TypeAlias = int | float
+Args = t.ParamSpec("Args")
+Value = t.TypeVar("Value")
+
 
-class CachedProperty(object):
+class CachedProperty:
     """Wrapper to Cache the result of a function-call"""
 
-    __slots__ = ("lifetime", "func", "args", "_value", "_lifetimeEnds")
+    __slots__ = ("lifetime", "func", "args", "_value", "_lifetime_ends")
 
-    def __init__(self, lifetime, func, args=None):
+    def __init__(
+        self,
+        lifetime: dt | Seconds,
+        func: t.Callable[Args, Value],
+        args: Args | None = None,
+    ):
         """Initiate a new CachedProperty
 
         :param lifetime: Specifies in seconds how long the cache value should be valid
         :param func: The function that calculates the value
         :param args: Optional Arguments for the function
         """
         if not callable(func):
             raise TypeError("Argument *func* must be a callable function!")
         if args is not None and not isinstance(args, (tuple, list)):
             raise TypeError("Argument *args* must be a tuple, list or None!")
         super(CachedProperty, self).__init__()
-        self.lifetime = lifetime
+        self.lifetime: td = utils.parse.timedelta(lifetime)
         self.func = func
         self.args = tuple() if args is None else args
         self._value = None
-        self._lifetimeEnds = None
+        self._lifetime_ends = None
 
-    def get(self):
+    def get(self) -> Value:
         """Return the value of Property.
         Might be cached or freshly re-calculated."""
-        if self._value is not None and datetime.datetime.now() < self._lifetimeEnds:
+        if self._value is not None and utils.utcNow() < self._lifetime_ends:
             return self._value
         self._value = self.func(*self.args)
-        self._lifetimeEnds = datetime.datetime.now() + datetime.timedelta(seconds=self.lifetime)
+        self._lifetime_ends = utils.utcNow() + self.lifetime
         return self._value
```

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/report.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,18 @@
             writer = UnicodeDictWriter(io, fieldnames=header)
             writer.writerows(self.content)
         else:
             io.write("- no entries -")
         io.seek(0)
 
         # noinspection PyTypeChecker
-        return utils.sendEMail(
+        return email.sendEMail(
             dests=receiver,
             # language=Jinja2
-            name="""Subject: Report {{ skel["name"] }}
+            name="""Report {{ skel["name"] }}
 <table>
 	<thead>
 		<tr>
 			{% for col in skel["header"] %}
 				<th>{{ col }}</th>
 			{% endfor %}
 		</tr>
```

### Comparing `viur-toolkit-0.1.0.dev5/src/viur/toolkit/viur.py` & `viur_toolkit-0.1.0.dev6/src/viur/toolkit/viur.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Helper for ViUR-core types and behavior
 """
 
 import logging
+import typing as t
 
-from viur.core import current
+from viur.core import current, db
 from viur.core.skeleton import SkeletonInstance, skeletonByKind
 
 __all__ = [
     "change_language",
     "without_render_preparation",
     "get_full_skel_from_ref_skel",
+    "iter_skel",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def change_language(lang: str) -> None:
     """Change the current language"""
@@ -29,10 +31,27 @@
         skel = skel.clone()
         skel.renderPreparation = None
     return skel
 
 
 def get_full_skel_from_ref_skel(ref_skel: SkeletonInstance) -> SkeletonInstance:
     kind_name = ref_skel.skeletonCls.__name__.removeprefix("RefSkelFor")
-    skel = skeletonByKind(kind_name)()
+    skel: SkeletonInstance = skeletonByKind(kind_name)() # noqa
     skel.fromDB(ref_skel["key"])
     return skel
+
+
+def iter_skel(query: db.Query) -> t.Iterator[SkeletonInstance]:
+    """Fetch all entries for this query and yield the skel
+
+    Doesn't use fetch() due to the strange ViUR fetch limit (100).
+    Acts as generator to be not memory hungry...
+    """
+    skel: SkeletonInstance = query.srcSkel
+    for entry in query.iter():
+        skel = SkeletonInstance(skel.skeletonCls, clonedBoneMap=skel.boneMap)
+        skel.setEntity(entry)
+        try:
+            yield skel
+        except GeneratorExit:
+            logger.warning("GeneratorExit. Stop iteration.")
+            break
```

### Comparing `viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/PKG-INFO` & `viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev5 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev6 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/SOURCES.txt` & `viur_toolkit-0.1.0.dev6/src/viur_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

