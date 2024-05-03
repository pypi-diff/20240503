# Comparing `tmp/beetl-0.4.3.tar.gz` & `tmp/beetl-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.4.3.tar", last modified: Thu May  2 14:19:45 2024, max compression
+gzip compressed data, was "beetl-0.4.4.tar", last modified: Fri May  3 09:38:06 2024, max compression
```

## Comparing `beetl-0.4.3.tar` & `beetl-0.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:19:45.242211 beetl-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-02 14:19:45.238211 beetl-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-02 14:18:24.000000 beetl-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:19:45.242211 beetl-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-02 14:18:24.000000 beetl-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:19:45.234211 beetl-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:19:45.238211 beetl-0.4.3/src/beetl/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/beetl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:19:45.238211 beetl-0.4.3/src/beetl/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/sqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/sources/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:19:45.238211 beetl-0.4.3/src/beetl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-02 14:18:24.000000 beetl-0.4.3/src/beetl/transformers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:19:45.238211 beetl-0.4.3/src/beetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-02 14:19:45.000000 beetl-0.4.3/src/beetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 14:19:45.000000 beetl-0.4.3/src/beetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:19:45.000000 beetl-0.4.3/src/beetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 14:19:45.000000 beetl-0.4.3/src/beetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 14:19:45.000000 beetl-0.4.3/src/beetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 14:19:45.000000 beetl-0.4.3/src/beetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:19:45.000000 beetl-0.4.3/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.739242 beetl-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-03 09:38:06.739242 beetl-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-03 09:37:15.000000 beetl-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:38:06.739242 beetl-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 09:37:15.000000 beetl-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.735242 beetl-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.735242 beetl-0.4.4/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.739242 beetl-0.4.4/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.739242 beetl-0.4.4/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.735242 beetl-0.4.4/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.4.3/PKG-INFO` & `beetl-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.3
+Version: 0.4.4
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.3/README.md` & `beetl-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/setup.py` & `beetl-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/__version__.py` & `beetl-0.4.4/src/beetl/__version__.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/beetl.py` & `beetl-0.4.4/src/beetl/beetl.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/config.py` & `beetl-0.4.4/src/beetl/config.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/faker.py` & `beetl-0.4.4/src/beetl/sources/faker.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/interface.py` & `beetl-0.4.4/src/beetl/sources/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/itop.py` & `beetl-0.4.4/src/beetl/sources/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/mongodb.py` & `beetl-0.4.4/src/beetl/sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/mysql.py` & `beetl-0.4.4/src/beetl/sources/mysql.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/postgres.py` & `beetl-0.4.4/src/beetl/sources/postgres.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/rest.py` & `beetl-0.4.4/src/beetl/sources/rest.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/sources/sqlserver.py` & `beetl-0.4.4/src/beetl/sources/sqlserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,18 @@
             UPDATE TDEST
             SET {field_spec}
             FROM {self.source_configuration.table} AS TDEST
             INNER JOIN {tempDB} AS TTEMP ON {on_clause}
         """
 
         self._query(customQuery=query, returnData=False)
-        self._query(customQuery="DROP TABLE " + tempDB, returnData=False)
+        try:
+            self._query(customQuery="DROP TABLE " + tempDB, returnData=False)
+        except Exception:
+            pass
 
         return len(data)
 
     def delete(self, data: pl.DataFrame):
         if len(data) == 0:
             return 0
```

### Comparing `beetl-0.4.3/src/beetl/sources/static.py` & `beetl-0.4.4/src/beetl/sources/static.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/transformers/frames.py` & `beetl-0.4.4/src/beetl/transformers/frames.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/transformers/interface.py` & `beetl-0.4.4/src/beetl/transformers/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/transformers/itop.py` & `beetl-0.4.4/src/beetl/transformers/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/transformers/misc.py` & `beetl-0.4.4/src/beetl/transformers/misc.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/transformers/regex.py` & `beetl-0.4.4/src/beetl/transformers/regex.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl/transformers/strings.py` & `beetl-0.4.4/src/beetl/transformers/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,18 @@
 
         return data.with_columns(nCol.alias(outField))
     
     @staticmethod
     def join_listfield(
         data: pl.DataFrame, inField: str, outField: str, separator: str = ","
     ) -> pl.DataFrame:
-        
-        
-        data = data.with_columns(data[inField].arr.join(separator).alias(outField))
+        try:
+            data = data.with_columns(data[inField].arr.join(separator).alias(outField))
+        except Exception:
+            data = data.with_columns(data[inField].cast(pl.List).arr.join(separator).alias(outField))
         
         return data
 
     @staticmethod
     def split(
         data: pl.DataFrame, inField: str, outFields: list, separator: str = ""
     ) -> pl.DataFrame:
```

### Comparing `beetl-0.4.3/src/beetl/transformers/structs.py` & `beetl-0.4.4/src/beetl/transformers/structs.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.3/src/beetl.egg-info/PKG-INFO` & `beetl-0.4.4/src/beetl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.3
+Version: 0.4.4
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.3/src/beetl.egg-info/SOURCES.txt` & `beetl-0.4.4/src/beetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

