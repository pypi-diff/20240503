# Comparing `tmp/sparse_dot_mkl-0.9.2.tar.gz` & `tmp/sparse_dot_mkl-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse_dot_mkl-0.9.2.tar", last modified: Sun Apr 28 15:42:21 2024, max compression
+gzip compressed data, was "sparse_dot_mkl-0.9.3.tar", last modified: Fri May  3 17:27:31 2024, max compression
```

## Comparing `sparse_dot_mkl-0.9.2.tar` & `sparse_dot_mkl-0.9.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.612030 sparse_dot_mkl-0.9.2/
--rw-rw-r--   0 chris     (1000) chris     (1000)       26 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/.codecov.yml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1823 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/.gitignore
--rw-rw-r--   0 chris     (1000) chris     (1000)     3517 2024-04-28 15:35:27.000000 sparse_dot_mkl-0.9.2/CHANGELOG.md
--rw-rw-r--   0 chris     (1000) chris     (1000)     1065 2019-12-08 21:27:09.000000 sparse_dot_mkl-0.9.2/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-04-28 15:42:21.612030 sparse_dot_mkl-0.9.2/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     5568 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)     3855 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/demo.ipynb
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-04-28 15:42:21.612030 sparse_dot_mkl-0.9.2/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     1174 2024-04-28 15:13:54.000000 sparse_dot_mkl-0.9.2/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl/
--rw-rw-r--   0 chris     (1000) chris     (1000)      207 2024-04-28 15:14:12.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3582 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_dense_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9398 2023-10-11 19:33:52.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_gram_matrix.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3537 2024-04-28 15:32:58.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    21368 2024-04-28 15:05:24.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_cfunctions.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    30604 2023-10-11 18:36:54.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_common.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2198 2024-04-28 14:01:56.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_constants.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2824 2024-04-28 13:39:36.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_load_library.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1379 2023-10-11 17:19:36.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_structs.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6377 2023-10-11 20:03:18.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4120 2022-10-23 14:59:00.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_qr_solver.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6937 2024-02-28 20:24:05.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sparse.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4454 2023-10-12 21:10:13.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sypr.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4889 2023-10-12 20:56:33.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_vector.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7658 2024-02-28 20:16:02.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/sparse_dot.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-02-01 23:31:58.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4774 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_dense_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7149 2023-10-11 20:23:52.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_gram_matrix.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11819 2023-10-11 19:56:07.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_mkl.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2744 2022-10-23 14:57:09.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_qr_solver.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13253 2023-10-11 20:19:32.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_dense.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14859 2024-02-28 20:25:09.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_sparse.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12099 2023-10-11 20:09:30.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_vector.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 15:42:21.608030 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     1155 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       12 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       15 2024-04-28 15:42:21.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2020-01-15 17:20:36.000000 sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 17:27:31.382922 sparse_dot_mkl-0.9.3/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       26 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.3/.codecov.yml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1823 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.3/.gitignore
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3699 2024-05-03 17:20:27.000000 sparse_dot_mkl-0.9.3/CHANGELOG.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1065 2019-12-08 21:27:09.000000 sparse_dot_mkl-0.9.3/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-05-03 17:27:31.382922 sparse_dot_mkl-0.9.3/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5568 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.3/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3855 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.3/demo.ipynb
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-03 17:27:31.382922 sparse_dot_mkl-0.9.3/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1174 2024-05-03 16:55:12.000000 sparse_dot_mkl-0.9.3/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 17:27:31.378922 sparse_dot_mkl-0.9.3/sparse_dot_mkl/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      452 2024-05-03 17:19:17.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3582 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_dense_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9398 2023-10-11 19:33:52.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_gram_matrix.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 17:27:31.382922 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3844 2024-05-03 17:15:16.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    23278 2024-05-03 17:19:45.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_cfunctions.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    29973 2024-05-03 17:10:50.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_common.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2198 2024-04-28 14:01:56.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_constants.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2824 2024-04-28 13:39:36.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_load_library.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1847 2024-05-03 15:35:43.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_structs.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6377 2023-10-11 20:03:18.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4120 2022-10-23 14:59:00.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_qr_solver.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6937 2024-02-28 20:24:05.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_sparse.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4454 2023-10-12 21:10:13.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_sypr.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4889 2023-10-12 20:56:33.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_vector.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7706 2024-05-03 17:16:46.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/sparse_dot.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 17:27:31.382922 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-02-01 23:31:58.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4774 2022-10-22 16:14:48.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_dense_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7149 2023-10-11 20:23:52.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_gram_matrix.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11819 2023-10-11 19:56:07.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_mkl.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2744 2022-10-23 14:57:09.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_qr_solver.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1623 2024-05-03 17:23:18.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_service.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13253 2023-10-11 20:19:32.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_sparse_dense.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14859 2024-02-28 20:25:09.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_sparse_sparse.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12099 2023-10-11 20:09:30.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_sparse_vector.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 17:27:31.382922 sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6102 2024-05-03 17:27:31.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1192 2024-05-03 17:27:31.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-03 17:27:31.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       12 2024-05-03 17:27:31.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       15 2024-05-03 17:27:31.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2020-01-15 17:20:36.000000 sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/zip-safe
```

### Comparing `sparse_dot_mkl-0.9.2/.gitignore` & `sparse_dot_mkl-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/CHANGELOG.md` & `sparse_dot_mkl-0.9.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+### Version 0.9.3
+
+* Directly expose service functions `mkl_get_max_threads`, `mkl_set_num_threads`,
+  `mkl_set_num_threads_local`, `mkl_get_version`, and `mkl_get_version_string`.
+
 ### Version 0.9.2
 
 * Explicit check for interface env MKL_INTERFACE_LAYER and interface selection in python.
   Will raise a RuntimeWarning if ILP64 is requested but the 64-bit interface layer is unavailable.
   Note that the MKL_INTERFACE_LAYER env must be set before this package is imported.
 
 ### Version 0.9.1
```

### Comparing `sparse_dot_mkl-0.9.2/LICENSE` & `sparse_dot_mkl-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/PKG-INFO` & `sparse_dot_mkl-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse_dot_mkl
-Version: 0.9.2
+Version: 0.9.3
 Summary: Intel MKL wrapper for sparse matrix multiplication
 Home-page: https://github.com/flatironinstitute/sparse_dot
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparse_dot_mkl-0.9.2/README.md` & `sparse_dot_mkl-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/demo.ipynb` & `sparse_dot_mkl-0.9.3/demo.ipynb`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/setup.py` & `sparse_dot_mkl-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from setuptools import setup, find_packages
 
 DISTNAME = 'sparse_dot_mkl'
-VERSION = '0.9.2'
+VERSION = '0.9.3'
 DESCRIPTION = "Intel MKL wrapper for sparse matrix multiplication"
 MAINTAINER = 'Chris Jackson'
 MAINTAINER_EMAIL = 'cj59@nyu.edu'
 URL = 'https://github.com/flatironinstitute/sparse_dot'
 LICENSE = 'MIT'
 
 # Description from README.md
```

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_dense_dense.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_dense_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_gram_matrix.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_gram_matrix.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/__init__.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
     MKL_Complex8,
     MKL_Complex16,
     matrix_descr,
     sparse_matrix_t
 )
 from ._cfunctions import (
     MKL,
-    mkl_set_interface_layer
+    mkl_set_interface_layer,
+    mkl_get_max_threads,
+    mkl_set_num_threads,
+    mkl_set_num_threads_local,
+    mkl_get_version,
+    mkl_get_version_string
 )
 from ._common import (
     _create_mkl_sparse,
     _export_mkl,
     _check_return_value,
     _convert_to_csr,
     _is_allowed_sparse_format,
@@ -39,22 +44,25 @@
     _output_dtypes,
     _get_numpy_layout,
     _out_matrix,
     _mkl_scalar,
     _is_dense_vector,
     print_mkl_debug,
     set_debug_mode,
-    get_version_string,
     is_csr,
     is_csc,
     is_bsr,
     sparse_output_type
 )
 
 
+def mkl_interface_integer_dtype():
+    return MKL.MKL_INT_NUMPY
+
+
 def _validate_dtype():
     """
     Test to make sure that this library works by creating arandom sparse array
     in CSC format, then converting it to CSR format and making sure is has not
     raised an exception.
     """
 
@@ -130,7 +138,12 @@
     _empirical_set_dtype()
 elif MKL.MKL_INT is None:
     _empirical_set_dtype()
 
 
 if _sklearn_env is not None:
     os.environ["KMP_INIT_AT_FORK"] = _sklearn_env
+
+if mkl_get_version()[0] < 2020:
+    _warnings.warn(
+        f"Loaded version of MKL is out of date: {mkl_get_version_string()}"
+    )
```

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_cfunctions.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_cfunctions.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import ctypes as _ctypes
 
 from sparse_dot_mkl._mkl_interface._structs import (
     sparse_matrix_t,
     matrix_descr,
     MKL_Complex8,
     MKL_Complex16,
+    MKLVersion
 )
 
 from sparse_dot_mkl._mkl_interface._load_library import (
     mkl_library
 )
 
 import numpy as _np
@@ -134,14 +135,19 @@
 
     # Import function for QR solver - solve
     _mkl_sparse_d_qr_solve = _libmkl.mkl_sparse_d_qr_solve
     _mkl_sparse_s_qr_solve = _libmkl.mkl_sparse_s_qr_solve
 
     # Set interface function
     _mkl_set_interface_layer = _libmkl.MKL_Set_Interface_Layer
+    _mkl_get_max_threads = _libmkl.MKL_Get_Max_Threads
+    _mkl_set_num_threads = _libmkl.MKL_Set_Num_Threads
+    _mkl_set_num_threads_local = _libmkl.MKL_Set_Num_Threads_Local
+    _mkl_get_version = _libmkl.MKL_Get_Version
+    _mkl_get_version_string = _libmkl.MKL_Get_Version_String
 
     @classmethod
     def _set_int_type(cls, c_type, _np_type):
         cls.MKL_INT = c_type
         cls.MKL_INT_NUMPY = _np_type
 
         cls._set_int_type_create()
@@ -569,22 +575,74 @@
             _ctypes.POINTER(prec_type),
             MKL.MKL_INT,
             ndpointer(dtype=prec_type, ndim=2),
             MKL.MKL_INT,
         ]
 
 
+# Set argtypes and return types for service functions
+# not interface dependent
 MKL._mkl_set_interface_layer.argtypes = [_ctypes.c_int]
 MKL._mkl_set_interface_layer.restypes = [_ctypes.c_int]
+MKL._mkl_get_max_threads.argtypes = None
+MKL._mkl_get_max_threads.restypes = [_ctypes.c_int]
+MKL._mkl_set_num_threads.argtypes = [_ctypes.c_int]
+MKL._mkl_set_num_threads.restypes = None
+MKL._mkl_set_num_threads_local.argtypes = [_ctypes.c_int]
+MKL._mkl_set_num_threads_local.restypes = [_ctypes.c_int]
+MKL._mkl_get_version.argtypes = [_ctypes.POINTER(MKLVersion)]
+MKL._mkl_get_version.restypes = None
+MKL._mkl_get_version_string.argtypes = [
+    _ctypes.POINTER(_ctypes.c_char * 256),
+    _ctypes.c_int
+]
+MKL._mkl_get_version_string.restypes = None
 
 
 def mkl_set_interface_layer(layer_code):
+    if layer_code not in [0, 1, 2]:
+        raise ValueError(
+            f'{layer_code} invalid argument to mkl_set_interface_layer'
+        )
+
     return MKL._mkl_set_interface_layer(layer_code)
 
 
+def mkl_get_max_threads():
+    return MKL._mkl_get_max_threads()
+
+
+def mkl_set_num_threads(n_threads):
+    MKL._mkl_set_num_threads(n_threads)
+
+
+def mkl_set_num_threads_local(n_threads):
+    return MKL._mkl_set_num_threads_local(n_threads)
+
+
+def mkl_get_version():
+    mkl_version = MKLVersion()
+    MKL._mkl_get_version(mkl_version)
+    return (
+        mkl_version.MajorVersion,
+        mkl_version.MinorVersion,
+        mkl_version.UpdateVersion,
+        mkl_version.ProductStatus.contents.value.decode(),
+        mkl_version.Build.contents.value.decode(),
+        mkl_version.Processor.contents.value.decode(),
+        mkl_version.Platform.contents.value.decode()
+    )
+
+
+def mkl_get_version_string():
+    c_str = (_ctypes.c_char * 256)()
+    MKL._mkl_get_version_string(_ctypes.byref(c_str), 256)
+    return c_str.value.decode()
+
+
 _mkl_interface_env = os.getenv('MKL_INTERFACE_LAYER')
 
 
 if MKL.MKL_INT is None and _mkl_interface_env == 'ILP64':
     mkl_set_interface_layer(MKL_INTERFACE_ILP64)
     MKL._set_int_type(_ctypes.c_longlong, _np.int64)
 elif MKL.MKL_INT is None and _mkl_interface_env == 'LP64':
```

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_common.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,42 +11,18 @@
     MKL_Complex8,
     MKL_Complex16
 )
 
 import numpy as _np
 import ctypes as _ctypes
 from scipy import sparse as _spsparse
-import warnings
 import time
 
 from numpy.ctypeslib import as_array
 
-# Use mkl-service to check version if it's installed
-# Since it's not on PyPi I don't want to make this an actual package dependency
-# So without it just create mock functions and don't do version checking
-try:
-    from mkl import get_version, get_version_string, get_max_threads
-except ImportError:
-
-    def get_version():
-        return None
-
-    def get_version_string():
-        return None
-
-    def get_max_threads():
-        return None
-
-
-if get_version() is not None and get_version()["MajorVersion"] < 2020:
-    warnings.warn(
-        f"Loaded version of MKL is out of date: {get_version_string()}"
-    )
-
-
 # Dict keyed by ('sparse_type_str', 'double_precision_bool', 'complex_bool')
 _create_functions = {
     ("csr", False, False): MKL._mkl_sparse_s_create_csr,
     ("csr", True, False): MKL._mkl_sparse_d_create_csr,
     ("csr", False, True): MKL._mkl_sparse_c_create_csr,
     ("csr", True, True): MKL._mkl_sparse_z_create_csr,
     ("csc", False, False): MKL._mkl_sparse_s_create_csc,
```

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_constants.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_constants.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_load_library.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_load_library.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_mkl_interface/_structs.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_mkl_interface/_structs.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,7 +54,23 @@
     ]
 
     def __init__(self, cplx):
         super(MKL_Complex16, self).__init__(
             cplx.real,
             cplx.imag
         )
+
+
+# MKLVersion Struct
+# For mkl_get_version
+
+class MKLVersion(_ctypes.Structure):
+
+    _fields_ = [
+        ('MajorVersion', _ctypes.c_int),
+        ('MinorVersion', _ctypes.c_int),
+        ('UpdateVersion', _ctypes.c_int),
+        ('ProductStatus', _ctypes.POINTER(_ctypes.c_char*128)),
+        ('Build', _ctypes.POINTER(_ctypes.c_char*128)),
+        ('Processor', _ctypes.POINTER(_ctypes.c_char*128)),
+        ('Platform', _ctypes.POINTER(_ctypes.c_char*128))
+    ]
```

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_dense.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_qr_solver.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_qr_solver.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sparse.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_sparse.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_sypr.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_sypr.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/_sparse_vector.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/_sparse_vector.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/sparse_dot.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/sparse_dot.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sparse_dot_mkl._sparse_vector import _sparse_dot_vector as _sdv
 from sparse_dot_mkl._gram_matrix import _gram_matrix as _gm
 from sparse_dot_mkl._sparse_qr_solver import sparse_qr_solver as _qrs
 from sparse_dot_mkl._mkl_interface import (
     print_mkl_debug,
     _is_dense_vector,
     set_debug_mode,
-    get_version_string,
+    mkl_get_version_string,
 )
 import scipy.sparse as _spsparse
 import numpy as _np
 import warnings
 
 
 def dot_product_mkl(
@@ -246,7 +246,8 @@
     print_mkl_debug()
 
     return _qrs(matrix_a, matrix_b, cast=cast)
 
 
 # Alias for backwards compatibility
 dot_product_transpose_mkl = gram_matrix_mkl
+get_version_string = mkl_get_version_string
```

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_dense_dense.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_dense_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_gram_matrix.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_gram_matrix.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_mkl.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_mkl.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_qr_solver.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_qr_solver.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_dense.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_sparse_dense.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_sparse.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_sparse_sparse.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl/tests/test_sparse_vector.py` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl/tests/test_sparse_vector.py`

 * *Files identical despite different names*

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/PKG-INFO` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse_dot_mkl
-Version: 0.9.2
+Version: 0.9.3
 Summary: Intel MKL wrapper for sparse matrix multiplication
 Home-page: https://github.com/flatironinstitute/sparse_dot
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparse_dot_mkl-0.9.2/sparse_dot_mkl.egg-info/SOURCES.txt` & `sparse_dot_mkl-0.9.3/sparse_dot_mkl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,11 @@
 sparse_dot_mkl/_mkl_interface/_load_library.py
 sparse_dot_mkl/_mkl_interface/_structs.py
 sparse_dot_mkl/tests/__init__.py
 sparse_dot_mkl/tests/test_dense_dense.py
 sparse_dot_mkl/tests/test_gram_matrix.py
 sparse_dot_mkl/tests/test_mkl.py
 sparse_dot_mkl/tests/test_qr_solver.py
+sparse_dot_mkl/tests/test_service.py
 sparse_dot_mkl/tests/test_sparse_dense.py
 sparse_dot_mkl/tests/test_sparse_sparse.py
 sparse_dot_mkl/tests/test_sparse_vector.py
```

