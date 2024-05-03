# Comparing `tmp/pyquadkey2-0.3.0.tar.gz` & `tmp/pyquadkey2-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquadkey2-0.3.0.tar", last modified: Thu Apr  4 13:13:01 2024, max compression
+gzip compressed data, was "pyquadkey2-0.3.1.tar", last modified: Thu May  2 13:19:05 2024, max compression
```

## Comparing `pyquadkey2-0.3.0.tar` & `pyquadkey2-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-04-04 13:13:01.972484 pyquadkey2-0.3.0/
--rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)    11323 2020-10-30 20:07:11.000000 pyquadkey2-0.3.0/LICENSE
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     4497 2024-04-04 13:13:01.972484 pyquadkey2-0.3.0/PKG-INFO
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     3468 2024-04-04 13:03:33.000000 pyquadkey2-0.3.0/README.md
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)       38 2024-04-04 13:13:01.972484 pyquadkey2-0.3.0/setup.cfg
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     1909 2024-04-04 09:55:25.000000 pyquadkey2-0.3.0/setup.py
-drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-04-04 13:13:01.969484 pyquadkey2-0.3.0/src/
-drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-04-04 13:13:01.970484 pyquadkey2-0.3.0/src/pyquadkey2/
--rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)        0 2020-10-30 20:07:11.000000 pyquadkey2-0.3.0/src/pyquadkey2/__init__.py
-drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-04-04 13:13:01.971484 pyquadkey2-0.3.0/src/pyquadkey2/quadkey/
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     6631 2024-04-04 12:27:00.000000 pyquadkey2-0.3.0/src/pyquadkey2/quadkey/__init__.py
-drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-04-04 13:13:01.971484 pyquadkey2-0.3.0/src/pyquadkey2/quadkey/tilesystem/
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)   421824 2024-04-04 12:28:33.000000 pyquadkey2-0.3.0/src/pyquadkey2/quadkey/tilesystem/tilesystem.c
--rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)      687 2020-10-30 20:07:11.000000 pyquadkey2-0.3.0/src/pyquadkey2/quadkey/util.py
-drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-04-04 13:13:01.971484 pyquadkey2-0.3.0/src/pyquadkey2.egg-info/
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     4497 2024-04-04 13:13:01.000000 pyquadkey2-0.3.0/src/pyquadkey2.egg-info/PKG-INFO
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)      359 2024-04-04 13:13:01.000000 pyquadkey2-0.3.0/src/pyquadkey2.egg-info/SOURCES.txt
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)        1 2024-04-04 13:13:01.000000 pyquadkey2-0.3.0/src/pyquadkey2.egg-info/dependency_links.txt
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)       22 2024-04-04 13:13:01.000000 pyquadkey2-0.3.0/src/pyquadkey2.egg-info/top_level.txt
-drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-04-04 13:13:01.971484 pyquadkey2-0.3.0/tests/
--rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     4978 2024-04-04 09:55:30.000000 pyquadkey2-0.3.0/tests/test_quadkey.py
--rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)      546 2020-10-30 20:07:11.000000 pyquadkey2-0.3.0/tests/test_util.py
+drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-05-02 13:19:05.194002 pyquadkey2-0.3.1/
+-rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)    11323 2020-10-30 20:07:11.000000 pyquadkey2-0.3.1/LICENSE
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     4497 2024-05-02 13:19:05.194002 pyquadkey2-0.3.1/PKG-INFO
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     3468 2024-05-02 13:18:46.000000 pyquadkey2-0.3.1/README.md
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)       38 2024-05-02 13:19:05.194002 pyquadkey2-0.3.1/setup.cfg
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     1909 2024-05-02 13:18:30.000000 pyquadkey2-0.3.1/setup.py
+drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-05-02 13:19:05.192002 pyquadkey2-0.3.1/src/
+drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-05-02 13:19:05.192002 pyquadkey2-0.3.1/src/pyquadkey2/
+-rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)        0 2020-10-30 20:07:11.000000 pyquadkey2-0.3.1/src/pyquadkey2/__init__.py
+drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-05-02 13:19:05.193002 pyquadkey2-0.3.1/src/pyquadkey2/quadkey/
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     6631 2024-04-04 12:27:00.000000 pyquadkey2-0.3.1/src/pyquadkey2/quadkey/__init__.py
+drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-05-02 13:19:05.193002 pyquadkey2-0.3.1/src/pyquadkey2/quadkey/tilesystem/
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)   427818 2024-05-02 13:15:37.000000 pyquadkey2-0.3.1/src/pyquadkey2/quadkey/tilesystem/tilesystem.c
+-rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)      687 2020-10-30 20:07:11.000000 pyquadkey2-0.3.1/src/pyquadkey2/quadkey/util.py
+drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-05-02 13:19:05.194002 pyquadkey2-0.3.1/src/pyquadkey2.egg-info/
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     4497 2024-05-02 13:19:05.000000 pyquadkey2-0.3.1/src/pyquadkey2.egg-info/PKG-INFO
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)      359 2024-05-02 13:19:05.000000 pyquadkey2-0.3.1/src/pyquadkey2.egg-info/SOURCES.txt
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)        1 2024-05-02 13:19:05.000000 pyquadkey2-0.3.1/src/pyquadkey2.egg-info/dependency_links.txt
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)       22 2024-05-02 13:19:05.000000 pyquadkey2-0.3.1/src/pyquadkey2.egg-info/top_level.txt
+drwxr-xr-x   0 ferdinand  (1000) ferdinand  (1000)        0 2024-05-02 13:19:05.194002 pyquadkey2-0.3.1/tests/
+-rw-r--r--   0 ferdinand  (1000) ferdinand  (1000)     5112 2024-05-02 13:18:30.000000 pyquadkey2-0.3.1/tests/test_quadkey.py
+-rw-rw-r--   0 ferdinand  (1000) ferdinand  (1000)      546 2020-10-30 20:07:11.000000 pyquadkey2-0.3.1/tests/test_util.py
```

### Comparing `pyquadkey2-0.3.0/LICENSE` & `pyquadkey2-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquadkey2-0.3.0/PKG-INFO` & `pyquadkey2-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquadkey2
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python implementation of geographical tiling using QuadKeys as proposed by Microsoft
 Home-page: https://github.com/muety/pyquadkey2
 Author: Ferdinand Mütsch
 Author-email: ferdinand@muetsch.io
 Project-URL: Bug Tracker, https://github.com/muety/pyquadkey2/issues
 Project-URL: Source Code, https://github.com/muety/pyquadkey2
 Project-URL: Documentation, https://docs.muetsch.io/pyquadkey2/
@@ -57,16 +57,16 @@
 $ pip install pyquadkey2
 ```
 
 Pip installation is only tested for Linux and Mac, yet. If you encounter problems with the installation on Windows, please report them as a new issue.
 
 ### From archive
 ```bash
-$ wget https://github.com/muety/pyquadkey2/releases/download/0.3.0/pyquadkey2-0.3.0.tar.gz
-$ pip install pyquadkey2-0.3.0.tar.gz
+$ wget https://github.com/muety/pyquadkey2/releases/download/0.3.1/pyquadkey2-0.3.1.tar.gz
+$ pip install pyquadkey2-0.3.1.tar.gz
 ```
 
 ### From source
 #### Prerequisites (`Linux`)
 * `gcc`
     * Fedora: `dnf install @development-tools`
     * Ubuntu / Debian: `apt install build-essential`
@@ -107,17 +107,17 @@
 
 ### Release
 
 See [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
 ```bash
 pip install setuptools wheel auditwheel
-python setup.py bdist_wheel
+python -m build
 cd dist
 auditwheel repair *.whl
-twine upload --repository testpypi wheelhouse/*
+twine upload --repository testpypi wheelhouse/* ../*.tar.gz
 ```
 
 ## License
 Apache 2.0
 
 [![Buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoff.ee/n1try)
```

### Comparing `pyquadkey2-0.3.0/README.md` & `pyquadkey2-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 $ pip install pyquadkey2
 ```
 
 Pip installation is only tested for Linux and Mac, yet. If you encounter problems with the installation on Windows, please report them as a new issue.
 
 ### From archive
 ```bash
-$ wget https://github.com/muety/pyquadkey2/releases/download/0.3.0/pyquadkey2-0.3.0.tar.gz
-$ pip install pyquadkey2-0.3.0.tar.gz
+$ wget https://github.com/muety/pyquadkey2/releases/download/0.3.1/pyquadkey2-0.3.1.tar.gz
+$ pip install pyquadkey2-0.3.1.tar.gz
 ```
 
 ### From source
 #### Prerequisites (`Linux`)
 * `gcc`
     * Fedora: `dnf install @development-tools`
     * Ubuntu / Debian: `apt install build-essential`
@@ -82,17 +82,17 @@
 
 ### Release
 
 See [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
 ```bash
 pip install setuptools wheel auditwheel
-python setup.py bdist_wheel
+python -m build
 cd dist
 auditwheel repair *.whl
-twine upload --repository testpypi wheelhouse/*
+twine upload --repository testpypi wheelhouse/* ../*.tar.gz
 ```
 
 ## License
 Apache 2.0
 
 [![Buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoff.ee/n1try)
```

### Comparing `pyquadkey2-0.3.0/setup.py` & `pyquadkey2-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pyquadkey2',
-    version='0.3.0',
+    version='0.3.1',
     description='Python implementation of geographical tiling using QuadKeys as proposed by Microsoft',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ferdinand Mütsch',
     author_email='ferdinand@muetsch.io',
     url='https://github.com/muety/pyquadkey2',
     packages=find_packages('src'),
```

### Comparing `pyquadkey2-0.3.0/src/pyquadkey2/quadkey/__init__.py` & `pyquadkey2-0.3.1/src/pyquadkey2/quadkey/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquadkey2-0.3.0/src/pyquadkey2/quadkey/tilesystem/tilesystem.c` & `pyquadkey2-0.3.1/src/pyquadkey2/quadkey/tilesystem/tilesystem.c`

 * *Files 0% similar despite different names*

```diff
@@ -1770,14 +1770,29 @@
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
+/* PyFloatBinop.proto */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyFloat_TrueDivideObjC(PyObject *op1, PyObject *op2, double floatval, int inplace, int zerodivision_check);
+#else
+#define __Pyx_PyFloat_TrueDivideObjC(op1, op2, floatval, inplace, zerodivision_check)\
+    (inplace ? PyNumber_InPlaceTrueDivide(op1, op2) : PyNumber_TrueDivide(op1, op2))
+#endif
+
+/* PyIntFromDouble.proto */
+#if PY_MAJOR_VERSION < 3
+static CYTHON_INLINE PyObject* __Pyx_PyInt_FromDouble(double value);
+#else
+#define __Pyx_PyInt_FromDouble(value) PyLong_FromDouble(value)
+#endif
+
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
 }
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = -1;
@@ -2266,14 +2281,15 @@
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_tile;
   PyObject *__pyx_n_s_tile_to_pixel;
   PyObject *__pyx_n_s_tile_to_quadkey;
   PyObject *__pyx_n_s_tilesystem;
   PyObject *__pyx_kp_s_tilesystem_pyx;
+  PyObject *__pyx_float_1e12;
   PyObject *__pyx_int_3;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__10;
   PyObject *__pyx_tuple__12;
@@ -2357,14 +2373,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_tile);
   Py_CLEAR(clear_module_state->__pyx_n_s_tile_to_pixel);
   Py_CLEAR(clear_module_state->__pyx_n_s_tile_to_quadkey);
   Py_CLEAR(clear_module_state->__pyx_n_s_tilesystem);
   Py_CLEAR(clear_module_state->__pyx_kp_s_tilesystem_pyx);
+  Py_CLEAR(clear_module_state->__pyx_float_1e12);
   Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
   Py_CLEAR(clear_module_state->__pyx_tuple__12);
@@ -2426,14 +2443,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_tile);
   Py_VISIT(traverse_module_state->__pyx_n_s_tile_to_pixel);
   Py_VISIT(traverse_module_state->__pyx_n_s_tile_to_quadkey);
   Py_VISIT(traverse_module_state->__pyx_n_s_tilesystem);
   Py_VISIT(traverse_module_state->__pyx_kp_s_tilesystem_pyx);
+  Py_VISIT(traverse_module_state->__pyx_float_1e12);
   Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
   Py_VISIT(traverse_module_state->__pyx_tuple__12);
@@ -2509,14 +2527,15 @@
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_tile __pyx_mstate_global->__pyx_n_s_tile
 #define __pyx_n_s_tile_to_pixel __pyx_mstate_global->__pyx_n_s_tile_to_pixel
 #define __pyx_n_s_tile_to_quadkey __pyx_mstate_global->__pyx_n_s_tile_to_quadkey
 #define __pyx_n_s_tilesystem __pyx_mstate_global->__pyx_n_s_tilesystem
 #define __pyx_kp_s_tilesystem_pyx __pyx_mstate_global->__pyx_kp_s_tilesystem_pyx
+#define __pyx_float_1e12 __pyx_mstate_global->__pyx_float_1e12
 #define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
@@ -3145,20 +3164,25 @@
   double __pyx_v_y;
   double __pyx_v_lat;
   double __pyx_v_lon;
   double __pyx_v_pixel_x;
   double __pyx_v_pixel_y;
   long __pyx_v_ms;
   __pyx_ctuple_double__and_double __pyx_r;
+  __Pyx_RefNannyDeclarations
   long __pyx_t_1;
   __pyx_ctuple_double__and_double __pyx_t_2;
   double __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  double __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("pixel_to_geo", 1);
 
   /* "tilesystem.pyx":56
  *     cdef double x, y, lat, lon, pixel_x, pixel_y
  *     cdef long ms
  *     pixel_x = pixel[0]             # <<<<<<<<<<<<<<
  *     pixel_y = pixel[1]
  *     ms = map_size(level)
@@ -3209,52 +3233,69 @@
   __pyx_v_y = (0.5 - (__pyx_t_3 / ((double)__pyx_v_ms)));
 
   /* "tilesystem.pyx":61
  *     x = (clip(pixel_x, (0, ms - 1)) / ms) - 0.5
  *     y = 0.5 - (clip(pixel_y, (0, ms - 1)) / ms)
  *     lat = 90 - 360 * math.atan(math.exp(-y * 2 * math.pi)) / math.pi             # <<<<<<<<<<<<<<
  *     lon = 360 * x
- *     return math.round(lat * 1e12) / 1e12, math.round(lon * 1e12) / 1e12
+ *     return int(lat * 1e12) / 1e12, int(lon * 1e12) / 1e12
  */
   __pyx_v_lat = (90.0 - ((360.0 * atan(exp((((-__pyx_v_y) * 2.0) * M_PI)))) / ((double)M_PI)));
 
   /* "tilesystem.pyx":62
  *     y = 0.5 - (clip(pixel_y, (0, ms - 1)) / ms)
  *     lat = 90 - 360 * math.atan(math.exp(-y * 2 * math.pi)) / math.pi
  *     lon = 360 * x             # <<<<<<<<<<<<<<
- *     return math.round(lat * 1e12) / 1e12, math.round(lon * 1e12) / 1e12
+ *     return int(lat * 1e12) / 1e12, int(lon * 1e12) / 1e12
  * 
  */
   __pyx_v_lon = (360.0 * __pyx_v_x);
 
   /* "tilesystem.pyx":63
  *     lat = 90 - 360 * math.atan(math.exp(-y * 2 * math.pi)) / math.pi
  *     lon = 360 * x
- *     return math.round(lat * 1e12) / 1e12, math.round(lon * 1e12) / 1e12             # <<<<<<<<<<<<<<
+ *     return int(lat * 1e12) / 1e12, int(lon * 1e12) / 1e12             # <<<<<<<<<<<<<<
  * 
  * cpdef (long, long) pixel_to_tile(const (long, long) pixel):
  */
-  __pyx_t_2.f0 = (round((__pyx_v_lat * 1e12)) / 1e12);
-  __pyx_t_2.f1 = (round((__pyx_v_lon * 1e12)) / 1e12);
+  __pyx_t_4 = __Pyx_PyInt_FromDouble((__pyx_v_lat * 1e12)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_4, __pyx_float_1e12, 1e12, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_FromDouble((__pyx_v_lon * 1e12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = __Pyx_PyFloat_TrueDivideObjC(__pyx_t_5, __pyx_float_1e12, 1e12, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2.f0 = __pyx_t_3;
+  __pyx_t_2.f1 = __pyx_t_6;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
   /* "tilesystem.pyx":53
  *     return pixel_x, pixel_y
  * 
  * cpdef (double, double) pixel_to_geo((double, double) pixel, const long level):             # <<<<<<<<<<<<<<
  *     cdef double x, y, lat, lon, pixel_x, pixel_y
  *     cdef long ms
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("tilesystem.pixel_to_geo", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10tilesystem_5pixel_to_geo(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -3390,15 +3431,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "tilesystem.pyx":65
- *     return math.round(lat * 1e12) / 1e12, math.round(lon * 1e12) / 1e12
+ *     return int(lat * 1e12) / 1e12, int(lon * 1e12) / 1e12
  * 
  * cpdef (long, long) pixel_to_tile(const (long, long) pixel):             # <<<<<<<<<<<<<<
  *     return pixel[0] // 256, pixel[1] // 256
  * 
  */
 
 static PyObject *__pyx_pw_10tilesystem_7pixel_to_tile(PyObject *__pyx_self, 
@@ -3421,15 +3462,15 @@
  */
   __pyx_t_1.f0 = (__pyx_v_pixel.f0 / 0x100);
   __pyx_t_1.f1 = (__pyx_v_pixel.f1 / 0x100);
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
   /* "tilesystem.pyx":65
- *     return math.round(lat * 1e12) / 1e12, math.round(lon * 1e12) / 1e12
+ *     return int(lat * 1e12) / 1e12, int(lon * 1e12) / 1e12
  * 
  * cpdef (long, long) pixel_to_tile(const (long, long) pixel):             # <<<<<<<<<<<<<<
  *     return pixel[0] // 256, pixel[1] // 256
  * 
  */
 
   /* function exit code */
@@ -5191,15 +5232,15 @@
  */
   __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_s_pixel, __pyx_n_s_level); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
   __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tilesystem_pyx, __pyx_n_s_pixel_to_geo, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 53, __pyx_L1_error)
 
   /* "tilesystem.pyx":65
- *     return math.round(lat * 1e12) / 1e12, math.round(lon * 1e12) / 1e12
+ *     return int(lat * 1e12) / 1e12, int(lon * 1e12) / 1e12
  * 
  * cpdef (long, long) pixel_to_tile(const (long, long) pixel):             # <<<<<<<<<<<<<<
  *     return pixel[0] // 256, pixel[1] // 256
  * 
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_pixel); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
@@ -5268,14 +5309,15 @@
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_float_1e12 = PyFloat_FromDouble(1e12); if (unlikely(!__pyx_float_1e12)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
@@ -5691,15 +5733,15 @@
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10tilesystem_5pixel_to_geo, 0, __pyx_n_s_pixel_to_geo, NULL, __pyx_n_s_tilesystem, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pixel_to_geo, __pyx_t_3) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "tilesystem.pyx":65
- *     return math.round(lat * 1e12) / 1e12, math.round(lon * 1e12) / 1e12
+ *     return int(lat * 1e12) / 1e12, int(lon * 1e12) / 1e12
  * 
  * cpdef (long, long) pixel_to_tile(const (long, long) pixel):             # <<<<<<<<<<<<<<
  *     return pixel[0] // 256, pixel[1] // 256
  * 
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10tilesystem_7pixel_to_tile, 0, __pyx_n_s_pixel_to_tile, NULL, __pyx_n_s_tilesystem, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -6420,14 +6462,107 @@
     #endif
 bad:
     Py_XDECREF(key);
     Py_XDECREF(value);
     return -1;
 }
 
+/* PyFloatBinop */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyFloat_TrueDivideObjC(PyObject *op1, PyObject *op2, double floatval, int inplace, int zerodivision_check) {
+    const double b = floatval;
+    double a, result;
+    CYTHON_UNUSED_VAR(inplace);
+    CYTHON_UNUSED_VAR(zerodivision_check);
+    if (likely(PyFloat_CheckExact(op1))) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        a = __pyx_PyFloat_AsDouble(op1);
+#else
+        a = PyFloat_AS_DOUBLE(op1);
+#endif
+        
+    } else
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        a = (double) PyInt_AS_LONG(op1);
+        
+    } else
+    #endif
+    if (likely(PyLong_CheckExact(op1))) {
+        #if CYTHON_USE_PYLONG_INTERNALS
+        if (__Pyx_PyLong_IsZero(op1)) {
+            a = 0.0;
+            
+        } else if (__Pyx_PyLong_IsCompact(op1)) {
+            a = (double) __Pyx_PyLong_CompactValue(op1);
+        } else {
+            const digit* digits = __Pyx_PyLong_Digits(op1);
+            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
+            switch (size) {
+                case -2:
+                case 2:
+                    if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT && ((8 * sizeof(unsigned long) < 53) || (1 * PyLong_SHIFT < 53))) {
+                        a = (double) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        if ((8 * sizeof(unsigned long) < 53) || (2 * PyLong_SHIFT < 53) || (a < (double) ((PY_LONG_LONG)1 << 53))) {
+                            if (size == -2)
+                                a = -a;
+                            break;
+                        }
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -3:
+                case 3:
+                    if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT && ((8 * sizeof(unsigned long) < 53) || (2 * PyLong_SHIFT < 53))) {
+                        a = (double) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        if ((8 * sizeof(unsigned long) < 53) || (3 * PyLong_SHIFT < 53) || (a < (double) ((PY_LONG_LONG)1 << 53))) {
+                            if (size == -3)
+                                a = -a;
+                            break;
+                        }
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -4:
+                case 4:
+                    if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT && ((8 * sizeof(unsigned long) < 53) || (3 * PyLong_SHIFT < 53))) {
+                        a = (double) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        if ((8 * sizeof(unsigned long) < 53) || (4 * PyLong_SHIFT < 53) || (a < (double) ((PY_LONG_LONG)1 << 53))) {
+                            if (size == -4)
+                                a = -a;
+                            break;
+                        }
+                    }
+                    CYTHON_FALLTHROUGH;
+                default:
+        #endif
+                    a = PyLong_AsDouble(op1);
+                    if (unlikely(a == -1.0 && PyErr_Occurred())) return NULL;
+        #if CYTHON_USE_PYLONG_INTERNALS
+            }
+        }
+        #endif
+    } else {
+        return (inplace ? PyNumber_InPlaceTrueDivide : PyNumber_TrueDivide)(op1, op2);
+    }
+        PyFPE_START_PROTECT("divide", return NULL)
+        result = a / b;
+        PyFPE_END_PROTECT(result)
+        return PyFloat_FromDouble(result);
+}
+#endif
+
+/* PyIntFromDouble */
+#if PY_MAJOR_VERSION < 3
+static CYTHON_INLINE PyObject* __Pyx_PyInt_FromDouble(double value) {
+    if (value >= (double)LONG_MIN && value <= (double)LONG_MAX) {
+        return PyInt_FromLong((long)value);
+    }
+    return PyLong_FromDouble(value);
+}
+#endif
+
 /* decode_c_string */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
     if (unlikely((start < 0) | (stop < 0))) {
```

### Comparing `pyquadkey2-0.3.0/src/pyquadkey2/quadkey/util.py` & `pyquadkey2-0.3.1/src/pyquadkey2/quadkey/util.py`

 * *Files identical despite different names*

### Comparing `pyquadkey2-0.3.0/src/pyquadkey2.egg-info/PKG-INFO` & `pyquadkey2-0.3.1/src/pyquadkey2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquadkey2
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python implementation of geographical tiling using QuadKeys as proposed by Microsoft
 Home-page: https://github.com/muety/pyquadkey2
 Author: Ferdinand Mütsch
 Author-email: ferdinand@muetsch.io
 Project-URL: Bug Tracker, https://github.com/muety/pyquadkey2/issues
 Project-URL: Source Code, https://github.com/muety/pyquadkey2
 Project-URL: Documentation, https://docs.muetsch.io/pyquadkey2/
@@ -57,16 +57,16 @@
 $ pip install pyquadkey2
 ```
 
 Pip installation is only tested for Linux and Mac, yet. If you encounter problems with the installation on Windows, please report them as a new issue.
 
 ### From archive
 ```bash
-$ wget https://github.com/muety/pyquadkey2/releases/download/0.3.0/pyquadkey2-0.3.0.tar.gz
-$ pip install pyquadkey2-0.3.0.tar.gz
+$ wget https://github.com/muety/pyquadkey2/releases/download/0.3.1/pyquadkey2-0.3.1.tar.gz
+$ pip install pyquadkey2-0.3.1.tar.gz
 ```
 
 ### From source
 #### Prerequisites (`Linux`)
 * `gcc`
     * Fedora: `dnf install @development-tools`
     * Ubuntu / Debian: `apt install build-essential`
@@ -107,17 +107,17 @@
 
 ### Release
 
 See [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
 ```bash
 pip install setuptools wheel auditwheel
-python setup.py bdist_wheel
+python -m build
 cd dist
 auditwheel repair *.whl
-twine upload --repository testpypi wheelhouse/*
+twine upload --repository testpypi wheelhouse/* ../*.tar.gz
 ```
 
 ## License
 Apache 2.0
 
 [![Buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoff.ee/n1try)
```

### Comparing `pyquadkey2-0.3.0/tests/test_quadkey.py` & `pyquadkey2-0.3.1/tests/test_quadkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     def testInitInvalidKey(self):
         with self.assertRaises(AssertionError):
             quadkey.from_str('0156510012')
 
     def testFromGeo(self):
         self.assertEqual('1202032333311320', quadkey.from_geo((49.014205, 8.420025), 16).key)
+        self.assertEqual('311213', quadkey.from_geo((-27.052395, 152.97702), 6).key)  # https://github.com/muety/pyquadkey2/issues/13
 
     def testFromGeoInvalidLevel(self):
         with self.assertRaises(AssertionError):
             quadkey.from_geo((49.014205, 8.420025), 32)
 
     def testEquality(self):
         one = quadkey.from_str('00')
```

### Comparing `pyquadkey2-0.3.0/tests/test_util.py` & `pyquadkey2-0.3.1/tests/test_util.py`

 * *Files identical despite different names*

