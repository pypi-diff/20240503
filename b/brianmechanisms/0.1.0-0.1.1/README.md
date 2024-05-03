# Comparing `tmp/brianmechanisms-0.1.0.tar.gz` & `tmp/brianmechanisms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brianmechanisms-0.1.0.tar", last modified: Thu May  2 10:21:09 2024, max compression
+gzip compressed data, was "brianmechanisms-0.1.1.tar", last modified: Thu May  2 12:05:08 2024, max compression
```

## Comparing `brianmechanisms-0.1.0.tar` & `brianmechanisms-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:21:09.323344 brianmechanisms-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-02 10:20:54.000000 brianmechanisms-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-02 10:21:09.323344 brianmechanisms-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 10:20:54.000000 brianmechanisms-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:21:09.323344 brianmechanisms-0.1.0/brianmechanisms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-02 10:21:09.000000 brianmechanisms-0.1.0/brianmechanisms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-02 10:21:09.000000 brianmechanisms-0.1.0/brianmechanisms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:21:09.000000 brianmechanisms-0.1.0/brianmechanisms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:21:09.000000 brianmechanisms-0.1.0/brianmechanisms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 10:20:54.000000 brianmechanisms-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:21:09.323344 brianmechanisms-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:05:08.993390 brianmechanisms-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-02 12:04:57.000000 brianmechanisms-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 12:05:08.993390 brianmechanisms-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 12:04:57.000000 brianmechanisms-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 12:04:57.000000 brianmechanisms-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:05:08.993390 brianmechanisms-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:05:08.989390 brianmechanisms-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:05:08.989390 brianmechanisms-0.1.1/src/brianmechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 12:04:57.000000 brianmechanisms-0.1.1/src/brianmechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-02 12:04:57.000000 brianmechanisms-0.1.1/src/brianmechanisms/appproximateStraightLineMechanism1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:05:08.993390 brianmechanisms-0.1.1/src/brianmechanisms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 12:05:08.000000 brianmechanisms-0.1.1/src/brianmechanisms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 12:05:08.000000 brianmechanisms-0.1.1/src/brianmechanisms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:05:08.000000 brianmechanisms-0.1.1/src/brianmechanisms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 12:05:08.000000 brianmechanisms-0.1.1/src/brianmechanisms.egg-info/top_level.txt
```

### Comparing `brianmechanisms-0.1.0/LICENSE` & `brianmechanisms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.0/PKG-INFO` & `brianmechanisms-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Issues, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
+Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `brianmechanisms-0.1.0/README.md` & `brianmechanisms-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.0/brianmechanisms.egg-info/PKG-INFO` & `brianmechanisms-0.1.1/src/brianmechanisms.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Issues, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
+Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

