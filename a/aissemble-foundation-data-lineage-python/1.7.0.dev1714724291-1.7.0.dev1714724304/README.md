# Comparing `tmp/aissemble_foundation_data_lineage_python-1.7.0.dev1714724291.tar.gz` & `tmp/aissemble_foundation_data_lineage_python-1.7.0.dev1714724304.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_data_lineage_python-1.7.0.dev1714724291.tar", max compression
+gzip compressed data, was "aissemble_foundation_data_lineage_python-1.7.0.dev1714724304.tar", max compression
```

## Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291.tar` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     9580 2024-05-03 08:17:49.511819 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/LICENSE
--rw-r--r--   0        0        0     3584 2024-05-03 08:12:09.264240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/README.md
--rw-r--r--   0        0        0     1045 2024-05-03 08:18:12.018790 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/pyproject.toml
--rw-r--r--   0        0        0      557 2024-05-03 08:12:09.264240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/__init__.py
--rw-r--r--   0        0        0     4277 2024-05-03 08:12:09.264240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/data_lineage_config.py
--rw-r--r--   0        0        0     3888 2024-05-03 08:12:09.264240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/dataset.py
--rw-r--r--   0        0        0      674 2024-05-03 08:12:09.264240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/default_properties/microprofile-config.properties
--rw-r--r--   0        0        0     3129 2024-05-03 08:12:09.264240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/emitter.py
--rw-r--r--   0        0        0     3244 2024-05-03 08:12:09.265240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/facet.py
--rw-r--r--   0        0        0     1260 2024-05-03 08:12:09.265240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/job.py
--rw-r--r--   0        0        0     1924 2024-05-03 08:12:09.265240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/lineage_base.py
--rw-r--r--   0        0        0      988 2024-05-03 08:12:09.265240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/run.py
--rw-r--r--   0        0        0     3267 2024-05-03 08:12:09.265240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/run_event.py
--rw-r--r--   0        0        0      414 2024-05-03 08:12:09.265240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/transport.py
--rw-r--r--   0        0        0     6788 2024-05-03 08:12:09.265240 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/util/lineage_util.py
--rw-r--r--   0        0        0     4162 1970-01-01 00:00:00.000000 aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 08:17:59.651896 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/LICENSE
+-rw-r--r--   0        0        0     3584 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/README.md
+-rw-r--r--   0        0        0     1045 2024-05-03 08:18:25.011201 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/__init__.py
+-rw-r--r--   0        0        0     4277 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/data_lineage_config.py
+-rw-r--r--   0        0        0     3888 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/dataset.py
+-rw-r--r--   0        0        0      674 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/default_properties/microprofile-config.properties
+-rw-r--r--   0        0        0     3129 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/emitter.py
+-rw-r--r--   0        0        0     3244 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/facet.py
+-rw-r--r--   0        0        0     1260 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/job.py
+-rw-r--r--   0        0        0     1924 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/lineage_base.py
+-rw-r--r--   0        0        0      988 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/run.py
+-rw-r--r--   0        0        0     3267 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/run_event.py
+-rw-r--r--   0        0        0      414 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/transport.py
+-rw-r--r--   0        0        0     6788 2024-05-03 08:12:09.151401 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/util/lineage_util.py
+-rw-r--r--   0        0        0     4162 1970-01-01 00:00:00.000000 aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/PKG-INFO
```

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/LICENSE` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/README.md` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/pyproject.toml` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-data-lineage-python"
-version = "1.7.0.dev1714724291"
+version = "1.7.0.dev1714724304"
 description = "Data lineage API for Python scripts"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "aissemble_data_lineage", from = "src"}
 ]
 include = [
```

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/__init__.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/data_lineage_config.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/data_lineage_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/dataset.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/dataset.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/default_properties/microprofile-config.properties` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/default_properties/microprofile-config.properties`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/emitter.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/emitter.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/facet.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/facet.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/job.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/job.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/lineage_base.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/lineage_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/run.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/run.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/run_event.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/run_event.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/src/aissemble_data_lineage/util/lineage_util.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/src/aissemble_data_lineage/util/lineage_util.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1714724291/PKG-INFO` & `aissemble_foundation_data_lineage_python-1.7.0.dev1714724304/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-data-lineage-python
-Version: 1.7.0.dev1714724291
+Version: 1.7.0.dev1714724304
 Summary: Data lineage API for Python scripts
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-foundation-messaging-python (==1.7.0.*)
```

