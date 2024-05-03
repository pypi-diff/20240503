# Comparing `tmp/beetl-0.4.5.tar.gz` & `tmp/beetl-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.4.5.tar", last modified: Fri May  3 10:53:29 2024, max compression
+gzip compressed data, was "beetl-0.4.6.tar", last modified: Fri May  3 12:44:09 2024, max compression
```

## Comparing `beetl-0.4.5.tar` & `beetl-0.4.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 10:53:29.855733 beetl-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-03 10:52:44.000000 beetl-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:53:29.855733 beetl-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 10:52:44.000000 beetl-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.851734 beetl-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.851734 beetl-0.4.5/src/beetl/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/beetl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/src/beetl/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/sqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/src/beetl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/src/beetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.434563 beetl-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 12:44:09.434563 beetl-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-03 12:43:35.000000 beetl-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:44:09.434563 beetl-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 12:43:35.000000 beetl-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.426563 beetl-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.4.5/PKG-INFO` & `beetl-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.5
+Version: 0.4.6
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.5/README.md` & `beetl-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/setup.py` & `beetl-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/__version__.py` & `beetl-0.4.6/src/beetl/__version__.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/beetl.py` & `beetl-0.4.6/src/beetl/beetl.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/config.py` & `beetl-0.4.6/src/beetl/config.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/faker.py` & `beetl-0.4.6/src/beetl/sources/faker.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/interface.py` & `beetl-0.4.6/src/beetl/sources/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/itop.py` & `beetl-0.4.6/src/beetl/sources/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/mongodb.py` & `beetl-0.4.6/src/beetl/sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/mysql.py` & `beetl-0.4.6/src/beetl/sources/mysql.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/postgres.py` & `beetl-0.4.6/src/beetl/sources/postgres.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/rest.py` & `beetl-0.4.6/src/beetl/sources/rest.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/sqlserver.py` & `beetl-0.4.6/src/beetl/sources/sqlserver.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/sources/static.py` & `beetl-0.4.6/src/beetl/sources/static.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/frames.py` & `beetl-0.4.6/src/beetl/transformers/frames.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/integer.py` & `beetl-0.4.6/src/beetl/transformers/integer.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/interface.py` & `beetl-0.4.6/src/beetl/transformers/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/itop.py` & `beetl-0.4.6/src/beetl/transformers/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/misc.py` & `beetl-0.4.6/src/beetl/transformers/misc.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/regex.py` & `beetl-0.4.6/src/beetl/transformers/regex.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/strings.py` & `beetl-0.4.6/src/beetl/transformers/strings.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl/transformers/structs.py` & `beetl-0.4.6/src/beetl/transformers/structs.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.5/src/beetl.egg-info/PKG-INFO` & `beetl-0.4.6/src/beetl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.5
+Version: 0.4.6
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.5/src/beetl.egg-info/SOURCES.txt` & `beetl-0.4.6/src/beetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

