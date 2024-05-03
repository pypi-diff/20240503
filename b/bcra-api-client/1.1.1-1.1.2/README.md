# Comparing `tmp/bcra-api-client-1.1.1.tar.gz` & `tmp/bcra-api-client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra-api-client-1.1.1.tar", last modified: Fri May  3 21:32:50 2024, max compression
+gzip compressed data, was "bcra-api-client-1.1.2.tar", last modified: Fri May  3 21:52:53 2024, max compression
```

## Comparing `bcra-api-client-1.1.1.tar` & `bcra-api-client-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.918116 bcra-api-client-1.1.1/
--rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      708 2024-05-03 21:32:50.916122 bcra-api-client-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.897174 bcra-api-client-1.1.1/bcra/
--rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.1/bcra/__init__.py
--rw-rw-rw-   0        0        0     1203 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/base.py
--rw-rw-rw-   0        0        0      301 2024-05-03 21:27:11.000000 bcra-api-client-1.1.1/bcra/client.py
--rw-rw-rw-   0        0        0      394 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.902159 bcra-api-client-1.1.1/bcra/statistics/
--rw-rw-rw-   0        0        0      228 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/statistics/__init__.py
--rw-rw-rw-   0        0        0      642 2024-05-03 21:22:17.000000 bcra-api-client-1.1.1/bcra/statistics/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:32:50.914127 bcra-api-client-1.1.1/bcra_api_client.egg-info/
--rw-rw-rw-   0        0        0      708 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 21:32:50.000000 bcra-api-client-1.1.1/bcra_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-03 21:27:21.000000 bcra-api-client-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 21:32:50.919115 bcra-api-client-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.812816 bcra-api-client-1.1.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      708 2024-05-03 21:52:53.810822 bcra-api-client-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.795863 bcra-api-client-1.1.2/bcra/
+-rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.2/bcra/__init__.py
+-rw-rw-rw-   0        0        0     1203 2024-05-03 21:22:17.000000 bcra-api-client-1.1.2/bcra/base.py
+-rw-rw-rw-   0        0        0      301 2024-05-03 21:27:11.000000 bcra-api-client-1.1.2/bcra/client.py
+-rw-rw-rw-   0        0        0      394 2024-05-03 21:22:17.000000 bcra-api-client-1.1.2/bcra/config.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.800848 bcra-api-client-1.1.2/bcra/statistics/
+-rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.2/bcra/statistics/__init__.py
+-rw-rw-rw-   0        0        0      614 2024-05-03 21:48:25.000000 bcra-api-client-1.1.2/bcra/statistics/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.808827 bcra-api-client-1.1.2/bcra_api_client.egg-info/
+-rw-rw-rw-   0        0        0      708 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2024-05-03 21:50:47.000000 bcra-api-client-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:52:53.813813 bcra-api-client-1.1.2/setup.cfg
```

### Comparing `bcra-api-client-1.1.1/LICENSE` & `bcra-api-client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.1/PKG-INFO` & `bcra-api-client-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.1/bcra/base.py` & `bcra-api-client-1.1.2/bcra/base.py`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.1/bcra/statistics/variables.py` & `bcra-api-client-1.1.2/bcra/statistics/variables.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from bcra.base import BaseClient
 from bcra.config import ConfigClient
-from bcra.statistics import PATH_ROOT
 
 
 class Variables(BaseClient):
 
-    def __init__(self, config: ConfigClient) -> None:
-        self.path = PATH_ROOT + "principalesvariables"
+    def __init__(self, config: ConfigClient, path_root) -> None:
+        self.path = path_root + "principalesvariables"
         super().__init__(config)
 
     def get(self,
             id_variable: int = None,
             from_: str = None,
             to: str = None):
         path_params = ""
```

### Comparing `bcra-api-client-1.1.1/bcra_api_client.egg-info/PKG-INFO` & `bcra-api-client-1.1.2/bcra_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.1/pyproject.toml` & `bcra-api-client-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcra-api-client"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Emmanuel Paiva", email="none@email.com"},
 ]
 description = "Consumo de datos de la API del banco central de la Republica Argentina"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

