# Comparing `tmp/clappform-integrations-1.0.8.tar.gz` & `tmp/clappform-integrations-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-integrations-1.0.8.tar", last modified: Thu Dec 21 15:02:01 2023, max compression
+gzip compressed data, was "clappform-integrations-1.0.9.tar", last modified: Fri Dec 22 09:03:38 2023, max compression
```

## Comparing `clappform-integrations-1.0.8.tar` & `clappform-integrations-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-21 15:01:47.000000 clappform-integrations-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-21 15:01:47.000000 clappform-integrations-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-12-21 15:01:47.000000 clappform-integrations-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/src/clappform_integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-21 15:01:47.000000 clappform-integrations-1.0.8/src/clappform_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itris/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itris/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itris/src/clappform_itris/
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2023-12-21 15:01:49.000000 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itris/src/clappform_itris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itsperfect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itsperfect/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itsperfect/src/clappform_itsperfect/
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2023-12-21 15:01:49.000000 clappform-integrations-1.0.8/src/clappform_integrations/clappform_itsperfect/src/clappform_itsperfect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_rudholm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_rudholm/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_rudholm/src/clappform_rudholm/
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2023-12-21 15:01:49.000000 clappform-integrations-1.0.8/src/clappform_integrations/clappform_rudholm/src/clappform_rudholm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_transus/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.433914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_transus/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/src/clappform_integrations/clappform_transus/src/clappform_transus/
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-12-21 15:01:49.000000 clappform-integrations-1.0.8/src/clappform_integrations/clappform_transus/src/clappform_transus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:02:01.437914 clappform-integrations-1.0.8/src/clappform_integrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-21 15:02:01.000000 clappform-integrations-1.0.8/src/clappform_integrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-21 15:02:01.000000 clappform-integrations-1.0.8/src/clappform_integrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 15:02:01.000000 clappform-integrations-1.0.8/src/clappform_integrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-21 15:02:01.000000 clappform-integrations-1.0.8/src/clappform_integrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-21 15:02:01.000000 clappform-integrations-1.0.8/src/clappform_integrations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-22 09:03:28.000000 clappform-integrations-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-22 09:03:28.000000 clappform-integrations-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-12-22 09:03:28.000000 clappform-integrations-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.619651 clappform-integrations-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-22 09:03:28.000000 clappform-integrations-1.0.9/src/clappform_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.619651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itris/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.619651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itris/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itris/src/clappform_itris/
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2023-12-22 09:03:29.000000 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itris/src/clappform_itris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.619651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itsperfect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.619651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itsperfect/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itsperfect/src/clappform_itsperfect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2023-12-22 09:03:29.000000 clappform-integrations-1.0.9/src/clappform_integrations/clappform_itsperfect/src/clappform_itsperfect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.619651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_rudholm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_rudholm/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_rudholm/src/clappform_rudholm/
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2023-12-22 09:03:29.000000 clappform-integrations-1.0.9/src/clappform_integrations/clappform_rudholm/src/clappform_rudholm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_transus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_transus/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations/clappform_transus/src/clappform_transus/
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-12-22 09:03:29.000000 clappform-integrations-1.0.9/src/clappform_integrations/clappform_transus/src/clappform_transus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 09:03:38.623651 clappform-integrations-1.0.9/src/clappform_integrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-22 09:03:38.000000 clappform-integrations-1.0.9/src/clappform_integrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-22 09:03:38.000000 clappform-integrations-1.0.9/src/clappform_integrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 09:03:38.000000 clappform-integrations-1.0.9/src/clappform_integrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-22 09:03:38.000000 clappform-integrations-1.0.9/src/clappform_integrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 09:03:38.000000 clappform-integrations-1.0.9/src/clappform_integrations.egg-info/top_level.txt
```

### Comparing `clappform-integrations-1.0.8/LICENSE` & `clappform-integrations-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-integrations-1.0.8/PKG-INFO` & `clappform-integrations-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform-integrations
-Version: 1.0.8
+Version: 1.0.9
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-integrations
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-integrations-1.0.8/pyproject.toml` & `clappform-integrations-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform-integrations"
-version = "1.0.8"
+version = "1.0.9"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `clappform-integrations-1.0.8/src/clappform_integrations/clappform_itris/src/clappform_itris/__init__.py` & `clappform-integrations-1.0.9/src/clappform_integrations/clappform_itris/src/clappform_itris/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 __version__ = "0.0.4"
 __author__ = "Clappform B.V."
 __email__ = "info@clappform.com"
 __license__ = "MIT"
 __doc__ = "Clappform Python API wrapper"
 
 
-# %%
+ 
 import requests
 import logging
 import json
 import pandas as pd
 import re
 
 from bs4 import BeautifulSoup
 from enum import Enum, auto
 import xml.etree.ElementTree as ET
 import xmltodict
 
-# %%
+ 
 class ItrisException(Exception):
     """REST Exceptions Class"""
 
 
 class ItrisSOAPException(Exception):
     """SOAP Exceptions Class"""
 
@@ -132,16 +132,15 @@
 
         if not endpoint:
             raise ItrisException(f"Endpoint '{translated_endpoint_id}' not found!")
 
         # Initial URL
         url = f"{self.base_url}/{endpoint['path']}{self.__add_filter(filters)}"
 
-        # logging.info(f"Constructed URL: {url}")
-        logging.info(f"Constructed URL: {url}")
+       # logging.info(f"Constructed URL: {url}")
         # Extract skip value if provided in filters
         initial_skip = int(filters.get("$skip", 0))
 
 
         return self.__fetch_odata_data(url, initial_skip)
 
     def __fetch_odata_data(self, url: str, skip: int = 0) -> list:
@@ -155,15 +154,15 @@
         if "$skip=" in url:
             url = re.sub(r"\$skip=\d+", f"$skip={skip}", url)
         else:
             separator = "&" if "?" in url else "?"
             url = f"{url}{separator}$skip={skip}"
 
         response = requests.get(url, headers=headers_with_token, timeout=self.timeout)
-        logging.info(url)
+        #logging.info(url)
 
         if response.status_code > 204:
             logging.info(response.text)
             logging.info("Request URL: %s", url)
             raise ItrisException(f"Failed to fetch data! HTTP Status Code: {response.status_code}")
 
         if response.status_code == 200:
@@ -345,22 +344,22 @@
 
             response = requests.post(self.base_url, data=soap_request, headers=self.headers, timeout=self.timeout)
 
             if response.status_code != 200:
                 raise ItrisSOAPException("Failed to retrieve data from the API")
 
             try:
-                response_text = response.content.decode('utf-8')
-                logging.info("Decoded with UTF-8")
+                response_text = response.content.decode('utf-8') #Decoded with UTF-8
+               # logging.info("Decoded with UTF-8")
             except UnicodeDecodeError:
                 logging.info("Failed to decode with UTF-8, trying ISO-8859-1")
                 try:
                     response_text = response.content.decode('ISO-8859-1')
                 except UnicodeDecodeError as e:
-                    logging.info("Failed to decode with ISO-8859-1 as well")
+                    #logging.info("Failed to decode with ISO-8859-1 as well")
                     raise ItrisSOAPException("Failed to decode the response") from e
 
             try:
                 return self.transform_response_to_json(response_text)
             except Exception as e:
                 logging.info("Failed to transform response to JSON")
                 raise ItrisSOAPException(f"Failed to parse the response: {e}") from e
```

### Comparing `clappform-integrations-1.0.8/src/clappform_integrations/clappform_itsperfect/src/clappform_itsperfect/__init__.py` & `clappform-integrations-1.0.9/src/clappform_integrations/clappform_itsperfect/src/clappform_itsperfect/__init__.py`

 * *Files identical despite different names*

### Comparing `clappform-integrations-1.0.8/src/clappform_integrations/clappform_rudholm/src/clappform_rudholm/__init__.py` & `clappform-integrations-1.0.9/src/clappform_integrations/clappform_rudholm/src/clappform_rudholm/__init__.py`

 * *Files identical despite different names*

### Comparing `clappform-integrations-1.0.8/src/clappform_integrations/clappform_transus/src/clappform_transus/__init__.py` & `clappform-integrations-1.0.9/src/clappform_integrations/clappform_transus/src/clappform_transus/__init__.py`

 * *Files identical despite different names*

### Comparing `clappform-integrations-1.0.8/src/clappform_integrations.egg-info/PKG-INFO` & `clappform-integrations-1.0.9/src/clappform_integrations.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform-integrations
-Version: 1.0.8
+Version: 1.0.9
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-integrations
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-integrations-1.0.8/src/clappform_integrations.egg-info/SOURCES.txt` & `clappform-integrations-1.0.9/src/clappform_integrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

