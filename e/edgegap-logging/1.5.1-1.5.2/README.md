# Comparing `tmp/edgegap_logging-1.5.1.tar.gz` & `tmp/edgegap_logging-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_logging-1.5.1.tar", max compression
+gzip compressed data, was "edgegap_logging-1.5.2.tar", max compression
```

## Comparing `edgegap_logging-1.5.1.tar` & `edgegap_logging-1.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1993 2024-05-03 03:42:53.857214 edgegap_logging-1.5.1/LICENSE
--rw-r--r--   0        0        0     2216 2024-05-03 03:42:53.857500 edgegap_logging-1.5.1/README.md
--rw-r--r--   0        0        0       17 2024-05-03 03:42:53.857617 edgegap_logging-1.5.1/edgegap_logging/BUILD
--rw-r--r--   0        0        0      217 2024-05-03 03:42:53.857780 edgegap_logging-1.5.1/edgegap_logging/__init__.py
--rw-r--r--   0        0        0      847 2024-05-03 03:42:53.857952 edgegap_logging-1.5.1/edgegap_logging/_configuration.py
--rw-r--r--   0        0        0      942 2024-05-03 03:42:53.858150 edgegap_logging-1.5.1/edgegap_logging/_format.py
--rw-r--r--   0        0        0     1299 2024-05-03 03:42:53.858341 edgegap_logging-1.5.1/edgegap_logging/_logging.py
--rw-r--r--   0        0        0      647 2024-05-03 14:08:45.549944 edgegap_logging-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 edgegap_logging-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 14:42:17.466940 edgegap_logging-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2216 2024-05-03 14:42:17.466940 edgegap_logging-1.5.2/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 14:42:17.466940 edgegap_logging-1.5.2/edgegap_logging/BUILD
+-rw-r--r--   0        0        0      217 2024-05-03 14:42:17.466940 edgegap_logging-1.5.2/edgegap_logging/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-03 14:42:17.466940 edgegap_logging-1.5.2/edgegap_logging/_configuration.py
+-rw-r--r--   0        0        0      942 2024-05-03 14:42:17.466940 edgegap_logging-1.5.2/edgegap_logging/_format.py
+-rw-r--r--   0        0        0     1299 2024-05-03 14:42:17.466940 edgegap_logging-1.5.2/edgegap_logging/_logging.py
+-rw-r--r--   0        0        0      647 2024-05-03 14:42:52.611142 edgegap_logging-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 edgegap_logging-1.5.2/PKG-INFO
```

### Comparing `edgegap_logging-1.5.1/LICENSE` & `edgegap_logging-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.5.1/README.md` & `edgegap_logging-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.5.1/edgegap_logging/_configuration.py` & `edgegap_logging-1.5.2/edgegap_logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.5.1/edgegap_logging/_format.py` & `edgegap_logging-1.5.2/edgegap_logging/_format.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.5.1/edgegap_logging/_logging.py` & `edgegap_logging-1.5.2/edgegap_logging/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.5.1/pyproject.toml` & `edgegap_logging-1.5.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-logging"
-version = "1.5.1"
+version = "1.5.2"
 description = "The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 colorama = "^0.4.6"
```

### Comparing `edgegap_logging-1.5.1/PKG-INFO` & `edgegap_logging-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-logging
-Version: 1.5.1
+Version: 1.5.2
 Summary: The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Logging Library
 
 This is the README for the Edgegap Logging Helper, which is part of the Edgegap suite of helpers.
```

