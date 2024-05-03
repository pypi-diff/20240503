# Comparing `tmp/nettigo_air_monitor-3.0.0.tar.gz` & `tmp/nettigo_air_monitor-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettigo_air_monitor-3.0.0.tar", last modified: Fri Apr 19 13:53:59 2024, max compression
+gzip compressed data, was "nettigo_air_monitor-3.0.1.tar", last modified: Fri May  3 12:06:08 2024, max compression
```

## Comparing `nettigo_air_monitor-3.0.0.tar` & `nettigo_air_monitor-3.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.026881 nettigo_air_monitor-3.0.0/nettigo_air_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.026881 nettigo_air_monitor-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.258569 nettigo_air_monitor-3.0.1/nettigo_air_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.258569 nettigo_air_monitor-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/tests/test_init.py
```

### Comparing `nettigo_air_monitor-3.0.0/LICENSE` & `nettigo_air_monitor-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.0/PKG-INFO` & `nettigo_air_monitor-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettigo_air_monitor
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nettigo_air_monitor-3.0.0/README.md` & `nettigo_air_monitor-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.0/nettigo_air_monitor/__init__.py` & `nettigo_air_monitor-3.0.1/nettigo_air_monitor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     def __init__(self, session: ClientSession, options: ConnectionOptions) -> None:
         """Initialize."""
         self.host = options.host
         self._last_data: dict[str, Any] = {}
         self._options = options
         self._session = session
-        self._software_version: str
+        self._software_version: str | None = None
         self._update_errors: int = 0
         self._auth_enabled: bool = False
 
     @classmethod
     async def create(
         cls, session: ClientSession, options: ConnectionOptions
     ) -> NettigoAirMonitor:
@@ -64,15 +64,15 @@
 
         try:
             config = await self.async_check_credentials()
         except AuthFailedError:
             self._auth_enabled = True
         else:
             self._auth_enabled = config["www_basicauth_enabled"]
-            self._software_version = config.get("SOFTWARE_VERSION", "")
+            self._software_version = config.get("SOFTWARE_VERSION")
 
     @staticmethod
     def _construct_url(arg: str, **kwargs: str) -> str:
         """Construct Nettigo Air Monitor URL."""
         return ENDPOINTS[arg].format(**kwargs)
 
     @staticmethod
@@ -189,15 +189,15 @@
             resp = await self._async_http_request("get", url)
         except NotRespondingError as error:
             raise ApiError(error.status) from error
 
         return await resp.json()
 
     @property
-    def software_version(self) -> str:
+    def software_version(self) -> str | None:
         """Return software version."""
         return self._software_version
 
     @property
     def auth_enabled(self) -> bool:
         """Return True if basic auth is enabled."""
         return self._auth_enabled
```

### Comparing `nettigo_air_monitor-3.0.0/nettigo_air_monitor/const.py` & `nettigo_air_monitor-3.0.1/nettigo_air_monitor/const.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.0/nettigo_air_monitor/exceptions.py` & `nettigo_air_monitor-3.0.1/nettigo_air_monitor/exceptions.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.0/nettigo_air_monitor/model.py` & `nettigo_air_monitor-3.0.1/nettigo_air_monitor/model.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/PKG-INFO` & `nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettigo_air_monitor
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nettigo_air_monitor-3.0.0/pyproject.toml` & `nettigo_air_monitor-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.0/setup.py` & `nettigo_air_monitor-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "3.0.0"
+VERSION = "3.0.1"
 
 setup(
     name="nettigo_air_monitor",
     version=VERSION,
     author="Maciej Bieniek",
     description=(
         "Python wrapper for getting air quality data from Nettigo Air Monitor devices."
```

### Comparing `nettigo_air_monitor-3.0.0/tests/test_init.py` & `nettigo_air_monitor-3.0.1/tests/test_init.py`

 * *Files identical despite different names*

