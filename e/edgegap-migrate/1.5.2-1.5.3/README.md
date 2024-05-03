# Comparing `tmp/edgegap_migrate-1.5.2.tar.gz` & `tmp/edgegap_migrate-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_migrate-1.5.2.tar", max compression
+gzip compressed data, was "edgegap_migrate-1.5.3.tar", max compression
```

## Comparing `edgegap_migrate-1.5.2.tar` & `edgegap_migrate-1.5.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1993 2024-05-03 14:42:17.466940 edgegap_migrate-1.5.2/LICENSE
--rw-r--r--   0        0        0     2164 2024-05-03 14:42:17.466940 edgegap_migrate-1.5.2/README.md
--rw-r--r--   0        0        0        0 2024-05-03 14:42:17.466940 edgegap_migrate-1.5.2/edgegap_migrate/__init__.py
--rw-r--r--   0        0        0      571 2024-05-03 14:42:57.219169 edgegap_migrate-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 edgegap_migrate-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 19:51:34.394796 edgegap_migrate-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2164 2024-05-03 19:51:34.394796 edgegap_migrate-1.5.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 19:51:34.394796 edgegap_migrate-1.5.3/edgegap_migrate/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-03 19:51:55.731017 edgegap_migrate-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 edgegap_migrate-1.5.3/PKG-INFO
```

### Comparing `edgegap_migrate-1.5.2/LICENSE` & `edgegap_migrate-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_migrate-1.5.2/README.md` & `edgegap_migrate-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_migrate-1.5.2/pyproject.toml` & `edgegap_migrate-1.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-migrate"
-version = "1.5.2"
+version = "1.5.3"
 description = "The Edgegap library to handle migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 console-menu = "^0.8.0"
```

### Comparing `edgegap_migrate-1.5.2/PKG-INFO` & `edgegap_migrate-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-migrate
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Edgegap library to handle migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

