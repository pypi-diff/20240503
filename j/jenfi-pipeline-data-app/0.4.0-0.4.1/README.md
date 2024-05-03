# Comparing `tmp/jenfi_pipeline_data_app-0.4.0.tar.gz` & `tmp/jenfi_pipeline_data_app-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenfi_pipeline_data_app-0.4.0.tar", max compression
+gzip compressed data, was "jenfi_pipeline_data_app-0.4.1.tar", max compression
```

## Comparing `jenfi_pipeline_data_app-0.4.0.tar` & `jenfi_pipeline_data_app-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      510 2023-01-20 08:43:07.713833 jenfi_pipeline_data_app-0.4.0/README.md
--rw-r--r--   0        0        0     1313 2022-09-28 02:32:06.697627 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/API.md
--rw-r--r--   0        0        0     1526 2023-05-09 02:21:49.104886 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/__init__.py
--rw-r--r--   0        0        0      354 2023-05-09 01:55:02.513098 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/_pdoc.py
--rw-r--r--   0        0        0     2222 2023-05-09 01:55:30.035561 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app.py
--rw-r--r--   0        0        0      345 2023-05-09 01:55:01.490867 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_constants.py
--rw-r--r--   0        0        0     1107 2023-05-09 01:56:23.563197 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_db_handler.py
--rw-r--r--   0        0        0     1066 2022-11-02 00:33:49.627056 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_exit_program.py
--rw-r--r--   0        0        0     1074 2023-05-09 01:55:02.723840 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_models_s3.py
--rw-r--r--   0        0        0     1323 2023-05-09 02:13:40.620671 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_parameters.py
--rw-r--r--   0        0        0     1282 2023-05-09 02:21:49.112873 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_query.py
--rw-r--r--   0        0        0     2896 2023-05-09 01:57:09.624035 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_result.py
--rw-r--r--   0        0        0      569 2023-05-09 01:58:34.501284 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
--rw-r--r--   0        0        0     1419 2023-05-09 01:58:06.146777 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/config/db.py
--rw-r--r--   0        0        0      395 2023-05-09 01:55:01.562329 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/config/s3.py
--rw-r--r--   0        0        0       43 2023-05-09 01:58:34.496937 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/__init__.py
--rw-r--r--   0        0        0     3838 2023-05-09 01:55:02.728505 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/cacher.py
--rw-r--r--   0        0        0     1771 2023-05-09 02:14:47.825830 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/db_cache.py
--rw-r--r--   0        0        0     2050 2023-05-09 01:58:45.726647 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_models.py
--rw-r--r--   0        0        0      941 2023-05-09 02:16:15.078822 jenfi_pipeline_data_app-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-01-16 03:30:30.019998 jenfi_pipeline_data_app-0.4.1/README.md
+-rw-r--r--   0        0        0     1313 2023-01-16 02:40:26.715779 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/API.md
+-rw-r--r--   0        0        0     1526 2023-05-30 09:11:12.212975 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/__init__.py
+-rw-r--r--   0        0        0      354 2023-05-30 09:11:12.213698 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/_pdoc.py
+-rw-r--r--   0        0        0     2367 2024-05-02 16:14:34.857722 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app.py
+-rw-r--r--   0        0        0      345 2023-05-30 09:11:12.214511 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_constants.py
+-rw-r--r--   0        0        0     1107 2024-02-22 07:39:24.264183 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_db_handler.py
+-rw-r--r--   0        0        0     1066 2023-01-16 02:40:26.716191 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_exit_program.py
+-rw-r--r--   0        0        0     1074 2023-05-30 09:11:12.215285 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_models_s3.py
+-rw-r--r--   0        0        0     1323 2023-05-30 09:11:12.216581 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_parameters.py
+-rw-r--r--   0        0        0     1282 2023-05-30 09:11:12.216967 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_query.py
+-rw-r--r--   0        0        0     2896 2023-05-30 09:11:12.217328 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_result.py
+-rw-r--r--   0        0        0      569 2023-05-30 09:11:12.217681 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
+-rw-r--r--   0        0        0     1419 2024-02-22 07:14:05.283471 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/config/db.py
+-rw-r--r--   0        0        0      395 2023-05-30 09:11:12.218386 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/config/s3.py
+-rw-r--r--   0        0        0       43 2023-05-30 09:11:12.218741 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/db_cache/__init__.py
+-rw-r--r--   0        0        0     3838 2023-05-30 09:11:12.219328 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/db_cache/cacher.py
+-rw-r--r--   0        0        0     1973 2024-05-03 04:51:38.484307 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/db_cache/db_cache.py
+-rw-r--r--   0        0        0     2050 2023-05-30 09:11:12.220034 jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/db_models.py
+-rw-r--r--   0        0        0      982 2024-05-02 16:16:26.111227 jenfi_pipeline_data_app-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.4.1/PKG-INFO
```

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/API.md` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/API.md`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/__init__.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/__init__.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,16 +64,20 @@
                 "/tmp" if platform.system() == "Darwin" else tempfile.gettempdir()
             )
 
         return Path(tmp_path)
 
     def tmp_filepath(self, rel_filepath) -> Path:
         tmp_path = self.tmp_dir()
+        file_path = Path(os.path.join(tmp_path, rel_filepath))
 
-        return Path(os.path.join(tmp_path, rel_filepath))
+        # Create the directory if it doesn't exist
+        os.makedirs(os.path.dirname(file_path), exist_ok=True)
+
+        return file_path
 
     def __repr__(self):
         return self.__dict__
 
     if "pytest" in sys.modules:
         from .app_funcs._test_funcs import (
             _test_access_global_var,
```

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_db_handler.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_db_handler.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_exit_program.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_exit_program.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_models_s3.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_models_s3.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_parameters.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_parameters.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_query.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_query.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_result.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_result.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_test_funcs.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/app_funcs/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/config/db.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/config/db.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/cacher.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/db_cache/cacher.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/db_cache.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/db_cache/db_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,22 @@
 
         pass
 
     def df_query(self, query_str: str, rebuild_cache: bool) -> pd.DataFrame:
         return self._with_cacher(self._df_query, query_str, rebuild_cache)
 
     def _df_query(self, query_str: str) -> pd.DataFrame:
-        return pd.read_sql(query_str, self.db_engine)
+        # For pandas 2.2.0
+        # https://stackoverflow.com/a/77949093
+
+        # Debugging
+        print(query_str)
+        print(self.db_engine)
+        with self.db_engine.connect() as conn:
+            return pd.read_sql(query_str, conn.connection)
 
     def query_one(self, query_str: str, rebuild_cache: bool):
         return self._with_cacher(self._query_one, query_str, rebuild_cache)
 
     def _query_one(self, query_str: str):
         return self.db.execute(query_str).fetchone()
```

### Comparing `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_models.py` & `jenfi_pipeline_data_app-0.4.1/jenfi_pipeline_data_app/db_models.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.0/pyproject.toml` & `jenfi_pipeline_data_app-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "jenfi-pipeline-data-app"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 readme = "README.md"
 authors = ["Justin Louie <224840+nitsujri@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 SQLAlchemy = "^1.4.40"
 numpy = "^1.23.2"
 python-dotenv = "^0.20.0"
 psycopg2 = "^2.9.3"
-pandas = "^1.4.3"
+pandas = "2.2"
 boto3 = "^1.24.78"
 sqlparse = "^0.4.2"
 scikit-learn = "^1.1.2"
 sagemaker = "^2.150.0"
 statsmodels = "^0.13.5"
 jupyterlab-git = "^0.41.0"
+levenshtein = "^0.21.0"
+catboost = "^1.2.3"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 pytest = "^7.1.3"
 pdoc3 = "^0.10.0"
 papermill = "^2.4.0"
 jupyterlab = "^3.4.7"
```

### Comparing `jenfi_pipeline_data_app-0.4.0/PKG-INFO` & `jenfi_pipeline_data_app-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: jenfi-pipeline-data-app
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Justin Louie
 Author-email: 224840+nitsujri@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0)
 Requires-Dist: boto3 (>=1.24.78,<2.0.0)
+Requires-Dist: catboost (>=1.2.3,<2.0.0)
 Requires-Dist: jupyterlab-git (>=0.41.0,<0.42.0)
+Requires-Dist: levenshtein (>=0.21.0,<0.22.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: pandas (==2.2)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: sagemaker (>=2.150.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
 Description-Content-Type: text/markdown
```

