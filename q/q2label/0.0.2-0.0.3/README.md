# Comparing `tmp/q2label-0.0.2.tar.gz` & `tmp/q2label-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2label-0.0.2.tar", last modified: Fri Apr 26 13:06:18 2024, max compression
+gzip compressed data, was "q2label-0.0.3.tar", last modified: Fri May  3 05:20:09 2024, max compression
```

## Comparing `q2label-0.0.2.tar` & `q2label-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 13:06:18.061847 q2label-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-04-26 12:32:13.000000 q2label-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1634 2024-04-26 13:06:18.060842 q2label-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-04-26 11:31:27.000000 q2label-0.0.2/README.md
--rw-rw-rw-   0        0        0      914 2024-04-26 13:06:04.000000 q2label-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      510 2024-04-14 07:04:04.000000 q2label-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 13:06:18.062842 q2label-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 13:06:18.022717 q2label-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 13:06:18.036715 q2label-0.0.2/src/q2label/
--rw-rw-rw-   0        0        0        0 2024-04-13 07:49:06.000000 q2label-0.0.2/src/q2label/__init__.py
--rw-rw-rw-   0        0        0     1029 2024-04-26 13:01:38.000000 q2label-0.0.2/src/q2label/datalake.py
--rw-rw-rw-   0        0        0      861 2024-04-14 06:48:45.000000 q2label-0.0.2/src/q2label/local.py
--rw-rw-rw-   0        0        0     1501 2024-04-26 13:01:48.000000 q2label-0.0.2/src/q2label/target.py
--rw-rw-rw-   0        0        0      946 2024-04-19 15:06:44.000000 q2label-0.0.2/src/q2label/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 13:06:18.058842 q2label-0.0.2/src/q2label.egg-info/
--rw-rw-rw-   0        0        0     1634 2024-04-26 13:06:17.000000 q2label-0.0.2/src/q2label.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-26 13:06:18.000000 q2label-0.0.2/src/q2label.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 13:06:17.000000 q2label-0.0.2/src/q2label.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      485 2024-04-26 13:06:17.000000 q2label-0.0.2/src/q2label.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 13:06:17.000000 q2label-0.0.2/src/q2label.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 05:20:09.357042 q2label-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-26 12:32:13.000000 q2label-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1605 2024-05-03 05:20:09.353042 q2label-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-04-26 11:31:27.000000 q2label-0.0.3/README.md
+-rw-rw-rw-   0        0        0      914 2024-05-03 05:19:30.000000 q2label-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      496 2024-05-03 05:19:49.000000 q2label-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 05:20:09.358050 q2label-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 05:20:09.258335 q2label-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 05:20:09.299997 q2label-0.0.3/src/q2label/
+-rw-rw-rw-   0        0        0        0 2024-04-13 07:49:06.000000 q2label-0.0.3/src/q2label/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-04-26 13:01:38.000000 q2label-0.0.3/src/q2label/datalake.py
+-rw-rw-rw-   0        0        0      861 2024-04-14 06:48:45.000000 q2label-0.0.3/src/q2label/local.py
+-rw-rw-rw-   0        0        0     1501 2024-04-26 13:01:48.000000 q2label-0.0.3/src/q2label/target.py
+-rw-rw-rw-   0        0        0      946 2024-04-19 15:06:44.000000 q2label-0.0.3/src/q2label/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:20:09.350063 q2label-0.0.3/src/q2label.egg-info/
+-rw-rw-rw-   0        0        0     1605 2024-05-03 05:20:09.000000 q2label-0.0.3/src/q2label.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-03 05:20:09.000000 q2label-0.0.3/src/q2label.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 05:20:09.000000 q2label-0.0.3/src/q2label.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      472 2024-05-03 05:20:09.000000 q2label-0.0.3/src/q2label.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 05:20:09.000000 q2label-0.0.3/src/q2label.egg-info/top_level.txt
```

### Comparing `q2label-0.0.2/LICENSE` & `q2label-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `q2label-0.0.2/PKG-INFO` & `q2label-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2label
-Version: 0.0.2
+Version: 0.0.3
 Summary: Transfer your data to our datalake and integrate in your computer vision pipeline. For more information, go to our website: www.q2label.com.
 Author-email: Erik van der Poel <erikvdpoel@hotmail.com>
 Project-URL: Homepage, https://www.q2label.com
 Keywords: data transfer image labelling
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -29,14 +29,13 @@
 Requires-Dist: msal==1.28.0
 Requires-Dist: msal-extensions==1.1.0
 Requires-Dist: packaging==24.0
 Requires-Dist: portalocker==2.8.2
 Requires-Dist: pycparser==2.22
 Requires-Dist: PyJWT==2.8.0
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: pywin32==306
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: urllib3==2.2.1
 
 Welcome to Q2label!
```

### Comparing `q2label-0.0.2/pyproject.toml` & `q2label-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "q2label"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Erik van der Poel", email="erikvdpoel@hotmail.com" },
 ]
 dynamic = ["dependencies"]
 description = "Transfer your data to our datalake and integrate in your computer vision pipeline. For more information, go to our website: www.q2label.com."
 keywords = ["data transfer image labelling"]
 readme = "README.md"
```

### Comparing `q2label-0.0.2/src/q2label/datalake.py` & `q2label-0.0.3/src/q2label/datalake.py`

 * *Files identical despite different names*

### Comparing `q2label-0.0.2/src/q2label/local.py` & `q2label-0.0.3/src/q2label/local.py`

 * *Files identical despite different names*

### Comparing `q2label-0.0.2/src/q2label/target.py` & `q2label-0.0.3/src/q2label/target.py`

 * *Files identical despite different names*

### Comparing `q2label-0.0.2/src/q2label/utils.py` & `q2label-0.0.3/src/q2label/utils.py`

 * *Files identical despite different names*

### Comparing `q2label-0.0.2/src/q2label.egg-info/PKG-INFO` & `q2label-0.0.3/src/q2label.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2label
-Version: 0.0.2
+Version: 0.0.3
 Summary: Transfer your data to our datalake and integrate in your computer vision pipeline. For more information, go to our website: www.q2label.com.
 Author-email: Erik van der Poel <erikvdpoel@hotmail.com>
 Project-URL: Homepage, https://www.q2label.com
 Keywords: data transfer image labelling
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -29,14 +29,13 @@
 Requires-Dist: msal==1.28.0
 Requires-Dist: msal-extensions==1.1.0
 Requires-Dist: packaging==24.0
 Requires-Dist: portalocker==2.8.2
 Requires-Dist: pycparser==2.22
 Requires-Dist: PyJWT==2.8.0
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: pywin32==306
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: urllib3==2.2.1
 
 Welcome to Q2label!
```

