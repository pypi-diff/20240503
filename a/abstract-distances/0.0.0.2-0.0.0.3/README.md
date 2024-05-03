# Comparing `tmp/abstract_distances-0.0.0.2.tar.gz` & `tmp/abstract_distances-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_distances-0.0.0.2.tar", last modified: Fri May  3 16:59:10 2024, max compression
+gzip compressed data, was "abstract_distances-0.0.0.3.tar", last modified: Fri May  3 17:03:34 2024, max compression
```

## Comparing `abstract_distances-0.0.0.2.tar` & `abstract_distances-0.0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 16:59:10.752464 abstract_distances-0.0.0.2/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-03 16:59:10.752464 abstract_distances-0.0.0.2/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.2/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-03 16:59:10.752464 abstract_distances-0.0.0.2/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      982 2024-05-03 16:59:04.000000 abstract_distances-0.0.0.2/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 16:59:10.748464 abstract_distances-0.0.0.2/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 16:59:10.752464 abstract_distances-0.0.0.2/src/abstract_distances/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-26 00:28:14.000000 abstract_distances-0.0.0.2/src/abstract_distances/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.2/src/abstract_distances/char_compar.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    11341 2024-05-03 16:58:52.000000 abstract_distances-0.0.0.2/src/abstract_distances/distance_cals.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.2/src/abstract_distances/do_distance.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    28890 2024-04-24 20:49:04.000000 abstract_distances-0.0.0.2/src/abstract_distances/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    11516 2024-04-10 19:06:49.000000 abstract_distances-0.0.0.2/src/abstract_distances/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5673 2024-04-30 13:35:58.000000 abstract_distances-0.0.0.2/src/abstract_distances/geo_pandas.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1460 2024-04-30 05:13:04.000000 abstract_distances-0.0.0.2/src/abstract_distances/geo_spec.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1975 2024-04-30 09:59:39.000000 abstract_distances-0.0.0.2/src/abstract_distances/get_conversion.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.2/src/abstract_distances/word_compare.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 16:59:10.752464 abstract_distances-0.0.0.2/src/abstract_distances.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-03 16:59:10.000000 abstract_distances-0.0.0.2/src/abstract_distances.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      625 2024-05-03 16:59:10.000000 abstract_distances-0.0.0.2/src/abstract_distances.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-03 16:59:10.000000 abstract_distances-0.0.0.2/src/abstract_distances.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-03 16:59:10.000000 abstract_distances-0.0.0.2/src/abstract_distances.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-03 16:59:10.000000 abstract_distances-0.0.0.2/src/abstract_distances.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:03:34.805628 abstract_distances-0.0.0.3/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-03 17:03:34.805628 abstract_distances-0.0.0.3/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.3/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-03 17:03:34.805628 abstract_distances-0.0.0.3/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      982 2024-05-03 17:03:15.000000 abstract_distances-0.0.0.3/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:03:34.805628 abstract_distances-0.0.0.3/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:03:34.805628 abstract_distances-0.0.0.3/src/abstract_distances/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-26 00:28:14.000000 abstract_distances-0.0.0.3/src/abstract_distances/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.3/src/abstract_distances/char_compar.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    11430 2024-05-03 17:03:04.000000 abstract_distances-0.0.0.3/src/abstract_distances/distance_cals.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.3/src/abstract_distances/do_distance.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    28890 2024-04-24 20:49:04.000000 abstract_distances-0.0.0.3/src/abstract_distances/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    11516 2024-04-10 19:06:49.000000 abstract_distances-0.0.0.3/src/abstract_distances/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5673 2024-04-30 13:35:58.000000 abstract_distances-0.0.0.3/src/abstract_distances/geo_pandas.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1460 2024-04-30 05:13:04.000000 abstract_distances-0.0.0.3/src/abstract_distances/geo_spec.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1975 2024-04-30 09:59:39.000000 abstract_distances-0.0.0.3/src/abstract_distances/get_conversion.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.3/src/abstract_distances/word_compare.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:03:34.805628 abstract_distances-0.0.0.3/src/abstract_distances.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-03 17:03:34.000000 abstract_distances-0.0.0.3/src/abstract_distances.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      625 2024-05-03 17:03:34.000000 abstract_distances-0.0.0.3/src/abstract_distances.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-03 17:03:34.000000 abstract_distances-0.0.0.3/src/abstract_distances.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-03 17:03:34.000000 abstract_distances-0.0.0.3/src/abstract_distances.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-03 17:03:34.000000 abstract_distances-0.0.0.3/src/abstract_distances.egg-info/top_level.txt
```

### Comparing `abstract_distances-0.0.0.2/PKG-INFO` & `abstract_distances-0.0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.2
+Version: 0.0.0.3
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_distances-0.0.0.2/setup.py` & `abstract_distances-0.0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_distances',
-    version='0.0.0.2',
+    version='0.0.0.3',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/char_compar.py` & `abstract_distances-0.0.0.3/src/abstract_distances/char_compar.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/distance_cals.py` & `abstract_distances-0.0.0.3/src/abstract_distances/distance_cals.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,29 +95,31 @@
     if text_finds:
         text_find_list = make_list(text_finds)
         if text_find_list and isinstance(text_find_list, list) and len(text_find_list) > 0:
             text_find_list = text_find_list[0]
         if text_find_list and isinstance(text_find_list, str):
             return text_find_list.split(' ')[0]
     return text_finds
-async def calculateDistance(origin, destination,travelMode = 'DRIVING',api_key=None,return_all = False):
+async def calculateDistance(origin, destination,travelMode = 'DRIVING',api_key=None,print_response = True,return_all = False):
     api_key =api_key or get_default_google_api_key()
     base_url = f"https://maps.googleapis.com/maps/api/distancematrix/json?origins={origin}&destinations={destination}&travelMode={travelMode}&units=imperial&key={api_key}"
     
     async with httpx.AsyncClient() as client:
         response = await client.get(base_url)
         
         if response.status_code != 200:
             # Handle error or retry as needed
-            print(response.text)
+            if print_response:
+                print(response.text)
             return None
-        print(response.text)
+        if print_response:
+            print(response.text)
         response = response.json()
         # Your existing logic to extract distance
-        if return_all = False:
+        if return_all == False:
             response = get_from_distance_response(response)
         return response
 
 def get_address_header_association(headers_js,df,index,spec_headers=False):
     print(headers_js)
     if not isinstance(headers_js,dict):
         headers_js = get_closest_headers(headers_js)
```

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/do_distance.py` & `abstract_distances-0.0.0.3/src/abstract_distances/do_distance.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/excel_module.py` & `abstract_distances-0.0.0.3/src/abstract_distances/excel_module.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/functions.py` & `abstract_distances-0.0.0.3/src/abstract_distances/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/geo_pandas.py` & `abstract_distances-0.0.0.3/src/abstract_distances/geo_pandas.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/geo_spec.py` & `abstract_distances-0.0.0.3/src/abstract_distances/geo_spec.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/get_conversion.py` & `abstract_distances-0.0.0.3/src/abstract_distances/get_conversion.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances/word_compare.py` & `abstract_distances-0.0.0.3/src/abstract_distances/word_compare.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances.egg-info/PKG-INFO` & `abstract_distances-0.0.0.3/src/abstract_distances.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.2
+Version: 0.0.0.3
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_distances-0.0.0.2/src/abstract_distances.egg-info/SOURCES.txt` & `abstract_distances-0.0.0.3/src/abstract_distances.egg-info/SOURCES.txt`

 * *Files identical despite different names*

