# Comparing `tmp/edgegap_api-1.5.0.tar.gz` & `tmp/edgegap_api-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_api-1.5.0.tar", max compression
+gzip compressed data, was "edgegap_api-1.5.1.tar", max compression
```

## Comparing `edgegap_api-1.5.0.tar` & `edgegap_api-1.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.987672 edgegap_api-1.5.0/LICENSE
--rw-r--r--   0        0        0     2171 2024-05-02 18:20:19.987672 edgegap_api-1.5.0/README.md
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.987672 edgegap_api-1.5.0/edgegap_api/BUILD
--rw-r--r--   0        0        0      132 2024-05-02 18:20:19.987672 edgegap_api-1.5.0/edgegap_api/__init__.py
--rw-r--r--   0        0        0      648 2024-05-02 18:20:19.987672 edgegap_api-1.5.0/edgegap_api/_configuration.py
--rw-r--r--   0        0        0     3990 2024-05-02 18:20:19.987672 edgegap_api-1.5.0/edgegap_api/_helper.py
--rw-r--r--   0        0        0      763 2024-05-02 18:20:28.703894 edgegap_api-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 edgegap_api-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 03:42:53.844048 edgegap_api-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2171 2024-05-03 03:42:53.844381 edgegap_api-1.5.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.844547 edgegap_api-1.5.1/edgegap_api/BUILD
+-rw-r--r--   0        0        0      132 2024-05-03 03:42:53.844956 edgegap_api-1.5.1/edgegap_api/__init__.py
+-rw-r--r--   0        0        0      648 2024-05-03 03:42:53.845229 edgegap_api-1.5.1/edgegap_api/_configuration.py
+-rw-r--r--   0        0        0     3990 2024-05-03 03:42:53.845559 edgegap_api-1.5.1/edgegap_api/_helper.py
+-rw-r--r--   0        0        0      763 2024-05-03 14:08:27.648163 edgegap_api-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 edgegap_api-1.5.1/PKG-INFO
```

### Comparing `edgegap_api-1.5.0/LICENSE` & `edgegap_api-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.5.0/README.md` & `edgegap_api-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.5.0/edgegap_api/_configuration.py` & `edgegap_api-1.5.1/edgegap_api/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.5.0/edgegap_api/_helper.py` & `edgegap_api-1.5.1/edgegap_api/_helper.py`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.5.0/pyproject.toml` & `edgegap_api-1.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-api"
-version = "1.5.0"
+version = "1.5.1"
 description = "The Edgegap API library includes various tools and helpers for interacting with RESTful and other types of APIs. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_api-1.5.0/PKG-INFO` & `edgegap_api-1.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-api
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Edgegap API library includes various tools and helpers for interacting with RESTful and other types of APIs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp[speedups] (>=3.9.5,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap API Library
```

