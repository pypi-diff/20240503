# Comparing `tmp/aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035.tar.gz` & `tmp/aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035.tar", max compression
+gzip compressed data, was "aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059.tar", max compression
```

## Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035.tar` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9580 2024-05-03 08:30:15.371798 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/LICENSE
--rw-r--r--   0        0        0      118 2024-05-03 08:12:09.081403 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/README.md
--rw-r--r--   0        0        0      650 2024-05-03 08:30:36.091230 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/pyproject.toml
--rw-r--r--   0        0        0      205 2024-05-03 08:12:09.081403 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/src/data_delivery_spark_py/__init__.py
--rw-r--r--   0        0        0      205 2024-05-03 08:12:09.081403 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/src/data_delivery_spark_py/test_utils/__init__.py
--rw-r--r--   0        0        0     2822 2024-05-03 08:12:09.081403 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/src/data_delivery_spark_py/test_utils/spark_session_manager.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 08:30:39.024111 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-03 08:12:09.206240 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/README.md
+-rw-r--r--   0        0        0      650 2024-05-03 08:30:59.432097 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-05-03 08:12:09.206240 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/src/data_delivery_spark_py/__init__.py
+-rw-r--r--   0        0        0      205 2024-05-03 08:12:09.206240 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/src/data_delivery_spark_py/test_utils/__init__.py
+-rw-r--r--   0        0        0     2822 2024-05-03 08:12:09.206240 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/src/data_delivery_spark_py/test_utils/spark_session_manager.py
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/PKG-INFO
```

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/LICENSE` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/pyproject.toml` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-data-delivery-spark-py"
-version = "1.7.0.dev1714725035"
+version = "1.7.0.dev1714725059"
 description = "Contains the core Python functionality of data delivery for Spark"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "data_delivery_spark_py", from="src"},
 ]
```

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/src/data_delivery_spark_py/test_utils/spark_session_manager.py` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/src/data_delivery_spark_py/test_utils/spark_session_manager.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725035/PKG-INFO` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714725059/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-data-delivery-spark-py
-Version: 1.7.0.dev1714725035
+Version: 1.7.0.dev1714725059
 Summary: Contains the core Python functionality of data delivery for Spark
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: krausening (>=19)
```

