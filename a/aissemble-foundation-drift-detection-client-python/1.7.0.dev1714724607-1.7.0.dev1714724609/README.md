# Comparing `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607.tar.gz` & `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607.tar", max compression
+gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609.tar", max compression
```

## Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607.tar` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     9580 2024-05-03 08:23:14.860460 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/LICENSE
--rw-r--r--   0        0        0        0 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/README.md
--rw-r--r--   0        0        0      661 2024-05-03 08:23:27.548446 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/pyproject.toml
--rw-r--r--   0        0        0      194 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/config/__init__.py
--rw-r--r--   0        0        0      672 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/config/rest_config.py
--rw-r--r--   0        0        0      194 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/drift/__init__.py
--rw-r--r--   0        0        0      194 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/drift/detection/__init__.py
--rw-r--r--   0        0        0      194 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/drift/detection/rest/__init__.py
--rw-r--r--   0        0        0      194 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/drift/detection/rest/client/__init__.py
--rw-r--r--   0        0        0     1755 2024-05-03 08:12:09.255240 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/drift/detection/rest/client/drift_rest_client.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 08:23:15.953262 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/README.md
+-rw-r--r--   0        0        0      661 2024-05-03 08:23:29.932880 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/pyproject.toml
+-rw-r--r--   0        0        0      194 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/config/__init__.py
+-rw-r--r--   0        0        0      672 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/config/rest_config.py
+-rw-r--r--   0        0        0      194 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/drift/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/drift/detection/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/drift/detection/rest/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/drift/detection/rest/client/__init__.py
+-rw-r--r--   0        0        0     1755 2024-05-03 08:12:09.141402 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/drift/detection/rest/client/drift_rest_client.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/PKG-INFO
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/LICENSE` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/pyproject.toml` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-drift-detection-client-python"
-version = "1.7.0.dev1714724607"
+version = "1.7.0.dev1714724609"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "config", from = "src"},
     {include = "drift", from = "src"}
 ]
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/config/rest_config.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/config/rest_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/src/drift/detection/rest/client/drift_rest_client.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/src/drift/detection/rest/client/drift_rest_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724607/PKG-INFO` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714724609/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-drift-detection-client-python
-Version: 1.7.0.dev1714724607
+Version: 1.7.0.dev1714724609
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0.4)
```

