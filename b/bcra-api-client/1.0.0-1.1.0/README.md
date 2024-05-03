# Comparing `tmp/bcra-api-client-1.0.0.tar.gz` & `tmp/bcra-api-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra-api-client-1.0.0.tar", last modified: Fri May  3 19:47:01 2024, max compression
+gzip compressed data, was "bcra-api-client-1.1.0.tar", last modified: Fri May  3 20:10:41 2024, max compression
```

## Comparing `bcra-api-client-1.0.0.tar` & `bcra-api-client-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 19:47:01.717123 bcra-api-client-1.0.0/
--rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      708 2024-05-03 19:47:01.714128 bcra-api-client-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 19:47:01.689194 bcra-api-client-1.0.0/bcra/
--rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.0.0/bcra/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-05-03 19:05:11.000000 bcra-api-client-1.0.0/bcra/base.py
--rw-rw-rw-   0        0        0      289 2024-05-03 18:33:43.000000 bcra-api-client-1.0.0/bcra/client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:47:01.702159 bcra-api-client-1.0.0/bcra/statistics/
--rw-rw-rw-   0        0        0      167 2024-05-03 19:10:13.000000 bcra-api-client-1.0.0/bcra/statistics/__init__.py
--rw-rw-rw-   0        0        0       81 2024-05-03 19:14:53.000000 bcra-api-client-1.0.0/bcra/statistics/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:47:01.713130 bcra-api-client-1.0.0/bcra_api_client.egg-info/
--rw-rw-rw-   0        0        0      708 2024-05-03 19:47:01.000000 bcra-api-client-1.0.0/bcra_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-03 19:47:01.000000 bcra-api-client-1.0.0/bcra_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 19:47:01.000000 bcra-api-client-1.0.0/bcra_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 19:47:01.000000 bcra-api-client-1.0.0/bcra_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-03 19:22:14.000000 bcra-api-client-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 19:47:01.717123 bcra-api-client-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.474481 bcra-api-client-1.1.0/
+-rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      708 2024-05-03 20:10:41.472488 bcra-api-client-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.458523 bcra-api-client-1.1.0/bcra/
+-rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.0/bcra/__init__.py
+-rw-rw-rw-   0        0        0     1255 2024-05-03 19:56:30.000000 bcra-api-client-1.1.0/bcra/base.py
+-rw-rw-rw-   0        0        0      289 2024-05-03 18:33:43.000000 bcra-api-client-1.1.0/bcra/client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.461516 bcra-api-client-1.1.0/bcra/statistics/
+-rw-rw-rw-   0        0        0      167 2024-05-03 19:10:13.000000 bcra-api-client-1.1.0/bcra/statistics/__init__.py
+-rw-rw-rw-   0        0        0      556 2024-05-03 20:04:09.000000 bcra-api-client-1.1.0/bcra/statistics/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:10:41.471489 bcra-api-client-1.1.0/bcra_api_client.egg-info/
+-rw-rw-rw-   0        0        0      708 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 20:10:41.000000 bcra-api-client-1.1.0/bcra_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2024-05-03 20:08:50.000000 bcra-api-client-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 20:10:41.474481 bcra-api-client-1.1.0/setup.cfg
```

### Comparing `bcra-api-client-1.0.0/LICENSE` & `bcra-api-client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.0.0/PKG-INFO` & `bcra-api-client-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.0.0
+Version: 1.1.0
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.0.0/bcra/base.py` & `bcra-api-client-1.1.0/bcra/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             self.BASE + path,
             fields = params,
             headers = self.headers
         )
         
 
         if response.status != 200 :
-            raise "Mverga"
+            raise "Error in Query"
         
         try:
             obj = self._decoded(response)
         except Exception as e:
             print(f"Error json response: {e.message}")
```

### Comparing `bcra-api-client-1.0.0/bcra_api_client.egg-info/PKG-INFO` & `bcra-api-client-1.1.0/bcra_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.0.0
+Version: 1.1.0
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.0.0/pyproject.toml` & `bcra-api-client-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcra-api-client"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Emmanuel Paiva", email="none@email.com"},
 ]
 description = "Consumo de datos de la API del banco central de la Republica Argentina"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

