# Comparing `tmp/eppo_server_sdk-3.0.1.tar.gz` & `tmp/eppo_server_sdk-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo_server_sdk-3.0.1.tar", last modified: Fri Apr 26 21:52:56 2024, max compression
+gzip compressed data, was "eppo_server_sdk-3.0.2.tar", last modified: Thu May  2 23:36:50 2024, max compression
```

## Comparing `eppo_server_sdk-3.0.1.tar` & `eppo_server_sdk-3.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:52:56.283689 eppo_server_sdk-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-26 21:52:56.283689 eppo_server_sdk-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:52:56.283689 eppo_server_sdk-3.0.1/eppo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/assignment_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/configuration_requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/configuration_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/read_write_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/sharders.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/eppo_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:52:56.283689 eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-26 21:52:56.000000 eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-26 21:52:56.000000 eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:52:56.000000 eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 21:52:56.000000 eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 21:52:56.000000 eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 21:52:52.000000 eppo_server_sdk-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 21:52:56.283689 eppo_server_sdk-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/eppo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/assignment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/configuration_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/configuration_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/read_write_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/sharders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-02 23:36:50.571749 eppo_server_sdk-3.0.2/setup.cfg
```

### Comparing `eppo_server_sdk-3.0.1/LICENSE` & `eppo_server_sdk-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/PKG-INFO` & `eppo_server_sdk-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 3.0.1
+Version: 3.0.2
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo_server_sdk-3.0.1/eppo_client/__init__.py` & `eppo_server_sdk-3.0.2/eppo_client/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional
 from eppo_client.client import EppoClient
 from eppo_client.config import Config
 from eppo_client.configuration_requestor import (
     ExperimentConfigurationRequestor,
 )
 from eppo_client.configuration_store import ConfigurationStore
-from eppo_client.constants import MAX_CACHE_ENTRIES
 from eppo_client.http_client import HttpClient, SdkParams
 from eppo_client.models import Flag
 from eppo_client.read_write_lock import ReadWriteLock
 from eppo_client.version import __version__
 
 
 __client: Optional[EppoClient] = None
@@ -27,51 +26,43 @@
     :type config: Config
     """
     config._validate()
     sdk_params = SdkParams(
         apiKey=config.api_key, sdkName="python", sdkVersion=__version__
     )
     http_client = HttpClient(base_url=config.base_url, sdk_params=sdk_params)
-    config_store: ConfigurationStore[Flag] = ConfigurationStore(
-        max_size=MAX_CACHE_ENTRIES
-    )
+    config_store: ConfigurationStore[Flag] = ConfigurationStore()
     config_requestor = ExperimentConfigurationRequestor(
         http_client=http_client, config_store=config_store
     )
     assignment_logger = config.assignment_logger
     is_graceful_mode = config.is_graceful_mode
     global __client
     global __lock
-    try:
-        __lock.acquire_write()
+    with __lock.writer():
         if __client:
             # if a client was already initialized, stop the background processes of the old client
             __client._shutdown()
         __client = EppoClient(
             config_requestor=config_requestor,
             assignment_logger=assignment_logger,
             is_graceful_mode=is_graceful_mode,
         )
         return __client
-    finally:
-        __lock.release_write()
 
 
 def get_instance() -> EppoClient:
     """Used to access an initialized client instance
 
     Use this method to get a client instance for assigning variants.
     This method may only be called after invocation of :func:`eppo_client.init()`, otherwise it throws an exception.
 
     :return: a shared client instance
     :rtype: EppoClient
     """
     global __client
     global __lock
-    try:
-        __lock.acquire_read()
+    with __lock.reader():
         if __client:
             return __client
         else:
             raise Exception("init() must be called before get_instance()")
-    finally:
-        __lock.release_read()
```

### Comparing `eppo_server_sdk-3.0.1/eppo_client/client.py` & `eppo_server_sdk-3.0.2/eppo_client/client.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_client/configuration_requestor.py` & `eppo_server_sdk-3.0.2/eppo_client/configuration_requestor.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_client/configuration_store.py` & `eppo_server_sdk-3.0.2/eppo_client/configuration_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 from typing import Dict, Optional, TypeVar, Generic
-from cachetools import LRUCache
 
 from eppo_client.read_write_lock import ReadWriteLock
 
 T = TypeVar("T")
 
 
 class ConfigurationStore(Generic[T]):
-    def __init__(self, max_size: int):
-        self.__cache: LRUCache = LRUCache(maxsize=max_size)
+    def __init__(self):
+        self.__cache: Dict[str, T] = {}
         self.__lock = ReadWriteLock()
 
     def get_configuration(self, key: str) -> Optional[T]:
-        try:
-            self.__lock.acquire_read()
-            return self.__cache[key]
-        except KeyError:
-            return None  # key does not exist
-        finally:
-            self.__lock.release_read()
+        with self.__lock.reader():
+            return self.__cache.get(key, None)
 
     def set_configurations(self, configs: Dict[str, T]):
-        try:
-            self.__lock.acquire_write()
-            self.__cache.clear()
-            for key, config in configs.items():
-                self.__cache[key] = config
-        finally:
-            self.__lock.release_write()
+        with self.__lock.writer():
+            self.__cache = configs
 
     def get_keys(self):
-        return list(self.__cache.keys())
+        with self.__lock.reader():
+            return list(self.__cache.keys())
```

### Comparing `eppo_server_sdk-3.0.1/eppo_client/eval.py` & `eppo_server_sdk-3.0.2/eppo_client/eval.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_client/http_client.py` & `eppo_server_sdk-3.0.2/eppo_client/http_client.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_client/models.py` & `eppo_server_sdk-3.0.2/eppo_client/models.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_client/poller.py` & `eppo_server_sdk-3.0.2/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_client/read_write_lock.py` & `eppo_server_sdk-3.0.2/eppo_client/read_write_lock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 import threading
+from contextlib import contextmanager
 
-# Copied from: https://www.oreilly.com/library/view/python-cookbook/0596001673/ch06s04.html
+# Adapted from: https://www.oreilly.com/library/view/python-cookbook/0596001673/ch06s04.html
 
 
 class ReadWriteLock:
     """A lock object that allows many simultaneous "read locks", but
     only one "write lock." """
 
     def __init__(self):
         self._read_ready = threading.Condition(threading.Lock())
         self._readers = 0
 
     def acquire_read(self):
         """Acquire a read lock. Blocks only if a thread has
         acquired the write lock."""
-        self._read_ready.acquire()
-        try:
+        with self._read_ready:
             self._readers += 1
-        finally:
-            self._read_ready.release()
 
     def release_read(self):
         """Release a read lock."""
-        self._read_ready.acquire()
-        try:
+        with self._read_ready:
             self._readers -= 1
             if not self._readers:
                 self._read_ready.notify_all()
-        finally:
-            self._read_ready.release()
 
     def acquire_write(self):
         """Acquire a write lock. Blocks until there are no
         acquired read or write locks."""
         self._read_ready.acquire()
         while self._readers > 0:
             self._read_ready.wait()
 
     def release_write(self):
         """Release a write lock."""
         self._read_ready.release()
+
+    @contextmanager
+    def reader(self):
+        try:
+            self.acquire_read()
+            yield
+        finally:
+            self.release_read()
+
+    @contextmanager
+    def writer(self):
+        try:
+            self.acquire_write()
+            yield
+        finally:
+            self.release_write()
```

### Comparing `eppo_server_sdk-3.0.1/eppo_client/rules.py` & `eppo_server_sdk-3.0.2/eppo_client/rules.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_client/sharders.py` & `eppo_server_sdk-3.0.2/eppo_client/sharders.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/PKG-INFO` & `eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 3.0.1
+Version: 3.0.2
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo_server_sdk-3.0.1/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.1/setup.cfg` & `eppo_server_sdk-3.0.2/setup.cfg`

 * *Files identical despite different names*

