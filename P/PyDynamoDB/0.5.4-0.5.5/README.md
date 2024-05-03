# Comparing `tmp/PyDynamoDB-0.5.4.tar.gz` & `tmp/PyDynamoDB-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDynamoDB-0.5.4.tar", last modified: Fri Sep  8 13:20:48 2023, max compression
+gzip compressed data, was "PyDynamoDB-0.5.5.tar", last modified: Fri Oct 20 16:03:57 2023, max compression
```

## Comparing `PyDynamoDB-0.5.4.tar` & `PyDynamoDB-0.5.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:20:48.703503 PyDynamoDB-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2023-09-08 13:20:48.703503 PyDynamoDB-0.5.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:20:48.699503 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2023-09-08 13:20:48.000000 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-09-08 13:20:48.000000 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 13:20:48.000000 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-09-08 13:20:48.000000 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 13:20:48.000000 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-09-08 13:20:48.000000 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-08 13:20:48.000000 PyDynamoDB-0.5.4/PyDynamoDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:20:48.699503 PyDynamoDB-0.5.4/pydynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    21495 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/result_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:20:48.703503 PyDynamoDB-0.5.4/pydynamodb/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/ddl_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/ddl_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/ddl_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/ddl_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/dml_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sql/util_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:20:48.703503 PyDynamoDB-0.5.4/pydynamodb/sqlalchemy_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sqlalchemy_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:20:48.703503 PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/pydnamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/querydb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/querydb_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/pydynamodb/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-09-08 13:20:48.703503 PyDynamoDB-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-09-08 13:20:37.000000 PyDynamoDB-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 16:03:57.752265 PyDynamoDB-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2023-10-20 16:03:57.752265 PyDynamoDB-0.5.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 16:03:57.740265 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2023-10-20 16:03:57.000000 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-10-20 16:03:57.000000 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 16:03:57.000000 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-10-20 16:03:57.000000 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 16:03:57.000000 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-20 16:03:57.000000 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-20 16:03:57.000000 PyDynamoDB-0.5.5/PyDynamoDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 16:03:57.744265 PyDynamoDB-0.5.5/pydynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12355 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21525 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/result_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 16:03:57.748265 PyDynamoDB-0.5.5/pydynamodb/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/ddl_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/ddl_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/ddl_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/ddl_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/dml_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sql/util_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 16:03:57.748265 PyDynamoDB-0.5.5/pydynamodb/sqlalchemy_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sqlalchemy_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 16:03:57.752265 PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/pydnamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/querydb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/querydb_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/pydynamodb/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-20 16:03:57.752265 PyDynamoDB-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-10-20 16:03:46.000000 PyDynamoDB-0.5.5/setup.py
```

### Comparing `PyDynamoDB-0.5.4/LICENSE` & `PyDynamoDB-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/PKG-INFO` & `PyDynamoDB-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
```

### Comparing `PyDynamoDB-0.5.4/PyDynamoDB.egg-info/PKG-INFO` & `PyDynamoDB-0.5.5/PyDynamoDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
```

### Comparing `PyDynamoDB-0.5.4/PyDynamoDB.egg-info/SOURCES.txt` & `PyDynamoDB-0.5.5/PyDynamoDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/README.rst` & `PyDynamoDB-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/__init__.py` & `PyDynamoDB-0.5.5/pydynamodb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, FrozenSet
 
 from .error import *  # noqa
 
 if TYPE_CHECKING:
     from .connection import Connection
 
-__version__: str = "0.5.4"
+__version__: str = "0.5.5"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 3
 paramstyle: str = "qmark"
```

### Comparing `PyDynamoDB-0.5.4/pydynamodb/common.py` & `PyDynamoDB-0.5.5/pydynamodb/common.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/connection.py` & `PyDynamoDB-0.5.5/pydynamodb/connection.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/converter.py` & `PyDynamoDB-0.5.5/pydynamodb/converter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/cursor.py` & `PyDynamoDB-0.5.5/pydynamodb/cursor.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/error.py` & `PyDynamoDB-0.5.5/pydynamodb/error.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/executor.py` & `PyDynamoDB-0.5.5/pydynamodb/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             _logger.exception("Failed to execute statement.")
             raise OperationalError(*e.args) from e
         else:
             return cast(Dict[str, Any], response)
 
     def close(self) -> None:
         self._metadata = None
-        self._rows = None
-        self._errors = None
+        self._rows = self._rows.clear()
+        self._errors = self._errors.clear()
         self._next_token = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
```

### Comparing `PyDynamoDB-0.5.4/pydynamodb/model.py` & `PyDynamoDB-0.5.5/pydynamodb/model.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/result_set.py` & `PyDynamoDB-0.5.5/pydynamodb/result_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,27 +83,30 @@
             for column_info in self._executor.metadata
         ]
 
     def fetchone(
         self,
     ) -> Optional[Dict[Any, Optional[Any]]]:
         limit_ = self._statements.limit
-        if not self._executor.rows and self._executor.next_token:
+        while len(self._executor.rows) == 0 and self._executor.next_token:
             if not limit_ or (limit_ and self._rownumber < limit_):
                 self._executor.execute()
+            else:
+                break
         if not self._executor.rows:
             return None
         else:
             if self._rownumber is None:
                 self._rownumber = 0
             if limit_ and self._rownumber >= limit_:
                 self._executor.rows.clear()
                 return None
+            row = self._executor.rows.popleft()
             self._rownumber += 1
-            return self._executor.rows.popleft()
+            return row
 
     def fetchmany(self, size: Optional[int] = None) -> List[Dict[Any, Optional[Any]]]:
         if not size or size <= 0:
             size = self._arraysize
         rows = []
         for _ in range(size):
             row = self.fetchone()
```

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/base.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/base.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/common.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/common.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/ddl_alter.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/ddl_alter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/ddl_create.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/ddl_create.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/ddl_drop.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/ddl_drop.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/ddl_sql.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/ddl_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/dml_select.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/dml_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,15 @@
             if converted_ is None:
                 converted_ = dict()
             option_name = option[0]
             option_value = option[1]
 
             if option_name == "Limit":
                 self._limit = option_value
+                continue
             elif option_name == "ConsistentRead":
                 self._consistent_read = option_value
             elif option_name == "ReturnConsumedCapacity":
                 self._return_consumed_capacity = option_value
 
             converted_.update({option_name: option_value})
```

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/dml_sql.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/dml_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/parser.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/parser.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/util.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/util.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sql/util_sql.py` & `PyDynamoDB-0.5.5/pydynamodb/sql/util_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py` & `PyDynamoDB-0.5.5/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/dml_select.py` & `PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/dml_select.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/helper.py` & `PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/helper.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/pydnamodb.py` & `PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/pydnamodb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/querydb.py` & `PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/querydb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/superset_dynamodb/querydb_sqlite.py` & `PyDynamoDB-0.5.5/pydynamodb/superset_dynamodb/querydb_sqlite.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/pydynamodb/util.py` & `PyDynamoDB-0.5.5/pydynamodb/util.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.4/setup.py` & `PyDynamoDB-0.5.5/setup.py`

 * *Files identical despite different names*

