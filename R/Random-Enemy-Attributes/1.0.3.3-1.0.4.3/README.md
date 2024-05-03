# Comparing `tmp/Random_Enemy_Attributes-1.0.3.3.tar.gz` & `tmp/Random_Enemy_Attributes-1.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Random_Enemy_Attributes-1.0.3.3.tar", last modified: Wed Nov  8 00:04:34 2023, max compression
+gzip compressed data, was "random_enemy_attributes-1.0.4.3.tar", last modified: Fri May  3 17:50:37 2024, max compression
```

## Comparing `Random_Enemy_Attributes-1.0.3.3.tar` & `Random_Enemy_Attributes-1.0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-08 00:04:34.093982 Random_Enemy_Attributes-1.0.3.3/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-08 00:04:34.084368 Random_Enemy_Attributes-1.0.3.3/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-08 00:04:34.086612 Random_Enemy_Attributes-1.0.3.3/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     2539 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     1068 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     1255 2023-11-08 00:04:34.093495 Random_Enemy_Attributes-1.0.3.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      907 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-08 00:04:34.089584 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/
--rw-r--r--   0 runner     (501) staff       (20)     6925 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Enemy_Offset_Locations.h
--rw-r--r--   0 runner     (501) staff       (20)    82568 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1748 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes.h
--rw-r--r--   0 runner     (501) staff       (20)   651349 2023-11-08 00:04:33.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1468 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pxd
--rw-r--r--   0 runner     (501) staff       (20)     4773 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pyx
--rw-r--r--   0 runner     (501) staff       (20)    22983 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/patternedAI_Array.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-08 00:04:34.090952 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1255 2023-11-08 00:04:34.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      783 2023-11-08 00:04:34.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-11-08 00:04:34.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       24 2023-11-08 00:04:34.000000 Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      141 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       15 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-11-08 00:04:34.094082 Random_Enemy_Attributes-1.0.3.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1118 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-11-08 00:04:34.092889 Random_Enemy_Attributes-1.0.3.3/tools/
--rw-r--r--   0 runner     (501) staff       (20)      438 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/tools/build-ci.sh
--rw-r--r--   0 runner     (501) staff       (20)      195 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/tools/build-cython.sh
--rw-r--r--   0 runner     (501) staff       (20)      220 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/tools/build-standalone.sh
--rw-r--r--   0 runner     (501) staff       (20)      502 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/tools/build-wheel.sh
--rw-r--r--   0 runner     (501) staff       (20)      326 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/tools/clean.sh
--rw-r--r--   0 runner     (501) staff       (20)      409 2023-11-08 00:03:45.000000 Random_Enemy_Attributes-1.0.3.3/tools/venv.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 17:50:37.071841 random_enemy_attributes-1.0.4.3/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 17:50:37.067514 random_enemy_attributes-1.0.4.3/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 17:50:37.068527 random_enemy_attributes-1.0.4.3/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     2641 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)     1068 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     1255 2024-05-03 17:50:37.071617 random_enemy_attributes-1.0.4.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      907 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 17:50:37.069793 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/
+-rw-r--r--   0 runner     (501) staff       (20)     6925 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Enemy_Offset_Locations.h
+-rw-r--r--   0 runner     (501) staff       (20)    82568 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1767 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes.h
+-rw-r--r--   0 runner     (501) staff       (20)   652864 2024-05-03 17:50:36.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1468 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     4773 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pyx
+-rw-r--r--   0 runner     (501) staff       (20)    22983 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/patternedAI_Array.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 17:50:37.071339 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1255 2024-05-03 17:50:37.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      783 2024-05-03 17:50:37.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-03 17:50:37.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       24 2024-05-03 17:50:37.000000 random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      141 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       15 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-03 17:50:37.071881 random_enemy_attributes-1.0.4.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1118 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 17:50:37.071111 random_enemy_attributes-1.0.4.3/tools/
+-rw-r--r--   0 runner     (501) staff       (20)      439 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/tools/build-ci.sh
+-rw-r--r--   0 runner     (501) staff       (20)      195 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/tools/build-cython.sh
+-rw-r--r--   0 runner     (501) staff       (20)      220 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/tools/build-standalone.sh
+-rw-r--r--   0 runner     (501) staff       (20)      502 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/tools/build-wheel.sh
+-rw-r--r--   0 runner     (501) staff       (20)      326 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/tools/clean.sh
+-rw-r--r--   0 runner     (501) staff       (20)      409 2024-05-03 17:50:21.000000 random_enemy_attributes-1.0.4.3/tools/venv.sh
```

### Comparing `Random_Enemy_Attributes-1.0.3.3/.github/workflows/release-pypi.yml` & `random_enemy_attributes-1.0.4.3/.github/workflows/release-pypi.yml`

 * *Files 10% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
     runs-on: ${{ matrix.os }}
 
     name: ${{ matrix.os }} - Python ${{ matrix.python }}
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
           submodules: 'recursive'
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
      
       - name: Install Python packages
         run: python -m pip install --upgrade build pip cython wheel auditwheel
 
       - name: build wheel
@@ -50,64 +50,65 @@
         shell: bash
 
       - name: build sdist
         run: python -m build --sdist
         if: ${{ matrix.os == 'macos-latest' && matrix.python == '3.12' }}
 
       - name: Store the packages
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         with:
-          name: python-package-distributions
+          name: python-package-distributions-${{ matrix.os }}-${{ matrix.python }}
           path: dist
 
   linux-build:
     strategy:
       fail-fast: false
       matrix:
         python:
           - 'cp38-cp38'
           - 'cp39-cp39'
           - 'cp310-cp310'
           - 'cp311-cp311'
           - 'cp312-cp312'
 
     runs-on: ubuntu-latest
-    container: quay.io/pypa/manylinux2014_x86_64
+    container: quay.io/pypa/manylinux_2_28_x86_64
 
     name: Linux - Python ${{ matrix.python }}
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
           submodules: 'recursive'
 
       - name: build wheel
         run: |
           chmod 777 ./tools/build-ci.sh && PYTHON_VERSION=${{ matrix.python }} ./tools/build-ci.sh
       
       - name: Store the packages
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         with:
-          name: python-package-distributions
+          name: python-package-distributions-linux-${{ matrix.python }}
           path: dist
 
   pypi:
     runs-on: 'ubuntu-latest'
     needs:
       - build
       - linux-build
 
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v4
         with:
-          name: python-package-distributions
           path: dist/
+          pattern: python-package-distributions-*
+          merge-multiple: true
 
       - name: Publish 📦 to PyPI
         if: ${{ github.ref == 'refs/heads/master' }}
         uses: pypa/gh-action-pypi-publish@master
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `Random_Enemy_Attributes-1.0.3.3/LICENSE` & `random_enemy_attributes-1.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/PKG-INFO` & `random_enemy_attributes-1.0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Random_Enemy_Attributes
-Version: 1.0.3.3
+Version: 1.0.4.3
 Summary: Randomizes enemy stat values for most of the enemies in the game Metroid Prime.
 Home-page: https://github.com/Fantaselion/PARAMETEREDITOR
 Author: Fantaselion
 Author-email: fantaselion@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Random_Enemy_Attributes-1.0.3.3/README.md` & `random_enemy_attributes-1.0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Enemy_Offset_Locations.h` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Enemy_Offset_Locations.h`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes.cpp` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes.cpp`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes.h` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #pragma once
 #include <fstream>
 #include <vector>
-
+#include <cstdint>
 
 using namespace std;
 
 
 class Random_Enemy_Attributes
 {
 
@@ -40,8 +40,8 @@
 	float knockbackPowerLow = 0.1;
 	float knockbackPowerHigh = 40.0;
 	bool randoScaleSeperate = true;
 	string inputLocation;
 	string outputLocation;
 	int times = 0;
 	int cur_Pak = 0;
-};
+};
```

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.cpp` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.5 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "Random_Enemy_Attributes/Random_Enemy_Attributes.h"
         ],
@@ -63,18 +63,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_5" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030005F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -158,14 +158,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -219,14 +221,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -280,60 +284,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -416,14 +443,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -624,26 +654,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -656,15 +687,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -689,15 +719,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -775,16 +805,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -984,15 +1019,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1128,15 +1163,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1215,15 +1250,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1242,14 +1277,15 @@
 #include <string.h>
 #include <string>
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <stdio.h>
+#include <stddef.h>
 #include "pythread.h"
 #include <stdint.h>
 #include <vector>
 #include "Random_Enemy_Attributes.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
@@ -1325,32 +1361,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1392,15 +1411,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1742,33 +1761,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-    static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -1904,30 +1924,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_5
-#define __PYX_HAVE_RT_ImportType_proto_3_0_5
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_5(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_5(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_5 {
-   __Pyx_ImportType_CheckSize_Error_3_0_5 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_5 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_5 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_5(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_5 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -2012,15 +2032,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -2280,14 +2300,16 @@
 
 /* Module declarations from "__builtin__" */
 
 /* Module declarations from "cpython.complex" */
 
 /* Module declarations from "cpython.string" */
 
+/* Module declarations from "libc.stddef" */
+
 /* Module declarations from "cpython.unicode" */
 
 /* Module declarations from "cpython.pyport" */
 
 /* Module declarations from "cpython.dict" */
 
 /* Module declarations from "cpython.instance" */
@@ -2323,22 +2345,22 @@
 /* Module declarations from "libc.stdint" */
 
 /* Module declarations from "libcpp.vector" */
 
 /* Module declarations from "Random_Enemy_Attributes_wrapper" */
 
 /* Module declarations from "Random_Enemy_Attributes.Random_Enemy_Attributes" */
-static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
+static std::string __pyx_convert_string_from_py_6libcpp_6string_std__in_string(PyObject *); /*proto*/
 static std::vector<unsigned int>  __pyx_convert_vector_from_py_unsigned_int(PyObject *); /*proto*/
 static std::vector<std::vector<unsigned int> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_unsigned_int_3e___(PyObject *); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
-static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string(std::string const &); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "Random_Enemy_Attributes.Random_Enemy_Attributes"
 extern int __pyx_module_is_main_Random_Enemy_Attributes__Random_Enemy_Attributes;
 int __pyx_module_is_main_Random_Enemy_Attributes__Random_Enemy_Attributes = 0;
 
 /* Implementation of "Random_Enemy_Attributes.Random_Enemy_Attributes" */
@@ -2608,14 +2630,16 @@
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes;
   #endif
   PyTypeObject *__pyx_ptype_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes;
   PyObject *__pyx_n_s_DAMAGE_H;
   PyObject *__pyx_n_s_DAMAGE_L;
   PyObject *__pyx_n_s_HEALTH_H;
   PyObject *__pyx_n_s_HEALTH_L;
@@ -3163,14 +3187,16 @@
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
 #define __pyx_type_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes __pyx_mstate_global->__pyx_type_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes
 #endif
 #define __pyx_ptype_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes __pyx_mstate_global->__pyx_ptype_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes
 #define __pyx_n_s_DAMAGE_H __pyx_mstate_global->__pyx_n_s_DAMAGE_H
 #define __pyx_n_s_DAMAGE_L __pyx_mstate_global->__pyx_n_s_DAMAGE_L
 #define __pyx_n_s_HEALTH_H __pyx_mstate_global->__pyx_n_s_HEALTH_H
 #define __pyx_n_s_HEALTH_L __pyx_mstate_global->__pyx_n_s_HEALTH_L
@@ -3288,41 +3314,41 @@
 #define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 /* #### Code section: module_code ### */
 
 /* "string.from_py":13
  * 
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_string_from_py_6libcpp_6string_std__in_string")
+ * cdef string __pyx_convert_string_from_py_6libcpp_6string_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = 0
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  */
 
-static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
+static std::string __pyx_convert_string_from_py_6libcpp_6string_std__in_string(PyObject *__pyx_v_o) {
   Py_ssize_t __pyx_v_length;
   char const *__pyx_v_data;
   std::string __pyx_r;
   char const *__pyx_t_1;
   std::string __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
   /* "string.from_py":14
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ * @cname("__pyx_convert_string_from_py_6libcpp_6string_std__in_string")
+ * cdef string __pyx_convert_string_from_py_6libcpp_6string_std__in_string(object o) except *:
  *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  *     return string(data, length)
  */
   __pyx_v_length = 0;
 
   /* "string.from_py":15
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ * cdef string __pyx_convert_string_from_py_6libcpp_6string_std__in_string(object o) except *:
  *     cdef Py_ssize_t length = 0
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)             # <<<<<<<<<<<<<<
  *     return string(data, length)
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((char const *)NULL))) __PYX_ERR(0, 15, __pyx_L1_error)
   __pyx_v_data = __pyx_t_1;
@@ -3341,23 +3367,23 @@
     __PYX_ERR(0, 16, __pyx_L1_error)
   }
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
   /* "string.from_py":13
  * 
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_string_from_py_6libcpp_6string_std__in_string")
+ * cdef string __pyx_convert_string_from_py_6libcpp_6string_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = 0
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_6libcpp_6string_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "vector.from_py":45
  * 
@@ -3629,320 +3655,320 @@
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":31
  * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
-static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 1);
+  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string", 1);
 
   /* "string.to_py":32
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
+ * @cname("__pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string(const string& s):
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "string.to_py":31
  * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_6libcpp_6string_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":37
  * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
-static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 1);
+  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string", 1);
 
   /* "string.to_py":38
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
+ * @cname("__pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string(const string& s):
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "string.to_py":37
  * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":43
  * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
-static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 1);
+  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string", 1);
 
   /* "string.to_py":44
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
+ * @cname("__pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string(const string& s):
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "string.to_py":43
  * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_6libcpp_6string_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":49
  * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
-static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 1);
+  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string", 1);
 
   /* "string.to_py":50
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
+ * @cname("__pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(const string& s):
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "string.to_py":49
  * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_6libcpp_6string_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":55
  * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
  * 
  */
 
-static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 1);
+  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string", 1);
 
   /* "string.to_py":56
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
+ * @cname("__pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string(const string& s):
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "string.to_py":55
  * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_6libcpp_6string_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -4407,16 +4433,16 @@
       values[8] = __Pyx_Arg_VARARGS(__pyx_args, 8);
       values[9] = __Pyx_Arg_VARARGS(__pyx_args, 9);
       values[10] = __Pyx_Arg_VARARGS(__pyx_args, 10);
       values[11] = __Pyx_Arg_VARARGS(__pyx_args, 11);
       values[12] = __Pyx_Arg_VARARGS(__pyx_args, 12);
       values[13] = __Pyx_Arg_VARARGS(__pyx_args, 13);
     }
-    __pyx_v_in_File = __pyx_convert_string_from_py_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
-    __pyx_v_out_File = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
+    __pyx_v_in_File = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
+    __pyx_v_out_File = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
     __pyx_v_gen_Seed = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_gen_Seed == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
     __pyx_v_SCALE_L = __pyx_PyFloat_AsFloat(values[3]); if (unlikely((__pyx_v_SCALE_L == (float)-1) && PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
     __pyx_v_SCALE_H = __pyx_PyFloat_AsFloat(values[4]); if (unlikely((__pyx_v_SCALE_H == (float)-1) && PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
     __pyx_v_HEALTH_L = __pyx_PyFloat_AsFloat(values[5]); if (unlikely((__pyx_v_HEALTH_L == (float)-1) && PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
     __pyx_v_HEALTH_H = __pyx_PyFloat_AsFloat(values[6]); if (unlikely((__pyx_v_HEALTH_H == (float)-1) && PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
     __pyx_v_SPEED_L = __pyx_PyFloat_AsFloat(values[7]); if (unlikely((__pyx_v_SPEED_L == (float)-1) && PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
     __pyx_v_SPEED_H = __pyx_PyFloat_AsFloat(values[8]); if (unlikely((__pyx_v_SPEED_H == (float)-1) && PyErr_Occurred())) __PYX_ERR(2, 13, __pyx_L3_error)
@@ -7829,15 +7855,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_PyUnicode_string_to_py_std__in_string(__pyx_v_self->thisptr->inputLocation); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 115, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string(__pyx_v_self->thisptr->inputLocation); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7875,15 +7901,15 @@
 
 static int __pyx_pf_23Random_Enemy_Attributes_23Random_Enemy_Attributes_25PyRandom_Enemy_Attributes_13inputLocation_2__set__(struct __pyx_obj_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes *__pyx_v_self, PyObject *__pyx_v_inputLocation) {
   int __pyx_r;
   std::string __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_inputLocation); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 116, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_v_inputLocation); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 116, __pyx_L1_error)
   __pyx_v_self->thisptr->inputLocation = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1);
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("Random_Enemy_Attributes.Random_Enemy_Attributes.PyRandom_Enemy_Attributes.inputLocation.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -7920,15 +7946,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_PyUnicode_string_to_py_std__in_string(__pyx_v_self->thisptr->outputLocation); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 119, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_PyUnicode_string_to_py_6libcpp_6string_std__in_string(__pyx_v_self->thisptr->outputLocation); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7966,15 +7992,15 @@
 
 static int __pyx_pf_23Random_Enemy_Attributes_23Random_Enemy_Attributes_25PyRandom_Enemy_Attributes_14outputLocation_2__set__(struct __pyx_obj_23Random_Enemy_Attributes_23Random_Enemy_Attributes_PyRandom_Enemy_Attributes *__pyx_v_self, PyObject *__pyx_v_outputLocation) {
   int __pyx_r;
   std::string __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_outputLocation); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 120, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_v_outputLocation); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 120, __pyx_L1_error)
   __pyx_v_self->thisptr->outputLocation = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1);
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("Random_Enemy_Attributes.Random_Enemy_Attributes.PyRandom_Enemy_Attributes.outputLocation.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -9188,31 +9214,31 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_5(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_5(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_5(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -9418,15 +9444,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("Random_Enemy_Attributes", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to Random_Enemy_Attributes pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "Random_Enemy_Attributes" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
@@ -10160,22 +10186,22 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
         return NULL;
     for (i=0; i<nkwargs; i++) {
         PyObject *key = PyTuple_GET_ITEM(kwnames, i);
@@ -10277,15 +10303,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -10296,15 +10322,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -10328,15 +10354,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -11115,46 +11141,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -11401,18 +11427,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_5
-#define __PYX_HAVE_RT_ImportType_3_0_5
-static PyTypeObject *__Pyx_ImportType_3_0_5(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_5 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -11458,23 +11484,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_5 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_5 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -12466,15 +12492,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -12951,15 +12977,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pxd` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pxd`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pyx` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/Random_Enemy_Attributes_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes/patternedAI_Array.h` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes/patternedAI_Array.h`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes.egg-info/PKG-INFO` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Random-Enemy-Attributes
-Version: 1.0.3.3
+Name: Random_Enemy_Attributes
+Version: 1.0.4.3
 Summary: Randomizes enemy stat values for most of the enemies in the game Metroid Prime.
 Home-page: https://github.com/Fantaselion/PARAMETEREDITOR
 Author: Fantaselion
 Author-email: fantaselion@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Random_Enemy_Attributes-1.0.3.3/Random_Enemy_Attributes.egg-info/SOURCES.txt` & `random_enemy_attributes-1.0.4.3/Random_Enemy_Attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Random_Enemy_Attributes-1.0.3.3/setup.py` & `random_enemy_attributes-1.0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                 language='c++')
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="Random_Enemy_Attributes",
-    version="1.0.3.3",
+    version="1.0.4.3",
     description="Randomizes enemy stat values for most of the enemies in the game Metroid Prime.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Fantaselion/PARAMETEREDITOR",
     author="Fantaselion",
     author_email="fantaselion@gmail.com",
     license="MIT",
```

