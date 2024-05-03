# Comparing `tmp/pytrivialsql-0.0.7.tar.gz` & `tmp/pytrivialsql-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.0.7.tar", last modified: Wed Jan 17 07:21:08 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.0.tar", last modified: Fri May  3 19:49:59 2024, max compression
```

## Comparing `pytrivialsql-0.0.7.tar` & `pytrivialsql-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:21:08.292478 pytrivialsql-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-01-17 07:21:08.292478 pytrivialsql-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 07:21:08.292478 pytrivialsql-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:21:08.288478 pytrivialsql-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:21:08.292478 pytrivialsql-0.0.7/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:21:08.292478 pytrivialsql-0.0.7/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-01-17 07:21:08.000000 pytrivialsql-0.0.7/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-17 07:21:08.000000 pytrivialsql-0.0.7/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 07:21:08.000000 pytrivialsql-0.0.7/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-17 07:21:08.000000 pytrivialsql-0.0.7/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:21:08.292478 pytrivialsql-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-17 07:20:56.000000 pytrivialsql-0.0.7/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.363769 pytrivialsql-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.0.7/LICENSE` & `pytrivialsql-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.0.7/PKG-INFO` & `pytrivialsql-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.0.7
+Version: 0.1.0
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psycopg[binary,pool]
 
 # PyTrivialSQL
 
 _A basic set of quality-of-life bindings for SQLite that I've copy/pasted more than twice_
```

### Comparing `pytrivialsql-0.0.7/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.0/src/pytrivialsql/sqlite.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.0.7/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.0/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.0.7
+Version: 0.1.0
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psycopg[binary,pool]
 
 # PyTrivialSQL
 
 _A basic set of quality-of-life bindings for SQLite that I've copy/pasted more than twice_
```

### Comparing `pytrivialsql-0.0.7/tests/test_sqlite.py` & `pytrivialsql-0.1.0/tests/test_sqlite.py`

 * *Files identical despite different names*

