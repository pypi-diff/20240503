# Comparing `tmp/edgegap_database-1.5.2.tar.gz` & `tmp/edgegap_database-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_database-1.5.2.tar", max compression
+gzip compressed data, was "edgegap_database-1.5.3.tar", max compression
```

## Comparing `edgegap_database-1.5.2.tar` & `edgegap_database-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/README.md
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/BUILD
--rw-r--r--   0        0        0      445 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/__init__.py
--rw-r--r--   0        0        0      754 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/_base.py
--rw-r--r--   0        0        0      580 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/_configuration.py
--rw-r--r--   0        0        0     1072 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/_engine.py
--rw-r--r--   0        0        0      796 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/_factory.py
--rw-r--r--   0        0        0      271 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/_model.py
--rw-r--r--   0        0        0     2339 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/_operator.py
--rw-r--r--   0        0        0      509 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/_session.py
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/errors/BUILD
--rw-r--r--   0        0        0      327 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/errors/__init__.py
--rw-r--r--   0        0        0      698 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/errors/_exceptions.py
--rw-r--r--   0        0        0      484 2024-05-03 14:42:17.466940 edgegap_database-1.5.2/edgegap_database/errors/_factory.py
--rw-r--r--   0        0        0      743 2024-05-03 14:42:33.615033 edgegap_database-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/BUILD
+-rw-r--r--   0        0        0      445 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/__init__.py
+-rw-r--r--   0        0        0      754 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/_base.py
+-rw-r--r--   0        0        0      580 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/_configuration.py
+-rw-r--r--   0        0        0     1072 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/_engine.py
+-rw-r--r--   0        0        0      796 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/_factory.py
+-rw-r--r--   0        0        0      271 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/_model.py
+-rw-r--r--   0        0        0     2339 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/_operator.py
+-rw-r--r--   0        0        0      509 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/_session.py
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/errors/BUILD
+-rw-r--r--   0        0        0      327 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/errors/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/errors/_exceptions.py
+-rw-r--r--   0        0        0      484 2024-05-03 19:51:34.390796 edgegap_database-1.5.3/edgegap_database/errors/_factory.py
+-rw-r--r--   0        0        0      743 2024-05-03 19:52:05.639124 edgegap_database-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.5.3/PKG-INFO
```

### Comparing `edgegap_database-1.5.2/LICENSE` & `edgegap_database-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/README.md` & `edgegap_database-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/edgegap_database/_base.py` & `edgegap_database-1.5.3/edgegap_database/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/edgegap_database/_configuration.py` & `edgegap_database-1.5.3/edgegap_database/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/edgegap_database/_engine.py` & `edgegap_database-1.5.3/edgegap_database/_engine.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/edgegap_database/_factory.py` & `edgegap_database-1.5.3/edgegap_database/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/edgegap_database/_operator.py` & `edgegap_database-1.5.3/edgegap_database/_operator.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/edgegap_database/errors/_exceptions.py` & `edgegap_database-1.5.3/edgegap_database/errors/_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.2/pyproject.toml` & `edgegap_database-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-database"
-version = "1.5.2"
+version = "1.5.3"
 description = "The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 psycopg-c = "^3.1.18"
```

### Comparing `edgegap_database-1.5.2/PKG-INFO` & `edgegap_database-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-database
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

