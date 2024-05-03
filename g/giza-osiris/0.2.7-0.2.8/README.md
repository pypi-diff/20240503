# Comparing `tmp/giza_osiris-0.2.7.tar.gz` & `tmp/giza_osiris-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_osiris-0.2.7.tar", max compression
+gzip compressed data, was "giza_osiris-0.2.8.tar", max compression
```

## Comparing `giza_osiris-0.2.7.tar` & `giza_osiris-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2024-04-30 16:57:38.515500 giza_osiris-0.2.7/LICENSE
--rw-r--r--   0        0        0     1657 2024-04-30 16:57:38.515500 giza_osiris-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/__init__.py
--rw-r--r--   0        0        0     4777 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/app.py
--rw-r--r--   0        0        0     1434 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/data_converter/data_converter.py
--rw-r--r--   0        0        0     2653 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/data_converter/data_statement_generator.py
--rw-r--r--   0        0        0     1773 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/data_converter/tensor_creator.py
--rw-r--r--   0        0        0     3334 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/file_manager/cairo_data.py
--rw-r--r--   0        0        0     2087 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/file_manager/file.py
--rw-r--r--   0        0        0      948 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/data_structures.py
--rw-r--r--   0        0        0     4689 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/deserialize.py
--rw-r--r--   0        0        0      809 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/serialize.py
--rw-r--r--   0        0        0     1035 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/cairo/serde/utils.py
--rw-r--r--   0        0        0      177 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/dtypes/cairo_dtypes.py
--rw-r--r--   0        0        0      117 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/dtypes/cairo_impls.py
--rw-r--r--   0        0        0      177 2024-04-30 16:57:38.519500 giza_osiris-0.2.7/osiris/dtypes/input_output_formats.py
--rw-r--r--   0        0        0     1290 2024-04-30 16:57:38.523500 giza_osiris-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 giza_osiris-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-03 13:28:11.901027 giza_osiris-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1657 2024-05-03 13:28:11.901027 giza_osiris-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 13:28:11.905027 giza_osiris-0.2.8/osiris/__init__.py
+-rw-r--r--   0        0        0     4777 2024-05-03 13:28:11.905027 giza_osiris-0.2.8/osiris/app.py
+-rw-r--r--   0        0        0     1434 2024-05-03 13:28:11.905027 giza_osiris-0.2.8/osiris/cairo/data_converter/data_converter.py
+-rw-r--r--   0        0        0     2653 2024-05-03 13:28:11.905027 giza_osiris-0.2.8/osiris/cairo/data_converter/data_statement_generator.py
+-rw-r--r--   0        0        0     1773 2024-05-03 13:28:11.905027 giza_osiris-0.2.8/osiris/cairo/data_converter/tensor_creator.py
+-rw-r--r--   0        0        0     3334 2024-05-03 13:28:11.905027 giza_osiris-0.2.8/osiris/cairo/file_manager/cairo_data.py
+-rw-r--r--   0        0        0     2087 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/cairo/file_manager/file.py
+-rw-r--r--   0        0        0      948 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/cairo/serde/data_structures.py
+-rw-r--r--   0        0        0     4689 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/cairo/serde/deserialize.py
+-rw-r--r--   0        0        0      913 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/cairo/serde/serialize.py
+-rw-r--r--   0        0        0     1035 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/cairo/serde/utils.py
+-rw-r--r--   0        0        0      177 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/dtypes/cairo_dtypes.py
+-rw-r--r--   0        0        0      117 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/dtypes/cairo_impls.py
+-rw-r--r--   0        0        0      177 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/osiris/dtypes/input_output_formats.py
+-rw-r--r--   0        0        0     1290 2024-05-03 13:28:11.909027 giza_osiris-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 giza_osiris-0.2.8/PKG-INFO
```

### Comparing `giza_osiris-0.2.7/LICENSE` & `giza_osiris-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/README.md` & `giza_osiris-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/app.py` & `giza_osiris-0.2.8/osiris/app.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/data_converter/data_converter.py` & `giza_osiris-0.2.8/osiris/cairo/data_converter/data_converter.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/data_converter/data_statement_generator.py` & `giza_osiris-0.2.8/osiris/cairo/data_converter/data_statement_generator.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/data_converter/tensor_creator.py` & `giza_osiris-0.2.8/osiris/cairo/data_converter/tensor_creator.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/file_manager/cairo_data.py` & `giza_osiris-0.2.8/osiris/cairo/file_manager/cairo_data.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/file_manager/file.py` & `giza_osiris-0.2.8/osiris/cairo/file_manager/file.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/serde/data_structures.py` & `giza_osiris-0.2.8/osiris/cairo/serde/data_structures.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/serde/deserialize.py` & `giza_osiris-0.2.8/osiris/cairo/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/osiris/cairo/serde/serialize.py` & `giza_osiris-0.2.8/osiris/cairo/serde/serialize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 from osiris.cairo.serde.data_structures import (
     FixedPoint,
     Int,
     Tensor,
 )
 from osiris.cairo.serde.utils import int_to_felt
 
@@ -12,14 +14,15 @@
     elif isinstance(data, int):
             return f"{int_to_felt(data)}"
     elif isinstance(data, Int):
             return f"{int_to_felt(data.val)}"
     elif isinstance(data, (list, tuple)):
         joined_elements = ' '.join(serializer(e) for e in data)
         return f"[{joined_elements}]"
+    elif isinstance(data, np.ndarray):
+        return f"{serializer(data.tolist())}"
     elif isinstance(data, Tensor):
         return f"{serializer(data.shape)} {serializer(data.data)}"
     elif isinstance(data, FixedPoint):
         return f"{serializer(data.mag)} {serializer(data.sign)}"
-
     else:
         raise ValueError("Unsupported data type for serialization")
```

### Comparing `giza_osiris-0.2.7/osiris/cairo/serde/utils.py` & `giza_osiris-0.2.8/osiris/cairo/serde/utils.py`

 * *Files identical despite different names*

### Comparing `giza_osiris-0.2.7/pyproject.toml` & `giza_osiris-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-osiris"
-version = "0.2.7"
+version = "0.2.8"
 description = "Osiris is a Python library designed for efficient data conversion and management, primarily transforming data into Cairo programs"
 authors = ["Fran Algaba <fran@gizatech.xyz>"]
 readme = "README.md"
 packages = [{include = "osiris"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `giza_osiris-0.2.7/PKG-INFO` & `giza_osiris-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-osiris
-Version: 0.2.7
+Version: 0.2.8
 Summary: Osiris is a Python library designed for efficient data conversion and management, primarily transforming data into Cairo programs
 Author: Fran Algaba
 Author-email: fran@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

