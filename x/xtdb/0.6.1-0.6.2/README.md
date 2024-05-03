# Comparing `tmp/xtdb-0.6.1.tar.gz` & `tmp/xtdb-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtdb-0.6.1.tar", max compression
+gzip compressed data, was "xtdb-0.6.2.tar", max compression
```

## Comparing `xtdb-0.6.1.tar` & `xtdb-0.6.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-11-21 13:51:13.787994 xtdb-0.6.1/LICENSE
--rw-r--r--   0        0        0     5140 2023-11-21 13:51:13.787994 xtdb-0.6.1/README.md
--rw-r--r--   0        0        0     1737 2023-11-21 13:51:13.791994 xtdb-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-21 13:51:13.791994 xtdb-0.6.1/xtdb/__init__.py
--rw-r--r--   0        0        0      211 2023-11-21 13:51:13.791994 xtdb-0.6.1/xtdb/__main__.py
--rw-r--r--   0        0        0    16361 2023-11-21 13:51:13.791994 xtdb-0.6.1/xtdb/datalog.py
--rw-r--r--   0        0        0      315 2023-11-21 13:51:13.791994 xtdb-0.6.1/xtdb/exceptions.py
--rw-r--r--   0        0        0     1786 2023-11-21 13:51:13.791994 xtdb-0.6.1/xtdb/orm.py
--rw-r--r--   0        0        0     6477 2023-11-21 13:51:13.791994 xtdb-0.6.1/xtdb/query.py
--rw-r--r--   0        0        0    13467 2023-11-21 13:51:13.791994 xtdb-0.6.1/xtdb/session.py
--rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 xtdb-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-11-22 07:32:17.144499 xtdb-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5140 2023-11-22 07:32:17.144499 xtdb-0.6.2/README.md
+-rw-r--r--   0        0        0     1737 2023-11-22 07:32:17.148499 xtdb-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-22 07:32:17.148499 xtdb-0.6.2/xtdb/__init__.py
+-rw-r--r--   0        0        0      211 2023-11-22 07:32:17.148499 xtdb-0.6.2/xtdb/__main__.py
+-rw-r--r--   0        0        0    16361 2023-11-22 07:32:17.148499 xtdb-0.6.2/xtdb/datalog.py
+-rw-r--r--   0        0        0      315 2023-11-22 07:32:17.148499 xtdb-0.6.2/xtdb/exceptions.py
+-rw-r--r--   0        0        0     1786 2023-11-22 07:32:17.148499 xtdb-0.6.2/xtdb/orm.py
+-rw-r--r--   0        0        0     6477 2023-11-22 07:32:17.148499 xtdb-0.6.2/xtdb/query.py
+-rw-r--r--   0        0        0    13554 2023-11-22 07:32:17.148499 xtdb-0.6.2/xtdb/session.py
+-rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 xtdb-0.6.2/PKG-INFO
```

### Comparing `xtdb-0.6.1/LICENSE` & `xtdb-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xtdb-0.6.1/README.md` & `xtdb-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `xtdb-0.6.1/pyproject.toml` & `xtdb-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtdb"
-version = "0.6.1"
+version = "0.6.2"
 packages = [{ include = "xtdb" }]
 include  = ["xtdb/**"]
 exclude = [
     "**/.idea",
     "**/.git*",
     "**/.*ignore",
     "**/.flake8",
```

### Comparing `xtdb-0.6.1/xtdb/datalog.py` & `xtdb-0.6.2/xtdb/datalog.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.6.1/xtdb/orm.py` & `xtdb-0.6.2/xtdb/orm.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.6.1/xtdb/query.py` & `xtdb-0.6.2/xtdb/query.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.6.1/xtdb/session.py` & `xtdb-0.6.2/xtdb/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,16 +298,18 @@
         key: str, parameter: Union[None, datetime, int, str, bool], current_params: Optional[Dict] = None
     ) -> Dict:
         if current_params is None:
             current_params = {}
 
         if isinstance(parameter, datetime):
             current_params[key] = parameter.isoformat()
-        if isinstance(parameter, (int, str, bool)):
+        elif isinstance(parameter, bool):
             current_params[key] = str(parameter).lower()
+        elif isinstance(parameter, (int, str)):
+            current_params[key] = str(parameter)
 
         return current_params
 
 
 class XTDBSession:
     def __init__(self, base_url: str):
         self.client = XTDBClient(base_url)
```

### Comparing `xtdb-0.6.1/PKG-INFO` & `xtdb-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtdb
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python ORM for XTDB.
 Home-page: https://github.com/Donnype/xtdb-py
 Author: Donny Peeters
 Author-email: donny.peeters@hotmail.com
 Maintainer: Donny Peeters
 Maintainer-email: donny.peeters@hotmail.com
 Requires-Python: >=3.8,<4.0
```

