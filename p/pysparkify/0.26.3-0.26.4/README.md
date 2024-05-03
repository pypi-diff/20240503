# Comparing `tmp/pysparkify-0.26.3.tar.gz` & `tmp/pysparkify-0.26.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.26.3.tar", last modified: Wed May  1 15:48:49 2024, max compression
+gzip compressed data, was "pysparkify-0.26.4.tar", last modified: Fri May  3 06:09:51 2024, max compression
```

## Comparing `pysparkify-0.26.3.tar` & `pysparkify-0.26.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.817455 pysparkify-0.26.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-01 15:48:49.817455 pysparkify-0.26.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-01 15:48:46.000000 pysparkify-0.26.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/redshift_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/s3_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/redshift_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/s3_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.817455 pysparkify-0.26.3/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:48:49.817455 pysparkify-0.26.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 15:48:46.000000 pysparkify-0.26.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.817455 pysparkify-0.26.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 15:48:46.000000 pysparkify-0.26.3/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:51.255748 pysparkify-0.26.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-03 06:09:51.255748 pysparkify-0.26.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-03 06:09:48.000000 pysparkify-0.26.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:51.251748 pysparkify-0.26.4/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:51.251748 pysparkify-0.26.4/lib/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/sink/redshift_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/sink/s3_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:51.255748 pysparkify-0.26.4/lib/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/source/redshift_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/source/s3_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:51.255748 pysparkify-0.26.4/lib/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-03 06:09:48.000000 pysparkify-0.26.4/lib/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:51.255748 pysparkify-0.26.4/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-03 06:09:51.000000 pysparkify-0.26.4/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-03 06:09:51.000000 pysparkify-0.26.4/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:09:51.000000 pysparkify-0.26.4/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 06:09:51.000000 pysparkify-0.26.4/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 06:09:51.000000 pysparkify-0.26.4/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 06:09:51.000000 pysparkify-0.26.4/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:09:51.255748 pysparkify-0.26.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 06:09:48.000000 pysparkify-0.26.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:51.255748 pysparkify-0.26.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 06:09:48.000000 pysparkify-0.26.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-03 06:09:48.000000 pysparkify-0.26.4/tests/test_app.py
```

### Comparing `pysparkify-0.26.3/PKG-INFO` & `pysparkify-0.26.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.3
+Version: 0.26.4
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -91,15 +91,15 @@
 
 
 ### Usage
 
 This library can be run as a command line tool:
 
 ```bash
-pysparkify 'path/to/recipe.yml'
+pysparkify 'path/to/recipe.yml' --spark-config 'path/to/spark-config.conf'
 ```
 
 Or use it in your Python scripts:
 
 ```python
 
 from pysparkify.lib.app import run
```

### Comparing `pysparkify-0.26.3/README.md` & `pysparkify-0.26.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 
 ### Usage
 
 This library can be run as a command line tool:
 
 ```bash
-pysparkify 'path/to/recipe.yml'
+pysparkify 'path/to/recipe.yml' --spark-config 'path/to/spark-config.conf'
 ```
 
 Or use it in your Python scripts:
 
 ```python
 
 from pysparkify.lib.app import run
```

### Comparing `pysparkify-0.26.3/lib/app.py` & `pysparkify-0.26.4/lib/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import yaml
 from pyspark.sql import SparkSession
 import pyspark
 from .context_manager import get_spark_session
 from configparser import ConfigParser
 
 # import sources
-from lib.source.source_factory import SourceFactory
+from pysparkify.lib.source.source_factory import SourceFactory
 
 # import sinks
-from lib.sink.sink_factory import SinkFactory
+from pysparkify.lib.sink.sink_factory import SinkFactory
 
 # import transformers
-from lib.transformer.transformer_factory import TransformerFactory
+from pysparkify.lib.transformer.transformer_factory import TransformerFactory
 
 # Initialize lists to store sources, sinks, and transformers
 source_list = []
 sink_list = []
 transformer_list = []
 
 def instantiate_source(config):
```

### Comparing `pysparkify-0.26.3/lib/sink/redshift_sink.py` & `pysparkify-0.26.4/lib/sink/redshift_sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyspark.sql import SparkSession
-from lib.sink.sink import Sink
+from .sink import Sink
 from pyspark.sql import DataFrame
 import os
 
 class RedshiftSink(Sink):
     def __init__(self, config):
         super().__init__(config)
         self.host = os.environ.get(config['connection']['host'])
```

### Comparing `pysparkify-0.26.3/lib/sink/sink_factory.py` & `pysparkify-0.26.4/lib/sink/sink_factory.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.3/lib/source/redshift_source.py` & `pysparkify-0.26.4/lib/source/redshift_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyspark.sql import SparkSession
 import psycopg2
-from lib.source.source import Source
+from .source import Source
 from pyspark.sql.types import StructType, StructField, StringType, IntegerType, LongType, TimestampType, BooleanType
 import os
 
 class RedshiftSource(Source):
     def __init__(self, config):
         super().__init__(config)
         self.host = os.environ.get(config['connection']['host'])
```

### Comparing `pysparkify-0.26.3/lib/source/s3_source.py` & `pysparkify-0.26.4/lib/source/s3_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from lib.source.source import Source
-from lib.exceptions.source_exception import SourceException
+from pysparkify.lib.source.source import Source
 from pyspark.sql.functions import input_file_name, expr
 
 class S3Source(Source):
     def __init__(self, config):
         super().__init__(config)
         self.bucket_name = config['bucket_name']
         self.file_path = config['file_path']
```

### Comparing `pysparkify-0.26.3/lib/source/source_factory.py` & `pysparkify-0.26.4/lib/source/source_factory.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.3/lib/transformer/sql_transformer.py` & `pysparkify-0.26.4/lib/transformer/sql_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyspark.sql import SparkSession
-from lib.transformer.transformer import Transformer
+from .transformer import Transformer
 
 class SQLTransformer(Transformer):
     def __init__(self, config):
         super().__init__(config)
 
     def transform(self, spark, sources, sinks):
         # Register temporary tables from source configurations
```

### Comparing `pysparkify-0.26.3/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.26.4/pysparkify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.3
+Version: 0.26.4
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -91,15 +91,15 @@
 
 
 ### Usage
 
 This library can be run as a command line tool:
 
 ```bash
-pysparkify 'path/to/recipe.yml'
+pysparkify 'path/to/recipe.yml' --spark-config 'path/to/spark-config.conf'
 ```
 
 Or use it in your Python scripts:
 
 ```python
 
 from pysparkify.lib.app import run
```

### Comparing `pysparkify-0.26.3/pysparkify.egg-info/SOURCES.txt` & `pysparkify-0.26.4/pysparkify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.3/setup.py` & `pysparkify-0.26.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.26.3',
+    version='0.26.4',
     description='Spark based ETL',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hammad Aslam KHAN',
     author_email='raohammad@gmail.com',
     license='MIT',
     keywords=['python', 'pysparkify', 'etl', 'bigdata'],
```

### Comparing `pysparkify-0.26.3/tests/test_app.py` & `pysparkify-0.26.4/tests/test_app.py`

 * *Files identical despite different names*

