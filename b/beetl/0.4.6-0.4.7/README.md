# Comparing `tmp/beetl-0.4.6.tar.gz` & `tmp/beetl-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.4.6.tar", last modified: Fri May  3 12:44:09 2024, max compression
+gzip compressed data, was "beetl-0.4.7.tar", last modified: Fri May  3 15:04:04 2024, max compression
```

## Comparing `beetl-0.4.6.tar` & `beetl-0.4.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.434563 beetl-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 12:44:09.434563 beetl-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-03 12:43:35.000000 beetl-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:44:09.434563 beetl-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 12:43:35.000000 beetl-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.426563 beetl-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/beetl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/sqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/sources/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 12:43:35.000000 beetl-0.4.6/src/beetl/transformers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:09.430563 beetl-0.4.6/src/beetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:44:09.000000 beetl-0.4.6/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:04:04.094856 beetl-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 15:04:04.094856 beetl-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-03 15:03:28.000000 beetl-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:04:04.094856 beetl-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 15:03:28.000000 beetl-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:04:04.090856 beetl-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:04:04.090856 beetl-0.4.7/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:04:04.094856 beetl-0.4.7/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:04:04.094856 beetl-0.4.7/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 15:03:28.000000 beetl-0.4.7/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:04:04.090856 beetl-0.4.7/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 15:04:04.000000 beetl-0.4.7/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 15:04:04.000000 beetl-0.4.7/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:04:04.000000 beetl-0.4.7/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 15:04:04.000000 beetl-0.4.7/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 15:04:04.000000 beetl-0.4.7/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 15:04:04.000000 beetl-0.4.7/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:04:04.000000 beetl-0.4.7/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.4.6/PKG-INFO` & `beetl-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.6
+Version: 0.4.7
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.6/README.md` & `beetl-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/setup.py` & `beetl-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/__version__.py` & `beetl-0.4.7/src/beetl/__version__.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/beetl.py` & `beetl-0.4.7/src/beetl/beetl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Union
 from .config import BeetlConfig, SyncConfiguration
 from .transformers.interface import TransformerConfiguration
 import polars as pl
 from time import perf_counter
+from tabulate import tabulate
 
 BENCHMARK = []
 
 
 class Beetl:
     """The main class for BeETL. This class is responsible for orchestrating the ETL process."""
 
@@ -74,29 +75,29 @@
         columns = destination.columns if len(columns) == 0 else columns
 
         for column in columns:
             
             if column not in source.columns and column not in destination.columns:
                 raise Exception(f"Column {column} does not exist in any of the datasets")
             
-            if column not in source.columns:
+            if column not in source.columns and len(source) > 0:
                 source = source.with_columns(pl.lit(None).alias(column).cast(source[column].dtype))
             
-            if column not in destination.columns:
+            if column not in destination.columns and len(destination) > 0:
                 destination = destination.with_columns(pl.lit(None).alias(column).cast(source[column].dtype))
 
         # If source is empty, delete all in destination
         if len(source) == 0:
             return source.select(keys + columns), source.select(keys + columns), destination.select(keys)
 
         # If destination is empty, create all from source
         if len(destination) == 0:
             return (
                 source.select(keys + columns if keys != columns else keys),
-                destination.select(keys + columns if keys != columns else keys), 
+                destination, 
                 destination
             )
        
         try:
             # Get rows that only exist in source (Creates)
             create = source.join(destination, on=keys, how="anti")
 
@@ -160,14 +161,15 @@
 
         3. Compare source and destination data with compare_datasets
 
         4. Execute the respective insert, update and delete queries
 
         """
         self.benchmark("Starting sync and retrieving source data")
+        allAmounts = []
         for i, sync in enumerate(self.config.sync_list, 1):
             if sync.name != "":
                 print(f"Starting sync: {sync.name}")
             else:
                 print(f"Starting sync {i}")
             source_data = sync.source.query(sync.sourceConfig)
             self.benchmark("Finished data retrieval from source")
@@ -211,8 +213,11 @@
 
             self.benchmark("Finished deletes, sync finished")
 
             print("Inserted: " + str(amount["inserts"]))
             print("Updated: " + str(amount["updates"]))
             print("Deleted: " + str(amount["deletes"]))
 
-        return amount
+            allAmounts.append([sync.name, *amount.values()])
+        
+        print("\r\n\r\n" + tabulate(allAmounts, headers=["Sync", "Inserts", "Updates", "Deletes"]))
+        return allAmounts
```

### Comparing `beetl-0.4.6/src/beetl/config.py` & `beetl-0.4.7/src/beetl/config.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/faker.py` & `beetl-0.4.7/src/beetl/sources/faker.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/interface.py` & `beetl-0.4.7/src/beetl/sources/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/itop.py` & `beetl-0.4.7/src/beetl/sources/itop.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,19 @@
         self.has_foreign = False
         self.comparison_columns = (
             self.get_output_fields_for_request()
             if comparison_columns is None
             else comparison_columns
         )
         self.soft_delete = soft_delete
+        
+        for field in self.columns:
+            if field.custom_options is not None:
+                if field.custom_options.get("itop", {}).get("comparison_field", False):
+                    self.has_foreign = True
 
     def get_output_fields_for_request(self):
         output = []
         for field in self.columns:
             if field.custom_options is not None:
                 if field.custom_options.get("itop", {}).get("comparison_field", False):
                     self.has_foreign = True
```

### Comparing `beetl-0.4.6/src/beetl/sources/mongodb.py` & `beetl-0.4.7/src/beetl/sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/mysql.py` & `beetl-0.4.7/src/beetl/sources/mysql.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/postgres.py` & `beetl-0.4.7/src/beetl/sources/postgres.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/rest.py` & `beetl-0.4.7/src/beetl/sources/rest.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/sqlserver.py` & `beetl-0.4.7/src/beetl/sources/sqlserver.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/sources/static.py` & `beetl-0.4.7/src/beetl/sources/static.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/transformers/frames.py` & `beetl-0.4.7/src/beetl/transformers/frames.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/transformers/integer.py` & `beetl-0.4.7/src/beetl/transformers/integer.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/transformers/interface.py` & `beetl-0.4.7/src/beetl/transformers/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/transformers/itop.py` & `beetl-0.4.7/src/beetl/transformers/itop.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @register_transformer_class("itop")
 class ItopTransformer(TransformerInterface):
     @staticmethod
     def orgcode(data: pl.DataFrame, inFields: list, outField: str, toplevel: str):
         """Takes a number of columns, joins them and hashes the result"""
 
         def make_code(st):
-            concat_and_sha("-", toplevel, *st.values())
+            return concat_and_sha("-", toplevel, *st.values())
 
         new = data.with_columns(pl.struct(inFields).apply(make_code).alias(outField))
 
         return new
 
     @staticmethod
     def orgtree(
@@ -80,15 +80,15 @@
             pl.DataFrame: The resulting DataFrame
         """
         if not kwargs.get("sync", False):
             raise Exception(
                 "Error: include_sync option is not set for transformer itop.relations"
             )
 
-        if kwargs["sync"].destination.source_configuration.has_foreign:
+        if kwargs["sync"].destination.source_configuration.has_foreign and len(data.columns) > 1:
             transformed = data.clone()
             for field in kwargs["sync"].destination.source_configuration.columns:
                 fk_def = getattr(field, "custom_options", {})
                 if fk_def is not None:
                     fk_def = fk_def.get("itop", None)
                     if fk_def is not None:
                         try:
```

### Comparing `beetl-0.4.6/src/beetl/transformers/misc.py` & `beetl-0.4.7/src/beetl/transformers/misc.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/transformers/regex.py` & `beetl-0.4.7/src/beetl/transformers/regex.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/transformers/strings.py` & `beetl-0.4.7/src/beetl/transformers/strings.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl/transformers/structs.py` & `beetl-0.4.7/src/beetl/transformers/structs.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.6/src/beetl.egg-info/PKG-INFO` & `beetl-0.4.7/src/beetl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.6
+Version: 0.4.7
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.6/src/beetl.egg-info/SOURCES.txt` & `beetl-0.4.7/src/beetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

