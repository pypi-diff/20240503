# Comparing `tmp/fortiedr-3.6.1.tar.gz` & `tmp/fortiedr-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortiedr-3.6.1.tar", last modified: Fri May  3 20:02:14 2024, max compression
+gzip compressed data, was "fortiedr-3.6.3.tar", last modified: Fri May  3 20:19:59 2024, max compression
```

## Comparing `fortiedr-3.6.1.tar` & `fortiedr-3.6.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:02:14.715087 fortiedr-3.6.1/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1070 2024-05-03 20:00:35.000000 fortiedr-3.6.1/LICENSE
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       61 2024-05-03 20:00:35.000000 fortiedr-3.6.1/MANIFEST.in
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2730 2024-05-03 20:02:14.715087 fortiedr-3.6.1/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     2117 2024-05-03 20:00:35.000000 fortiedr-3.6.1/README.md
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:02:14.715087 fortiedr-3.6.1/fortiedr/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      930 2024-05-03 20:00:35.000000 fortiedr-3.6.1/fortiedr/__init__.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1633 2024-05-03 20:00:35.000000 fortiedr-3.6.1/fortiedr/auth.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     4311 2024-05-03 20:00:35.000000 fortiedr-3.6.1/fortiedr/connector.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)   241312 2024-05-03 20:00:35.000000 fortiedr-3.6.1/fortiedr/fortiedr.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:02:14.715087 fortiedr-3.6.1/fortiedr.egg-info/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2730 2024-05-03 20:02:14.000000 fortiedr-3.6.1/fortiedr.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      279 2024-05-03 20:02:14.000000 fortiedr-3.6.1/fortiedr.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-05-03 20:02:14.000000 fortiedr-3.6.1/fortiedr.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        9 2024-05-03 20:02:14.000000 fortiedr-3.6.1/fortiedr.egg-info/top_level.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      571 2024-05-03 20:00:35.000000 fortiedr-3.6.1/pyproject.toml
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       36 2024-05-03 20:00:35.000000 fortiedr-3.6.1/requirements.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-05-03 20:02:14.715087 fortiedr-3.6.1/setup.cfg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      880 2024-05-03 20:02:09.000000 fortiedr-3.6.1/setup.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:19:59.754229 fortiedr-3.6.3/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1070 2024-05-03 20:00:35.000000 fortiedr-3.6.3/LICENSE
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       62 2024-05-03 20:14:00.000000 fortiedr-3.6.3/MANIFEST.in
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2730 2024-05-03 20:19:59.754229 fortiedr-3.6.3/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     2117 2024-05-03 20:00:35.000000 fortiedr-3.6.3/README.md
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:19:59.754229 fortiedr-3.6.3/fortiedr/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      930 2024-05-03 20:00:35.000000 fortiedr-3.6.3/fortiedr/__init__.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)    21615 2024-05-03 20:00:35.000000 fortiedr-3.6.3/fortiedr/api_parameters.json
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1633 2024-05-03 20:00:35.000000 fortiedr-3.6.3/fortiedr/auth.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4311 2024-05-03 20:00:35.000000 fortiedr-3.6.3/fortiedr/connector.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)   241314 2024-05-03 20:19:20.000000 fortiedr-3.6.3/fortiedr/fortiedr.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:19:59.754229 fortiedr-3.6.3/fortiedr.egg-info/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2730 2024-05-03 20:19:59.000000 fortiedr-3.6.3/fortiedr.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      308 2024-05-03 20:19:59.000000 fortiedr-3.6.3/fortiedr.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-05-03 20:19:59.000000 fortiedr-3.6.3/fortiedr.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        9 2024-05-03 20:19:59.000000 fortiedr-3.6.3/fortiedr.egg-info/top_level.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      571 2024-05-03 20:19:29.000000 fortiedr-3.6.3/pyproject.toml
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       36 2024-05-03 20:00:35.000000 fortiedr-3.6.3/requirements.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-05-03 20:19:59.754229 fortiedr-3.6.3/setup.cfg
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      880 2024-05-03 20:19:25.000000 fortiedr-3.6.3/setup.py
```

### Comparing `fortiedr-3.6.1/LICENSE` & `fortiedr-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.1/PKG-INFO` & `fortiedr-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.1
+Version: 3.6.3
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.1/README.md` & `fortiedr-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.1/fortiedr/__init__.py` & `fortiedr-3.6.3/fortiedr/__init__.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.1/fortiedr/auth.py` & `fortiedr-3.6.3/fortiedr/auth.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.1/fortiedr/connector.py` & `fortiedr-3.6.3/fortiedr/connector.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.1/fortiedr/fortiedr.py` & `fortiedr-3.6.3/fortiedr/fortiedr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import os
 import json
 from typing import BinaryIO
 from fortiedr.auth import Auth as fedrAuth
 from fortiedr.connector import FortiEDR_API_GW
 
-version = 3.6.1
+version = "3.6.3"
 
 fortiedr_connection = None
 
 class ApplicationControl:
 	'''Application Control Rest Api Controller'''
 
 	def get_applications(self, currentPage: int, organization: str, fileName: str = None, path: str = None, signer: str = None, enabled: bool = None, hash: str = None, operatingSystem: str = None, policyIds: list = None, tag: str = None) -> tuple[bool, None]:
```

### Comparing `fortiedr-3.6.1/fortiedr.egg-info/PKG-INFO` & `fortiedr-3.6.3/fortiedr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.1
+Version: 3.6.3
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.1/pyproject.toml` & `fortiedr-3.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fortiedr"
-version = "3.6.1"
+version = "3.6.3"
 authors = [
   { name="Rafael Foster", email="rafaelgfoster@gmail.com" }
 ]
 description = "This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fortiedr-3.6.1/setup.py` & `fortiedr-3.6.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cur_dir = os.path.dirname(__file__)
 
 with open(f"{cur_dir}/requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="fortiedr",
-    version="3.6.1",
+    version="3.6.3",
     description="This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.",
     author="Rafael Foster",
     author_email="rafaelgfoster@gmail.com",
     project_urls={
         "GitHub": "https://github.com/rafaelfoster/fortiedr",
     },
     python_requires=">=3.8",
```

