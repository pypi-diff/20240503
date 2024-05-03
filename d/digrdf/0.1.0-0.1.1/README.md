# Comparing `tmp/digrdf-0.1.0.tar.gz` & `tmp/digrdf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digrdf-0.1.0.tar", max compression
+gzip compressed data, was "digrdf-0.1.1.tar", max compression
```

## Comparing `digrdf-0.1.0.tar` & `digrdf-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      361 2024-05-03 02:01:18.811371 digrdf-0.1.0/README.md
--rw-r--r--   0        0        0       34 2024-05-03 01:56:05.040357 digrdf-0.1.0/digrdf/__init__.py
--rw-r--r--   0        0        0     4037 2024-05-03 02:02:42.742934 digrdf-0.1.0/digrdf/__main__.py
--rw-r--r--   0        0        0      658 2024-05-03 00:07:38.359667 digrdf-0.1.0/digrdf/prefixes.py
--rw-r--r--   0        0        0      388 2024-05-03 02:05:16.244602 digrdf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 digrdf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      553 2024-05-03 02:27:36.265857 digrdf-0.1.1/README.md
+-rw-r--r--   0        0        0       35 2024-05-03 02:09:26.222263 digrdf-0.1.1/digrdf/__init__.py
+-rw-r--r--   0        0        0     3856 2024-05-03 02:25:13.187926 digrdf-0.1.1/digrdf/__main__.py
+-rw-r--r--   0        0        0      658 2024-05-03 00:07:38.359667 digrdf-0.1.1/digrdf/prefixes.py
+-rw-r--r--   0        0        0      289 2024-05-03 02:20:38.722830 digrdf-0.1.1/digrdf/query.sparql
+-rw-r--r--   0        0        0      388 2024-05-03 02:27:16.307161 digrdf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 digrdf-0.1.1/PKG-INFO
```

### Comparing `digrdf-0.1.0/digrdf/prefixes.py` & `digrdf-0.1.1/digrdf/prefixes.py`

 * *Files identical despite different names*

### Comparing `digrdf-0.1.0/PKG-INFO` & `digrdf-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digrdf
-Version: 0.1.0
+Version: 0.1.1
 Summary: RDF Schema Diagram creation tool
 Author: Lawson Lewis
 Author-email: lawson@kurrawong.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -27,11 +27,19 @@
 pip install digrdf
 ```
 ## Usage
 
 from the command line
 
 ```bash
+python -m digrdf -i myfiles/
+```
+
+This will create a file called diagram.html in the working directory and open it for viewing.
 
+to see all the cmdline options run
+
+```bash
+python -m digrdf -h
 ```
```

