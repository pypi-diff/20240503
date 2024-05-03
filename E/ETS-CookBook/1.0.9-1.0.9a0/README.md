# Comparing `tmp/ETS_CookBook-1.0.9.tar.gz` & `tmp/ETS_CookBook-1.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ETS_CookBook-1.0.9.tar", last modified: Sat Feb 17 19:18:11 2024, max compression
+gzip compressed data, was "ETS_CookBook-1.0.9a0.tar", last modified: Sat Feb 17 19:25:07 2024, max compression
```

## Comparing `ETS_CookBook-1.0.9.tar` & `ETS_CookBook-1.0.9a0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 19:18:11.000151 ETS_CookBook-1.0.9/
--rw-rw-rw-   0        0        0       17 2023-10-05 09:13:14.000000 ETS_CookBook-1.0.9/.gitignore
--rw-rw-rw-   0        0        0    11536 2023-02-16 14:24:48.000000 ETS_CookBook-1.0.9/LICENCE
--rw-rw-rw-   0        0        0    11357 2023-10-06 10:39:20.000000 ETS_CookBook-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     2078 2023-08-07 12:21:09.000000 ETS_CookBook-1.0.9/MOPO_logo_main.svg
--rw-rw-rw-   0        0        0     8321 2024-02-17 19:18:10.998152 ETS_CookBook-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5869 2024-02-17 19:16:42.000000 ETS_CookBook-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-02-17 19:18:10.906148 ETS_CookBook-1.0.9/dist/
--rw-rw-rw-   0        0        0    22918 2023-10-06 12:14:22.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.4-py3-none-any.whl
--rw-rw-rw-   0        0        0   155964 2023-10-06 12:14:00.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.4.tar.gz
--rw-rw-rw-   0        0        0    23065 2024-01-08 18:00:20.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.5-py3-none-any.whl
--rw-rw-rw-   0        0        0   247629 2024-01-08 17:59:58.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.5.tar.gz
--rw-rw-rw-   0        0        0    25147 2024-01-25 23:00:43.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.6-py3-none-any.whl
--rw-rw-rw-   0        0        0   520273 2024-01-25 23:00:25.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.6.tar.gz
--rw-rw-rw-   0        0        0    25530 2024-01-31 13:46:49.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.7-py3-none-any.whl
--rw-rw-rw-   0        0        0  1066355 2024-01-31 13:46:31.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.7.tar.gz
--rw-rw-rw-   0        0        0    25548 2024-02-02 09:50:43.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.8-py3-none-any.whl
--rw-rw-rw-   0        0        0  2157003 2024-02-02 09:50:26.000000 ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.8.tar.gz
--rw-rw-rw-   0        0        0    55634 2023-02-15 12:46:32.000000 ETS_CookBook-1.0.9/eu-emblem-low-res.jpg
--rw-rw-rw-   0        0        0      690 2024-02-17 19:17:22.000000 ETS_CookBook-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0     1052 2024-01-31 13:46:01.000000 ETS_CookBook-1.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-17 19:18:11.001152 ETS_CookBook-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-17 19:18:10.655151 ETS_CookBook-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-02-17 19:18:10.934150 ETS_CookBook-1.0.9/src/ETS_CookBook/
--rw-rw-rw-   0        0        0    51518 2024-02-17 19:16:30.000000 ETS_CookBook-1.0.9/src/ETS_CookBook/ETS_CookBook.py
--rw-rw-rw-   0        0        0        0 2023-10-06 11:35:41.000000 ETS_CookBook-1.0.9/src/ETS_CookBook/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-17 19:18:10.996152 ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/
--rw-rw-rw-   0        0        0     8321 2024-02-17 19:18:10.000000 ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2024-02-17 19:18:10.000000 ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 19:18:10.000000 ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      992 2024-02-17 19:18:10.000000 ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-17 19:18:10.000000 ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-17 19:25:07.557358 ETS_CookBook-1.0.9a0/
+-rw-rw-rw-   0        0        0       17 2023-10-05 09:13:14.000000 ETS_CookBook-1.0.9a0/.gitignore
+-rw-rw-rw-   0        0        0    11536 2023-02-16 14:24:48.000000 ETS_CookBook-1.0.9a0/LICENCE
+-rw-rw-rw-   0        0        0    11357 2023-10-06 10:39:20.000000 ETS_CookBook-1.0.9a0/LICENSE
+-rw-rw-rw-   0        0        0     2078 2023-08-07 12:21:09.000000 ETS_CookBook-1.0.9a0/MOPO_logo_main.svg
+-rw-rw-rw-   0        0        0     8323 2024-02-17 19:25:07.555358 ETS_CookBook-1.0.9a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5869 2024-02-17 19:16:42.000000 ETS_CookBook-1.0.9a0/README.md
+drwxrwxrwx   0        0        0        0 2024-02-17 19:25:07.476370 ETS_CookBook-1.0.9a0/dist/
+-rw-rw-rw-   0        0        0    22918 2023-10-06 12:14:22.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.4-py3-none-any.whl
+-rw-rw-rw-   0        0        0   155964 2023-10-06 12:14:00.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.4.tar.gz
+-rw-rw-rw-   0        0        0    23065 2024-01-08 18:00:20.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.5-py3-none-any.whl
+-rw-rw-rw-   0        0        0   247629 2024-01-08 17:59:58.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.5.tar.gz
+-rw-rw-rw-   0        0        0    25147 2024-01-25 23:00:43.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.6-py3-none-any.whl
+-rw-rw-rw-   0        0        0   520273 2024-01-25 23:00:25.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.6.tar.gz
+-rw-rw-rw-   0        0        0    25530 2024-01-31 13:46:49.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.7-py3-none-any.whl
+-rw-rw-rw-   0        0        0  1066355 2024-01-31 13:46:31.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.7.tar.gz
+-rw-rw-rw-   0        0        0    25548 2024-02-02 09:50:43.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.8-py3-none-any.whl
+-rw-rw-rw-   0        0        0  2157003 2024-02-02 09:50:26.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.8.tar.gz
+-rw-rw-rw-   0        0        0    25856 2024-02-17 19:18:35.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.9-py3-none-any.whl
+-rw-rw-rw-   0        0        0  4339994 2024-02-17 19:18:11.000000 ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.9.tar.gz
+-rw-rw-rw-   0        0        0    55634 2023-02-15 12:46:32.000000 ETS_CookBook-1.0.9a0/eu-emblem-low-res.jpg
+-rw-rw-rw-   0        0        0      692 2024-02-17 19:24:12.000000 ETS_CookBook-1.0.9a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1052 2024-01-31 13:46:01.000000 ETS_CookBook-1.0.9a0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-02-17 19:25:07.557358 ETS_CookBook-1.0.9a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-17 19:25:07.261359 ETS_CookBook-1.0.9a0/src/
+drwxrwxrwx   0        0        0        0 2024-02-17 19:25:07.503358 ETS_CookBook-1.0.9a0/src/ETS_CookBook/
+-rw-rw-rw-   0        0        0    51513 2024-02-17 19:23:58.000000 ETS_CookBook-1.0.9a0/src/ETS_CookBook/ETS_CookBook.py
+-rw-rw-rw-   0        0        0        0 2023-10-06 11:35:41.000000 ETS_CookBook-1.0.9a0/src/ETS_CookBook/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-17 19:25:07.553357 ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/
+-rw-rw-rw-   0        0        0     8323 2024-02-17 19:25:07.000000 ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      802 2024-02-17 19:25:07.000000 ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-17 19:25:07.000000 ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      992 2024-02-17 19:25:07.000000 ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-02-17 19:25:07.000000 ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/top_level.txt
```

### Comparing `ETS_CookBook-1.0.9/LICENCE` & `ETS_CookBook-1.0.9a0/LICENCE`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/LICENSE` & `ETS_CookBook-1.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/MOPO_logo_main.svg` & `ETS_CookBook-1.0.9a0/MOPO_logo_main.svg`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/PKG-INFO` & `ETS_CookBook-1.0.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ETS_CookBook
-Version: 1.0.9
+Version: 1.0.9a0
 Summary: The ETS (TNO) CookBook of useful Python Scripts
 Author-email: Omar Usmani <Omar.Usmani@TNO.nl>
 Project-URL: Homepage, https://github.com/TNO/ETS_CookBook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ETS_CookBook-1.0.9/README.md` & `ETS_CookBook-1.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.4-py3-none-any.whl` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.4.tar.gz` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.5-py3-none-any.whl` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.5.tar.gz` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.5.tar.gz`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.6-py3-none-any.whl` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.6-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.6.tar.gz` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.6.tar.gz`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.7-py3-none-any.whl` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.7.tar.gz` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.7.tar.gz`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.8-py3-none-any.whl` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/dist/ETS_CookBook-1.0.8.tar.gz` & `ETS_CookBook-1.0.9a0/dist/ETS_CookBook-1.0.8.tar.gz`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/eu-emblem-low-res.jpg` & `ETS_CookBook-1.0.9a0/eu-emblem-low-res.jpg`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/pyproject.toml` & `ETS_CookBook-1.0.9a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ['setuptools', 'setuptools-scm']
 build-backend = 'setuptools.build_meta'
 
 
 
 [project]
 name = 'ETS_CookBook'
-version = '1.0.9'
+version = '1.0.9.a'
 authors = [
   { name='Omar Usmani', email='Omar.Usmani@TNO.nl' },
 ]
 description = 'The ETS (TNO) CookBook of useful Python Scripts'
 readme = 'README.md'
 requires-python = '>=3.11'
 classifiers = [
```

### Comparing `ETS_CookBook-1.0.9/requirements.txt` & `ETS_CookBook-1.0.9a0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ETS_CookBook-1.0.9/src/ETS_CookBook/ETS_CookBook.py` & `ETS_CookBook-1.0.9a0/src/ETS_CookBook/ETS_CookBook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1328,15 +1328,15 @@
 def get_rgb_255_code_string(color_name, parameters):
     '''
     Creates a string with rgb values (0-255),
     rgb(111, 233, 66)
     This is used for plotly.
     '''
     # We convert the color name to an RGB (0-255)
-    rgb_255 = 255 * cook.get_rgb_from_name(color_name, parameters)
+    rgb_255 = 255 * get_rgb_from_name(color_name, parameters)
     # We make it a string (and remove the 0 decimal via int conversion)
     rgb_255 = list(map(str, map(int, rgb_255)))
     rgb_255_code_string = f'({", ".join(rgb_255)})'
 
     return rgb_255_code_string
```

### Comparing `ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/PKG-INFO` & `ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ETS_CookBook
-Version: 1.0.9
+Version: 1.0.9a0
 Summary: The ETS (TNO) CookBook of useful Python Scripts
 Author-email: Omar Usmani <Omar.Usmani@TNO.nl>
 Project-URL: Homepage, https://github.com/TNO/ETS_CookBook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/SOURCES.txt` & `ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 dist/ETS_CookBook-1.0.5.tar.gz
 dist/ETS_CookBook-1.0.6-py3-none-any.whl
 dist/ETS_CookBook-1.0.6.tar.gz
 dist/ETS_CookBook-1.0.7-py3-none-any.whl
 dist/ETS_CookBook-1.0.7.tar.gz
 dist/ETS_CookBook-1.0.8-py3-none-any.whl
 dist/ETS_CookBook-1.0.8.tar.gz
+dist/ETS_CookBook-1.0.9-py3-none-any.whl
+dist/ETS_CookBook-1.0.9.tar.gz
 src/ETS_CookBook/ETS_CookBook.py
 src/ETS_CookBook/__init__.py
 src/ETS_CookBook.egg-info/PKG-INFO
 src/ETS_CookBook.egg-info/SOURCES.txt
 src/ETS_CookBook.egg-info/dependency_links.txt
 src/ETS_CookBook.egg-info/requires.txt
 src/ETS_CookBook.egg-info/top_level.txt
```

### Comparing `ETS_CookBook-1.0.9/src/ETS_CookBook.egg-info/requires.txt` & `ETS_CookBook-1.0.9a0/src/ETS_CookBook.egg-info/requires.txt`

 * *Files identical despite different names*

