# Comparing `tmp/gen_wrappers-0.2.0.tar.gz` & `tmp/gen_wrappers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.2.0.tar", last modified: Fri May  3 18:22:15 2024, max compression
+gzip compressed data, was "gen_wrappers-0.2.1.tar", last modified: Fri May  3 18:57:39 2024, max compression
```

## Comparing `gen_wrappers-0.2.0.tar` & `gen_wrappers-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.375227 gen_wrappers-0.2.0/
--rw-rw-rw-   0        0        0      823 2024-05-03 18:22:15.373127 gen_wrappers-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.301812 gen_wrappers-0.2.0/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.0/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.319567 gen_wrappers-0.2.0/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.0/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.2.0/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4184 2024-05-02 20:52:05.000000 gen_wrappers-0.2.0/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.330583 gen_wrappers-0.2.0/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.0/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.0/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.2.0/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.0/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.338575 gen_wrappers-0.2.0/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.0/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9441 2024-05-02 21:06:52.000000 gen_wrappers-0.2.0/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.2.0/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.347480 gen_wrappers-0.2.0/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.0/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.0/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.0/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.0/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:22:15.371056 gen_wrappers-0.2.0/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 18:22:15.000000 gen_wrappers-0.2.0/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 18:22:15.376227 gen_wrappers-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-03 18:22:12.000000 gen_wrappers-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:57:39.508583 gen_wrappers-0.2.1/
+-rw-rw-rw-   0        0        0      847 2024-05-03 18:57:39.506577 gen_wrappers-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 18:57:39.414417 gen_wrappers-0.2.1/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.1/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:57:39.426524 gen_wrappers-0.2.1/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.1/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.2.1/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4184 2024-05-02 20:52:05.000000 gen_wrappers-0.2.1/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.1/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:57:39.435472 gen_wrappers-0.2.1/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.1/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.2.1/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.1/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     2941 2024-05-03 18:57:36.000000 gen_wrappers-0.2.1/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.1/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:57:39.446938 gen_wrappers-0.2.1/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.1/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9441 2024-05-02 21:06:52.000000 gen_wrappers-0.2.1/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.2.1/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.1/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:57:39.457868 gen_wrappers-0.2.1/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.1/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.1/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.1/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.1/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:57:39.504578 gen_wrappers-0.2.1/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-03 18:57:39.000000 gen_wrappers-0.2.1/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-03 18:57:39.000000 gen_wrappers-0.2.1/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 18:57:39.000000 gen_wrappers-0.2.1/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-03 18:57:39.000000 gen_wrappers-0.2.1/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 18:57:39.000000 gen_wrappers-0.2.1/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 18:57:39.509579 gen_wrappers-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-03 18:57:36.000000 gen_wrappers-0.2.1/setup.py
```

### Comparing `gen_wrappers-0.2.0/PKG-INFO` & `gen_wrappers-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,7 +15,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
 Requires-Dist: requests
 Requires-Dist: pydantic
+Requires-Dist: fastapi
```

### Comparing `gen_wrappers-0.2.0/creator/auto/creator_auto.py` & `gen_wrappers-0.2.1/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/auto/request_auto.py` & `gen_wrappers-0.2.1/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/auto/response_auto.py` & `gen_wrappers-0.2.1/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/base/base_app.py` & `gen_wrappers-0.2.1/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/base/base_request.py` & `gen_wrappers-0.2.1/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.2.1/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.2.1/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.2.1/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.2.1/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.2.1/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.2.1/gen_wrappers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,7 +15,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
 Requires-Dist: requests
 Requires-Dist: pydantic
+Requires-Dist: fastapi
```

### Comparing `gen_wrappers-0.2.0/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.2.1/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.0/setup.py` & `gen_wrappers-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.2.0',
+    version='0.2.1',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
         "httpx",
         "requests",
-        "pydantic"
+        "pydantic",
+        "fastapi"
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

