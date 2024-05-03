# Comparing `tmp/edgegap_database-1.5.0.tar.gz` & `tmp/edgegap_database-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_database-1.5.0.tar", max compression
+gzip compressed data, was "edgegap_database-1.5.1.tar", max compression
```

## Comparing `edgegap_database-1.5.0.tar` & `edgegap_database-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/README.md
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/BUILD
--rw-r--r--   0        0        0      445 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/__init__.py
--rw-r--r--   0        0        0      754 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_base.py
--rw-r--r--   0        0        0      580 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_configuration.py
--rw-r--r--   0        0        0     1072 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_engine.py
--rw-r--r--   0        0        0      796 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_factory.py
--rw-r--r--   0        0        0      271 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_model.py
--rw-r--r--   0        0        0     2339 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_operator.py
--rw-r--r--   0        0        0      509 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_session.py
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/BUILD
--rw-r--r--   0        0        0      327 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/__init__.py
--rw-r--r--   0        0        0      698 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/_exceptions.py
--rw-r--r--   0        0        0      484 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/_factory.py
--rw-r--r--   0        0        0      743 2024-05-02 18:20:40.544195 edgegap_database-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 03:42:53.852066 edgegap_database-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-03 03:42:53.852469 edgegap_database-1.5.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.852625 edgegap_database-1.5.1/edgegap_database/BUILD
+-rw-r--r--   0        0        0      445 2024-05-03 03:42:53.852992 edgegap_database-1.5.1/edgegap_database/__init__.py
+-rw-r--r--   0        0        0      754 2024-05-03 03:42:53.853211 edgegap_database-1.5.1/edgegap_database/_base.py
+-rw-r--r--   0        0        0      580 2024-05-03 03:42:53.853368 edgegap_database-1.5.1/edgegap_database/_configuration.py
+-rw-r--r--   0        0        0     1072 2024-05-03 03:42:53.853581 edgegap_database-1.5.1/edgegap_database/_engine.py
+-rw-r--r--   0        0        0      796 2024-05-03 03:42:53.853835 edgegap_database-1.5.1/edgegap_database/_factory.py
+-rw-r--r--   0        0        0      271 2024-05-03 03:42:53.854108 edgegap_database-1.5.1/edgegap_database/_model.py
+-rw-r--r--   0        0        0     2339 2024-05-03 03:42:53.854279 edgegap_database-1.5.1/edgegap_database/_operator.py
+-rw-r--r--   0        0        0      509 2024-05-03 03:42:53.854528 edgegap_database-1.5.1/edgegap_database/_session.py
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.854656 edgegap_database-1.5.1/edgegap_database/errors/BUILD
+-rw-r--r--   0        0        0      327 2024-05-03 03:42:53.854905 edgegap_database-1.5.1/edgegap_database/errors/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-03 03:42:53.855123 edgegap_database-1.5.1/edgegap_database/errors/_exceptions.py
+-rw-r--r--   0        0        0      484 2024-05-03 03:42:53.855312 edgegap_database-1.5.1/edgegap_database/errors/_factory.py
+-rw-r--r--   0        0        0      743 2024-05-03 14:08:36.663130 edgegap_database-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 edgegap_database-1.5.1/PKG-INFO
```

### Comparing `edgegap_database-1.5.0/LICENSE` & `edgegap_database-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/README.md` & `edgegap_database-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/edgegap_database/_base.py` & `edgegap_database-1.5.1/edgegap_database/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/edgegap_database/_configuration.py` & `edgegap_database-1.5.1/edgegap_database/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/edgegap_database/_engine.py` & `edgegap_database-1.5.1/edgegap_database/_engine.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/edgegap_database/_factory.py` & `edgegap_database-1.5.1/edgegap_database/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/edgegap_database/_operator.py` & `edgegap_database-1.5.1/edgegap_database/_operator.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/edgegap_database/errors/_exceptions.py` & `edgegap_database-1.5.1/edgegap_database/errors/_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.5.0/pyproject.toml` & `edgegap_database-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-database"
-version = "1.5.0"
+version = "1.5.1"
 description = "The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 psycopg-c = "^3.1.18"
```

### Comparing `edgegap_database-1.5.0/PKG-INFO` & `edgegap_database-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-database
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: psycopg-c (>=3.1.18,<4.0.0)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Description-Content-Type: text/markdown
```

