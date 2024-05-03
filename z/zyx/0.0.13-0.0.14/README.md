# Comparing `tmp/zyx-0.0.13.tar.gz` & `tmp/zyx-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyx-0.0.13.tar", last modified: Wed May  1 03:15:18 2024, max compression
+gzip compressed data, was "zyx-0.0.14.tar", last modified: Fri May  3 04:07:31 2024, max compression
```

## Comparing `zyx-0.0.13.tar` & `zyx-0.0.14.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.498622 zyx-0.0.13/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-01 03:15:18.498622 zyx-0.0.13/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1293 2024-05-01 03:08:18.000000 zyx-0.0.13/README.md
--rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-01 03:15:18.498622 zyx-0.0.13/setup.cfg
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1122 2024-05-01 03:14:30.000000 zyx-0.0.13/setup.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.493622 zyx-0.0.13/src/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.494622 zyx-0.0.13/src/zyx/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 01:28:40.000000 zyx-0.0.13/src/zyx/__cli__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      225 2024-05-01 03:15:10.000000 zyx-0.0.13/src/zyx/__init__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.495622 zyx-0.0.13/src/zyx/core/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:11:43.000000 zyx-0.0.13/src/zyx/core/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-01 02:06:18.000000 zyx-0.0.13/src/zyx/core/chat.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 01:18:32.000000 zyx-0.0.13/src/zyx/core/input.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 01:31:09.000000 zyx-0.0.13/src/zyx/core/lightning.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 02:08:43.000000 zyx-0.0.13/src/zyx/core/loaders.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1976 2024-05-01 02:58:35.000000 zyx-0.0.13/src/zyx/core/print.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 01:34:11.000000 zyx-0.0.13/src/zyx/core/validate_path.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 01:46:21.000000 zyx-0.0.13/src/zyx/core/validate_type.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.497622 zyx-0.0.13/src/zyx/functions/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 02:59:15.000000 zyx-0.0.13/src/zyx/functions/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 01:40:07.000000 zyx-0.0.13/src/zyx/functions/create_id.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 01:35:35.000000 zyx-0.0.13/src/zyx/functions/generate_name.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 01:43:00.000000 zyx-0.0.13/src/zyx/functions/get_system_info.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.497622 zyx-0.0.13/src/zyx/jupyter/
--rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 01:35:07.000000 zyx-0.0.13/src/zyx/jupyter/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 01:03:56.000000 zyx-0.0.13/src/zyx/jupyter/tailwind.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.497622 zyx-0.0.13/src/zyx/text/
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 01:17:17.000000 zyx-0.0.13/src/zyx/text/__chunker__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 02:01:55.000000 zyx-0.0.13/src/zyx/text/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-01 01:32:22.000000 zyx-0.0.13/src/zyx/text/__read_doc__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:15:18.497622 zyx-0.0.13/src/zyx.egg-info/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-01 03:15:18.000000 zyx-0.0.13/src/zyx.egg-info/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      716 2024-05-01 03:15:18.000000 zyx-0.0.13/src/zyx.egg-info/SOURCES.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-01 03:15:18.000000 zyx-0.0.13/src/zyx.egg-info/dependency_links.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-01 03:15:18.000000 zyx-0.0.13/src/zyx.egg-info/entry_points.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)      104 2024-05-01 03:15:18.000000 zyx-0.0.13/src/zyx.egg-info/requires.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-01 03:15:18.000000 zyx-0.0.13/src/zyx.egg-info/top_level.txt
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.184996 zyx-0.0.14/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.179995 zyx-0.0.14/.zyx/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.179995 zyx-0.0.14/.zyx/src/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.180995 zyx-0.0.14/.zyx/src/zyx/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/__cli__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      225 2024-05-01 03:37:03.000000 zyx-0.0.14/.zyx/src/zyx/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.182995 zyx-0.0.14/.zyx/src/zyx/core/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-02 05:26:48.000000 zyx-0.0.14/.zyx/src/zyx/core/chat.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/input.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/lightning.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/loaders.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1976 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/print.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/validate_path.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/validate_type.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.183996 zyx-0.0.14/.zyx/src/zyx/functions/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/create_id.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/generate_name.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/get_system_info.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.183996 zyx-0.0.14/.zyx/src/zyx/jupyter/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/jupyter/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/jupyter/tailwind.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.184996 zyx-0.0.14/.zyx/src/zyx/text/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/text/__chunker__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/text/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-02 01:36:57.000000 zyx-0.0.14/.zyx/src/zyx/text/__read_doc__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.184996 zyx-0.0.14/.zyx/src/zyx.egg-info/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      841 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/entry_points.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      104 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/requires.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/top_level.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-03 04:07:31.184996 zyx-0.0.14/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      667 2024-05-01 04:05:03.000000 zyx-0.0.14/README.md
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-03 04:07:31.184996 zyx-0.0.14/setup.cfg
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1191 2024-05-03 04:07:20.000000 zyx-0.0.14/setup.py
```

### Comparing `zyx-0.0.13/setup.py` & `zyx-0.0.14/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     author = "Hammad Saeed",
     author_email="hammad@supportvectors.com",
 
     name = 'zyx',
-    version = '0.0.13',
-    packages = find_packages(where='src'),
-    package_dir = {'': 'src'},
+    version = '0.0.14',
+    packages = find_packages(where='.zyx/src'),
+    package_dir = {'': '.zyx/src'},
 
     python_requires = '>=3.8',
 
+    package_data={
+        '': ['vendor/*.whl'],  
+    },
+
     install_requires = [
         # Art | ASCII Art
         'art',
 
         # IPython | Interactive Python
         'ipython',
```

### Comparing `zyx-0.0.13/src/zyx/core/chat.py` & `zyx-0.0.14/.zyx/src/zyx/core/chat.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/core/input.py` & `zyx-0.0.14/.zyx/src/zyx/core/input.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/core/lightning.py` & `zyx-0.0.14/.zyx/src/zyx/core/lightning.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/core/loaders.py` & `zyx-0.0.14/.zyx/src/zyx/core/loaders.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/core/print.py` & `zyx-0.0.14/.zyx/src/zyx/core/print.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/core/validate_path.py` & `zyx-0.0.14/.zyx/src/zyx/core/validate_path.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/core/validate_type.py` & `zyx-0.0.14/.zyx/src/zyx/core/validate_type.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/functions/__init__.py` & `zyx-0.0.14/.zyx/src/zyx/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/functions/create_id.py` & `zyx-0.0.14/.zyx/src/zyx/functions/create_id.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/functions/generate_name.py` & `zyx-0.0.14/.zyx/src/zyx/functions/generate_name.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/functions/get_system_info.py` & `zyx-0.0.14/.zyx/src/zyx/functions/get_system_info.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/jupyter/tailwind.py` & `zyx-0.0.14/.zyx/src/zyx/jupyter/tailwind.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/text/__chunker__.py` & `zyx-0.0.14/.zyx/src/zyx/text/__chunker__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.13/src/zyx/text/__read_doc__.py` & `zyx-0.0.14/.zyx/src/zyx/text/__read_doc__.py`

 * *Files identical despite different names*

