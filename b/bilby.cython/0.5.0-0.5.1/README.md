# Comparing `tmp/bilby_cython-0.5.0.tar.gz` & `tmp/bilby_cython-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilby_cython-0.5.0.tar", last modified: Wed Apr 17 13:36:39 2024, max compression
+gzip compressed data, was "bilby_cython-0.5.1.tar", last modified: Thu May  2 22:10:02 2024, max compression
```

## Comparing `bilby_cython-0.5.0.tar` & `bilby_cython-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:36:39.407165 bilby_cython-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-17 08:04:24.000000 bilby_cython-0.5.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5310 2024-04-17 13:34:31.000000 bilby_cython-0.5.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1068 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4516 2024-04-17 13:36:39.406165 bilby_cython-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3879 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:36:39.405165 bilby_cython-0.5.0/bilby.cython.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4516 2024-04-17 13:36:39.000000 bilby_cython-0.5.0/bilby.cython.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-17 13:36:39.000000 bilby_cython-0.5.0/bilby.cython.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 13:36:39.000000 bilby_cython-0.5.0/bilby.cython.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-17 13:36:39.000000 bilby_cython-0.5.0/bilby.cython.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-17 13:36:39.000000 bilby_cython-0.5.0/bilby.cython.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:36:39.401165 bilby_cython-0.5.0/bilby_cython/
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-17 08:04:24.000000 bilby_cython-0.5.0/bilby_cython/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-17 13:36:38.000000 bilby_cython-0.5.0/bilby_cython/_version.py
--rw-r--r--   0 root         (0) root         (0)  1317670 2024-04-17 13:36:36.000000 bilby_cython-0.5.0/bilby_cython/geometry.c
--rw-rw-rw-   0 root         (0) root         (0)    15187 2024-04-17 08:04:24.000000 bilby_cython-0.5.0/bilby_cython/geometry.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:36:39.403165 bilby_cython-0.5.0/bilby_cython/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 13:34:31.000000 bilby_cython-0.5.0/bilby_cython/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6963 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/bilby_cython/test/old_code.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2024-04-17 08:04:24.000000 bilby_cython-0.5.0/bilby_cython/test/test_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     1617 2024-04-17 12:30:26.000000 bilby_cython-0.5.0/bilby_cython/test/test_time.py
--rw-rw-rw-   0 root         (0) root         (0)     4874 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/bilby_cython/test/timing.py
--rw-r--r--   0 root         (0) root         (0)  1258545 2024-04-17 13:36:37.000000 bilby_cython-0.5.0/bilby_cython/time.c
--rw-rw-rw-   0 root         (0) root         (0)     3488 2024-04-17 12:30:26.000000 bilby_cython-0.5.0/bilby_cython/time.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:36:39.405165 bilby_cython-0.5.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      605 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5606 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/docs/geometry.rst
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-15 18:25:19.000000 bilby_cython-0.5.0/docs/time.rst
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-04-17 13:34:31.000000 bilby_cython-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 13:36:39.407165 bilby_cython-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-17 08:04:24.000000 bilby_cython-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 22:10:02.548772 bilby_cython-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5291 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4567 2024-05-02 22:10:02.548772 bilby_cython-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 22:10:02.547773 bilby_cython-0.5.1/bilby.cython.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4567 2024-05-02 22:10:02.000000 bilby_cython-0.5.1/bilby.cython.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      669 2024-05-02 22:10:02.000000 bilby_cython-0.5.1/bilby.cython.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 22:10:02.000000 bilby_cython-0.5.1/bilby.cython.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-02 22:10:02.000000 bilby_cython-0.5.1/bilby.cython.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-02 22:10:02.000000 bilby_cython-0.5.1/bilby.cython.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 22:10:02.545772 bilby_cython-0.5.1/bilby_cython/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-02 22:10:02.000000 bilby_cython-0.5.1/bilby_cython/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/conftest.py
+-rw-r--r--   0 root         (0) root         (0)  1317670 2024-05-02 22:09:59.000000 bilby_cython-0.5.1/bilby_cython/geometry.c
+-rw-rw-rw-   0 root         (0) root         (0)    15187 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/geometry.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 22:10:02.546772 bilby_cython-0.5.1/bilby_cython/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 22:09:34.000000 bilby_cython-0.5.1/bilby_cython/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6963 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/test/old_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/test/test_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/test/test_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     4874 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/test/timing.py
+-rw-r--r--   0 root         (0) root         (0)  1309342 2024-05-02 22:10:01.000000 bilby_cython-0.5.1/bilby_cython/time.c
+-rw-rw-rw-   0 root         (0) root         (0)     3516 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/bilby_cython/time.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 22:10:02.547773 bilby_cython-0.5.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/docs/geometry.rst
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/docs/time.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 22:10:02.548772 bilby_cython-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-05-02 21:59:09.000000 bilby_cython-0.5.1/setup.py
```

### Comparing `bilby_cython-0.5.0/.gitlab-ci.yml` & `bilby_cython-0.5.1/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     - *install-local
     - *basic-tests
 
 unit-tests:
   stage: test
   parallel:
     matrix:
-      - PY_VERSION: [ "3.8", "3.9", "3.10", "3.11" ]
+      - PY_VERSION: [ "3.8", "3.9", "3.10", "3.11", "3.12" ]
   image: $IMAGE_ROOT:$PY_VERSION
   before_script:
     - python -m pip install --upgrade pip setuptools
     - python -m pip install Cython numpy
     - python -m pip install pytest-cov
     - python -m pip install bilby
     - python -m pip install lalsuite astropy
@@ -107,15 +107,15 @@
   - python -m pip install oldest-supported-numpy Cython
 
 # job template for wheel builds
 .wheel:
   stage: wheels
   parallel:
     matrix:
-      - PY_VERSION: [ "38", "39", "310", "311" ]
+      - PY_VERSION: [ "38", "39", "310", "311", "312" ]
   except:
     variables:
       # allow these jobs to be skipped by including
       # `[skip wheels]` in the commit message
       - $CI_COMMIT_MESSAGE =~ /\[skip wheels\]/
   artifacts:
     expire_in: 18h
@@ -159,15 +159,15 @@
     - tags
     - schedules
 
 # Build wheels for all supported platforms
 wheel:manylinux2014:
   extends:
     - .wheel:manylinux
-  image: containers.ligo.org/lscsoft/lalsuite-manylinux/manylinux2014_x86_64
+  image: quay.io/pypa/manylinux2014_x86_64
 
 build-dist:
   stage: wheels
   image: $PRIMARY_IMAGE
   except:
     variables:
       # allow these jobs to be skipped by including
```

### Comparing `bilby_cython-0.5.0/CONTRIBUTING.md` & `bilby_cython-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/LICENSE` & `bilby_cython-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/PKG-INFO` & `bilby_cython-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: bilby.cython
-Version: 0.5.0
+Version: 0.5.1
 Summary: Optimized functionality for Bilby
 Author-email: Colm Talbot <colm.talbot@ligo.org>
 License: MIT
 Project-URL: Homepage, https://git.ligo.org/colm.talbot/bilby-cython
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `bilby_cython-0.5.0/README.md` & `bilby_cython-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/bilby.cython.egg-info/PKG-INFO` & `bilby_cython-0.5.1/bilby.cython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: bilby.cython
-Version: 0.5.0
+Version: 0.5.1
 Summary: Optimized functionality for Bilby
 Author-email: Colm Talbot <colm.talbot@ligo.org>
 License: MIT
 Project-URL: Homepage, https://git.ligo.org/colm.talbot/bilby-cython
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `bilby_cython-0.5.0/bilby.cython.egg-info/SOURCES.txt` & `bilby_cython-0.5.1/bilby.cython.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 bilby.cython.egg-info/PKG-INFO
 bilby.cython.egg-info/SOURCES.txt
 bilby.cython.egg-info/dependency_links.txt
 bilby.cython.egg-info/requires.txt
 bilby.cython.egg-info/top_level.txt
 bilby_cython/__init__.py
 bilby_cython/_version.py
+bilby_cython/conftest.py
 bilby_cython/geometry.c
 bilby_cython/geometry.pyx
 bilby_cython/time.c
 bilby_cython/time.pyx
 bilby_cython/test/__init__.py
 bilby_cython/test/old_code.py
 bilby_cython/test/test_geometry.py
```

### Comparing `bilby_cython-0.5.0/bilby_cython/geometry.c` & `bilby_cython-0.5.1/bilby_cython/geometry.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/core/include"
+            "/tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "bilby_cython.geometry",
         "sources": [
             "bilby_cython/geometry.pyx"
         ]
     },
     "module_name": "bilby_cython.geometry"
@@ -1669,177 +1669,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1872,42 +1872,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18177,261 +18177,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18440,29 +18440,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18473,15 +18473,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18490,29 +18490,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18523,15 +18523,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18540,29 +18540,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18573,15 +18573,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18590,29 +18590,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18623,15 +18623,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18640,29 +18640,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18673,217 +18673,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18899,15 +18899,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18915,68 +18915,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18984,15 +18984,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19007,15 +19007,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19031,15 +19031,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19047,68 +19047,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19116,15 +19116,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19139,15 +19139,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19163,15 +19163,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19179,68 +19179,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19248,15 +19248,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19271,170 +19271,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25308,26 +25308,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `bilby_cython-0.5.0/bilby_cython/geometry.pyx` & `bilby_cython-0.5.1/bilby_cython/geometry.pyx`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/bilby_cython/test/old_code.py` & `bilby_cython-0.5.1/bilby_cython/test/old_code.py`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/bilby_cython/test/test_geometry.py` & `bilby_cython-0.5.1/bilby_cython/test/test_geometry.py`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/bilby_cython/test/test_time.py` & `bilby_cython-0.5.1/bilby_cython/test/test_time.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,38 +2,51 @@
 
 import lal
 import numpy as np
 from astropy.time import Time
 from bilby_cython.time import (
     greenwich_sidereal_time,
     greenwich_mean_sidereal_time,
+    gps_time_to_utc,
+    utc_to_julian_day,
 )
 
 
-def test_gmst():
-    times = np.random.uniform(1325623903, 1345623903, 100000)
+def test_gps_time_to_julian_day(types):
+    times = np.random.uniform(1325623903, 1345623903, 100000).astype(types)
+    diffs = list()
+    for tt in times:
+        diffs.append(
+            utc_to_julian_day(gps_time_to_utc(tt))
+            - lal.JulianDay(lal.GPSToUTC(int(tt)))
+        )
+    assert max(np.abs(diffs)) < 1e-10
+
+
+def test_gmst(types):
+    times = np.random.uniform(1325623903, 1345623903, 100000).astype(types)
     diffs = list()
     for tt in times:
         diffs.append(
             greenwich_mean_sidereal_time(tt)
             - lal.GreenwichMeanSiderealTime(tt)
         )
     assert max(np.abs(diffs)) < 1e-10
 
 
-def test_gmst_vectorized():
-    times = np.random.uniform(1325623903, 1345623903, 100000)
+def test_gmst_vectorized(types):
+    times = np.random.uniform(1325623903, 1345623903, 100000).astype(types)
     diffs = list()
     cy_gmst = greenwich_mean_sidereal_time(times)
     lal_gmst = np.array([lal.GreenwichMeanSiderealTime(tt) for tt in times])
     assert max(np.abs(cy_gmst - lal_gmst)) < 1e-10
 
 
-def test_gmt():
-    times = np.random.uniform(1325623903, 1345623903, 100000)
+def test_gmt(types):
+    times = np.random.uniform(1325623903, 1345623903, 100000).astype(types)
     equinoxes = np.random.uniform(0, 2 * np.pi, 100000)
     diffs = list()
     for tt, eq in zip(times, equinoxes):
         diffs.append(
             greenwich_sidereal_time(tt, eq)
             - lal.GreenwichSiderealTime(tt, eq)
         )
```

### Comparing `bilby_cython-0.5.0/bilby_cython/test/timing.py` & `bilby_cython-0.5.1/bilby_cython/test/timing.py`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/bilby_cython/time.c` & `bilby_cython-0.5.1/bilby_cython/time.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "include_dirs": [
-            "/tmp/build-env-26hbsek_/lib/python3.9/site-packages/numpy/core/include"
+            "/tmp/build-env-vt3gxg9a/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "bilby_cython.time",
         "sources": [
             "bilby_cython/time.pyx"
         ]
     },
     "module_name": "bilby_cython.time"
@@ -2468,21 +2468,14 @@
 /* HasAttr.proto */
 #if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
 #define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
 #else
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 #endif
 
-/* PyIntFromDouble.proto */
-#if PY_MAJOR_VERSION < 3
-static CYTHON_INLINE PyObject* __Pyx_PyInt_FromDouble(double value);
-#else
-#define __Pyx_PyInt_FromDouble(value) PyLong_FromDouble(value)
-#endif
-
 /* PyFloatBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyFloat_TrueDivideObjC(PyObject *op1, PyObject *op2, double floatval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyFloat_TrueDivideObjC(op1, op2, floatval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceTrueDivide(op1, op2) : PyNumber_TrueDivide(op1, op2))
 #endif
@@ -2815,29 +2808,33 @@
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
 static double __pyx_f_12bilby_cython_4time_utc_to_julian_day(PyDateTime_DateTime *); /*proto*/
 static int __pyx_fuse_0__pyx_f_12bilby_cython_4time_n_leap_seconds(short); /*proto*/
 static int __pyx_fuse_1__pyx_f_12bilby_cython_4time_n_leap_seconds(int); /*proto*/
 static int __pyx_fuse_2__pyx_f_12bilby_cython_4time_n_leap_seconds(long); /*proto*/
 static int __pyx_fuse_3__pyx_f_12bilby_cython_4time_n_leap_seconds(float); /*proto*/
 static int __pyx_fuse_4__pyx_f_12bilby_cython_4time_n_leap_seconds(double); /*proto*/
+static int __pyx_fuse_5__pyx_f_12bilby_cython_4time_n_leap_seconds(long double); /*proto*/
 static PyDateTime_DateTime *__pyx_fuse_0__pyx_f_12bilby_cython_4time_gps_time_to_utc(short); /*proto*/
 static PyDateTime_DateTime *__pyx_fuse_1__pyx_f_12bilby_cython_4time_gps_time_to_utc(int); /*proto*/
 static PyDateTime_DateTime *__pyx_fuse_2__pyx_f_12bilby_cython_4time_gps_time_to_utc(long); /*proto*/
 static PyDateTime_DateTime *__pyx_fuse_3__pyx_f_12bilby_cython_4time_gps_time_to_utc(float); /*proto*/
 static PyDateTime_DateTime *__pyx_fuse_4__pyx_f_12bilby_cython_4time_gps_time_to_utc(double); /*proto*/
-static PyObject *__pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(short); /*proto*/
-static PyObject *__pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(int); /*proto*/
-static PyObject *__pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(long); /*proto*/
-static PyObject *__pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(float); /*proto*/
-static PyObject *__pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(double); /*proto*/
-static PyObject *__pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(short, short); /*proto*/
-static PyObject *__pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(int, int); /*proto*/
-static PyObject *__pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(long, long); /*proto*/
-static PyObject *__pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(float, float); /*proto*/
-static PyObject *__pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(double, double); /*proto*/
+static PyDateTime_DateTime *__pyx_fuse_5__pyx_f_12bilby_cython_4time_gps_time_to_utc(long double); /*proto*/
+static double __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(short); /*proto*/
+static double __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(int); /*proto*/
+static double __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(long); /*proto*/
+static double __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(float); /*proto*/
+static double __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(double); /*proto*/
+static double __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(long double); /*proto*/
+static double __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(short, short); /*proto*/
+static double __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(int, int); /*proto*/
+static double __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(long, long); /*proto*/
+static double __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(float, float); /*proto*/
+static double __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(double, double); /*proto*/
+static double __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(long double, long double); /*proto*/
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static int assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
 static struct __pyx_memoryview_obj *__pyx_memview_slice(struct __pyx_memoryview_obj *, PyObject *); /*proto*/
@@ -19699,69 +19696,69 @@
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "bilby_cython/time.pyx":40
+/* "bilby_cython/time.pyx":41
  * 
  * @cython.ufunc
  * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
  *     """
  *     Find the number of leap seconds required for the specified date.
  */
 
 static int __pyx_fuse_0__pyx_f_12bilby_cython_4time_n_leap_seconds(short __pyx_v_date) {
   int __pyx_v_n_leaps;
   int __pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "bilby_cython/time.pyx":47
+  /* "bilby_cython/time.pyx":48
  *     be after the most recent leap.
  *     """
  *     cdef int n_leaps = NUM_LEAPS             # <<<<<<<<<<<<<<
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  */
   __pyx_v_n_leaps = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
 
-  /* "bilby_cython/time.pyx":48
+  /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   __pyx_t_1 = (__pyx_v_12bilby_cython_4time_NUM_LEAPS - 1);
   __pyx_t_2 = (__pyx_v_date > (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
   if (__pyx_t_2) {
 
-    /* "bilby_cython/time.pyx":49
+    /* "bilby_cython/time.pyx":50
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS             # <<<<<<<<<<<<<<
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  */
     __pyx_r = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
     goto __pyx_L0;
 
-    /* "bilby_cython/time.pyx":48
+    /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   }
 
-  /* "bilby_cython/time.pyx":50
+  /* "bilby_cython/time.pyx":51
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):             # <<<<<<<<<<<<<<
  *         n_leaps -= 1
  *     return n_leaps
  */
   while (1) {
@@ -19773,35 +19770,35 @@
     }
     __pyx_t_1 = (__pyx_v_n_leaps - 1);
     __pyx_t_3 = (__pyx_v_date < (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
     __pyx_t_2 = __pyx_t_3;
     __pyx_L6_bool_binop_done:;
     if (!__pyx_t_2) break;
 
-    /* "bilby_cython/time.pyx":51
+    /* "bilby_cython/time.pyx":52
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1             # <<<<<<<<<<<<<<
  *     return n_leaps
  * 
  */
     __pyx_v_n_leaps = (__pyx_v_n_leaps - 1);
   }
 
-  /* "bilby_cython/time.pyx":52
+  /* "bilby_cython/time.pyx":53
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  *     return n_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_n_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":40
+  /* "bilby_cython/time.pyx":41
  * 
  * @cython.ufunc
  * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
  *     """
  *     Find the number of leap seconds required for the specified date.
  */
 
@@ -19813,54 +19810,54 @@
 static int __pyx_fuse_1__pyx_f_12bilby_cython_4time_n_leap_seconds(int __pyx_v_date) {
   int __pyx_v_n_leaps;
   int __pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "bilby_cython/time.pyx":47
+  /* "bilby_cython/time.pyx":48
  *     be after the most recent leap.
  *     """
  *     cdef int n_leaps = NUM_LEAPS             # <<<<<<<<<<<<<<
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  */
   __pyx_v_n_leaps = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
 
-  /* "bilby_cython/time.pyx":48
+  /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   __pyx_t_1 = (__pyx_v_12bilby_cython_4time_NUM_LEAPS - 1);
   __pyx_t_2 = (__pyx_v_date > (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
   if (__pyx_t_2) {
 
-    /* "bilby_cython/time.pyx":49
+    /* "bilby_cython/time.pyx":50
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS             # <<<<<<<<<<<<<<
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  */
     __pyx_r = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
     goto __pyx_L0;
 
-    /* "bilby_cython/time.pyx":48
+    /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   }
 
-  /* "bilby_cython/time.pyx":50
+  /* "bilby_cython/time.pyx":51
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):             # <<<<<<<<<<<<<<
  *         n_leaps -= 1
  *     return n_leaps
  */
   while (1) {
@@ -19872,35 +19869,35 @@
     }
     __pyx_t_1 = (__pyx_v_n_leaps - 1);
     __pyx_t_3 = (__pyx_v_date < (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
     __pyx_t_2 = __pyx_t_3;
     __pyx_L6_bool_binop_done:;
     if (!__pyx_t_2) break;
 
-    /* "bilby_cython/time.pyx":51
+    /* "bilby_cython/time.pyx":52
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1             # <<<<<<<<<<<<<<
  *     return n_leaps
  * 
  */
     __pyx_v_n_leaps = (__pyx_v_n_leaps - 1);
   }
 
-  /* "bilby_cython/time.pyx":52
+  /* "bilby_cython/time.pyx":53
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  *     return n_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_n_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":40
+  /* "bilby_cython/time.pyx":41
  * 
  * @cython.ufunc
  * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
  *     """
  *     Find the number of leap seconds required for the specified date.
  */
 
@@ -19912,54 +19909,54 @@
 static int __pyx_fuse_2__pyx_f_12bilby_cython_4time_n_leap_seconds(long __pyx_v_date) {
   int __pyx_v_n_leaps;
   int __pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "bilby_cython/time.pyx":47
+  /* "bilby_cython/time.pyx":48
  *     be after the most recent leap.
  *     """
  *     cdef int n_leaps = NUM_LEAPS             # <<<<<<<<<<<<<<
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  */
   __pyx_v_n_leaps = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
 
-  /* "bilby_cython/time.pyx":48
+  /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   __pyx_t_1 = (__pyx_v_12bilby_cython_4time_NUM_LEAPS - 1);
   __pyx_t_2 = (__pyx_v_date > (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
   if (__pyx_t_2) {
 
-    /* "bilby_cython/time.pyx":49
+    /* "bilby_cython/time.pyx":50
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS             # <<<<<<<<<<<<<<
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  */
     __pyx_r = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
     goto __pyx_L0;
 
-    /* "bilby_cython/time.pyx":48
+    /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   }
 
-  /* "bilby_cython/time.pyx":50
+  /* "bilby_cython/time.pyx":51
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):             # <<<<<<<<<<<<<<
  *         n_leaps -= 1
  *     return n_leaps
  */
   while (1) {
@@ -19971,35 +19968,35 @@
     }
     __pyx_t_1 = (__pyx_v_n_leaps - 1);
     __pyx_t_3 = (__pyx_v_date < (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
     __pyx_t_2 = __pyx_t_3;
     __pyx_L6_bool_binop_done:;
     if (!__pyx_t_2) break;
 
-    /* "bilby_cython/time.pyx":51
+    /* "bilby_cython/time.pyx":52
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1             # <<<<<<<<<<<<<<
  *     return n_leaps
  * 
  */
     __pyx_v_n_leaps = (__pyx_v_n_leaps - 1);
   }
 
-  /* "bilby_cython/time.pyx":52
+  /* "bilby_cython/time.pyx":53
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  *     return n_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_n_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":40
+  /* "bilby_cython/time.pyx":41
  * 
  * @cython.ufunc
  * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
  *     """
  *     Find the number of leap seconds required for the specified date.
  */
 
@@ -20011,54 +20008,54 @@
 static int __pyx_fuse_3__pyx_f_12bilby_cython_4time_n_leap_seconds(float __pyx_v_date) {
   int __pyx_v_n_leaps;
   int __pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "bilby_cython/time.pyx":47
+  /* "bilby_cython/time.pyx":48
  *     be after the most recent leap.
  *     """
  *     cdef int n_leaps = NUM_LEAPS             # <<<<<<<<<<<<<<
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  */
   __pyx_v_n_leaps = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
 
-  /* "bilby_cython/time.pyx":48
+  /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   __pyx_t_1 = (__pyx_v_12bilby_cython_4time_NUM_LEAPS - 1);
   __pyx_t_2 = (__pyx_v_date > (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
   if (__pyx_t_2) {
 
-    /* "bilby_cython/time.pyx":49
+    /* "bilby_cython/time.pyx":50
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS             # <<<<<<<<<<<<<<
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  */
     __pyx_r = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
     goto __pyx_L0;
 
-    /* "bilby_cython/time.pyx":48
+    /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   }
 
-  /* "bilby_cython/time.pyx":50
+  /* "bilby_cython/time.pyx":51
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):             # <<<<<<<<<<<<<<
  *         n_leaps -= 1
  *     return n_leaps
  */
   while (1) {
@@ -20070,35 +20067,35 @@
     }
     __pyx_t_1 = (__pyx_v_n_leaps - 1);
     __pyx_t_3 = (__pyx_v_date < (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
     __pyx_t_2 = __pyx_t_3;
     __pyx_L6_bool_binop_done:;
     if (!__pyx_t_2) break;
 
-    /* "bilby_cython/time.pyx":51
+    /* "bilby_cython/time.pyx":52
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1             # <<<<<<<<<<<<<<
  *     return n_leaps
  * 
  */
     __pyx_v_n_leaps = (__pyx_v_n_leaps - 1);
   }
 
-  /* "bilby_cython/time.pyx":52
+  /* "bilby_cython/time.pyx":53
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  *     return n_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_n_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":40
+  /* "bilby_cython/time.pyx":41
  * 
  * @cython.ufunc
  * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
  *     """
  *     Find the number of leap seconds required for the specified date.
  */
 
@@ -20110,54 +20107,153 @@
 static int __pyx_fuse_4__pyx_f_12bilby_cython_4time_n_leap_seconds(double __pyx_v_date) {
   int __pyx_v_n_leaps;
   int __pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "bilby_cython/time.pyx":47
+  /* "bilby_cython/time.pyx":48
  *     be after the most recent leap.
  *     """
  *     cdef int n_leaps = NUM_LEAPS             # <<<<<<<<<<<<<<
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  */
   __pyx_v_n_leaps = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
 
-  /* "bilby_cython/time.pyx":48
+  /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   __pyx_t_1 = (__pyx_v_12bilby_cython_4time_NUM_LEAPS - 1);
   __pyx_t_2 = (__pyx_v_date > (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
   if (__pyx_t_2) {
 
+    /* "bilby_cython/time.pyx":50
+ *     cdef int n_leaps = NUM_LEAPS
+ *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
+ *         return NUM_LEAPS             # <<<<<<<<<<<<<<
+ *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
+ *         n_leaps -= 1
+ */
+    __pyx_r = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
+    goto __pyx_L0;
+
     /* "bilby_cython/time.pyx":49
+ *     """
+ *     cdef int n_leaps = NUM_LEAPS
+ *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
+ *         return NUM_LEAPS
+ *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
+ */
+  }
+
+  /* "bilby_cython/time.pyx":51
+ *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
+ *         return NUM_LEAPS
+ *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):             # <<<<<<<<<<<<<<
+ *         n_leaps -= 1
+ *     return n_leaps
+ */
+  while (1) {
+    __pyx_t_3 = (__pyx_v_n_leaps > 0);
+    if (__pyx_t_3) {
+    } else {
+      __pyx_t_2 = __pyx_t_3;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_1 = (__pyx_v_n_leaps - 1);
+    __pyx_t_3 = (__pyx_v_date < (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
+    __pyx_t_2 = __pyx_t_3;
+    __pyx_L6_bool_binop_done:;
+    if (!__pyx_t_2) break;
+
+    /* "bilby_cython/time.pyx":52
+ *         return NUM_LEAPS
+ *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
+ *         n_leaps -= 1             # <<<<<<<<<<<<<<
+ *     return n_leaps
+ * 
+ */
+    __pyx_v_n_leaps = (__pyx_v_n_leaps - 1);
+  }
+
+  /* "bilby_cython/time.pyx":53
+ *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
+ *         n_leaps -= 1
+ *     return n_leaps             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_n_leaps;
+  goto __pyx_L0;
+
+  /* "bilby_cython/time.pyx":41
+ * 
+ * @cython.ufunc
+ * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
+ *     """
+ *     Find the number of leap seconds required for the specified date.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+static int __pyx_fuse_5__pyx_f_12bilby_cython_4time_n_leap_seconds(long double __pyx_v_date) {
+  int __pyx_v_n_leaps;
+  int __pyx_r;
+  Py_ssize_t __pyx_t_1;
+  int __pyx_t_2;
+  int __pyx_t_3;
+
+  /* "bilby_cython/time.pyx":48
+ *     be after the most recent leap.
+ *     """
+ *     cdef int n_leaps = NUM_LEAPS             # <<<<<<<<<<<<<<
+ *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
+ *         return NUM_LEAPS
+ */
+  __pyx_v_n_leaps = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
+
+  /* "bilby_cython/time.pyx":49
+ *     """
+ *     cdef int n_leaps = NUM_LEAPS
+ *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
+ *         return NUM_LEAPS
+ *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
+ */
+  __pyx_t_1 = (__pyx_v_12bilby_cython_4time_NUM_LEAPS - 1);
+  __pyx_t_2 = (__pyx_v_date > (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
+  if (__pyx_t_2) {
+
+    /* "bilby_cython/time.pyx":50
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS             # <<<<<<<<<<<<<<
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  */
     __pyx_r = __pyx_v_12bilby_cython_4time_NUM_LEAPS;
     goto __pyx_L0;
 
-    /* "bilby_cython/time.pyx":48
+    /* "bilby_cython/time.pyx":49
  *     """
  *     cdef int n_leaps = NUM_LEAPS
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:             # <<<<<<<<<<<<<<
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  */
   }
 
-  /* "bilby_cython/time.pyx":50
+  /* "bilby_cython/time.pyx":51
  *     if date > LEAP_SECONDS[NUM_LEAPS - 1]:
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):             # <<<<<<<<<<<<<<
  *         n_leaps -= 1
  *     return n_leaps
  */
   while (1) {
@@ -20169,35 +20265,35 @@
     }
     __pyx_t_1 = (__pyx_v_n_leaps - 1);
     __pyx_t_3 = (__pyx_v_date < (*((long *) ( /* dim=0 */ (__pyx_v_12bilby_cython_4time_LEAP_SECONDS.data + __pyx_t_1 * __pyx_v_12bilby_cython_4time_LEAP_SECONDS.strides[0]) ))));
     __pyx_t_2 = __pyx_t_3;
     __pyx_L6_bool_binop_done:;
     if (!__pyx_t_2) break;
 
-    /* "bilby_cython/time.pyx":51
+    /* "bilby_cython/time.pyx":52
  *         return NUM_LEAPS
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1             # <<<<<<<<<<<<<<
  *     return n_leaps
  * 
  */
     __pyx_v_n_leaps = (__pyx_v_n_leaps - 1);
   }
 
-  /* "bilby_cython/time.pyx":52
+  /* "bilby_cython/time.pyx":53
  *     while (n_leaps > 0) and (date < LEAP_SECONDS[n_leaps - 1]):
  *         n_leaps -= 1
  *     return n_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_n_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":40
+  /* "bilby_cython/time.pyx":41
  * 
  * @cython.ufunc
  * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
  *     """
  *     Find the number of leap seconds required for the specified date.
  */
 
@@ -21120,15 +21216,197 @@
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_4n_leap_seconds_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
 }
 
-/* "bilby_cython/time.pyx":56
+static void __pyx_fuse_5n_leap_seconds_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
+  CYTHON_UNUSED npy_intp __pyx_v_i;
+  npy_intp __pyx_v_n;
+  char *__pyx_v_in_0;
+  long double __pyx_v_cast_in_0;
+  char *__pyx_v_out_0;
+  int __pyx_v_cast_out_0;
+  npy_intp __pyx_v_step_0;
+  npy_intp __pyx_v_step_1;
+  npy_intp __pyx_t_1;
+  npy_intp __pyx_t_2;
+  npy_intp __pyx_t_3;
+  int __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
+
+  /* "UFuncDefinition":13
+ * cdef void __pyx_fuse_5n_leap_seconds_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ */
+  __pyx_v_n = (__pyx_v_dimensions[0]);
+
+  /* "UFuncDefinition":14
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ *     cdef char* in_0 = args[0]             # <<<<<<<<<<<<<<
+ *     cdef long double cast_in_0
+ *     cdef char* out_0 = args[1]
+ */
+  __pyx_v_in_0 = (__pyx_v_args[0]);
+
+  /* "UFuncDefinition":16
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
+ *     cdef int cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ */
+  __pyx_v_out_0 = (__pyx_v_args[1]);
+
+  /* "UFuncDefinition":18
+ *     cdef char* out_0 = args[1]
+ *     cdef int cast_out_0
+ *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ */
+  __pyx_v_step_0 = (__pyx_v_steps[0]);
+
+  /* "UFuncDefinition":19
+ *     cdef int cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
+ * 
+ *     with gil:
+ */
+  __pyx_v_step_1 = (__pyx_v_steps[1]);
+
+  /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":22
+ * 
+ *     with gil:
+ *         for i in range(n):             # <<<<<<<<<<<<<<
+ *             cast_in_0 = (<long double*>in_0)[0]
+ * 
+ */
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
+
+          /* "UFuncDefinition":23
+ *     with gil:
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]             # <<<<<<<<<<<<<<
+ * 
+ *             cast_out_0 = \
+ */
+          __pyx_v_cast_in_0 = (((long double *)__pyx_v_in_0)[0]);
+
+          /* "UFuncDefinition":26
+ * 
+ *             cast_out_0 = \
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_n_leap_seconds(cast_in_0)             # <<<<<<<<<<<<<<
+ * 
+ *             (<int*>out_0)[0] = cast_out_0
+ */
+          __pyx_t_4 = __pyx_fuse_5__pyx_f_12bilby_cython_4time_n_leap_seconds(__pyx_v_cast_in_0); if (unlikely(__pyx_t_4 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
+
+          /* "UFuncDefinition":28
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_n_leap_seconds(cast_in_0)
+ * 
+ *             (<int*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
+ *             in_0 += step_0
+ *             out_0 += step_1
+ */
+          (((int *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
+
+          /* "UFuncDefinition":29
+ * 
+ *             (<int*>out_0)[0] = cast_out_0
+ *             in_0 += step_0             # <<<<<<<<<<<<<<
+ *             out_0 += step_1
+ * 
+ */
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+
+          /* "UFuncDefinition":30
+ *             (<int*>out_0)[0] = cast_out_0
+ *             in_0 += step_0
+ *             out_0 += step_1             # <<<<<<<<<<<<<<
+ * 
+ */
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+        }
+      }
+
+      /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "UFuncDefinition":11
+ * 
+ * @cname("__pyx_fuse_5n_leap_seconds_ufunc_def")
+ * cdef void __pyx_fuse_5n_leap_seconds_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
+  __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_5n_leap_seconds_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
+  __pyx_L0:;
+}
+
+/* "bilby_cython/time.pyx":57
  * 
  * @cython.ufunc
  * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from GPS time to UTC, this is a necessary intermediate step in
  */
 
@@ -21144,84 +21422,81 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0gps_time_to_utc", 1);
 
-  /* "bilby_cython/time.pyx":69
+  /* "bilby_cython/time.pyx":70
  *     """
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))             # <<<<<<<<<<<<<<
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))             # <<<<<<<<<<<<<<
  *     return date_before_leaps
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_short(__pyx_v_secs); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((double)__pyx_v_secs)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_short(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_short(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
+  __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_5)) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_6};
+    PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 69, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 70, __pyx_L1_error)
   __pyx_v_date_before_leaps = ((PyDateTime_DateTime *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bilby_cython/time.pyx":70
+  /* "bilby_cython/time.pyx":71
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))
  *     return date_before_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_date_before_leaps);
   __pyx_r = __pyx_v_date_before_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":56
+  /* "bilby_cython/time.pyx":57
  * 
  * @cython.ufunc
  * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from GPS time to UTC, this is a necessary intermediate step in
  */
 
@@ -21254,84 +21529,81 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1gps_time_to_utc", 1);
 
-  /* "bilby_cython/time.pyx":69
+  /* "bilby_cython/time.pyx":70
  *     """
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))             # <<<<<<<<<<<<<<
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))             # <<<<<<<<<<<<<<
  *     return date_before_leaps
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_secs); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((double)__pyx_v_secs)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
+  __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_5)) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_6};
+    PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 69, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 70, __pyx_L1_error)
   __pyx_v_date_before_leaps = ((PyDateTime_DateTime *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bilby_cython/time.pyx":70
+  /* "bilby_cython/time.pyx":71
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))
  *     return date_before_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_date_before_leaps);
   __pyx_r = __pyx_v_date_before_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":56
+  /* "bilby_cython/time.pyx":57
  * 
  * @cython.ufunc
  * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from GPS time to UTC, this is a necessary intermediate step in
  */
 
@@ -21364,84 +21636,81 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2gps_time_to_utc", 1);
 
-  /* "bilby_cython/time.pyx":69
+  /* "bilby_cython/time.pyx":70
  *     """
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))             # <<<<<<<<<<<<<<
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))             # <<<<<<<<<<<<<<
  *     return date_before_leaps
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_secs); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((double)__pyx_v_secs)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
+  __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_5)) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_6};
+    PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 69, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 70, __pyx_L1_error)
   __pyx_v_date_before_leaps = ((PyDateTime_DateTime *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bilby_cython/time.pyx":70
+  /* "bilby_cython/time.pyx":71
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))
  *     return date_before_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_date_before_leaps);
   __pyx_r = __pyx_v_date_before_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":56
+  /* "bilby_cython/time.pyx":57
  * 
  * @cython.ufunc
  * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from GPS time to UTC, this is a necessary intermediate step in
  */
 
@@ -21474,28 +21743,28 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3gps_time_to_utc", 1);
 
-  /* "bilby_cython/time.pyx":69
+  /* "bilby_cython/time.pyx":70
  *     """
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))             # <<<<<<<<<<<<<<
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))             # <<<<<<<<<<<<<<
  *     return date_before_leaps
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_secs); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((double)__pyx_v_secs)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_FromDouble(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
@@ -21508,47 +21777,47 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 69, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 70, __pyx_L1_error)
   __pyx_v_date_before_leaps = ((PyDateTime_DateTime *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bilby_cython/time.pyx":70
+  /* "bilby_cython/time.pyx":71
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))
  *     return date_before_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_date_before_leaps);
   __pyx_r = __pyx_v_date_before_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":56
+  /* "bilby_cython/time.pyx":57
  * 
  * @cython.ufunc
  * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from GPS time to UTC, this is a necessary intermediate step in
  */
 
@@ -21581,28 +21850,28 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_4gps_time_to_utc", 1);
 
-  /* "bilby_cython/time.pyx":69
+  /* "bilby_cython/time.pyx":70
  *     """
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))             # <<<<<<<<<<<<<<
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))             # <<<<<<<<<<<<<<
  *     return date_before_leaps
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_secs); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((double)__pyx_v_secs)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_FromDouble(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
@@ -21615,47 +21884,154 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 69, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 69, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 70, __pyx_L1_error)
   __pyx_v_date_before_leaps = ((PyDateTime_DateTime *)__pyx_t_1);
   __pyx_t_1 = 0;
 
+  /* "bilby_cython/time.pyx":71
+ *     cdef datetime date_before_leaps
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))
+ *     return date_before_leaps             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __Pyx_INCREF((PyObject *)__pyx_v_date_before_leaps);
+  __pyx_r = __pyx_v_date_before_leaps;
+  goto __pyx_L0;
+
+  /* "bilby_cython/time.pyx":57
+ * 
+ * @cython.ufunc
+ * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
+ *     """
+ *     Convert from GPS time to UTC, this is a necessary intermediate step in
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("bilby_cython.time.gps_time_to_utc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_date_before_leaps);
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyDateTime_DateTime *__pyx_fuse_5__pyx_f_12bilby_cython_4time_gps_time_to_utc(long double __pyx_v_secs) {
+  PyDateTime_DateTime *__pyx_v_date_before_leaps = 0;
+  PyDateTime_DateTime *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_fuse_5gps_time_to_utc", 1);
+
   /* "bilby_cython/time.pyx":70
+ *     """
+ *     cdef datetime date_before_leaps
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))             # <<<<<<<<<<<<<<
+ *     return date_before_leaps
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyFloat_FromDouble(((double)__pyx_v_secs)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_n_leap_seconds); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_secs); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 70, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  }
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_seconds, __pyx_t_4) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_8datetime_timedelta), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyNumber_Add(((PyObject *)__pyx_v_12bilby_cython_4time_GPS_EPOCH), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_7cpython_8datetime_datetime))))) __PYX_ERR(1, 70, __pyx_L1_error)
+  __pyx_v_date_before_leaps = ((PyDateTime_DateTime *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "bilby_cython/time.pyx":71
  *     cdef datetime date_before_leaps
- *     date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))
+ *     date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))
  *     return date_before_leaps             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_date_before_leaps);
   __pyx_r = __pyx_v_date_before_leaps;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":56
+  /* "bilby_cython/time.pyx":57
  * 
  * @cython.ufunc
  * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from GPS time to UTC, this is a necessary intermediate step in
  */
 
@@ -22390,76 +22766,218 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_4gps_time_to_utc_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cast_out_0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bilby_cython/time.pyx":74
+static void __pyx_fuse_5gps_time_to_utc_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
+  CYTHON_UNUSED npy_intp __pyx_v_i;
+  npy_intp __pyx_v_n;
+  char *__pyx_v_in_0;
+  long double __pyx_v_cast_in_0;
+  char *__pyx_v_out_0;
+  PyDateTime_DateTime *__pyx_v_cast_out_0 = 0;
+  npy_intp __pyx_v_step_0;
+  npy_intp __pyx_v_step_1;
+  __Pyx_RefNannyDeclarations
+  npy_intp __pyx_t_1;
+  npy_intp __pyx_t_2;
+  npy_intp __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_fuse_5gps_time_to_utc_ufunc_def", 1);
+
+  /* "UFuncDefinition":13
+ * cdef void __pyx_fuse_5gps_time_to_utc_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ */
+  __pyx_v_n = (__pyx_v_dimensions[0]);
+
+  /* "UFuncDefinition":14
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ *     cdef char* in_0 = args[0]             # <<<<<<<<<<<<<<
+ *     cdef long double cast_in_0
+ *     cdef char* out_0 = args[1]
+ */
+  __pyx_v_in_0 = (__pyx_v_args[0]);
+
+  /* "UFuncDefinition":16
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
+ *     cdef datetime cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ */
+  __pyx_v_out_0 = (__pyx_v_args[1]);
+
+  /* "UFuncDefinition":18
+ *     cdef char* out_0 = args[1]
+ *     cdef datetime cast_out_0
+ *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ */
+  __pyx_v_step_0 = (__pyx_v_steps[0]);
+
+  /* "UFuncDefinition":19
+ *     cdef datetime cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
+ * 
+ *     if True:
+ */
+  __pyx_v_step_1 = (__pyx_v_steps[1]);
+
+  /* "UFuncDefinition":22
+ * 
+ *     if True:
+ *         for i in range(n):             # <<<<<<<<<<<<<<
+ *             cast_in_0 = (<long double*>in_0)[0]
+ * 
+ */
+  __pyx_t_1 = __pyx_v_n;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_i = __pyx_t_3;
+
+    /* "UFuncDefinition":23
+ *     if True:
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]             # <<<<<<<<<<<<<<
+ * 
+ *             cast_out_0 = \
+ */
+    __pyx_v_cast_in_0 = (((long double *)__pyx_v_in_0)[0]);
+
+    /* "UFuncDefinition":26
+ * 
+ *             cast_out_0 = \
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_gps_time_to_utc(cast_in_0)             # <<<<<<<<<<<<<<
+ * 
+ *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ */
+    __pyx_t_4 = ((PyObject *)__pyx_fuse_5__pyx_f_12bilby_cython_4time_gps_time_to_utc(__pyx_v_cast_in_0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, ((PyDateTime_DateTime *)__pyx_t_4));
+    __pyx_t_4 = 0;
+
+    /* "UFuncDefinition":28
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_gps_time_to_utc(cast_in_0)
+ * 
+ *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             in_0 += step_0
+ *             out_0 += step_1
+ */
+    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(((PyObject *)__pyx_v_cast_out_0)));
+
+    /* "UFuncDefinition":29
+ * 
+ *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             in_0 += step_0             # <<<<<<<<<<<<<<
+ *             out_0 += step_1
+ * 
+ */
+    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+
+    /* "UFuncDefinition":30
+ *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             in_0 += step_0
+ *             out_0 += step_1             # <<<<<<<<<<<<<<
+ * 
+ */
+    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+  }
+
+  /* "UFuncDefinition":11
+ * 
+ * @cname("__pyx_fuse_5gps_time_to_utc_ufunc_def")
+ * cdef void __pyx_fuse_5gps_time_to_utc_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_5gps_time_to_utc_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_cast_out_0);
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "bilby_cython/time.pyx":75
  * 
  * @cython.ufunc
  * cdef double utc_to_julian_day(datetime time):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from UTC to Julian day, this is a necessary intermediate step in
  */
 
 static double __pyx_f_12bilby_cython_4time_utc_to_julian_day(PyDateTime_DateTime *__pyx_v_time) {
   int __pyx_v_year;
   int __pyx_v_month;
   int __pyx_v_day;
   double __pyx_v_second;
   double __pyx_r;
 
-  /* "bilby_cython/time.pyx":84
+  /* "bilby_cython/time.pyx":85
  *         The UTC time to convert
  *     """
  *     cdef int year = time.year             # <<<<<<<<<<<<<<
  *     cdef int month = time.month
  *     cdef int day = time.day
  */
   __pyx_v_year = __pyx_f_7cpython_8datetime_8datetime_4year_year(__pyx_v_time);
 
-  /* "bilby_cython/time.pyx":85
+  /* "bilby_cython/time.pyx":86
  *     """
  *     cdef int year = time.year
  *     cdef int month = time.month             # <<<<<<<<<<<<<<
  *     cdef int day = time.day
  *     cdef double second = time.second + 60 * (time.minute + 60 * time.hour)
  */
   __pyx_v_month = __pyx_f_7cpython_8datetime_8datetime_5month_month(__pyx_v_time);
 
-  /* "bilby_cython/time.pyx":86
+  /* "bilby_cython/time.pyx":87
  *     cdef int year = time.year
  *     cdef int month = time.month
  *     cdef int day = time.day             # <<<<<<<<<<<<<<
  *     cdef double second = time.second + 60 * (time.minute + 60 * time.hour)
  *     return (
  */
   __pyx_v_day = __pyx_f_7cpython_8datetime_8datetime_3day_day(__pyx_v_time);
 
-  /* "bilby_cython/time.pyx":87
+  /* "bilby_cython/time.pyx":88
  *     cdef int month = time.month
  *     cdef int day = time.day
  *     cdef double second = time.second + 60 * (time.minute + 60 * time.hour)             # <<<<<<<<<<<<<<
  *     return (
  *         367 * year
  */
   __pyx_v_second = (__pyx_f_7cpython_8datetime_8datetime_6second_second(__pyx_v_time) + (60 * (__pyx_f_7cpython_8datetime_8datetime_6minute_minute(__pyx_v_time) + (60 * __pyx_f_7cpython_8datetime_8datetime_4hour_hour(__pyx_v_time)))));
 
-  /* "bilby_cython/time.pyx":95
+  /* "bilby_cython/time.pyx":96
  *         + 1721014
  *         + second / (60 * 60 * 24)
  *         - 0.5             # <<<<<<<<<<<<<<
  *     )
  * 
  */
   __pyx_r = (((((((0x16F * __pyx_v_year) - ((7 * (__pyx_v_year + ((__pyx_v_month + 9) / 12))) / 4)) + ((0x113 * __pyx_v_month) / 9)) + __pyx_v_day) + 0x1A42B6) + (__pyx_v_second / 86400.0)) - 0.5);
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":74
+  /* "bilby_cython/time.pyx":75
  * 
  * @cython.ufunc
  * cdef double utc_to_julian_day(datetime time):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from UTC to Julian day, this is a necessary intermediate step in
  */
 
@@ -22616,46 +23134,46 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("UFuncDefinition.utc_to_julian_day_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cast_in_0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bilby_cython/time.pyx":100
+/* "bilby_cython/time.pyx":101
  * 
  * @cython.ufunc
- * cdef greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time.
  */
 
-static PyObject *__pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(short __pyx_v_gps_time) {
-  PyObject *__pyx_r = NULL;
+static double __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(short __pyx_v_gps_time) {
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
+  double __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0greenwich_mean_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":109
+  /* "bilby_cython/time.pyx":110
  *         The GPS time to convert
  *     """
  *     return greenwich_sidereal_time(gps_time, 0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_short(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_short(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -22668,68 +23186,68 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_0};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_6;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":100
+  /* "bilby_cython/time.pyx":101
  * 
  * @cython.ufunc
- * cdef greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_mean_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(int __pyx_v_gps_time) {
-  PyObject *__pyx_r = NULL;
+static double __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(int __pyx_v_gps_time) {
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
+  double __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1greenwich_mean_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":109
+  /* "bilby_cython/time.pyx":110
  *         The GPS time to convert
  *     """
  *     return greenwich_sidereal_time(gps_time, 0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -22742,68 +23260,68 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_0};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_6;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":100
+  /* "bilby_cython/time.pyx":101
  * 
  * @cython.ufunc
- * cdef greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_mean_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(long __pyx_v_gps_time) {
-  PyObject *__pyx_r = NULL;
+static double __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(long __pyx_v_gps_time) {
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
+  double __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2greenwich_mean_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":109
+  /* "bilby_cython/time.pyx":110
  *         The GPS time to convert
  *     """
  *     return greenwich_sidereal_time(gps_time, 0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -22816,68 +23334,68 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_0};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_6;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":100
+  /* "bilby_cython/time.pyx":101
  * 
  * @cython.ufunc
- * cdef greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_mean_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(float __pyx_v_gps_time) {
-  PyObject *__pyx_r = NULL;
+static double __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(float __pyx_v_gps_time) {
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
+  double __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3greenwich_mean_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":109
+  /* "bilby_cython/time.pyx":110
  *         The GPS time to convert
  *     """
  *     return greenwich_sidereal_time(gps_time, 0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -22890,68 +23408,68 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_0};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_6;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":100
+  /* "bilby_cython/time.pyx":101
  * 
  * @cython.ufunc
- * cdef greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_mean_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(double __pyx_v_gps_time) {
-  PyObject *__pyx_r = NULL;
+static double __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(double __pyx_v_gps_time) {
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
+  double __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_4greenwich_mean_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":109
+  /* "bilby_cython/time.pyx":110
  *         The GPS time to convert
  *     """
  *     return greenwich_sidereal_time(gps_time, 0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -22964,73 +23482,148 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_0};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_6;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":100
+  /* "bilby_cython/time.pyx":101
  * 
  * @cython.ufunc
- * cdef greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_mean_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static double __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(long double __pyx_v_gps_time) {
+  double __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  double __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_fuse_5greenwich_mean_sidereal_time", 1);
+
+  /* "bilby_cython/time.pyx":110
+ *         The GPS time to convert
+ *     """
+ *     return greenwich_sidereal_time(gps_time, 0)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_greenwich_sidereal_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_5 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_0};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 110, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 110, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_6;
+  goto __pyx_L0;
+
+  /* "bilby_cython/time.pyx":101
+ * 
+ * @cython.ufunc
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ *     """
+ *     Compute the Greenwich mean sidereal time from the GPS time.
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("bilby_cython.time.greenwich_mean_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
 static void __pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   short __pyx_v_cast_in_0;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef short cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -23043,136 +23636,176 @@
  */
   __pyx_v_in_0 = (__pyx_v_args[0]);
 
   /* "UFuncDefinition":16
  *     cdef char* in_0 = args[0]
  *     cdef short cast_in_0
  *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* out_0 = args[1]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  * 
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":19
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
-  /* "UFuncDefinition":22
+  /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<short*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":22
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<short*>in_0)[0]
  * 
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":23
- *     if True:
+          /* "UFuncDefinition":23
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<short*>in_0)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_0 = (((short *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((short *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":26
+          /* "UFuncDefinition":26
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":28
+          /* "UFuncDefinition":28
  *                 __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             out_0 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":29
+          /* "UFuncDefinition":29
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             out_0 += step_1
  * 
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":30
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":30
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             out_0 += step_1             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+        }
+      }
+
+      /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<short*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   int __pyx_v_cast_in_0;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef int cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -23185,136 +23818,176 @@
  */
   __pyx_v_in_0 = (__pyx_v_args[0]);
 
   /* "UFuncDefinition":16
  *     cdef char* in_0 = args[0]
  *     cdef int cast_in_0
  *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* out_0 = args[1]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  * 
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":19
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
-  /* "UFuncDefinition":22
+  /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<int*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":22
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<int*>in_0)[0]
  * 
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":23
- *     if True:
+          /* "UFuncDefinition":23
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<int*>in_0)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_0 = (((int *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((int *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":26
+          /* "UFuncDefinition":26
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":28
+          /* "UFuncDefinition":28
  *                 __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             out_0 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":29
+          /* "UFuncDefinition":29
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             out_0 += step_1
  * 
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":30
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":30
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             out_0 += step_1             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+        }
+      }
+
+      /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<int*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   long __pyx_v_cast_in_0;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef long cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -23327,136 +24000,176 @@
  */
   __pyx_v_in_0 = (__pyx_v_args[0]);
 
   /* "UFuncDefinition":16
  *     cdef char* in_0 = args[0]
  *     cdef long cast_in_0
  *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* out_0 = args[1]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  * 
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":19
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
-  /* "UFuncDefinition":22
+  /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":22
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<long*>in_0)[0]
  * 
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":23
- *     if True:
+          /* "UFuncDefinition":23
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<long*>in_0)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_0 = (((long *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((long *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":26
+          /* "UFuncDefinition":26
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":28
+          /* "UFuncDefinition":28
  *                 __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             out_0 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":29
+          /* "UFuncDefinition":29
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             out_0 += step_1
  * 
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":30
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":30
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             out_0 += step_1             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+        }
+      }
+
+      /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   float __pyx_v_cast_in_0;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef float cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -23469,136 +24182,176 @@
  */
   __pyx_v_in_0 = (__pyx_v_args[0]);
 
   /* "UFuncDefinition":16
  *     cdef char* in_0 = args[0]
  *     cdef float cast_in_0
  *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* out_0 = args[1]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  * 
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":19
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
-  /* "UFuncDefinition":22
+  /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<float*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":22
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<float*>in_0)[0]
  * 
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":23
- *     if True:
+          /* "UFuncDefinition":23
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<float*>in_0)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_0 = (((float *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((float *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":26
+          /* "UFuncDefinition":26
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":28
+          /* "UFuncDefinition":28
  *                 __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             out_0 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":29
+          /* "UFuncDefinition":29
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             out_0 += step_1
  * 
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":30
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":30
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             out_0 += step_1             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+        }
+      }
+
+      /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<float*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   double __pyx_v_cast_in_0;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef double cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -23611,156 +24364,377 @@
  */
   __pyx_v_in_0 = (__pyx_v_args[0]);
 
   /* "UFuncDefinition":16
  *     cdef char* in_0 = args[0]
  *     cdef double cast_in_0
  *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* out_0 = args[1]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  * 
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":19
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
-  /* "UFuncDefinition":22
+  /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<double*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":22
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<double*>in_0)[0]
  * 
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":23
- *     if True:
+          /* "UFuncDefinition":23
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<double*>in_0)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_0 = (((double *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((double *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":26
+          /* "UFuncDefinition":26
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":28
+          /* "UFuncDefinition":28
  *                 __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             out_0 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":29
+          /* "UFuncDefinition":29
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             out_0 += step_1
  * 
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":30
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":30
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             out_0 += step_1             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+        }
+      }
+
+      /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<double*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
-/* "bilby_cython/time.pyx":113
+static void __pyx_fuse_5greenwich_mean_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
+  CYTHON_UNUSED npy_intp __pyx_v_i;
+  npy_intp __pyx_v_n;
+  char *__pyx_v_in_0;
+  long double __pyx_v_cast_in_0;
+  char *__pyx_v_out_0;
+  double __pyx_v_cast_out_0;
+  npy_intp __pyx_v_step_0;
+  npy_intp __pyx_v_step_1;
+  npy_intp __pyx_t_1;
+  npy_intp __pyx_t_2;
+  npy_intp __pyx_t_3;
+  double __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
+
+  /* "UFuncDefinition":13
+ * cdef void __pyx_fuse_5greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ */
+  __pyx_v_n = (__pyx_v_dimensions[0]);
+
+  /* "UFuncDefinition":14
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ *     cdef char* in_0 = args[0]             # <<<<<<<<<<<<<<
+ *     cdef long double cast_in_0
+ *     cdef char* out_0 = args[1]
+ */
+  __pyx_v_in_0 = (__pyx_v_args[0]);
+
+  /* "UFuncDefinition":16
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ *     cdef char* out_0 = args[1]             # <<<<<<<<<<<<<<
+ *     cdef double cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ */
+  __pyx_v_out_0 = (__pyx_v_args[1]);
+
+  /* "UFuncDefinition":18
+ *     cdef char* out_0 = args[1]
+ *     cdef double cast_out_0
+ *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ */
+  __pyx_v_step_0 = (__pyx_v_steps[0]);
+
+  /* "UFuncDefinition":19
+ *     cdef double cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
+ * 
+ *     with gil:
+ */
+  __pyx_v_step_1 = (__pyx_v_steps[1]);
+
+  /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":22
+ * 
+ *     with gil:
+ *         for i in range(n):             # <<<<<<<<<<<<<<
+ *             cast_in_0 = (<long double*>in_0)[0]
+ * 
+ */
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
+
+          /* "UFuncDefinition":23
+ *     with gil:
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]             # <<<<<<<<<<<<<<
+ * 
+ *             cast_out_0 = \
+ */
+          __pyx_v_cast_in_0 = (((long double *)__pyx_v_in_0)[0]);
+
+          /* "UFuncDefinition":26
+ * 
+ *             cast_out_0 = \
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)             # <<<<<<<<<<<<<<
+ * 
+ *             (<double*>out_0)[0] = cast_out_0
+ */
+          __pyx_t_4 = __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(__pyx_v_cast_in_0); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
+
+          /* "UFuncDefinition":28
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_mean_sidereal_time(cast_in_0)
+ * 
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
+ *             in_0 += step_0
+ *             out_0 += step_1
+ */
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
+
+          /* "UFuncDefinition":29
+ * 
+ *             (<double*>out_0)[0] = cast_out_0
+ *             in_0 += step_0             # <<<<<<<<<<<<<<
+ *             out_0 += step_1
+ * 
+ */
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+
+          /* "UFuncDefinition":30
+ *             (<double*>out_0)[0] = cast_out_0
+ *             in_0 += step_0
+ *             out_0 += step_1             # <<<<<<<<<<<<<<
+ * 
+ */
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_1);
+        }
+      }
+
+      /* "UFuncDefinition":21
+ *     cdef npy_intp step_1 = steps[1]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "UFuncDefinition":11
+ * 
+ * @cname("__pyx_fuse_5greenwich_mean_sidereal_time_ufunc_def")
+ * cdef void __pyx_fuse_5greenwich_mean_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
+  __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_5greenwich_mean_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
+  __pyx_L0:;
+}
+
+/* "bilby_cython/time.pyx":114
  * 
  * @cython.ufunc
- * cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time and equation of
  */
 
-static PyObject *__pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(short __pyx_v_gps_time, short __pyx_v_equation_of_equinoxes) {
+static double __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(short __pyx_v_gps_time, short __pyx_v_equation_of_equinoxes) {
   double __pyx_v_julian_day;
   double __pyx_v_t_hi;
   double __pyx_v_t_lo;
   double __pyx_v_t;
   double __pyx_v_sidereal_time;
-  PyObject *__pyx_r = NULL;
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0greenwich_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":128
+  /* "bilby_cython/time.pyx":129
  *     """
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))             # <<<<<<<<<<<<<<
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))             # <<<<<<<<<<<<<<
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_long((__pyx_v_gps_time / 1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_short(__pyx_v_gps_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
@@ -23773,15 +24747,15 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -23796,172 +24770,171 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_julian_day = __pyx_t_8;
 
-  /* "bilby_cython/time.pyx":129
+  /* "bilby_cython/time.pyx":130
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0             # <<<<<<<<<<<<<<
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  */
   __pyx_v_t_hi = ((__pyx_v_julian_day - __pyx_v_12bilby_cython_4time_EPOCH_J2000_0_JD) / 36525.0);
 
-  /* "bilby_cython/time.pyx":130
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+  /* "bilby_cython/time.pyx":131
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)             # <<<<<<<<<<<<<<
  * 
  *     t = t_hi + t_lo
  */
   __pyx_v_t_lo = (((double)(__pyx_v_gps_time % 1)) / (36525.0 * 86400.0));
 
-  /* "bilby_cython/time.pyx":132
+  /* "bilby_cython/time.pyx":133
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  *     t = t_hi + t_lo             # <<<<<<<<<<<<<<
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  */
   __pyx_v_t = (__pyx_v_t_hi + __pyx_v_t_lo);
 
-  /* "bilby_cython/time.pyx":134
+  /* "bilby_cython/time.pyx":135
  *     t = t_hi + t_lo
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  */
   __pyx_v_sidereal_time = ((__pyx_v_equation_of_equinoxes + (((-6.2e-6 * __pyx_v_t) + 0.093104) * pow(__pyx_v_t, 2.0))) + 67310.54841);
 
-  /* "bilby_cython/time.pyx":135
+  /* "bilby_cython/time.pyx":136
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":136
+  /* "bilby_cython/time.pyx":137
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":137
+  /* "bilby_cython/time.pyx":138
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":138
+  /* "bilby_cython/time.pyx":139
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi             # <<<<<<<<<<<<<<
  * 
  *     return sidereal_time * pi / 43200.0
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":140
+  /* "bilby_cython/time.pyx":141
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  *     return sidereal_time * pi / 43200.0             # <<<<<<<<<<<<<<
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_8;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":113
+  /* "bilby_cython/time.pyx":114
  * 
  * @cython.ufunc
- * cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time and equation of
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(int __pyx_v_gps_time, int __pyx_v_equation_of_equinoxes) {
+static double __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(int __pyx_v_gps_time, int __pyx_v_equation_of_equinoxes) {
   double __pyx_v_julian_day;
   double __pyx_v_t_hi;
   double __pyx_v_t_lo;
   double __pyx_v_t;
   double __pyx_v_sidereal_time;
-  PyObject *__pyx_r = NULL;
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1greenwich_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":128
+  /* "bilby_cython/time.pyx":129
  *     """
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))             # <<<<<<<<<<<<<<
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))             # <<<<<<<<<<<<<<
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_long((__pyx_v_gps_time / 1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_gps_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
@@ -23974,15 +24947,15 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -23997,172 +24970,171 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_julian_day = __pyx_t_8;
 
-  /* "bilby_cython/time.pyx":129
+  /* "bilby_cython/time.pyx":130
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0             # <<<<<<<<<<<<<<
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  */
   __pyx_v_t_hi = ((__pyx_v_julian_day - __pyx_v_12bilby_cython_4time_EPOCH_J2000_0_JD) / 36525.0);
 
-  /* "bilby_cython/time.pyx":130
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+  /* "bilby_cython/time.pyx":131
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)             # <<<<<<<<<<<<<<
  * 
  *     t = t_hi + t_lo
  */
   __pyx_v_t_lo = (((double)(__pyx_v_gps_time % 1)) / (36525.0 * 86400.0));
 
-  /* "bilby_cython/time.pyx":132
+  /* "bilby_cython/time.pyx":133
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  *     t = t_hi + t_lo             # <<<<<<<<<<<<<<
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  */
   __pyx_v_t = (__pyx_v_t_hi + __pyx_v_t_lo);
 
-  /* "bilby_cython/time.pyx":134
+  /* "bilby_cython/time.pyx":135
  *     t = t_hi + t_lo
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  */
   __pyx_v_sidereal_time = ((__pyx_v_equation_of_equinoxes + (((-6.2e-6 * __pyx_v_t) + 0.093104) * pow(__pyx_v_t, 2.0))) + 67310.54841);
 
-  /* "bilby_cython/time.pyx":135
+  /* "bilby_cython/time.pyx":136
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":136
+  /* "bilby_cython/time.pyx":137
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":137
+  /* "bilby_cython/time.pyx":138
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":138
+  /* "bilby_cython/time.pyx":139
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi             # <<<<<<<<<<<<<<
  * 
  *     return sidereal_time * pi / 43200.0
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":140
+  /* "bilby_cython/time.pyx":141
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  *     return sidereal_time * pi / 43200.0             # <<<<<<<<<<<<<<
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_8;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":113
+  /* "bilby_cython/time.pyx":114
  * 
  * @cython.ufunc
- * cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time and equation of
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(long __pyx_v_gps_time, long __pyx_v_equation_of_equinoxes) {
+static double __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(long __pyx_v_gps_time, long __pyx_v_equation_of_equinoxes) {
   double __pyx_v_julian_day;
   double __pyx_v_t_hi;
   double __pyx_v_t_lo;
   double __pyx_v_t;
   double __pyx_v_sidereal_time;
-  PyObject *__pyx_r = NULL;
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2greenwich_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":128
+  /* "bilby_cython/time.pyx":129
  *     """
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))             # <<<<<<<<<<<<<<
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))             # <<<<<<<<<<<<<<
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_long((__pyx_v_gps_time / 1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_gps_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
@@ -24175,15 +25147,15 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -24198,172 +25170,171 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_julian_day = __pyx_t_8;
 
-  /* "bilby_cython/time.pyx":129
+  /* "bilby_cython/time.pyx":130
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0             # <<<<<<<<<<<<<<
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  */
   __pyx_v_t_hi = ((__pyx_v_julian_day - __pyx_v_12bilby_cython_4time_EPOCH_J2000_0_JD) / 36525.0);
 
-  /* "bilby_cython/time.pyx":130
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+  /* "bilby_cython/time.pyx":131
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)             # <<<<<<<<<<<<<<
  * 
  *     t = t_hi + t_lo
  */
   __pyx_v_t_lo = (((double)(__pyx_v_gps_time % 1)) / (36525.0 * 86400.0));
 
-  /* "bilby_cython/time.pyx":132
+  /* "bilby_cython/time.pyx":133
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  *     t = t_hi + t_lo             # <<<<<<<<<<<<<<
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  */
   __pyx_v_t = (__pyx_v_t_hi + __pyx_v_t_lo);
 
-  /* "bilby_cython/time.pyx":134
+  /* "bilby_cython/time.pyx":135
  *     t = t_hi + t_lo
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  */
   __pyx_v_sidereal_time = ((__pyx_v_equation_of_equinoxes + (((-6.2e-6 * __pyx_v_t) + 0.093104) * pow(__pyx_v_t, 2.0))) + 67310.54841);
 
-  /* "bilby_cython/time.pyx":135
+  /* "bilby_cython/time.pyx":136
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":136
+  /* "bilby_cython/time.pyx":137
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":137
+  /* "bilby_cython/time.pyx":138
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":138
+  /* "bilby_cython/time.pyx":139
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi             # <<<<<<<<<<<<<<
  * 
  *     return sidereal_time * pi / 43200.0
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":140
+  /* "bilby_cython/time.pyx":141
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  *     return sidereal_time * pi / 43200.0             # <<<<<<<<<<<<<<
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_8;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":113
+  /* "bilby_cython/time.pyx":114
  * 
  * @cython.ufunc
- * cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time and equation of
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(float __pyx_v_gps_time, float __pyx_v_equation_of_equinoxes) {
+static double __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(float __pyx_v_gps_time, float __pyx_v_equation_of_equinoxes) {
   double __pyx_v_julian_day;
   double __pyx_v_t_hi;
   double __pyx_v_t_lo;
   double __pyx_v_t;
   double __pyx_v_sidereal_time;
-  PyObject *__pyx_r = NULL;
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3greenwich_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":128
+  /* "bilby_cython/time.pyx":129
  *     """
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))             # <<<<<<<<<<<<<<
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))             # <<<<<<<<<<<<<<
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyFloat_FromDouble(floor(__pyx_v_gps_time / 1.0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
@@ -24376,15 +25347,15 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -24399,172 +25370,171 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_julian_day = __pyx_t_8;
 
-  /* "bilby_cython/time.pyx":129
+  /* "bilby_cython/time.pyx":130
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0             # <<<<<<<<<<<<<<
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  */
   __pyx_v_t_hi = ((__pyx_v_julian_day - __pyx_v_12bilby_cython_4time_EPOCH_J2000_0_JD) / 36525.0);
 
-  /* "bilby_cython/time.pyx":130
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+  /* "bilby_cython/time.pyx":131
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)             # <<<<<<<<<<<<<<
  * 
  *     t = t_hi + t_lo
  */
   __pyx_v_t_lo = (((double)fmodf(__pyx_v_gps_time, 1.0)) / (36525.0 * 86400.0));
 
-  /* "bilby_cython/time.pyx":132
+  /* "bilby_cython/time.pyx":133
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  *     t = t_hi + t_lo             # <<<<<<<<<<<<<<
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  */
   __pyx_v_t = (__pyx_v_t_hi + __pyx_v_t_lo);
 
-  /* "bilby_cython/time.pyx":134
+  /* "bilby_cython/time.pyx":135
  *     t = t_hi + t_lo
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  */
   __pyx_v_sidereal_time = ((__pyx_v_equation_of_equinoxes + (((-6.2e-6 * __pyx_v_t) + 0.093104) * pow(__pyx_v_t, 2.0))) + 67310.54841);
 
-  /* "bilby_cython/time.pyx":135
+  /* "bilby_cython/time.pyx":136
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":136
+  /* "bilby_cython/time.pyx":137
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":137
+  /* "bilby_cython/time.pyx":138
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":138
+  /* "bilby_cython/time.pyx":139
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi             # <<<<<<<<<<<<<<
  * 
  *     return sidereal_time * pi / 43200.0
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":140
+  /* "bilby_cython/time.pyx":141
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  *     return sidereal_time * pi / 43200.0             # <<<<<<<<<<<<<<
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_8;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":113
+  /* "bilby_cython/time.pyx":114
  * 
  * @cython.ufunc
- * cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time and equation of
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(double __pyx_v_gps_time, double __pyx_v_equation_of_equinoxes) {
+static double __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(double __pyx_v_gps_time, double __pyx_v_equation_of_equinoxes) {
   double __pyx_v_julian_day;
   double __pyx_v_t_hi;
   double __pyx_v_t_lo;
   double __pyx_v_t;
   double __pyx_v_sidereal_time;
-  PyObject *__pyx_r = NULL;
+  double __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_4greenwich_sidereal_time", 1);
 
-  /* "bilby_cython/time.pyx":128
+  /* "bilby_cython/time.pyx":129
  *     """
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))             # <<<<<<<<<<<<<<
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))             # <<<<<<<<<<<<<<
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyFloat_FromDouble(floor(__pyx_v_gps_time / 1.0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
@@ -24577,15 +25547,15 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -24600,171 +25570,371 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 128, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_julian_day = __pyx_t_8;
 
-  /* "bilby_cython/time.pyx":129
+  /* "bilby_cython/time.pyx":130
  *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0             # <<<<<<<<<<<<<<
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  */
   __pyx_v_t_hi = ((__pyx_v_julian_day - __pyx_v_12bilby_cython_4time_EPOCH_J2000_0_JD) / 36525.0);
 
-  /* "bilby_cython/time.pyx":130
- *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+  /* "bilby_cython/time.pyx":131
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
  *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)             # <<<<<<<<<<<<<<
  * 
  *     t = t_hi + t_lo
  */
   __pyx_v_t_lo = (fmod(__pyx_v_gps_time, 1.0) / (36525.0 * 86400.0));
 
-  /* "bilby_cython/time.pyx":132
+  /* "bilby_cython/time.pyx":133
  *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
  * 
  *     t = t_hi + t_lo             # <<<<<<<<<<<<<<
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  */
   __pyx_v_t = (__pyx_v_t_hi + __pyx_v_t_lo);
 
-  /* "bilby_cython/time.pyx":134
+  /* "bilby_cython/time.pyx":135
  *     t = t_hi + t_lo
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  */
   __pyx_v_sidereal_time = ((__pyx_v_equation_of_equinoxes + (((-6.2e-6 * __pyx_v_t) + 0.093104) * pow(__pyx_v_t, 2.0))) + 67310.54841);
 
-  /* "bilby_cython/time.pyx":135
+  /* "bilby_cython/time.pyx":136
  * 
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":136
+  /* "bilby_cython/time.pyx":137
  *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo             # <<<<<<<<<<<<<<
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_lo));
 
-  /* "bilby_cython/time.pyx":137
+  /* "bilby_cython/time.pyx":138
  *     sidereal_time += 8640184.812866 * t_lo
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi             # <<<<<<<<<<<<<<
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_hi));
 
+  /* "bilby_cython/time.pyx":139
+ *     sidereal_time += 3155760000.0 * t_lo
+ *     sidereal_time += 8640184.812866 * t_hi
+ *     sidereal_time += 3155760000.0 * t_hi             # <<<<<<<<<<<<<<
+ * 
+ *     return sidereal_time * pi / 43200.0
+ */
+  __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_hi));
+
+  /* "bilby_cython/time.pyx":141
+ *     sidereal_time += 3155760000.0 * t_hi
+ * 
+ *     return sidereal_time * pi / 43200.0             # <<<<<<<<<<<<<<
+ */
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_8;
+  goto __pyx_L0;
+
+  /* "bilby_cython/time.pyx":114
+ * 
+ * @cython.ufunc
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ *     """
+ *     Compute the Greenwich mean sidereal time from the GPS time and equation of
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("bilby_cython.time.greenwich_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static double __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(long double __pyx_v_gps_time, long double __pyx_v_equation_of_equinoxes) {
+  double __pyx_v_julian_day;
+  double __pyx_v_t_hi;
+  double __pyx_v_t_lo;
+  double __pyx_v_t;
+  double __pyx_v_sidereal_time;
+  double __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  double __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_fuse_5greenwich_sidereal_time", 1);
+
+  /* "bilby_cython/time.pyx":129
+ *     """
+ *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))             # <<<<<<<<<<<<<<
+ *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
+ *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utc_to_julian_day); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_gps_time_to_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_gps_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 129, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  }
+  __pyx_t_4 = NULL;
+  __pyx_t_7 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 129, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 129, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_julian_day = __pyx_t_8;
+
+  /* "bilby_cython/time.pyx":130
+ *     cdef double julian_day, t_hi, t_lo, t, sidereal_time
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
+ *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0             # <<<<<<<<<<<<<<
+ *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
+ * 
+ */
+  __pyx_v_t_hi = ((__pyx_v_julian_day - __pyx_v_12bilby_cython_4time_EPOCH_J2000_0_JD) / 36525.0);
+
+  /* "bilby_cython/time.pyx":131
+ *     julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
+ *     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
+ *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)             # <<<<<<<<<<<<<<
+ * 
+ *     t = t_hi + t_lo
+ */
+  __pyx_v_t_lo = (fmodl(__pyx_v_gps_time, 1.0) / ((long double)(36525.0 * 86400.0)));
+
+  /* "bilby_cython/time.pyx":133
+ *     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
+ * 
+ *     t = t_hi + t_lo             # <<<<<<<<<<<<<<
+ * 
+ *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
+ */
+  __pyx_v_t = (__pyx_v_t_hi + __pyx_v_t_lo);
+
+  /* "bilby_cython/time.pyx":135
+ *     t = t_hi + t_lo
+ * 
+ *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841             # <<<<<<<<<<<<<<
+ *     sidereal_time += 8640184.812866 * t_lo
+ *     sidereal_time += 3155760000.0 * t_lo
+ */
+  __pyx_v_sidereal_time = ((__pyx_v_equation_of_equinoxes + (((-6.2e-6 * __pyx_v_t) + 0.093104) * pow(__pyx_v_t, 2.0))) + 67310.54841);
+
+  /* "bilby_cython/time.pyx":136
+ * 
+ *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
+ *     sidereal_time += 8640184.812866 * t_lo             # <<<<<<<<<<<<<<
+ *     sidereal_time += 3155760000.0 * t_lo
+ *     sidereal_time += 8640184.812866 * t_hi
+ */
+  __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_lo));
+
+  /* "bilby_cython/time.pyx":137
+ *     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
+ *     sidereal_time += 8640184.812866 * t_lo
+ *     sidereal_time += 3155760000.0 * t_lo             # <<<<<<<<<<<<<<
+ *     sidereal_time += 8640184.812866 * t_hi
+ *     sidereal_time += 3155760000.0 * t_hi
+ */
+  __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_lo));
+
   /* "bilby_cython/time.pyx":138
+ *     sidereal_time += 8640184.812866 * t_lo
+ *     sidereal_time += 3155760000.0 * t_lo
+ *     sidereal_time += 8640184.812866 * t_hi             # <<<<<<<<<<<<<<
+ *     sidereal_time += 3155760000.0 * t_hi
+ * 
+ */
+  __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (8640184.812866 * __pyx_v_t_hi));
+
+  /* "bilby_cython/time.pyx":139
  *     sidereal_time += 3155760000.0 * t_lo
  *     sidereal_time += 8640184.812866 * t_hi
  *     sidereal_time += 3155760000.0 * t_hi             # <<<<<<<<<<<<<<
  * 
  *     return sidereal_time * pi / 43200.0
  */
   __pyx_v_sidereal_time = (__pyx_v_sidereal_time + (3155760000.0 * __pyx_v_t_hi));
 
-  /* "bilby_cython/time.pyx":140
+  /* "bilby_cython/time.pyx":141
  *     sidereal_time += 3155760000.0 * t_hi
  * 
  *     return sidereal_time * pi / 43200.0             # <<<<<<<<<<<<<<
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_sidereal_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_3, __pyx_float_43200_0, 43200.0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_8;
   goto __pyx_L0;
 
-  /* "bilby_cython/time.pyx":113
+  /* "bilby_cython/time.pyx":114
  * 
  * @cython.ufunc
- * cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time and equation of
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("bilby_cython.time.greenwich_sidereal_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_0greenwich_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_0greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_0greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
 static void __pyx_fuse_0greenwich_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   short __pyx_v_cast_in_0;
   char *__pyx_v_in_1;
   short __pyx_v_cast_in_1;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
   npy_intp __pyx_v_step_2;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0greenwich_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_0greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_0greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef short cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -24786,166 +25956,206 @@
  */
   __pyx_v_in_1 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* in_1 = args[1]
  *     cdef short cast_in_1
  *     cdef char* out_0 = args[2]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[2]);
 
   /* "UFuncDefinition":20
  *     cdef char* out_0 = args[2]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":21
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_2 = steps[2]
  * 
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
   /* "UFuncDefinition":22
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_2 = (__pyx_v_steps[2]);
 
-  /* "UFuncDefinition":25
+  /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<short*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":25
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<short*>in_0)[0]
  *             cast_in_1 = (<short*>in_1)[0]
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":26
- *     if True:
+          /* "UFuncDefinition":26
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<short*>in_0)[0]             # <<<<<<<<<<<<<<
  *             cast_in_1 = (<short*>in_1)[0]
  * 
  */
-    __pyx_v_cast_in_0 = (((short *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((short *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":27
+          /* "UFuncDefinition":27
  *         for i in range(n):
  *             cast_in_0 = (<short*>in_0)[0]
  *             cast_in_1 = (<short*>in_1)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_1 = (((short *)__pyx_v_in_1)[0]);
+          __pyx_v_cast_in_1 = (((short *)__pyx_v_in_1)[0]);
 
-    /* "UFuncDefinition":30
+          /* "UFuncDefinition":30
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":32
+          /* "UFuncDefinition":32
  *                 __pyx_fuse_0__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             in_1 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":33
+          /* "UFuncDefinition":33
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             in_1 += step_1
  *             out_0 += step_2
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":34
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":34
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             in_1 += step_1             # <<<<<<<<<<<<<<
  *             out_0 += step_2
  * 
  */
-    __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
+          __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
 
-    /* "UFuncDefinition":35
+          /* "UFuncDefinition":35
  *             in_0 += step_0
  *             in_1 += step_1
  *             out_0 += step_2             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+        }
+      }
+
+      /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<short*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_0greenwich_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_0greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_0greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_0greenwich_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_1greenwich_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   int __pyx_v_cast_in_0;
   char *__pyx_v_in_1;
   int __pyx_v_cast_in_1;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
   npy_intp __pyx_v_step_2;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1greenwich_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_1greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_1greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef int cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -24967,166 +26177,206 @@
  */
   __pyx_v_in_1 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* in_1 = args[1]
  *     cdef int cast_in_1
  *     cdef char* out_0 = args[2]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[2]);
 
   /* "UFuncDefinition":20
  *     cdef char* out_0 = args[2]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":21
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_2 = steps[2]
  * 
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
   /* "UFuncDefinition":22
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_2 = (__pyx_v_steps[2]);
 
-  /* "UFuncDefinition":25
+  /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<int*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":25
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<int*>in_0)[0]
  *             cast_in_1 = (<int*>in_1)[0]
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":26
- *     if True:
+          /* "UFuncDefinition":26
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<int*>in_0)[0]             # <<<<<<<<<<<<<<
  *             cast_in_1 = (<int*>in_1)[0]
  * 
  */
-    __pyx_v_cast_in_0 = (((int *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((int *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":27
+          /* "UFuncDefinition":27
  *         for i in range(n):
  *             cast_in_0 = (<int*>in_0)[0]
  *             cast_in_1 = (<int*>in_1)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_1 = (((int *)__pyx_v_in_1)[0]);
+          __pyx_v_cast_in_1 = (((int *)__pyx_v_in_1)[0]);
 
-    /* "UFuncDefinition":30
+          /* "UFuncDefinition":30
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":32
+          /* "UFuncDefinition":32
  *                 __pyx_fuse_1__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             in_1 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":33
+          /* "UFuncDefinition":33
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             in_1 += step_1
  *             out_0 += step_2
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":34
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":34
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             in_1 += step_1             # <<<<<<<<<<<<<<
  *             out_0 += step_2
  * 
  */
-    __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
+          __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
 
-    /* "UFuncDefinition":35
+          /* "UFuncDefinition":35
  *             in_0 += step_0
  *             in_1 += step_1
  *             out_0 += step_2             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+        }
+      }
+
+      /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<int*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_1greenwich_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_1greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_1greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_1greenwich_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_2greenwich_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   long __pyx_v_cast_in_0;
   char *__pyx_v_in_1;
   long __pyx_v_cast_in_1;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
   npy_intp __pyx_v_step_2;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2greenwich_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_2greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_2greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef long cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -25148,166 +26398,206 @@
  */
   __pyx_v_in_1 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* in_1 = args[1]
  *     cdef long cast_in_1
  *     cdef char* out_0 = args[2]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[2]);
 
   /* "UFuncDefinition":20
  *     cdef char* out_0 = args[2]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":21
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_2 = steps[2]
  * 
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
   /* "UFuncDefinition":22
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_2 = (__pyx_v_steps[2]);
 
-  /* "UFuncDefinition":25
+  /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":25
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<long*>in_0)[0]
  *             cast_in_1 = (<long*>in_1)[0]
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":26
- *     if True:
+          /* "UFuncDefinition":26
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<long*>in_0)[0]             # <<<<<<<<<<<<<<
  *             cast_in_1 = (<long*>in_1)[0]
  * 
  */
-    __pyx_v_cast_in_0 = (((long *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((long *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":27
+          /* "UFuncDefinition":27
  *         for i in range(n):
  *             cast_in_0 = (<long*>in_0)[0]
  *             cast_in_1 = (<long*>in_1)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_1 = (((long *)__pyx_v_in_1)[0]);
+          __pyx_v_cast_in_1 = (((long *)__pyx_v_in_1)[0]);
 
-    /* "UFuncDefinition":30
+          /* "UFuncDefinition":30
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":32
+          /* "UFuncDefinition":32
  *                 __pyx_fuse_2__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             in_1 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":33
+          /* "UFuncDefinition":33
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             in_1 += step_1
  *             out_0 += step_2
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":34
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":34
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             in_1 += step_1             # <<<<<<<<<<<<<<
  *             out_0 += step_2
  * 
  */
-    __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
+          __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
 
-    /* "UFuncDefinition":35
+          /* "UFuncDefinition":35
  *             in_0 += step_0
  *             in_1 += step_1
  *             out_0 += step_2             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+        }
+      }
+
+      /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_2greenwich_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_2greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_2greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_2greenwich_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_3greenwich_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   float __pyx_v_cast_in_0;
   char *__pyx_v_in_1;
   float __pyx_v_cast_in_1;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
   npy_intp __pyx_v_step_2;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3greenwich_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_3greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_3greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef float cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -25329,166 +26619,206 @@
  */
   __pyx_v_in_1 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* in_1 = args[1]
  *     cdef float cast_in_1
  *     cdef char* out_0 = args[2]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[2]);
 
   /* "UFuncDefinition":20
  *     cdef char* out_0 = args[2]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":21
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_2 = steps[2]
  * 
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
   /* "UFuncDefinition":22
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_2 = (__pyx_v_steps[2]);
 
-  /* "UFuncDefinition":25
+  /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<float*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":25
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<float*>in_0)[0]
  *             cast_in_1 = (<float*>in_1)[0]
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":26
- *     if True:
+          /* "UFuncDefinition":26
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<float*>in_0)[0]             # <<<<<<<<<<<<<<
  *             cast_in_1 = (<float*>in_1)[0]
  * 
  */
-    __pyx_v_cast_in_0 = (((float *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((float *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":27
+          /* "UFuncDefinition":27
  *         for i in range(n):
  *             cast_in_0 = (<float*>in_0)[0]
  *             cast_in_1 = (<float*>in_1)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_1 = (((float *)__pyx_v_in_1)[0]);
+          __pyx_v_cast_in_1 = (((float *)__pyx_v_in_1)[0]);
 
-    /* "UFuncDefinition":30
+          /* "UFuncDefinition":30
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":32
+          /* "UFuncDefinition":32
  *                 __pyx_fuse_3__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             in_1 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":33
+          /* "UFuncDefinition":33
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             in_1 += step_1
  *             out_0 += step_2
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":34
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":34
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             in_1 += step_1             # <<<<<<<<<<<<<<
  *             out_0 += step_2
  * 
  */
-    __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
+          __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
 
-    /* "UFuncDefinition":35
+          /* "UFuncDefinition":35
  *             in_0 += step_0
  *             in_1 += step_1
  *             out_0 += step_2             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+        }
+      }
+
+      /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<float*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_3greenwich_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_3greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_3greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_3greenwich_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_4greenwich_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
   CYTHON_UNUSED npy_intp __pyx_v_i;
   npy_intp __pyx_v_n;
   char *__pyx_v_in_0;
   double __pyx_v_cast_in_0;
   char *__pyx_v_in_1;
   double __pyx_v_cast_in_1;
   char *__pyx_v_out_0;
-  PyObject *__pyx_v_cast_out_0 = 0;
+  double __pyx_v_cast_out_0;
   npy_intp __pyx_v_step_0;
   npy_intp __pyx_v_step_1;
   npy_intp __pyx_v_step_2;
-  __Pyx_RefNannyDeclarations
   npy_intp __pyx_t_1;
   npy_intp __pyx_t_2;
   npy_intp __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_4greenwich_sidereal_time_ufunc_def", 1);
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
 
   /* "UFuncDefinition":13
- * cdef void __pyx_fuse_4greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :
+ * cdef void __pyx_fuse_4greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
  *     cdef char* in_0 = args[0]
  *     cdef double cast_in_0
  */
   __pyx_v_n = (__pyx_v_dimensions[0]);
 
@@ -25510,140 +26840,400 @@
  */
   __pyx_v_in_1 = (__pyx_v_args[1]);
 
   /* "UFuncDefinition":18
  *     cdef char* in_1 = args[1]
  *     cdef double cast_in_1
  *     cdef char* out_0 = args[2]             # <<<<<<<<<<<<<<
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  */
   __pyx_v_out_0 = (__pyx_v_args[2]);
 
   /* "UFuncDefinition":20
  *     cdef char* out_0 = args[2]
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]
  */
   __pyx_v_step_0 = (__pyx_v_steps[0]);
 
   /* "UFuncDefinition":21
- *     cdef object cast_out_0
+ *     cdef double cast_out_0
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
  *     cdef npy_intp step_2 = steps[2]
  * 
  */
   __pyx_v_step_1 = (__pyx_v_steps[1]);
 
   /* "UFuncDefinition":22
  *     cdef npy_intp step_0 = steps[0]
  *     cdef npy_intp step_1 = steps[1]
  *     cdef npy_intp step_2 = steps[2]             # <<<<<<<<<<<<<<
  * 
- *     if True:
+ *     with gil:
  */
   __pyx_v_step_2 = (__pyx_v_steps[2]);
 
-  /* "UFuncDefinition":25
+  /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
  * 
- *     if True:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<double*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":25
+ * 
+ *     with gil:
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             cast_in_0 = (<double*>in_0)[0]
  *             cast_in_1 = (<double*>in_1)[0]
  */
-  __pyx_t_1 = __pyx_v_n;
-  __pyx_t_2 = __pyx_t_1;
-  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
-    __pyx_v_i = __pyx_t_3;
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
 
-    /* "UFuncDefinition":26
- *     if True:
+          /* "UFuncDefinition":26
+ *     with gil:
  *         for i in range(n):
  *             cast_in_0 = (<double*>in_0)[0]             # <<<<<<<<<<<<<<
  *             cast_in_1 = (<double*>in_1)[0]
  * 
  */
-    __pyx_v_cast_in_0 = (((double *)__pyx_v_in_0)[0]);
+          __pyx_v_cast_in_0 = (((double *)__pyx_v_in_0)[0]);
 
-    /* "UFuncDefinition":27
+          /* "UFuncDefinition":27
  *         for i in range(n):
  *             cast_in_0 = (<double*>in_0)[0]
  *             cast_in_1 = (<double*>in_1)[0]             # <<<<<<<<<<<<<<
  * 
  *             cast_out_0 = \
  */
-    __pyx_v_cast_in_1 = (((double *)__pyx_v_in_1)[0]);
+          __pyx_v_cast_in_1 = (((double *)__pyx_v_in_1)[0]);
 
-    /* "UFuncDefinition":30
+          /* "UFuncDefinition":30
  * 
  *             cast_out_0 = \
  *                 __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)             # <<<<<<<<<<<<<<
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  */
-    __pyx_t_4 = __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_XDECREF_SET(__pyx_v_cast_out_0, __pyx_t_4);
-    __pyx_t_4 = 0;
+          __pyx_t_4 = __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
 
-    /* "UFuncDefinition":32
+          /* "UFuncDefinition":32
  *                 __pyx_fuse_4__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)             # <<<<<<<<<<<<<<
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
  *             in_0 += step_0
  *             in_1 += step_1
  */
-    (((void **)__pyx_v_out_0)[0]) = ((void *)__Pyx_NewRef(__pyx_v_cast_out_0));
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
 
-    /* "UFuncDefinition":33
+          /* "UFuncDefinition":33
  * 
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0             # <<<<<<<<<<<<<<
  *             in_1 += step_1
  *             out_0 += step_2
  */
-    __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
 
-    /* "UFuncDefinition":34
- *             (<void**>out_0)[0] = <void*>__Pyx_NewRef(cast_out_0)
+          /* "UFuncDefinition":34
+ *             (<double*>out_0)[0] = cast_out_0
  *             in_0 += step_0
  *             in_1 += step_1             # <<<<<<<<<<<<<<
  *             out_0 += step_2
  * 
  */
-    __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
+          __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
 
-    /* "UFuncDefinition":35
+          /* "UFuncDefinition":35
  *             in_0 += step_0
  *             in_1 += step_1
  *             out_0 += step_2             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+        }
+      }
+
+      /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<double*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
   }
 
   /* "UFuncDefinition":11
  * 
  * @cname("__pyx_fuse_4greenwich_sidereal_time_ufunc_def")
- * cdef void __pyx_fuse_4greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * :             # <<<<<<<<<<<<<<
+ * cdef void __pyx_fuse_4greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
  *     cdef npy_intp i
  *     cdef npy_intp n = dimensions[0]
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
   __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_4greenwich_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
+  __pyx_L0:;
+}
+
+static void __pyx_fuse_5greenwich_sidereal_time_ufunc_def(char **__pyx_v_args, npy_intp const *__pyx_v_dimensions, npy_intp const *__pyx_v_steps, CYTHON_UNUSED void *__pyx_v_data) {
+  CYTHON_UNUSED npy_intp __pyx_v_i;
+  npy_intp __pyx_v_n;
+  char *__pyx_v_in_0;
+  long double __pyx_v_cast_in_0;
+  char *__pyx_v_in_1;
+  long double __pyx_v_cast_in_1;
+  char *__pyx_v_out_0;
+  double __pyx_v_cast_out_0;
+  npy_intp __pyx_v_step_0;
+  npy_intp __pyx_v_step_1;
+  npy_intp __pyx_v_step_2;
+  npy_intp __pyx_t_1;
+  npy_intp __pyx_t_2;
+  npy_intp __pyx_t_3;
+  double __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
+
+  /* "UFuncDefinition":13
+ * cdef void __pyx_fuse_5greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]             # <<<<<<<<<<<<<<
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ */
+  __pyx_v_n = (__pyx_v_dimensions[0]);
+
+  /* "UFuncDefinition":14
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ *     cdef char* in_0 = args[0]             # <<<<<<<<<<<<<<
+ *     cdef long double cast_in_0
+ *     cdef char* in_1 = args[1]
+ */
+  __pyx_v_in_0 = (__pyx_v_args[0]);
+
+  /* "UFuncDefinition":16
+ *     cdef char* in_0 = args[0]
+ *     cdef long double cast_in_0
+ *     cdef char* in_1 = args[1]             # <<<<<<<<<<<<<<
+ *     cdef long double cast_in_1
+ *     cdef char* out_0 = args[2]
+ */
+  __pyx_v_in_1 = (__pyx_v_args[1]);
+
+  /* "UFuncDefinition":18
+ *     cdef char* in_1 = args[1]
+ *     cdef long double cast_in_1
+ *     cdef char* out_0 = args[2]             # <<<<<<<<<<<<<<
+ *     cdef double cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ */
+  __pyx_v_out_0 = (__pyx_v_args[2]);
+
+  /* "UFuncDefinition":20
+ *     cdef char* out_0 = args[2]
+ *     cdef double cast_out_0
+ *     cdef npy_intp step_0 = steps[0]             # <<<<<<<<<<<<<<
+ *     cdef npy_intp step_1 = steps[1]
+ *     cdef npy_intp step_2 = steps[2]
+ */
+  __pyx_v_step_0 = (__pyx_v_steps[0]);
+
+  /* "UFuncDefinition":21
+ *     cdef double cast_out_0
+ *     cdef npy_intp step_0 = steps[0]
+ *     cdef npy_intp step_1 = steps[1]             # <<<<<<<<<<<<<<
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ */
+  __pyx_v_step_1 = (__pyx_v_steps[1]);
+
+  /* "UFuncDefinition":22
+ *     cdef npy_intp step_0 = steps[0]
+ *     cdef npy_intp step_1 = steps[1]
+ *     cdef npy_intp step_2 = steps[2]             # <<<<<<<<<<<<<<
+ * 
+ *     with gil:
+ */
+  __pyx_v_step_2 = (__pyx_v_steps[2]);
+
+  /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      /*try:*/ {
+
+        /* "UFuncDefinition":25
+ * 
+ *     with gil:
+ *         for i in range(n):             # <<<<<<<<<<<<<<
+ *             cast_in_0 = (<long double*>in_0)[0]
+ *             cast_in_1 = (<long double*>in_1)[0]
+ */
+        __pyx_t_1 = __pyx_v_n;
+        __pyx_t_2 = __pyx_t_1;
+        for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+          __pyx_v_i = __pyx_t_3;
+
+          /* "UFuncDefinition":26
+ *     with gil:
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]             # <<<<<<<<<<<<<<
+ *             cast_in_1 = (<long double*>in_1)[0]
+ * 
+ */
+          __pyx_v_cast_in_0 = (((long double *)__pyx_v_in_0)[0]);
+
+          /* "UFuncDefinition":27
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]
+ *             cast_in_1 = (<long double*>in_1)[0]             # <<<<<<<<<<<<<<
+ * 
+ *             cast_out_0 = \
+ */
+          __pyx_v_cast_in_1 = (((long double *)__pyx_v_in_1)[0]);
+
+          /* "UFuncDefinition":30
+ * 
+ *             cast_out_0 = \
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)             # <<<<<<<<<<<<<<
+ * 
+ *             (<double*>out_0)[0] = cast_out_0
+ */
+          __pyx_t_4 = __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(__pyx_v_cast_in_0, __pyx_v_cast_in_1); if (unlikely(__pyx_t_4 == ((double)-1.0) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L4_error)
+          __pyx_v_cast_out_0 = __pyx_t_4;
+
+          /* "UFuncDefinition":32
+ *                 __pyx_fuse_5__pyx_f_12bilby_cython_4time_greenwich_sidereal_time(cast_in_0, cast_in_1)
+ * 
+ *             (<double*>out_0)[0] = cast_out_0             # <<<<<<<<<<<<<<
+ *             in_0 += step_0
+ *             in_1 += step_1
+ */
+          (((double *)__pyx_v_out_0)[0]) = __pyx_v_cast_out_0;
+
+          /* "UFuncDefinition":33
+ * 
+ *             (<double*>out_0)[0] = cast_out_0
+ *             in_0 += step_0             # <<<<<<<<<<<<<<
+ *             in_1 += step_1
+ *             out_0 += step_2
+ */
+          __pyx_v_in_0 = (__pyx_v_in_0 + __pyx_v_step_0);
+
+          /* "UFuncDefinition":34
+ *             (<double*>out_0)[0] = cast_out_0
+ *             in_0 += step_0
+ *             in_1 += step_1             # <<<<<<<<<<<<<<
+ *             out_0 += step_2
+ * 
+ */
+          __pyx_v_in_1 = (__pyx_v_in_1 + __pyx_v_step_1);
+
+          /* "UFuncDefinition":35
+ *             in_0 += step_0
+ *             in_1 += step_1
+ *             out_0 += step_2             # <<<<<<<<<<<<<<
+ * 
+ */
+          __pyx_v_out_0 = (__pyx_v_out_0 + __pyx_v_step_2);
+        }
+      }
+
+      /* "UFuncDefinition":24
+ *     cdef npy_intp step_2 = steps[2]
+ * 
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         for i in range(n):
+ *             cast_in_0 = (<long double*>in_0)[0]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "UFuncDefinition":11
+ * 
+ * @cname("__pyx_fuse_5greenwich_sidereal_time_ufunc_def")
+ * cdef void __pyx_fuse_5greenwich_sidereal_time_ufunc_def(char **args, const npy_intp *dimensions, const npy_intp* steps, void* data) except * nogil:             # <<<<<<<<<<<<<<
+ *     cdef npy_intp i
+ *     cdef npy_intp n = dimensions[0]
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
+  __Pyx_AddTraceback("UFuncDefinition.__pyx_fuse_5greenwich_sidereal_time_ufunc_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cast_out_0);
-  __Pyx_RefNannyFinishContext();
 }
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
@@ -28193,72 +29783,72 @@
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LEAP_SECONDS); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_10 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(1, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_12bilby_cython_4time_NUM_LEAPS = __pyx_t_10;
 
-  /* "bilby_cython/time.pyx":40
+  /* "bilby_cython/time.pyx":41
  * 
  * @cython.ufunc
  * cdef int n_leap_seconds(real date):             # <<<<<<<<<<<<<<
  *     """
  *     Find the number of leap seconds required for the specified date.
  */
-  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs(), __pyx_data, __pyx_types(), 5, 1, 1, PyUFunc_None, "n_leap_seconds", "\n    Find the number of leap seconds required for the specified date.\n\n    Search in reverse order as in practice, almost all requested times will\n    be after the most recent leap.\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs(), __pyx_data, __pyx_types(), 6, 1, 1, PyUFunc_None, "n_leap_seconds", "\n    Find the number of leap seconds required for the specified date.\n\n    Search in reverse order as in practice, almost all requested times will\n    be after the most recent leap.\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_n_leap_seconds, __pyx_t_5) < 0) __PYX_ERR(1, 40, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_n_leap_seconds, __pyx_t_5) < 0) __PYX_ERR(1, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "bilby_cython/time.pyx":56
+  /* "bilby_cython/time.pyx":57
  * 
  * @cython.ufunc
  * cdef datetime gps_time_to_utc(real secs):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from GPS time to UTC, this is a necessary intermediate step in
  */
-  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs1(), __pyx_data1, __pyx_types1(), 5, 1, 1, PyUFunc_None, "gps_time_to_utc", "\n    Convert from GPS time to UTC, this is a necessary intermediate step in\n    converting from GPS to GMST.\n\n    Add the number of seconds minus the leap seconds to the GPS epoch.\n\n    Parameters\n    ----------\n    secs: double\n        The time to convert in GPS time.\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 56, __pyx_L1_error)
+  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs1(), __pyx_data1, __pyx_types1(), 6, 1, 1, PyUFunc_None, "gps_time_to_utc", "\n    Convert from GPS time to UTC, this is a necessary intermediate step in\n    converting from GPS to GMST.\n\n    Add the number of seconds minus the leap seconds to the GPS epoch.\n\n    Parameters\n    ----------\n    secs: double\n        The time to convert in GPS time.\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_gps_time_to_utc, __pyx_t_5) < 0) __PYX_ERR(1, 56, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_gps_time_to_utc, __pyx_t_5) < 0) __PYX_ERR(1, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "bilby_cython/time.pyx":74
+  /* "bilby_cython/time.pyx":75
  * 
  * @cython.ufunc
  * cdef double utc_to_julian_day(datetime time):             # <<<<<<<<<<<<<<
  *     """
  *     Convert from UTC to Julian day, this is a necessary intermediate step in
  */
-  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs2(), __pyx_data2, __pyx_types2(), 1, 1, 1, PyUFunc_None, "utc_to_julian_day", "\n    Convert from UTC to Julian day, this is a necessary intermediate step in\n    converting from GPS to GMST.\n\n    Parameters\n    ----------\n    time: datetime\n        The UTC time to convert\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 74, __pyx_L1_error)
+  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs2(), __pyx_data2, __pyx_types2(), 1, 1, 1, PyUFunc_None, "utc_to_julian_day", "\n    Convert from UTC to Julian day, this is a necessary intermediate step in\n    converting from GPS to GMST.\n\n    Parameters\n    ----------\n    time: datetime\n        The UTC time to convert\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_utc_to_julian_day, __pyx_t_5) < 0) __PYX_ERR(1, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_utc_to_julian_day, __pyx_t_5) < 0) __PYX_ERR(1, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "bilby_cython/time.pyx":100
+  /* "bilby_cython/time.pyx":101
  * 
  * @cython.ufunc
- * cdef greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_mean_sidereal_time(real gps_time):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time.
  */
-  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs3(), __pyx_data3, __pyx_types3(), 5, 1, 1, PyUFunc_None, "greenwich_mean_sidereal_time", "\n    Compute the Greenwich mean sidereal time from the GPS time.\n\n    Parameters\n    ----------\n    gps_time: double\n        The GPS time to convert\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 100, __pyx_L1_error)
+  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs3(), __pyx_data3, __pyx_types3(), 6, 1, 1, PyUFunc_None, "greenwich_mean_sidereal_time", "\n    Compute the Greenwich mean sidereal time from the GPS time.\n\n    Parameters\n    ----------\n    gps_time: double\n        The GPS time to convert\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_greenwich_mean_sidereal_time, __pyx_t_5) < 0) __PYX_ERR(1, 100, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_greenwich_mean_sidereal_time, __pyx_t_5) < 0) __PYX_ERR(1, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "bilby_cython/time.pyx":113
+  /* "bilby_cython/time.pyx":114
  * 
  * @cython.ufunc
- * cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
+ * cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):             # <<<<<<<<<<<<<<
  *     """
  *     Compute the Greenwich mean sidereal time from the GPS time and equation of
  */
-  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs4(), __pyx_data4, __pyx_types4(), 5, 2, 1, PyUFunc_None, "greenwich_sidereal_time", "\n    Compute the Greenwich mean sidereal time from the GPS time and equation of\n    equinoxes.\n\n    Based on XLALGreenwichSiderealTime in lalsuite/lal/lib/XLALSiderealTime.c.\n\n    Parameters\n    ----------\n    gps_time: double\n        The GPS time to convert\n    equation_of_equinoxes: double\n        The equation of equinoxes\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 113, __pyx_L1_error)
+  __pyx_t_5 = PyUFunc_FromFuncAndData(__pyx_funcs4(), __pyx_data4, __pyx_types4(), 6, 2, 1, PyUFunc_None, "greenwich_sidereal_time", "\n    Compute the Greenwich mean sidereal time from the GPS time and equation of\n    equinoxes.\n\n    Based on XLALGreenwichSiderealTime in lalsuite/lal/lib/XLALSiderealTime.c.\n\n    Parameters\n    ----------\n    gps_time: double\n        The GPS time to convert\n    equation_of_equinoxes: double\n        The equation of equinoxes\n    ", 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_greenwich_sidereal_time, __pyx_t_5) < 0) __PYX_ERR(1, 113, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_greenwich_sidereal_time, __pyx_t_5) < 0) __PYX_ERR(1, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "bilby_cython/time.pyx":1
  * import numpy as np             # <<<<<<<<<<<<<<
  * from cmath import pi
  * from cpython.datetime cimport datetime, timedelta
  */
@@ -30750,24 +32340,14 @@
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
 #endif
 
-/* PyIntFromDouble */
-#if PY_MAJOR_VERSION < 3
-static CYTHON_INLINE PyObject* __Pyx_PyInt_FromDouble(double value) {
-    if (value >= (double)LONG_MIN && value <= (double)LONG_MAX) {
-        return PyInt_FromLong((long)value);
-    }
-    return PyLong_FromDouble(value);
-}
-#endif
-
 /* PyFloatBinop */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyFloat_TrueDivideObjC(PyObject *op1, PyObject *op2, double floatval, int inplace, int zerodivision_check) {
     const double b = floatval;
     double a, result;
     CYTHON_UNUSED_VAR(inplace);
     CYTHON_UNUSED_VAR(zerodivision_check);
@@ -31949,56 +33529,62 @@
 /* UFuncConsts */
 static PyUFuncGenericFunction* __pyx_funcs(void) {
     static PyUFuncGenericFunction arr[] = {
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_0n_leap_seconds_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_1n_leap_seconds_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_2n_leap_seconds_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_3n_leap_seconds_ufunc_def),
-        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4n_leap_seconds_ufunc_def)
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4n_leap_seconds_ufunc_def),
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_5n_leap_seconds_ufunc_def)
     };
     return arr;
 }
 static char* __pyx_types(void) {
     static char arr[] = {
         NPY_SHORT,
         NPY_INT,
         NPY_INT,
         NPY_INT,
         NPY_LONG,
         NPY_INT,
         NPY_FLOAT,
         NPY_INT,
         NPY_DOUBLE,
+        NPY_INT,
+        NPY_LONGDOUBLE,
         NPY_INT
     };
     return arr;
 }
 
 /* UFuncConsts */
 static PyUFuncGenericFunction* __pyx_funcs1(void) {
     static PyUFuncGenericFunction arr[] = {
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_0gps_time_to_utc_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_1gps_time_to_utc_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_2gps_time_to_utc_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_3gps_time_to_utc_ufunc_def),
-        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4gps_time_to_utc_ufunc_def)
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4gps_time_to_utc_ufunc_def),
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_5gps_time_to_utc_ufunc_def)
     };
     return arr;
 }
 static char* __pyx_types1(void) {
     static char arr[] = {
         NPY_SHORT,
         NPY_OBJECT,
         NPY_INT,
         NPY_OBJECT,
         NPY_LONG,
         NPY_OBJECT,
         NPY_FLOAT,
         NPY_OBJECT,
         NPY_DOUBLE,
+        NPY_OBJECT,
+        NPY_LONGDOUBLE,
         NPY_OBJECT
     };
     return arr;
 }
 
 /* UFuncConsts */
 static PyUFuncGenericFunction* __pyx_funcs2(void) {
@@ -32018,62 +33604,69 @@
 /* UFuncConsts */
 static PyUFuncGenericFunction* __pyx_funcs3(void) {
     static PyUFuncGenericFunction arr[] = {
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_0greenwich_mean_sidereal_time_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_1greenwich_mean_sidereal_time_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_2greenwich_mean_sidereal_time_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_3greenwich_mean_sidereal_time_ufunc_def),
-        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def)
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4greenwich_mean_sidereal_time_ufunc_def),
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_5greenwich_mean_sidereal_time_ufunc_def)
     };
     return arr;
 }
 static char* __pyx_types3(void) {
     static char arr[] = {
         NPY_SHORT,
-        NPY_OBJECT,
+        NPY_DOUBLE,
         NPY_INT,
-        NPY_OBJECT,
+        NPY_DOUBLE,
         NPY_LONG,
-        NPY_OBJECT,
+        NPY_DOUBLE,
         NPY_FLOAT,
-        NPY_OBJECT,
         NPY_DOUBLE,
-        NPY_OBJECT
+        NPY_DOUBLE,
+        NPY_DOUBLE,
+        NPY_LONGDOUBLE,
+        NPY_DOUBLE
     };
     return arr;
 }
 
 /* UFuncConsts */
 static PyUFuncGenericFunction* __pyx_funcs4(void) {
     static PyUFuncGenericFunction arr[] = {
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_0greenwich_sidereal_time_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_1greenwich_sidereal_time_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_2greenwich_sidereal_time_ufunc_def),
         __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_3greenwich_sidereal_time_ufunc_def),
-        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4greenwich_sidereal_time_ufunc_def)
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_4greenwich_sidereal_time_ufunc_def),
+        __PYX_PYUFUNCGENERICFUNCTION_CAST(&__pyx_fuse_5greenwich_sidereal_time_ufunc_def)
     };
     return arr;
 }
 static char* __pyx_types4(void) {
     static char arr[] = {
         NPY_SHORT,
         NPY_SHORT,
-        NPY_OBJECT,
+        NPY_DOUBLE,
         NPY_INT,
         NPY_INT,
-        NPY_OBJECT,
+        NPY_DOUBLE,
         NPY_LONG,
         NPY_LONG,
-        NPY_OBJECT,
+        NPY_DOUBLE,
         NPY_FLOAT,
         NPY_FLOAT,
-        NPY_OBJECT,
         NPY_DOUBLE,
         NPY_DOUBLE,
-        NPY_OBJECT
+        NPY_DOUBLE,
+        NPY_DOUBLE,
+        NPY_LONGDOUBLE,
+        NPY_LONGDOUBLE,
+        NPY_DOUBLE
     };
     return arr;
 }
 
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
```

### Comparing `bilby_cython-0.5.0/bilby_cython/time.pyx` & `bilby_cython-0.5.1/bilby_cython/time.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 ctypedef fused real:
     short
     int
     long
     float
     double
+    long double
 
 
 @cython.ufunc
 cdef int n_leap_seconds(real date):
     """
     Find the number of leap seconds required for the specified date.
 
@@ -62,15 +63,15 @@
 
     Parameters
     ----------
     secs: double
         The time to convert in GPS time.
     """
     cdef datetime date_before_leaps
-    date_before_leaps = GPS_EPOCH + timedelta(seconds=secs - n_leap_seconds(int(secs)))
+    date_before_leaps = GPS_EPOCH + timedelta(seconds=<double>secs - n_leap_seconds(secs))
     return date_before_leaps
 
 
 @cython.ufunc
 cdef double utc_to_julian_day(datetime time):
     """
     Convert from UTC to Julian day, this is a necessary intermediate step in
@@ -93,43 +94,43 @@
         + 1721014
         + second / (60 * 60 * 24)
         - 0.5
     )
 
 
 @cython.ufunc
-cdef greenwich_mean_sidereal_time(real gps_time):
+cdef double greenwich_mean_sidereal_time(real gps_time):
     """
     Compute the Greenwich mean sidereal time from the GPS time.
 
     Parameters
     ----------
     gps_time: double
         The GPS time to convert
     """
     return greenwich_sidereal_time(gps_time, 0)
 
 
 @cython.ufunc
-cdef greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):
+cdef double greenwich_sidereal_time(real gps_time, real equation_of_equinoxes):
     """
     Compute the Greenwich mean sidereal time from the GPS time and equation of
     equinoxes.
 
     Based on XLALGreenwichSiderealTime in lalsuite/lal/lib/XLALSiderealTime.c.
 
     Parameters
     ----------
     gps_time: double
         The GPS time to convert
     equation_of_equinoxes: double
         The equation of equinoxes
     """
     cdef double julian_day, t_hi, t_lo, t, sidereal_time
-    julian_day = utc_to_julian_day(gps_time_to_utc(gps_time // 1))
+    julian_day = utc_to_julian_day(gps_time_to_utc(gps_time))
     t_hi = (julian_day - EPOCH_J2000_0_JD) / 36525.0
     t_lo = (gps_time % 1) / (36525.0 * 86400.0)
 
     t = t_hi + t_lo
 
     sidereal_time = equation_of_equinoxes + (-6.2e-6 * t + 0.093104) * t**2 + 67310.54841
     sidereal_time += 8640184.812866 * t_lo
```

### Comparing `bilby_cython-0.5.0/docs/Makefile` & `bilby_cython-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/docs/conf.py` & `bilby_cython-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/docs/index.rst` & `bilby_cython-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bilby_cython-0.5.0/pyproject.toml` & `bilby_cython-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 description = "Optimized functionality for Bilby"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 license = {text = "MIT"}
 dependencies = ["numpy"]
 readme = "README.md"
 urls = {Homepage = "https://git.ligo.org/colm.talbot/bilby-cython"}
```

### Comparing `bilby_cython-0.5.0/setup.py` & `bilby_cython-0.5.1/setup.py`

 * *Files identical despite different names*

