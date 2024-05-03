# Comparing `tmp/edgegap_scheduling-1.5.2.tar.gz` & `tmp/edgegap_scheduling-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-1.5.2.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.5.3.tar", max compression
```

## Comparing `edgegap_scheduling-1.5.2.tar` & `edgegap_scheduling-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/LICENSE
--rw-r--r--   0        0        0     2164 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/README.md
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/BUILD
--rw-r--r--   0        0        0      380 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0     4688 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     5621 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1375 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1468 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      550 2024-05-03 14:42:17.466940 edgegap_scheduling-1.5.2/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     4351 2024-05-03 14:42:17.470940 edgegap_scheduling-1.5.2/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.470940 edgegap_scheduling-1.5.2/edgegap_scheduling/errors/BUILD
--rw-r--r--   0        0        0      133 2024-05-03 14:42:17.470940 edgegap_scheduling-1.5.2/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-05-03 14:42:17.470940 edgegap_scheduling-1.5.2/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      691 2024-05-03 14:42:29.459009 edgegap_scheduling-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2164 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/BUILD
+-rw-r--r--   0        0        0      380 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0     4688 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     5621 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1375 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1468 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      550 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     4351 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/errors/BUILD
+-rw-r--r--   0        0        0      133 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-03 19:51:34.394796 edgegap_scheduling-1.5.3/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      691 2024-05-03 19:51:50.198959 edgegap_scheduling-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.5.3/PKG-INFO
```

### Comparing `edgegap_scheduling-1.5.2/LICENSE` & `edgegap_scheduling-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/README.md` & `edgegap_scheduling-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.5.3/edgegap_scheduling/_runner.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.5.3/edgegap_scheduling/_scheduler.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.5.3/edgegap_scheduling/_signature.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.5.3/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/edgegap_scheduling/_state.py` & `edgegap_scheduling-1.5.3/edgegap_scheduling/_state.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.5.3/edgegap_scheduling/_task.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.2/pyproject.toml` & `edgegap_scheduling-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-scheduling"
-version = "1.5.2"
+version = "1.5.3"
 description = "The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.7.1"
```

### Comparing `edgegap_scheduling-1.5.2/PKG-INFO` & `edgegap_scheduling-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

