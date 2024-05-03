# Comparing `tmp/dbrepo-1.4.3rc2.tar.gz` & `tmp/dbrepo-1.4.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrepo-1.4.3rc2.tar", last modified: Mon Apr 29 15:14:26 2024, max compression
+gzip compressed data, was "dbrepo-1.4.3rc3.tar", last modified: Fri May  3 12:18:21 2024, max compression
```

## Comparing `dbrepo-1.4.3rc2.tar` & `dbrepo-1.4.3rc3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 15:14:26.124835 dbrepo-1.4.3rc2/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc2/LICENSE
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-29 15:14:26.124835 dbrepo-1.4.3rc2/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/README.md
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 15:14:26.120835 dbrepo-1.4.3rc2/dbrepo/
--rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/dbrepo/AmqpClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/dbrepo/RestClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/dbrepo/UploadClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc2/dbrepo/__init__.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 15:14:26.120835 dbrepo-1.4.3rc2/dbrepo/api/
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc2/dbrepo/api/__init__.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    21160 2024-04-29 15:14:05.000000 dbrepo-1.4.3rc2/dbrepo/api/dto.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.3rc2/dbrepo/api/encoder.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc2/dbrepo/api/exceptions.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 15:14:26.124835 dbrepo-1.4.3rc2/dbrepo.egg-info/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-29 15:14:26.000000 dbrepo-1.4.3rc2/dbrepo.egg-info/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-29 15:14:26.000000 dbrepo-1.4.3rc2/dbrepo.egg-info/SOURCES.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-29 15:14:26.000000 dbrepo-1.4.3rc2/dbrepo.egg-info/dependency_links.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-29 15:14:26.000000 dbrepo-1.4.3rc2/dbrepo.egg-info/requires.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-29 15:14:26.000000 dbrepo-1.4.3rc2/dbrepo.egg-info/top_level.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1102 2024-04-29 15:14:22.000000 dbrepo-1.4.3rc2/pyproject.toml
--rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-29 15:14:26.124835 dbrepo-1.4.3rc2/setup.cfg
--rw-r--r--   0 mweise    (1000) mweise    (1000)      410 2024-04-29 15:14:22.000000 dbrepo-1.4.3rc2/setup.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-29 15:14:26.124835 dbrepo-1.4.3rc2/tests/
--rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_analyse.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_container.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_database.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_identifier.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_license.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_query.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc2/tests/test_rest_client.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_table.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_user.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc2/tests/test_view.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/LICENSE
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/README.md
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.466653 dbrepo-1.4.3rc3/dbrepo/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/dbrepo/AmqpClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/dbrepo/RestClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/dbrepo/UploadClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/dbrepo/__init__.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.466653 dbrepo-1.4.3rc3/dbrepo/api/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/dbrepo/api/__init__.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    21236 2024-05-03 12:17:16.000000 dbrepo-1.4.3rc3/dbrepo/api/dto.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.3rc3/dbrepo/api/encoder.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/dbrepo/api/exceptions.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/dbrepo.egg-info/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/requires.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/top_level.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1102 2024-05-03 12:18:17.000000 dbrepo-1.4.3rc3/pyproject.toml
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/setup.cfg
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      410 2024-05-03 12:18:17.000000 dbrepo-1.4.3rc3/setup.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/tests/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_analyse.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_container.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_database.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_identifier.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_license.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_query.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/tests/test_rest_client.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_table.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_user.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_view.py
```

### Comparing `dbrepo-1.4.3rc2/LICENSE` & `dbrepo-1.4.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/PKG-INFO` & `dbrepo-1.4.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.3rc2
+Version: 1.4.3rc3
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.3rc2/README.md` & `dbrepo-1.4.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/dbrepo/AmqpClient.py` & `dbrepo-1.4.3rc3/dbrepo/AmqpClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/dbrepo/RestClient.py` & `dbrepo-1.4.3rc3/dbrepo/RestClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/dbrepo/UploadClient.py` & `dbrepo-1.4.3rc3/dbrepo/UploadClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/dbrepo/api/dto.py` & `dbrepo-1.4.3rc3/dbrepo/api/dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,14 +676,20 @@
     val_min: float
     val_max: float
     mean: float
     median: float
     std_dev: float
 
 
+class ApiError(BaseModel):
+    status: str
+    message: str
+    code: str
+
+
 class TableStatistics(BaseModel):
     columns: dict[str, ColumnStatistic]
 
 
 class Unit(BaseModel):
     id: int
     uri: str
```

### Comparing `dbrepo-1.4.3rc2/dbrepo/api/exceptions.py` & `dbrepo-1.4.3rc3/dbrepo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/dbrepo.egg-info/PKG-INFO` & `dbrepo-1.4.3rc3/dbrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.3rc2
+Version: 1.4.3rc3
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.3rc2/dbrepo.egg-info/SOURCES.txt` & `dbrepo-1.4.3rc3/dbrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/pyproject.toml` & `dbrepo-1.4.3rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbrepo"
-version = "1.4.3rc2"
+version = "1.4.3rc3"
 description = "DBRepo Python Library"
 keywords = [
     "DBRepo",
     "Database Repository"
 ]
 authors = [
     { name = "Martin Weise, TU Wien", email = "martin.weise@tuwien.ac.at" }
```

### Comparing `dbrepo-1.4.3rc2/tests/test_analyse.py` & `dbrepo-1.4.3rc3/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_container.py` & `dbrepo-1.4.3rc3/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_database.py` & `dbrepo-1.4.3rc3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_identifier.py` & `dbrepo-1.4.3rc3/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_license.py` & `dbrepo-1.4.3rc3/tests/test_license.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_query.py` & `dbrepo-1.4.3rc3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_rest_client.py` & `dbrepo-1.4.3rc3/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_table.py` & `dbrepo-1.4.3rc3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_user.py` & `dbrepo-1.4.3rc3/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc2/tests/test_view.py` & `dbrepo-1.4.3rc3/tests/test_view.py`

 * *Files identical despite different names*

