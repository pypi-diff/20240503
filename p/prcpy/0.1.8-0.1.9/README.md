# Comparing `tmp/prcpy-0.1.8.tar.gz` & `tmp/prcpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prcpy-0.1.8.tar", max compression
+gzip compressed data, was "prcpy-0.1.9.tar", max compression
```

## Comparing `prcpy-0.1.8.tar` & `prcpy-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1093 2024-03-08 08:22:15.751514 prcpy-0.1.8/LICENSE
--rw-r--r--   0        0        0      140 2024-03-15 09:27:34.329156 prcpy-0.1.8/prcpy/__init__.py
--rw-r--r--   0        0        0      250 2024-03-15 09:17:03.396732 prcpy-0.1.8/prcpy/DataHandling/__init__.py
--rw-r--r--   0        0        0      216 2024-02-28 15:07:41.855995 prcpy-0.1.8/prcpy/DataHandling/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1352 2024-02-28 20:16:05.209813 prcpy-0.1.8/prcpy/DataHandling/__pycache__/Data_processing.cpython-312.pyc
--rw-r--r--   0        0        0     1442 2024-03-09 22:52:06.651213 prcpy-0.1.8/prcpy/DataHandling/__pycache__/File_handlers.cpython-312.pyc
--rw-r--r--   0        0        0     2073 2024-03-07 15:21:05.539598 prcpy-0.1.8/prcpy/DataHandling/__pycache__/Path_handlers.cpython-312.pyc
--rw-r--r--   0        0        0     6574 2024-02-29 17:23:15.954465 prcpy-0.1.8/prcpy/DataHandling/__pycache__/Prepare_RC_Data.cpython-312.pyc
--rw-r--r--   0        0        0      844 2024-04-26 07:51:41.899763 prcpy-0.1.8/prcpy/DataHandling/File_handlers.py
--rw-r--r--   0        0        0      995 2024-03-15 09:19:02.979875 prcpy-0.1.8/prcpy/DataHandling/Path_handlers.py
--rw-r--r--   0        0        0       75 2024-04-26 06:49:10.151222 prcpy-0.1.8/prcpy/main.py
--rw-r--r--   0        0        0      274 2024-03-15 08:57:12.605116 prcpy-0.1.8/prcpy/Maths/__init__.py
--rw-r--r--   0        0        0      209 2024-02-28 20:34:47.687901 prcpy-0.1.8/prcpy/Maths/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5388 2024-02-21 15:10:04.071777 prcpy-0.1.8/prcpy/Maths/__pycache__/FMR_maths.cpython-312.pyc
--rw-r--r--   0        0        0     1762 2024-03-07 14:50:17.460581 prcpy-0.1.8/prcpy/Maths/__pycache__/Maths_functions.cpython-312.pyc
--rw-r--r--   0        0        0     2557 2024-03-07 14:50:17.447568 prcpy-0.1.8/prcpy/Maths/__pycache__/Target_functions.cpython-312.pyc
--rw-r--r--   0        0        0      778 2024-03-07 14:46:38.951984 prcpy-0.1.8/prcpy/Maths/Maths_functions.py
--rw-r--r--   0        0        0     1362 2024-03-15 10:09:20.211072 prcpy-0.1.8/prcpy/Maths/Target_functions.py
--rw-r--r--   0        0        0      410 2024-02-21 15:00:32.272383 prcpy-0.1.8/prcpy/Maths/Utils.py
--rw-r--r--   0        0        0        0 2024-03-07 15:14:19.485022 prcpy-0.1.8/prcpy/Plots/__init__.py
--rw-r--r--   0        0        0       55 2024-03-07 15:15:16.568343 prcpy-0.1.8/prcpy/Plots/Plot_RC.py
--rw-r--r--   0        0        0      147 2024-03-15 08:49:04.886793 prcpy-0.1.8/prcpy/RC/__init__.py
--rw-r--r--   0        0        0      378 2024-04-26 06:02:15.356173 prcpy-0.1.8/prcpy/RC/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     6851 2024-03-07 17:41:07.300036 prcpy-0.1.8/prcpy/RC/__pycache__/Perform_RC.cpython-312.pyc
--rw-r--r--   0        0        0     4156 2024-04-26 06:02:15.685994 prcpy-0.1.8/prcpy/RC/__pycache__/Pipeline_RC.cpython-312.pyc
--rw-r--r--   0        0        0     9062 2024-04-26 06:02:15.805103 prcpy-0.1.8/prcpy/RC/__pycache__/Prepare_RC.cpython-312.pyc
--rw-r--r--   0        0        0     6513 2024-02-29 18:06:59.368278 prcpy-0.1.8/prcpy/RC/__pycache__/Prepare_RC_Data.cpython-312.pyc
--rw-r--r--   0        0        0     4709 2024-03-07 17:17:25.986287 prcpy-0.1.8/prcpy/RC/Perform_RC.py
--rw-r--r--   0        0        0     2300 2024-03-15 09:43:44.989223 prcpy-0.1.8/prcpy/RC/Pipeline_RC.py
--rw-r--r--   0        0        0     5820 2024-03-15 09:49:51.215974 prcpy-0.1.8/prcpy/RC/Prepare_RC.py
--rw-r--r--   0        0        0      226 2024-03-15 08:57:12.605116 prcpy-0.1.8/prcpy/TrainingModels/__init__.py
--rw-r--r--   0        0        0      218 2024-03-01 09:10:14.692243 prcpy-0.1.8/prcpy/TrainingModels/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      861 2024-03-07 15:21:05.730825 prcpy-0.1.8/prcpy/TrainingModels/__pycache__/RegressionModels.cpython-312.pyc
--rw-r--r--   0        0        0      348 2024-03-07 15:20:47.202723 prcpy-0.1.8/prcpy/TrainingModels/RegressionModels.py
--rw-r--r--   0        0        0      230 2024-03-15 09:20:52.690305 prcpy-0.1.8/prcpy/Utilities/__init__.py
--rw-r--r--   0        0        0      213 2024-02-28 14:47:01.701171 prcpy-0.1.8/prcpy/Utilities/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2480 2024-02-28 14:53:04.897348 prcpy-0.1.8/prcpy/Utilities/__pycache__/file_handling.cpython-312.pyc
--rw-r--r--   0        0        0     1048 2024-02-28 16:09:23.170036 prcpy-0.1.8/prcpy/Utilities/__pycache__/os_check.cpython-312.pyc
--rw-r--r--   0        0        0      693 2024-02-28 14:36:22.618818 prcpy-0.1.8/prcpy/Utilities/__pycache__/sorting.cpython-312.pyc
--rw-r--r--   0        0        0      555 2024-03-15 09:19:11.568206 prcpy-0.1.8/prcpy/Utilities/os_check.py
--rw-r--r--   0        0        0      183 2021-10-14 17:29:54.000000 prcpy-0.1.8/prcpy/Utilities/sorting.py
--rw-r--r--   0        0        0      386 2024-04-26 07:55:29.160701 prcpy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4835 2024-03-15 11:21:32.495183 prcpy-0.1.8/README.md
--rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 prcpy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-03-08 08:22:15.751514 prcpy-0.1.9/LICENSE
+-rw-r--r--   0        0        0      140 2024-03-15 09:27:34.329156 prcpy-0.1.9/prcpy/__init__.py
+-rw-r--r--   0        0        0      250 2024-03-15 09:17:03.396732 prcpy-0.1.9/prcpy/DataHandling/__init__.py
+-rw-r--r--   0        0        0      216 2024-02-28 15:07:41.855995 prcpy-0.1.9/prcpy/DataHandling/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1352 2024-02-28 20:16:05.209813 prcpy-0.1.9/prcpy/DataHandling/__pycache__/Data_processing.cpython-312.pyc
+-rw-r--r--   0        0        0     1442 2024-03-09 22:52:06.651213 prcpy-0.1.9/prcpy/DataHandling/__pycache__/File_handlers.cpython-312.pyc
+-rw-r--r--   0        0        0     2073 2024-03-07 15:21:05.539598 prcpy-0.1.9/prcpy/DataHandling/__pycache__/Path_handlers.cpython-312.pyc
+-rw-r--r--   0        0        0     6574 2024-02-29 17:23:15.954465 prcpy-0.1.9/prcpy/DataHandling/__pycache__/Prepare_RC_Data.cpython-312.pyc
+-rw-r--r--   0        0        0      845 2024-04-26 07:58:12.194692 prcpy-0.1.9/prcpy/DataHandling/File_handlers.py
+-rw-r--r--   0        0        0      995 2024-03-15 09:19:02.979875 prcpy-0.1.9/prcpy/DataHandling/Path_handlers.py
+-rw-r--r--   0        0        0       75 2024-04-26 06:49:10.151222 prcpy-0.1.9/prcpy/main.py
+-rw-r--r--   0        0        0      274 2024-03-15 08:57:12.605116 prcpy-0.1.9/prcpy/Maths/__init__.py
+-rw-r--r--   0        0        0      209 2024-02-28 20:34:47.687901 prcpy-0.1.9/prcpy/Maths/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5388 2024-02-21 15:10:04.071777 prcpy-0.1.9/prcpy/Maths/__pycache__/FMR_maths.cpython-312.pyc
+-rw-r--r--   0        0        0     1762 2024-03-07 14:50:17.460581 prcpy-0.1.9/prcpy/Maths/__pycache__/Maths_functions.cpython-312.pyc
+-rw-r--r--   0        0        0     2557 2024-03-07 14:50:17.447568 prcpy-0.1.9/prcpy/Maths/__pycache__/Target_functions.cpython-312.pyc
+-rw-r--r--   0        0        0      778 2024-03-07 14:46:38.951984 prcpy-0.1.9/prcpy/Maths/Maths_functions.py
+-rw-r--r--   0        0        0     1362 2024-03-15 10:09:20.211072 prcpy-0.1.9/prcpy/Maths/Target_functions.py
+-rw-r--r--   0        0        0      410 2024-02-21 15:00:32.272383 prcpy-0.1.9/prcpy/Maths/Utils.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:14:19.485022 prcpy-0.1.9/prcpy/Plots/__init__.py
+-rw-r--r--   0        0        0       55 2024-03-07 15:15:16.568343 prcpy-0.1.9/prcpy/Plots/Plot_RC.py
+-rw-r--r--   0        0        0      147 2024-03-15 08:49:04.886793 prcpy-0.1.9/prcpy/RC/__init__.py
+-rw-r--r--   0        0        0      378 2024-04-26 06:02:15.356173 prcpy-0.1.9/prcpy/RC/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     6851 2024-03-07 17:41:07.300036 prcpy-0.1.9/prcpy/RC/__pycache__/Perform_RC.cpython-312.pyc
+-rw-r--r--   0        0        0     4156 2024-04-26 06:02:15.685994 prcpy-0.1.9/prcpy/RC/__pycache__/Pipeline_RC.cpython-312.pyc
+-rw-r--r--   0        0        0     9062 2024-04-26 06:02:15.805103 prcpy-0.1.9/prcpy/RC/__pycache__/Prepare_RC.cpython-312.pyc
+-rw-r--r--   0        0        0     6513 2024-02-29 18:06:59.368278 prcpy-0.1.9/prcpy/RC/__pycache__/Prepare_RC_Data.cpython-312.pyc
+-rw-r--r--   0        0        0     4709 2024-03-07 17:17:25.986287 prcpy-0.1.9/prcpy/RC/Perform_RC.py
+-rw-r--r--   0        0        0     2300 2024-03-15 09:43:44.989223 prcpy-0.1.9/prcpy/RC/Pipeline_RC.py
+-rw-r--r--   0        0        0     5820 2024-03-15 09:49:51.215974 prcpy-0.1.9/prcpy/RC/Prepare_RC.py
+-rw-r--r--   0        0        0      226 2024-03-15 08:57:12.605116 prcpy-0.1.9/prcpy/TrainingModels/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-01 09:10:14.692243 prcpy-0.1.9/prcpy/TrainingModels/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      861 2024-03-07 15:21:05.730825 prcpy-0.1.9/prcpy/TrainingModels/__pycache__/RegressionModels.cpython-312.pyc
+-rw-r--r--   0        0        0      348 2024-03-07 15:20:47.202723 prcpy-0.1.9/prcpy/TrainingModels/RegressionModels.py
+-rw-r--r--   0        0        0      230 2024-03-15 09:20:52.690305 prcpy-0.1.9/prcpy/Utilities/__init__.py
+-rw-r--r--   0        0        0      213 2024-02-28 14:47:01.701171 prcpy-0.1.9/prcpy/Utilities/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2480 2024-02-28 14:53:04.897348 prcpy-0.1.9/prcpy/Utilities/__pycache__/file_handling.cpython-312.pyc
+-rw-r--r--   0        0        0     1048 2024-02-28 16:09:23.170036 prcpy-0.1.9/prcpy/Utilities/__pycache__/os_check.cpython-312.pyc
+-rw-r--r--   0        0        0      693 2024-02-28 14:36:22.618818 prcpy-0.1.9/prcpy/Utilities/__pycache__/sorting.cpython-312.pyc
+-rw-r--r--   0        0        0      555 2024-03-15 09:19:11.568206 prcpy-0.1.9/prcpy/Utilities/os_check.py
+-rw-r--r--   0        0        0      183 2021-10-14 17:29:54.000000 prcpy-0.1.9/prcpy/Utilities/sorting.py
+-rw-r--r--   0        0        0      386 2024-04-26 07:58:37.763905 prcpy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4835 2024-03-15 11:21:32.495183 prcpy-0.1.9/README.md
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 prcpy-0.1.9/PKG-INFO
```

### Comparing `prcpy-0.1.8/LICENSE` & `prcpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/DataHandling/__pycache__/Data_processing.cpython-312.pyc` & `prcpy-0.1.9/prcpy/DataHandling/__pycache__/Data_processing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/DataHandling/__pycache__/File_handlers.cpython-312.pyc` & `prcpy-0.1.9/prcpy/DataHandling/__pycache__/File_handlers.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/DataHandling/__pycache__/Path_handlers.cpython-312.pyc` & `prcpy-0.1.9/prcpy/DataHandling/__pycache__/Path_handlers.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/DataHandling/__pycache__/Prepare_RC_Data.cpython-312.pyc` & `prcpy-0.1.9/prcpy/DataHandling/__pycache__/Prepare_RC_Data.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/DataHandling/File_handlers.py` & `prcpy-0.1.9/prcpy/DataHandling/File_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pyarrow as pa
 from pyarrow import csv
 from ..Utilities.os_check import check_and_create_directory
 
 def load_csv(path, delimiter=','):
     try:
-        data_table = csv.read_csv(path, read_options=csv.ParseOptions(delimiter=delimiter))
+        data_table = csv.read_csv(path, parse_options=csv.ParseOptions(delimiter=delimiter))
         df = data_table.to_pandas()
         return df
     except Exception as e:
         print(f"Error loading CSV file: {e}")
         return None
 
 def save_csv(df, save_path, fname="", delimiter=','):
```

### Comparing `prcpy-0.1.8/prcpy/DataHandling/Path_handlers.py` & `prcpy-0.1.9/prcpy/DataHandling/Path_handlers.py`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Maths/__pycache__/FMR_maths.cpython-312.pyc` & `prcpy-0.1.9/prcpy/Maths/__pycache__/FMR_maths.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Maths/__pycache__/Maths_functions.cpython-312.pyc` & `prcpy-0.1.9/prcpy/Maths/__pycache__/Maths_functions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Maths/__pycache__/Target_functions.cpython-312.pyc` & `prcpy-0.1.9/prcpy/Maths/__pycache__/Target_functions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Maths/Maths_functions.py` & `prcpy-0.1.9/prcpy/Maths/Maths_functions.py`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Maths/Target_functions.py` & `prcpy-0.1.9/prcpy/Maths/Target_functions.py`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/RC/__pycache__/Perform_RC.cpython-312.pyc` & `prcpy-0.1.9/prcpy/RC/__pycache__/Perform_RC.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/RC/__pycache__/Pipeline_RC.cpython-312.pyc` & `prcpy-0.1.9/prcpy/RC/__pycache__/Pipeline_RC.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/RC/__pycache__/Prepare_RC.cpython-312.pyc` & `prcpy-0.1.9/prcpy/RC/__pycache__/Prepare_RC.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/RC/__pycache__/Prepare_RC_Data.cpython-312.pyc` & `prcpy-0.1.9/prcpy/RC/__pycache__/Prepare_RC_Data.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/RC/Perform_RC.py` & `prcpy-0.1.9/prcpy/RC/Perform_RC.py`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/RC/Pipeline_RC.py` & `prcpy-0.1.9/prcpy/RC/Pipeline_RC.py`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/RC/Prepare_RC.py` & `prcpy-0.1.9/prcpy/RC/Prepare_RC.py`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/TrainingModels/__pycache__/RegressionModels.cpython-312.pyc` & `prcpy-0.1.9/prcpy/TrainingModels/__pycache__/RegressionModels.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Utilities/__pycache__/file_handling.cpython-312.pyc` & `prcpy-0.1.9/prcpy/Utilities/__pycache__/file_handling.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Utilities/__pycache__/os_check.cpython-312.pyc` & `prcpy-0.1.9/prcpy/Utilities/__pycache__/os_check.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Utilities/__pycache__/sorting.cpython-312.pyc` & `prcpy-0.1.9/prcpy/Utilities/__pycache__/sorting.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/prcpy/Utilities/os_check.py` & `prcpy-0.1.9/prcpy/Utilities/os_check.py`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/README.md` & `prcpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `prcpy-0.1.8/PKG-INFO` & `prcpy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prcpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Oscar Lee
 Author-email: zceesjl@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

