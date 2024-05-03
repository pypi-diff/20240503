# Comparing `tmp/mosek_license_server-0.9.3.tar.gz` & `tmp/mosek_license_server-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.9.3.tar", max compression
+gzip compressed data, was "mosek_license_server-0.9.4.tar", max compression
```

## Comparing `mosek_license_server-0.9.3.tar` & `mosek_license_server-0.9.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10761 2024-03-28 05:08:33.675248 mosek_license_server-0.9.3/LICENSE
--rw-r--r--   0        0        0      579 2024-03-28 05:08:33.675248 mosek_license_server-0.9.3/mosek_license/__init__.py
--rw-r--r--   0        0        0     1309 2024-03-28 05:08:33.675248 mosek_license_server-0.9.3/mosek_license/license.py
--rw-r--r--   0        0        0      761 2024-03-28 05:09:03.583237 mosek_license_server-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     3215 2024-03-28 05:08:33.675248 mosek_license_server-0.9.3/readme.md
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 mosek_license_server-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    10761 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/LICENSE
+-rw-r--r--   0        0        0      579 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/mosek_license/__init__.py
+-rw-r--r--   0        0        0     1309 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/mosek_license/license.py
+-rw-r--r--   0        0        0      761 2024-05-03 18:13:42.562429 mosek_license_server-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3215 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/readme.md
+-rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 mosek_license_server-0.9.4/PKG-INFO
```

### Comparing `mosek_license_server-0.9.3/LICENSE` & `mosek_license_server-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.3/mosek_license/__init__.py` & `mosek_license_server-0.9.4/mosek_license/__init__.py`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.3/mosek_license/license.py` & `mosek_license_server-0.9.4/mosek_license/license.py`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.3/pyproject.toml` & `mosek_license_server-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosek-license-server"
-version = "v0.9.3"
+version = "v0.9.4"
 description = "Expose a mosek license via a nginx server"
 authors = ["Thomas Schmelzer <thomas.schmelzer@gmail.com>"]
 license = "Apache 2.0"
 readme = "readme.md"
 repository = "https://github.com/tschm/mosek-license-server"
 packages = [{include = "mosek_license"}]
```

### Comparing `mosek_license_server-0.9.3/readme.md` & `mosek_license_server-0.9.4/readme.md`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.3/PKG-INFO` & `mosek_license_server-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.9.3
+Version: 0.9.4
 Summary: Expose a mosek license via a nginx server
 Home-page: https://github.com/tschm/mosek-license-server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
```

