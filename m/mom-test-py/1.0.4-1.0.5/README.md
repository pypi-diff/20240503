# Comparing `tmp/mom_test_py-1.0.4.tar.gz` & `tmp/mom_test_py-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mom_test_py-1.0.4.tar", last modified: Fri May  3 01:51:08 2024, max compression
+gzip compressed data, was "mom_test_py-1.0.5.tar", last modified: Fri May  3 02:08:30 2024, max compression
```

## Comparing `mom_test_py-1.0.4.tar` & `mom_test_py-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:51:08.875982 mom_test_py-1.0.4/
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1468 2024-05-03 01:51:08.875982 mom_test_py-1.0.4/PKG-INFO
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1269 2024-04-24 06:32:01.000000 mom_test_py-1.0.4/README.md
-drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:51:08.875982 mom_test_py-1.0.4/mom_test_py/
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       24 2024-05-03 01:47:10.000000 mom_test_py-1.0.4/mom_test_py/__init__.py
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     3758 2024-05-03 01:41:36.000000 mom_test_py-1.0.4/mom_test_py/main.py
-drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:51:08.875982 mom_test_py-1.0.4/mom_test_py/rest/
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       36 2024-04-24 10:03:26.000000 mom_test_py-1.0.4/mom_test_py/rest/__init__.py
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     6457 2024-05-02 09:43:00.000000 mom_test_py-1.0.4/mom_test_py/test_validation.py
-drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 01:51:08.875982 mom_test_py-1.0.4/mom_test_py.egg-info/
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1468 2024-05-03 01:51:08.000000 mom_test_py-1.0.4/mom_test_py.egg-info/PKG-INFO
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      262 2024-05-03 01:51:08.000000 mom_test_py-1.0.4/mom_test_py.egg-info/SOURCES.txt
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)        1 2024-05-03 01:51:08.000000 mom_test_py-1.0.4/mom_test_py.egg-info/dependency_links.txt
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       12 2024-05-03 01:51:08.000000 mom_test_py-1.0.4/mom_test_py.egg-info/top_level.txt
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       38 2024-05-03 01:51:08.875982 mom_test_py-1.0.4/setup.cfg
--rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      427 2024-05-03 01:48:02.000000 mom_test_py-1.0.4/setup.py
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 02:08:30.299976 mom_test_py-1.0.5/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1468 2024-05-03 02:08:30.299976 mom_test_py-1.0.5/PKG-INFO
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1269 2024-04-24 06:32:01.000000 mom_test_py-1.0.5/README.md
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 02:08:30.299976 mom_test_py-1.0.5/mom_test_py/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     3758 2024-05-03 01:41:36.000000 mom_test_py-1.0.5/mom_test_py/main.py
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 02:08:30.299976 mom_test_py-1.0.5/mom_test_py/rest/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       36 2024-04-24 10:03:26.000000 mom_test_py-1.0.5/mom_test_py/rest/__init__.py
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     6457 2024-05-02 09:43:00.000000 mom_test_py-1.0.5/mom_test_py/test_validation.py
+drwxrwxr-x   0 sreymom   (1000) sreymom   (1000)        0 2024-05-03 02:08:30.299976 mom_test_py-1.0.5/mom_test_py.egg-info/
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)     1468 2024-05-03 02:08:30.000000 mom_test_py-1.0.5/mom_test_py.egg-info/PKG-INFO
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      238 2024-05-03 02:08:30.000000 mom_test_py-1.0.5/mom_test_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)        1 2024-05-03 02:08:30.000000 mom_test_py-1.0.5/mom_test_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)        1 2024-05-03 02:08:30.000000 mom_test_py-1.0.5/mom_test_py.egg-info/top_level.txt
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)       38 2024-05-03 02:08:30.299976 mom_test_py-1.0.5/setup.cfg
+-rw-rw-r--   0 sreymom   (1000) sreymom   (1000)      427 2024-05-03 02:08:26.000000 mom_test_py-1.0.5/setup.py
```

### Comparing `mom_test_py-1.0.4/PKG-INFO` & `mom_test_py-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mom_test_py
-Version: 1.0.4
+Version: 1.0.5
 Summary: Helper library for working with tests
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### Supported Python Versions
```

### Comparing `mom_test_py-1.0.4/README.md` & `mom_test_py-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mom_test_py-1.0.4/mom_test_py/main.py` & `mom_test_py-1.0.5/mom_test_py/main.py`

 * *Files identical despite different names*

### Comparing `mom_test_py-1.0.4/mom_test_py/test_validation.py` & `mom_test_py-1.0.5/mom_test_py/test_validation.py`

 * *Files identical despite different names*

### Comparing `mom_test_py-1.0.4/mom_test_py.egg-info/PKG-INFO` & `mom_test_py-1.0.5/mom_test_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mom-test-py
-Version: 1.0.4
+Version: 1.0.5
 Summary: Helper library for working with tests
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### Supported Python Versions
```

