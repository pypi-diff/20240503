# Comparing `tmp/beetl-0.4.4.tar.gz` & `tmp/beetl-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.4.4.tar", last modified: Fri May  3 09:38:06 2024, max compression
+gzip compressed data, was "beetl-0.4.5.tar", last modified: Fri May  3 10:53:29 2024, max compression
```

## Comparing `beetl-0.4.4.tar` & `beetl-0.4.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.739242 beetl-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-03 09:38:06.739242 beetl-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-03 09:37:15.000000 beetl-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:38:06.739242 beetl-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 09:37:15.000000 beetl-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.735242 beetl-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.735242 beetl-0.4.4/src/beetl/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/beetl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.739242 beetl-0.4.4/src/beetl/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/sqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/sources/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.739242 beetl-0.4.4/src/beetl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 09:37:15.000000 beetl-0.4.4/src/beetl/transformers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:38:06.735242 beetl-0.4.4/src/beetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:38:06.000000 beetl-0.4.4/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 10:53:29.855733 beetl-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-03 10:52:44.000000 beetl-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:53:29.855733 beetl-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 10:52:44.000000 beetl-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.851734 beetl-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.851734 beetl-0.4.5/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 10:52:44.000000 beetl-0.4.5/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:53:29.855733 beetl-0.4.5/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:53:29.000000 beetl-0.4.5/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.4.4/PKG-INFO` & `beetl-0.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.4
+Version: 0.4.5
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,16 @@
 
 After building our 16th integration between the same two systems with another manual template, we decided to build BeETL. BeETL is currently limited to one datasource per source and destination per sync, but this will be expanded in the future. One configuration can contain multiple syncs.
 
 Note: Even though most of the configuration below is in YAML format, you can also use JSON or a python dictionary.
 
 ## Todo:
 - [ ] Soft Delete/Hard Delete
+- [ ] Output table at end
+
 
 ## TOC
 - [Installation](#installation)
   - [From PyPi](#from-pypi)
   - [From Source](#from-source)
 - [Quick Start](#quick-start)
 - [Documentation](https://beetl.hoglan.dev/en/latest/)
```

### Comparing `beetl-0.4.4/README.md` & `beetl-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 After building our 16th integration between the same two systems with another manual template, we decided to build BeETL. BeETL is currently limited to one datasource per source and destination per sync, but this will be expanded in the future. One configuration can contain multiple syncs.
 
 Note: Even though most of the configuration below is in YAML format, you can also use JSON or a python dictionary.
 
 ## Todo:
 - [ ] Soft Delete/Hard Delete
+- [ ] Output table at end
+
 
 ## TOC
 - [Installation](#installation)
   - [From PyPi](#from-pypi)
   - [From Source](#from-source)
 - [Quick Start](#quick-start)
 - [Documentation](https://beetl.hoglan.dev/en/latest/)
```

### Comparing `beetl-0.4.4/setup.py` & `beetl-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/__version__.py` & `beetl-0.4.5/src/beetl/__version__.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/beetl.py` & `beetl-0.4.5/src/beetl/beetl.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,15 +160,19 @@
 
         3. Compare source and destination data with compare_datasets
 
         4. Execute the respective insert, update and delete queries
 
         """
         self.benchmark("Starting sync and retrieving source data")
-        for sync in self.config.sync_list:
+        for i, sync in enumerate(self.config.sync_list, 1):
+            if sync.name != "":
+                print(f"Starting sync: {sync.name}")
+            else:
+                print(f"Starting sync {i}")
             source_data = sync.source.query(sync.sourceConfig)
             self.benchmark("Finished data retrieval from source")
 
             destination_data = sync.destination.query(sync.destinationConfig)
             self.benchmark("Finished data retrieval from destination")
 
             self.benchmark("Starting source data transformation")
```

### Comparing `beetl-0.4.4/src/beetl/config.py` & `beetl-0.4.5/src/beetl/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,20 @@
 
         self.config = getattr(source_class, f"{source_type}SourceConfig")(**config)
 
 
 @dataclass
 class SyncConfiguration:
     """The configuration for a single sync between two sources"""
-
+    
     source: SourceSettings
     sourceConfig: SourceInterfaceConfiguration
     destination: SourceSettings
     destinationConfig: SourceInterfaceConfiguration
+    name: str = ""
     sourceTransformers: TransformerConfiguration = None
     insertionTransformers: List[TransformerConfiguration] = None
 
     def __post_init__(self) -> None:
         self.source.config = self.sourceConfig
         self.destination.config = self.destinationConfig
 
@@ -66,14 +67,28 @@
         )
 
         # Transform this class into the versioned configuration class
         self.__class__ = config_class
         self.__dict__ = config_class(config).__dict__
         self.version = config.get("configVersion", "V1")
 
+
+    @classmethod
+    def from_yaml(cls, yamlData: str) -> "BeetlConfig":
+        """Import configuration from a YAML string
+
+        Args:
+            yaml (str): The YAML string containing the configuration
+
+        Returns:
+            BeetlConfig: Beetl Configuration
+        """
+        config = yaml.safe_load(yamlData)
+        return cls(config)
+
     @classmethod
     def from_yaml_file(cls, path: str, encoding: str = "utf-8") -> "BeetlConfig":
         """Import configuration from YAML file
 
         Args:
             path (str): The path to the configuration file
             encoding (str, optional): The encoding of the file. Defaults to 'utf-8'.
@@ -90,14 +105,27 @@
                 return cls(config)
         except FileNotFoundError as e:
             raise Exception(
                 f"The configuration file was not found at the path specified ({path})."
             ) from e
 
     @classmethod
+    def from_json(cls, jsonData: str) -> "BeetlConfig":
+        """Import configuration from a JSON string
+
+        Args:
+            jsonData (str): The JSON string containing the configuration
+
+        Returns:
+            BeetlConfig: Beetl Configuration
+        """
+        config = json.loads(jsonData)
+        return cls(config)
+
+    @classmethod
     def from_json_file(cls, path: str, encoding: str = "utf-8") -> "BeetlConfig":
         """Import configuration from YAML file
 
         Args:
             path (str): The path to the configuration file
             encoding (str, optional): The encoding of the file. Defaults to 'utf-8'.
 
@@ -169,21 +197,22 @@
             ):
                 raise Exception(
                     "One of the source/destination names in "
                     "the sync section does not match a source name "
                     "in the sources section."
                     "Please check your configuration.",
                 )
-
+            
             tmpSource = copy.deepcopy(self.sources[sync["source"]])
             tmpSource.set_sourceconfig(sync["sourceConfig"])
             tmpDestination = copy.deepcopy(self.sources[sync["destination"]])
             tmpDestination.set_sourceconfig(sync["destinationConfig"])
 
             syncConfig = SyncConfiguration(
+                name=sync.get('name', ''),
                 source=tmpSource,
                 sourceConfig=sync["sourceConfig"],
                 destination=tmpDestination,
                 destinationConfig=sync["destinationConfig"],
             )
 
             tmpSource = tmpDestination = None
```

### Comparing `beetl-0.4.4/src/beetl/sources/faker.py` & `beetl-0.4.5/src/beetl/sources/faker.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/interface.py` & `beetl-0.4.5/src/beetl/sources/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/itop.py` & `beetl-0.4.5/src/beetl/sources/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/mongodb.py` & `beetl-0.4.5/src/beetl/sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/mysql.py` & `beetl-0.4.5/src/beetl/sources/mysql.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/postgres.py` & `beetl-0.4.5/src/beetl/sources/postgres.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/rest.py` & `beetl-0.4.5/src/beetl/sources/rest.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/sqlserver.py` & `beetl-0.4.5/src/beetl/sources/sqlserver.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/sources/static.py` & `beetl-0.4.5/src/beetl/sources/static.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/transformers/frames.py` & `beetl-0.4.5/src/beetl/transformers/frames.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/transformers/interface.py` & `beetl-0.4.5/src/beetl/transformers/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/transformers/itop.py` & `beetl-0.4.5/src/beetl/transformers/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/transformers/misc.py` & `beetl-0.4.5/src/beetl/transformers/misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,25 +29,7 @@
             .struct.unnest()["field_0"]
             .str.splitn("=", 2)
             .struct.unnest()["field_1"]
             .alias(outField if outField is not None else inField)
         )
 
         return data
-
-    @staticmethod
-    def divide(data: pl.DataFrame, inField: str, outField: str, factor: int) -> pl.DataFrame:
-        """Divide the numbers in a given column with the given factor
-
-        Args:
-            data (pl.DataFrame): The dataFrame to modify
-            inField (str): The field to process
-            outField (str): The field to put the output into
-            factor (int): The field to divide by
-
-        Returns:
-            pl.DataFrame: The resulting DataFrame
-        """
-        
-        data = data.with_columns((data[inField].cast(pl.Int64) / factor).alias(outField))
-        
-        return data
```

### Comparing `beetl-0.4.4/src/beetl/transformers/regex.py` & `beetl-0.4.5/src/beetl/transformers/regex.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/transformers/strings.py` & `beetl-0.4.5/src/beetl/transformers/strings.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl/transformers/structs.py` & `beetl-0.4.5/src/beetl/transformers/structs.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.4/src/beetl.egg-info/PKG-INFO` & `beetl-0.4.5/src/beetl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.4
+Version: 0.4.5
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,16 @@
 
 After building our 16th integration between the same two systems with another manual template, we decided to build BeETL. BeETL is currently limited to one datasource per source and destination per sync, but this will be expanded in the future. One configuration can contain multiple syncs.
 
 Note: Even though most of the configuration below is in YAML format, you can also use JSON or a python dictionary.
 
 ## Todo:
 - [ ] Soft Delete/Hard Delete
+- [ ] Output table at end
+
 
 ## TOC
 - [Installation](#installation)
   - [From PyPi](#from-pypi)
   - [From Source](#from-source)
 - [Quick Start](#quick-start)
 - [Documentation](https://beetl.hoglan.dev/en/latest/)
```

### Comparing `beetl-0.4.4/src/beetl.egg-info/SOURCES.txt` & `beetl-0.4.5/src/beetl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 src/beetl/sources/mysql.py
 src/beetl/sources/postgres.py
 src/beetl/sources/rest.py
 src/beetl/sources/sqlserver.py
 src/beetl/sources/static.py
 src/beetl/transformers/__init__.py
 src/beetl/transformers/frames.py
+src/beetl/transformers/integer.py
 src/beetl/transformers/interface.py
 src/beetl/transformers/itop.py
 src/beetl/transformers/misc.py
 src/beetl/transformers/regex.py
 src/beetl/transformers/strings.py
 src/beetl/transformers/structs.py
```

