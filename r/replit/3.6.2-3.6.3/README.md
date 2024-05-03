# Comparing `tmp/replit-3.6.2.tar.gz` & `tmp/replit-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-3.6.2.tar", max compression
+gzip compressed data, was "replit-3.6.3.tar", max compression
```

## Comparing `replit-3.6.2.tar` & `replit-3.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      720 2024-04-10 13:42:36.208942 replit-3.6.2/LICENSE
--rw-r--r--   0        0        0     1491 2024-04-10 13:42:36.208942 replit-3.6.2/README.md
--rw-r--r--   0        0        0     1487 2024-04-10 13:42:46.180993 replit-3.6.2/pyproject.toml
--rw-r--r--   0        0        0      798 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/__init__.py
--rw-r--r--   0        0        0     3028 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/__main__.py
--rw-r--r--   0        0        0      171 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/Makefile
--rw-r--r--   0        0        0    13225 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/__init__.py
--rw-r--r--   0        0        0     1848 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/test.py
--rw-r--r--   0        0        0     3687 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/types.py
--rw-r--r--   0        0        0      861 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/__init__.py
--rw-r--r--   0        0        0    24452 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/database.py
--rw-r--r--   0        0        0     1520 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/default_db.py
--rw-r--r--   0        0        0     2641 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/server.py
--rw-r--r--   0        0        0       33 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/__init__.py
--rw-r--r--   0        0        0     5800 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/client_pb2.py
--rw-r--r--   0        0        0        0 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/features/__init__.py
--rw-r--r--   0        0        0     1606 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/features/features_pb2.py
--rw-r--r--   0        0        0        0 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/repl/__init__.py
--rw-r--r--   0        0        0     4642 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/repl/repl_pb2.py
--rw-r--r--   0        0        0     4963 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/signing_pb2.py
--rw-r--r--   0        0        0      174 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/__init__.py
--rw-r--r--   0        0        0      159 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/exceptions.py
--rw-r--r--   0        0        0     2110 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/sign.py
--rw-r--r--   0        0        0    13408 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/verify.py
--rw-r--r--   0        0        0     2734 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/info.py
--rw-r--r--   0        0        0      733 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/__init__.py
--rw-r--r--   0        0        0     2640 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/app.py
--rw-r--r--   0        0        0     3666 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/user.py
--rw-r--r--   0        0        0     8607 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/utils.py
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 replit-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0      720 2024-05-03 16:45:51.578735 replit-3.6.3/LICENSE
+-rw-r--r--   0        0        0     1491 2024-05-03 16:45:51.578735 replit-3.6.3/README.md
+-rw-r--r--   0        0        0     1487 2024-05-03 16:46:00.706749 replit-3.6.3/pyproject.toml
+-rw-r--r--   0        0        0      798 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/__init__.py
+-rw-r--r--   0        0        0     3029 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/__main__.py
+-rw-r--r--   0        0        0      171 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/Makefile
+-rw-r--r--   0        0        0    13225 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/__init__.py
+-rw-r--r--   0        0        0     1848 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/test.py
+-rw-r--r--   0        0        0     3687 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/types.py
+-rw-r--r--   0        0        0      862 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/__init__.py
+-rw-r--r--   0        0        0    24466 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/database.py
+-rw-r--r--   0        0        0     1521 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/default_db.py
+-rw-r--r--   0        0        0     2642 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/server.py
+-rw-r--r--   0        0        0       33 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/__init__.py
+-rw-r--r--   0        0        0     5800 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/client_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/features/__init__.py
+-rw-r--r--   0        0        0     1606 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/features/features_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/repl/__init__.py
+-rw-r--r--   0        0        0     4642 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/goval/api/repl/repl_pb2.py
+-rw-r--r--   0        0        0     4963 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/goval/api/signing_pb2.py
+-rw-r--r--   0        0        0      174 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/exceptions.py
+-rw-r--r--   0        0        0     2110 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/sign.py
+-rw-r--r--   0        0        0    13408 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/verify.py
+-rw-r--r--   0        0        0     2735 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/info.py
+-rw-r--r--   0        0        0      733 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/__init__.py
+-rw-r--r--   0        0        0     2640 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/app.py
+-rw-r--r--   0        0        0     3667 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/user.py
+-rw-r--r--   0        0        0     8607 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/utils.py
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 replit-3.6.3/PKG-INFO
```

### Comparing `replit-3.6.2/LICENSE` & `replit-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/README.md` & `replit-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/pyproject.toml` & `replit-3.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit"
-version = "3.6.2"  # Set by GitHub Actions
+version = "3.6.3"  # Set by GitHub Actions
 description = "A library for interacting with features of Replit"
 authors = ["Replit <contact@replit.com>", "mat <pypi@matdoes.dev>", "kennethreitz <me@kennethreitz.org>", "Scoder12 <pypi@scoder12.ml>", "AllAwesome497", ]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/replit/replit-py"
 homepage = "https://github.com/replit/replit-py"
 documentation = "https://replit-py.readthedocs.org/"
```

### Comparing `replit-3.6.2/src/replit/__init__.py` & `replit-3.6.3/src/replit/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/__main__.py` & `replit-3.6.3/src/replit/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI for interacting with your Repl's DB. Written as top-level script."""
+
 import json
 
 import click
 from replit import db as database
 
 
 reset = "\u001b[0m"
```

### Comparing `replit-3.6.2/src/replit/audio/__init__.py` & `replit-3.6.3/src/replit/audio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     def does_loop(self) -> bool:
         """Whether the source repeats itself or not."""
         return self._loops
 
     @property
     def duration(self) -> timedelta:
         """The duration of the source."""
-        return timedelta(millaseconds=self.__payload["Duration"])
+        return timedelta(milliseconds=self.__payload["Duration"])
 
     def get_volume(self) -> float:
         """The volume the source is set to."""
         self.__get_source()
         return self.__payload["Volume"]
 
     def set_volume(self, volume: float) -> None:
```

### Comparing `replit-3.6.2/src/replit/audio/test.py` & `replit-3.6.3/src/replit/audio/test.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/audio/types.py` & `replit-3.6.3/src/replit/audio/types.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/database/__init__.py` & `replit-3.6.3/src/replit/database/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interface with the Replit Database."""
+
 from typing import Any
 
 from . import default_db
 from .database import AsyncDatabase, Database, DBJSONEncoder, dumps, to_primitive
 from .server import make_database_proxy_blueprint, start_database_proxy
 
 __all__ = [
```

### Comparing `replit-3.6.2/src/replit/database/database.py` & `replit-3.6.3/src/replit/database/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 import urllib.parse
 
 import aiohttp
 from aiohttp_retry import ExponentialRetry, RetryClient  # type: ignore
 import requests
 from requests.adapters import HTTPAdapter, Retry
+from urllib3.filepost import encode_multipart_formdata
 
 
 def to_primitive(o: Any) -> Any:
     """If object is an observed object, converts to primitve, otherwise returns it.
 
     Args:
         o (Any): Any object.
@@ -58,26 +59,14 @@
     """
     return json.dumps(val, separators=(",", ":"), cls=DBJSONEncoder)
 
 
 _dumps = dumps
 
 
-def _sanitize_key(key: str) -> str:
-    """Strip slashes from the beginning of keys.
-
-    Args:
-        key (str): The key to strip
-
-    Returns:
-        str: The stripped key
-    """
-    return key.lstrip("/")
-
-
 class AsyncDatabase:
     """Async interface for Replit Database.
 
     :param str db_url: The Database URL to connect to
     :param int retry_count: How many retry attempts we should make
     :param get_db_url Callable: A callback that returns the current db_url
     :param unbind Callable: Permit additional behavior after Database close
@@ -119,14 +108,16 @@
 
         retry_options = ExponentialRetry(attempts=retry_count)
         self.client = RetryClient(client_session=self.sess, retry_options=retry_options)
 
         if self._get_db_url:
             self._refresh_timer = threading.Timer(3600, self._refresh_db)
             self._refresh_timer.start()
+        else:
+            self._refresh_timer = None
         watched_thread = threading.main_thread()
         self._watchdog_timer = threading.Timer(1, self._watchdog, args=[watched_thread])
         self._watchdog_timer.start()
 
     def _refresh_db(self) -> None:
         if self._refresh_timer:
             self._refresh_timer.cancel()
@@ -224,29 +215,29 @@
 
     async def set_bulk_raw(self, values: Dict[str, str]) -> None:
         """Set multiple values in the database.
 
         Args:
             values (Dict[str, str]): The key-value pairs to set.
         """
-        values = {_sanitize_key(k): v for k, v in values.items()}
         async with self.client.post(self.db_url, data=values) as response:
             response.raise_for_status()
 
     async def delete(self, key: str) -> None:
         """Delete a key from the database.
 
         Args:
             key (str): The key to delete
 
         Raises:
             KeyError: Key does not exist
         """
+        body, content_type = encode_multipart_formdata({"key": key})
         async with self.client.delete(
-            self.db_url + "/" + urllib.parse.quote(key)
+            self.db_url, data=body, headers={"Content-Type": content_type}
         ) as response:
             if response.status == 404:
                 raise KeyError(key)
             response.raise_for_status()
 
     async def list(self, prefix: str) -> Tuple[str, ...]:
         """List keys in the database which start with prefix.
@@ -546,14 +537,16 @@
         )
         self.sess.mount("http://", HTTPAdapter(max_retries=retries))
         self.sess.mount("https://", HTTPAdapter(max_retries=retries))
 
         if self._get_db_url:
             self._refresh_timer = threading.Timer(3600, self._refresh_db)
             self._refresh_timer.start()
+        else:
+            self._refresh_timer = None
         watched_thread = threading.main_thread()
         self._watchdog_timer = threading.Timer(1, self._watchdog, args=[watched_thread])
         self._watchdog_timer.start()
 
     def _refresh_db(self) -> None:
         if self._refresh_timer:
             self._refresh_timer.cancel()
@@ -681,28 +674,30 @@
 
     def set_bulk_raw(self, values: Dict[str, str]) -> None:
         """Set multiple values in the database.
 
         Args:
             values (Dict[str, str]): The key-value pairs to set.
         """
-        values = {_sanitize_key(k): v for k, v in values.items()}
         r = self.sess.post(self.db_url, data=values)
         r.raise_for_status()
 
     def __delitem__(self, key: str) -> None:
         """Delete a key from the database.
 
         Args:
             key (str): The key to delete
 
         Raises:
             KeyError: Key is not set
         """
-        r = self.sess.delete(self.db_url + "/" + urllib.parse.quote(key))
+        body, content_type = encode_multipart_formdata({"key": key})
+        r = self.sess.delete(
+            self.db_url, data=body, headers={"Content-Type": content_type}
+        )
         if r.status_code == 404:
             raise KeyError(key)
 
         r.raise_for_status()
 
     def __iter__(self) -> Iterator[str]:
         """Return an iterator for the database."""
```

### Comparing `replit-3.6.2/src/replit/database/default_db.py` & `replit-3.6.3/src/replit/database/default_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A module containing the default database."""
+
 import os
 import os.path
 from typing import Any, Optional
 
 from .database import Database
```

### Comparing `replit-3.6.2/src/replit/database/server.py` & `replit-3.6.3/src/replit/database/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A module containing a database proxy implementation."""
+
 from typing import Any
 from urllib.parse import quote
 
 from flask import Blueprint, Flask, request
 
 from . import default_db
```

### Comparing `replit-3.6.2/src/replit/goval/api/client_pb2.py` & `replit-3.6.3/src/replit/goval/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/goval/api/features/features_pb2.py` & `replit-3.6.3/src/replit/goval/api/features/features_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/goval/api/repl/repl_pb2.py` & `replit-3.6.3/src/replit/goval/api/repl/repl_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/goval/api/signing_pb2.py` & `replit-3.6.3/src/replit/goval/api/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/identity/sign.py` & `replit-3.6.3/src/replit/identity/sign.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/identity/verify.py` & `replit-3.6.3/src/replit/identity/verify.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/info.py` & `replit-3.6.3/src/replit/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Information about your repl."""
+
 import os
 from typing import Optional
 
 from typing_extensions import deprecated
 
 
 class ReplInfo:
```

### Comparing `replit-3.6.2/src/replit/web/__init__.py` & `replit-3.6.3/src/replit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/web/app.py` & `replit-3.6.3/src/replit/web/app.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/src/replit/web/user.py` & `replit-3.6.3/src/replit/web/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for working with user mappings."""
+
 from collections.abc import Mapping, MutableMapping
 from typing import Any, Iterator, Optional
 
 import flask
 
 from .app import ReplitAuthContext
 from .. import database
```

### Comparing `replit-3.6.2/src/replit/web/utils.py` & `replit-3.6.3/src/replit/web/utils.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.2/PKG-INFO` & `replit-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit
-Version: 3.6.2
+Version: 3.6.3
 Summary: A library for interacting with features of Replit
 Home-page: https://github.com/replit/replit-py
 License: ISC
 Author: Replit
 Author-email: contact@replit.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
```

