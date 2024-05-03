# Comparing `tmp/digrdf-0.1.1.tar.gz` & `tmp/digrdf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digrdf-0.1.1.tar", max compression
+gzip compressed data, was "digrdf-0.1.2.tar", max compression
```

## Comparing `digrdf-0.1.1.tar` & `digrdf-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      553 2024-05-03 02:27:36.265857 digrdf-0.1.1/README.md
--rw-r--r--   0        0        0       35 2024-05-03 02:09:26.222263 digrdf-0.1.1/digrdf/__init__.py
--rw-r--r--   0        0        0     3856 2024-05-03 02:25:13.187926 digrdf-0.1.1/digrdf/__main__.py
--rw-r--r--   0        0        0      658 2024-05-03 00:07:38.359667 digrdf-0.1.1/digrdf/prefixes.py
--rw-r--r--   0        0        0      289 2024-05-03 02:20:38.722830 digrdf-0.1.1/digrdf/query.sparql
--rw-r--r--   0        0        0      388 2024-05-03 02:27:16.307161 digrdf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 digrdf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      553 2024-05-03 02:27:36.265857 digrdf-0.1.2/README.md
+-rw-r--r--   0        0        0       35 2024-05-03 02:30:07.231145 digrdf-0.1.2/digrdf/__init__.py
+-rw-r--r--   0        0        0     3857 2024-05-03 02:29:58.823630 digrdf-0.1.2/digrdf/__main__.py
+-rw-r--r--   0        0        0      658 2024-05-03 00:07:38.359667 digrdf-0.1.2/digrdf/prefixes.py
+-rw-r--r--   0        0        0      289 2024-05-03 02:20:38.722830 digrdf-0.1.2/digrdf/query.sparql
+-rw-r--r--   0        0        0      388 2024-05-03 02:30:18.672300 digrdf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 digrdf-0.1.2/PKG-INFO
```

### Comparing `digrdf-0.1.1/README.md` & `digrdf-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `digrdf-0.1.1/digrdf/__main__.py` & `digrdf-0.1.2/digrdf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from itertools import product
 from pathlib import Path
 from subprocess import check_output
 
 from pyvis.network import Network
 
-from prefixes import prefix_map
+from .prefixes import prefix_map
 
 
 def get_label(uri: str) -> str:
     # handle xsd:text which comes through as ""
     if uri == "":
         uri = "http://www.w3.org/2001/XMLSchema#string"
     if "#" in uri:
```

### Comparing `digrdf-0.1.1/digrdf/prefixes.py` & `digrdf-0.1.2/digrdf/prefixes.py`

 * *Files identical despite different names*

### Comparing `digrdf-0.1.1/PKG-INFO` & `digrdf-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digrdf
-Version: 0.1.1
+Version: 0.1.2
 Summary: RDF Schema Diagram creation tool
 Author: Lawson Lewis
 Author-email: lawson@kurrawong.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

