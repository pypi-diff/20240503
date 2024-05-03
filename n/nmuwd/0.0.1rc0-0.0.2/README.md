# Comparing `tmp/nmuwd-0.0.1rc0.tar.gz` & `tmp/nmuwd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmuwd-0.0.1rc0.tar", last modified: Fri May  3 05:27:50 2024, max compression
+gzip compressed data, was "nmuwd-0.0.2.tar", last modified: Fri May  3 05:35:45 2024, max compression
```

## Comparing `nmuwd-0.0.1rc0.tar` & `nmuwd-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:27:50.895246 nmuwd-0.0.1rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 05:27:50.895246 nmuwd-0.0.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:27:50.891246 nmuwd-0.0.1rc0/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/backend/persister.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/backend/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/backend/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/backend/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:27:50.891246 nmuwd-0.0.1rc0/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/frontend/unifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:27:50.895246 nmuwd-0.0.1rc0/nmuwd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 05:27:50.000000 nmuwd-0.0.1rc0/nmuwd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 05:27:50.000000 nmuwd-0.0.1rc0/nmuwd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:27:50.000000 nmuwd-0.0.1rc0/nmuwd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 05:27:50.000000 nmuwd-0.0.1rc0/nmuwd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 05:27:50.000000 nmuwd-0.0.1rc0/nmuwd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:27:50.895246 nmuwd-0.0.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-03 05:27:47.000000 nmuwd-0.0.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.290938 nmuwd-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 05:35:40.000000 nmuwd-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 05:35:45.290938 nmuwd-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 05:35:40.000000 nmuwd-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.286938 nmuwd-0.0.2/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/persister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 05:35:40.000000 nmuwd-0.0.2/backend/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.286938 nmuwd-0.0.2/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:40.000000 nmuwd-0.0.2/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-03 05:35:40.000000 nmuwd-0.0.2/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-03 05:35:40.000000 nmuwd-0.0.2/frontend/unifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:35:45.290938 nmuwd-0.0.2/nmuwd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 05:35:45.000000 nmuwd-0.0.2/nmuwd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:35:45.290938 nmuwd-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-03 05:35:40.000000 nmuwd-0.0.2/setup.py
```

### Comparing `nmuwd-0.0.1rc0/LICENSE` & `nmuwd-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/backend/config.py` & `nmuwd-0.0.2/backend/config.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/backend/persister.py` & `nmuwd-0.0.2/backend/persister.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/backend/record.py` & `nmuwd-0.0.2/backend/record.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/backend/source.py` & `nmuwd-0.0.2/backend/source.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/backend/transformer.py` & `nmuwd-0.0.2/backend/transformer.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/frontend/cli.py` & `nmuwd-0.0.2/frontend/cli.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/frontend/unifier.py` & `nmuwd-0.0.2/frontend/unifier.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.1rc0/setup.py` & `nmuwd-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nmuwd",
-    version="0.0.1c",
+    version="0.0.2",
     author="Jake Ross",
     description="New Mexico Water Data Integration Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PychronLabsLLC/pcm",
     classifiers=[
         "Programming Language :: Python :: 3",
```

