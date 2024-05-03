# Comparing `tmp/bcra-api-client-1.1.0.tar.gz` & `tmp/bcra-api-client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra-api-client-1.1.0.tar", last modified: Fri May  3 20:10:41 2024, max compression
+gzip compressed data, was "bcra-api-client-1.1.1.tar", last modified: Fri May  3 21:32:50 2024, max compression
```

## Comparing `bcra-api-client-1.1.0.tar` & `bcra-api-client-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.474481 bcra-api-client-1.1.0/
--rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      708 2024-05-03 20:10:41.472488 bcra-api-client-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.458523 bcra-api-client-1.1.0/bcra/
--rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.0/bcra/__init__.py
--rw-rw-rw-   0        0        0     1255 2024-05-03 19:56:30.000000 bcra-api-client-1.1.0/bcra/base.py
--rw-rw-rw-   0        0        0      289 2024-05-03 18:33:43.000000 bcra-api-client-1.1.0/bcra/client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.461516 bcra-api-client-1.1.0/bcra/statistics/
--rw-rw-rw-   0        0        0      167 2024-05-03 19:10:13.000000 bcra-api-client-1.1.0/bcra/statistics/__init__.py
--rw-rw-rw-   0        0        0      556 2024-05-03 20:04:09.000000 bcra-api-client-1.1.0/bcra/statistics/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.471489 bcra-api-client-1.1.0/bcra_api_client.egg-info/
--rw-rw-rw-   0        0        0      708 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-03 20:08:50.000000 bcra-api-client-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 20:10:41.474481 bcra-api-client-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.918116 bcra-api-client-1.1.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      708 2024-05-03 21:32:50.916122 bcra-api-client-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.897174 bcra-api-client-1.1.1/bcra/
+-rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.1/bcra/__init__.py
+-rw-rw-rw-   0        0        0     1203 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/base.py
+-rw-rw-rw-   0        0        0      301 2024-05-03 21:27:11.000000 bcra-api-client-1.1.1/bcra/client.py
+-rw-rw-rw-   0        0        0      394 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/config.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.902159 bcra-api-client-1.1.1/bcra/statistics/
+-rw-rw-rw-   0        0        0      228 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/statistics/__init__.py
+-rw-rw-rw-   0        0        0      642 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/statistics/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.914127 bcra-api-client-1.1.1/bcra_api_client.egg-info/
+-rw-rw-rw-   0        0        0      708 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2024-05-03 21:27:21.000000 bcra-api-client-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:32:50.919115 bcra-api-client-1.1.1/setup.cfg
```

### Comparing `bcra-api-client-1.1.0/LICENSE` & `bcra-api-client-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.0/PKG-INFO` & `bcra-api-client-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.0/bcra/base.py` & `bcra-api-client-1.1.1/bcra/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,24 @@
+from .config import ConfigClient
 import pkg_resources
 import urllib3
 import json
 
 version = "unknown"
 
 try:
    version = pkg_resources.require("bcra-api-client")[0].version
 except:
     pass
 
 class BaseClient:
 
-    def __init__(self,
-                 api_key: str,
-                 connect_timeout: float,
-                 base : str
-                 ) -> None:
+    def __init__(self, config: ConfigClient) -> None:
         
-        self.BASE = base
+        self.base_url = config.base_url
         
         self.headers = {
             "Accept-Encoding": "gzip",
             "User-Agent": f"paivae/BCRA BCRA_Python_Client/{version}",
         }
 
         self.client = urllib3.PoolManager(
```

### Comparing `bcra-api-client-1.1.0/bcra/statistics/variables.py` & `bcra-api-client-1.1.1/bcra/statistics/variables.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from bcra.base import BaseClient
+from bcra.config import ConfigClient
 from bcra.statistics import PATH_ROOT
 
+
 class Variables(BaseClient):
-    
-    def __init__(self) -> None:
-        self.path = PATH_ROOT + "principalesvariables"
 
+    def __init__(self, config: ConfigClient) -> None:
+        self.path = PATH_ROOT + "principalesvariables"
+        super().__init__(config)
 
     def get(self,
-            idVariable: int = None,
+            id_variable: int = None,
             from_: str = None,
             to: str = None):
-        
         path_params = ""
 
-        if(idVariable != None and from_ != None and to != None):
-            path_params = f"{self.path}/{idVariable}/{from_}/{to}"
+        if (id_variable != None and from_ != None and to != None):
+            path_params = f"{self.path}/{id_variable}/{from_}/{to}"
 
-        return self._get(path=self.path, params=path_params)
+        return self._get(path=self.path, params=path_params)
```

### Comparing `bcra-api-client-1.1.0/bcra_api_client.egg-info/PKG-INFO` & `bcra-api-client-1.1.1/bcra_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.0/pyproject.toml` & `bcra-api-client-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcra-api-client"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Emmanuel Paiva", email="none@email.com"},
 ]
 description = "Consumo de datos de la API del banco central de la Republica Argentina"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

