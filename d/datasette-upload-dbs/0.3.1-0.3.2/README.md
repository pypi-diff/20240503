# Comparing `tmp/datasette-upload-dbs-0.3.1.tar.gz` & `tmp/datasette_upload_dbs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-upload-dbs-0.3.1.tar", last modified: Wed Sep 20 04:19:39 2023, max compression
+gzip compressed data, was "datasette_upload_dbs-0.3.2.tar", last modified: Fri May  3 00:13:00 2024, max compression
```

## Comparing `datasette-upload-dbs-0.3.1.tar` & `datasette_upload_dbs-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 04:19:39.878095 datasette-upload-dbs-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-20 04:19:17.000000 datasette-upload-dbs-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-09-20 04:19:39.878095 datasette-upload-dbs-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2023-09-20 04:19:17.000000 datasette-upload-dbs-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 04:19:39.874094 datasette-upload-dbs-0.3.1/datasette_upload_dbs/
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2023-09-20 04:19:17.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 04:19:39.878095 datasette-upload-dbs-0.3.1/datasette_upload_dbs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2023-09-20 04:19:17.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs/templates/upload_dbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 04:19:39.878095 datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-09-20 04:19:39.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-09-20 04:19:39.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 04:19:39.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-20 04:19:39.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-20 04:19:39.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-20 04:19:39.000000 datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-20 04:19:39.878095 datasette-upload-dbs-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-09-20 04:19:17.000000 datasette-upload-dbs-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 04:19:39.878095 datasette-upload-dbs-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2023-09-20 04:19:17.000000 datasette-upload-dbs-0.3.1/tests/test_upload_dbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:00.271099 datasette_upload_dbs-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 00:12:45.000000 datasette_upload_dbs-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-03 00:13:00.271099 datasette_upload_dbs-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-03 00:12:45.000000 datasette_upload_dbs-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:00.267099 datasette_upload_dbs-0.3.2/datasette_upload_dbs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-03 00:12:45.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:00.271099 datasette_upload_dbs-0.3.2/datasette_upload_dbs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-03 00:12:45.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs/templates/upload_dbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:00.271099 datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-03 00:13:00.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-03 00:13:00.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 00:13:00.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 00:13:00.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 00:13:00.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 00:13:00.000000 datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 00:13:00.271099 datasette_upload_dbs-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-03 00:12:45.000000 datasette_upload_dbs-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:13:00.271099 datasette_upload_dbs-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-03 00:12:45.000000 datasette_upload_dbs-0.3.2/tests/test_upload_dbs.py
```

### Comparing `datasette-upload-dbs-0.3.1/LICENSE` & `datasette_upload_dbs-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-upload-dbs-0.3.1/PKG-INFO` & `datasette_upload_dbs-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-upload-dbs
-Version: 0.3.1
+Version: 0.3.2
 Summary: Upload SQLite database files to Datasette
 Home-page: https://github.com/simonw/datasette-upload-dbs
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-upload-dbs/issues
 Project-URL: CI, https://github.com/simonw/datasette-upload-dbs/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-upload-dbs/releases
```

### Comparing `datasette-upload-dbs-0.3.1/README.md` & `datasette_upload_dbs-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `datasette-upload-dbs-0.3.1/datasette_upload_dbs/__init__.py` & `datasette_upload_dbs-0.3.2/datasette_upload_dbs/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette-upload-dbs-0.3.1/datasette_upload_dbs/templates/upload_dbs.html` & `datasette_upload_dbs-0.3.2/datasette_upload_dbs/templates/upload_dbs.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 progress {
     -webkit-appearance: none;
     appearance: none;
     border: none;
     width: 80%;
     height: 2em;
     margin-top: 1em;
+    margin-bottom: 1em;
 }
 progress::-webkit-progress-bar {
     background-color: #ddd;
 }
 progress::-webkit-progress-value {
     background-color: #124d77;
 }
```

### Comparing `datasette-upload-dbs-0.3.1/datasette_upload_dbs.egg-info/PKG-INFO` & `datasette_upload_dbs-0.3.2/datasette_upload_dbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-upload-dbs
-Version: 0.3.1
+Version: 0.3.2
 Summary: Upload SQLite database files to Datasette
 Home-page: https://github.com/simonw/datasette-upload-dbs
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-upload-dbs/issues
 Project-URL: CI, https://github.com/simonw/datasette-upload-dbs/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-upload-dbs/releases
```

### Comparing `datasette-upload-dbs-0.3.1/setup.py` & `datasette_upload_dbs-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette-upload-dbs-0.3.1/tests/test_upload_dbs.py` & `datasette_upload_dbs-0.3.2/tests/test_upload_dbs.py`

 * *Files identical despite different names*

