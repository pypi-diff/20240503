# Comparing `tmp/nmk-proto-0.5.2.tar.gz` & `tmp/nmk_proto-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-proto-0.5.2.tar", last modified: Tue Feb  6 07:45:27 2024, max compression
+gzip compressed data, was "nmk_proto-0.5.3.tar", last modified: Fri May  3 12:07:10 2024, max compression
```

## Comparing `nmk-proto-0.5.2.tar` & `nmk_proto-0.5.3.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:45:27.519003 nmk-proto-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-06 07:45:27.519003 nmk-proto-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-06 07:45:24.000000 nmk-proto-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-06 07:45:27.519003 nmk-proto-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-06 07:45:24.000000 nmk-proto-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:45:27.515003 nmk-proto-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:45:27.519003 nmk-proto-0.5.2/src/nmk_proto/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/badges.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/files.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/path.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/plugin-defs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/python.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:45:27.519003 nmk-proto-0.5.2/src/nmk_proto/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/templates/init.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/templates/python_package_data.cfg.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-06 07:44:56.000000 nmk-proto-0.5.2/src/nmk_proto/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:45:27.519003 nmk-proto-0.5.2/src/nmk_proto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-06 07:45:27.000000 nmk-proto-0.5.2/src/nmk_proto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-06 07:45:27.000000 nmk-proto-0.5.2/src/nmk_proto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 07:45:27.000000 nmk-proto-0.5.2/src/nmk_proto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-06 07:45:27.000000 nmk-proto-0.5.2/src/nmk_proto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-06 07:45:27.000000 nmk-proto-0.5.2/src/nmk_proto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:07:10.497648 nmk_proto-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-03 12:07:10.497648 nmk_proto-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-03 12:07:07.000000 nmk_proto-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-03 12:07:10.497648 nmk_proto-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 12:07:07.000000 nmk_proto-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:07:10.493648 nmk_proto-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:07:10.493648 nmk_proto-0.5.3/src/nmk_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/badges.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/files.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/python.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:07:10.497648 nmk_proto-0.5.3/src/nmk_proto/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/templates/init.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/templates/python_package_data.cfg.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-03 12:06:39.000000 nmk_proto-0.5.3/src/nmk_proto/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:07:10.497648 nmk_proto-0.5.3/src/nmk_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-03 12:07:10.000000 nmk_proto-0.5.3/src/nmk_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 12:07:10.000000 nmk_proto-0.5.3/src/nmk_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:07:10.000000 nmk_proto-0.5.3/src/nmk_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-03 12:07:10.000000 nmk_proto-0.5.3/src/nmk_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 12:07:10.000000 nmk_proto-0.5.3/src/nmk_proto.egg-info/top_level.txt
```

### Comparing `nmk-proto-0.5.2/LICENSE` & `nmk_proto-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/PKG-INFO` & `nmk_proto-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmk-proto
-Version: 0.5.2
+Version: 0.5.3
 Summary: Code generation plugin from proto files for nmk build system
 Home-page: https://github.com/dynod/nmk-proto
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nmk-proto-0.5.2/README.md` & `nmk_proto-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/setup.cfg` & `nmk_proto-0.5.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk-proto
 author = The dynod project
 maintainer = The dynod project
-version = 0.5.2
+version = 0.5.3
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `nmk-proto-0.5.2/src/nmk_proto/__init__.py` & `nmk_proto-0.5.3/src/nmk_proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/src/nmk_proto/files.py` & `nmk_proto-0.5.3/src/nmk_proto/files.py`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/src/nmk_proto/files.yml` & `nmk_proto-0.5.3/src/nmk_proto/files.yml`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/src/nmk_proto/plugin-defs.yml` & `nmk_proto-0.5.3/src/nmk_proto/plugin.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Proto plugin definition
 refs:
-    - path.yml    # Python path contrib
+    - pip://nmk-base!plugin.yml
     - files.yml   # Proto files config
     - python.yml  # Code generation for Python
     - badges.yml  # Badges generation
 
 # Extra config
 config:
```

### Comparing `nmk-proto-0.5.2/src/nmk_proto/python.py` & `nmk_proto-0.5.3/src/nmk_proto/python.py`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/src/nmk_proto/python.yml` & `nmk_proto-0.5.3/src/nmk_proto/python.yml`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/src/nmk_proto/utils.py` & `nmk_proto-0.5.3/src/nmk_proto/utils.py`

 * *Files identical despite different names*

### Comparing `nmk-proto-0.5.2/src/nmk_proto.egg-info/PKG-INFO` & `nmk_proto-0.5.3/src/nmk_proto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmk-proto
-Version: 0.5.2
+Version: 0.5.3
 Summary: Code generation plugin from proto files for nmk build system
 Home-page: https://github.com/dynod/nmk-proto
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nmk-proto-0.5.2/src/nmk_proto.egg-info/SOURCES.txt` & `nmk_proto-0.5.3/src/nmk_proto.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 README.md
 setup.cfg
 setup.py
 src/nmk_proto/__init__.py
 src/nmk_proto/badges.yml
 src/nmk_proto/files.py
 src/nmk_proto/files.yml
-src/nmk_proto/path.yml
-src/nmk_proto/plugin-defs.yml
 src/nmk_proto/plugin.yml
 src/nmk_proto/python.py
 src/nmk_proto/python.yml
 src/nmk_proto/utils.py
 src/nmk_proto.egg-info/PKG-INFO
 src/nmk_proto.egg-info/SOURCES.txt
 src/nmk_proto.egg-info/dependency_links.txt
```

