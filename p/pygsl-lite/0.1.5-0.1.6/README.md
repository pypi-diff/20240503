# Comparing `tmp/pygsl_lite-0.1.5.tar.gz` & `tmp/pygsl_lite-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygsl_lite-0.1.5.tar", last modified: Wed Apr  5 13:04:10 2023, max compression
+gzip compressed data, was "pygsl_lite-0.1.6.tar", last modified: Fri May  3 15:12:50 2024, max compression
```

## Comparing `pygsl_lite-0.1.5.tar` & `pygsl_lite-0.1.6.tar`

### file list

```diff
@@ -1,128 +1,133 @@
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:10.194790 pygsl_lite-0.1.5/
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:11.000000 pygsl_lite-0.1.5/Include/
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:11.000000 pygsl_lite-0.1.5/Include/pygsl_lite/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)       96 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/arrayobject.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    17048 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/block_helpers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      737 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/block_helpers_numpy.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3408 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/capsuletrunk.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      222 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/compilers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2808 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/complex_helpers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4028 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/error_helpers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      792 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/errorno.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     8213 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/function_helpers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     5742 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/general_helpers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     8846 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/intern.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      376 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/old_numpy_compat.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2624 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/profile.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      207 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/pygsl.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      427 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/pygsl_features.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    21150 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/pygsl_features_config.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1612 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/rng.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4824 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/rng_helpers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    10961 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/solver.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      700 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/string_helpers.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      783 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/transition.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1855 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/Include/pygsl_lite/utils.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    17992 2023-03-28 18:49:08.000000 pygsl_lite-0.1.5/LICENSE
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1662 2023-04-05 13:04:13.000000 pygsl_lite-0.1.5/PKG-INFO
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1357 2023-03-27 21:09:05.000000 pygsl_lite-0.1.5/README.rst
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:11.000000 pygsl_lite-0.1.5/gsl_dist/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)       51 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/gsl_dist/__init__.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      213 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/gsl_dist/array_includes.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     6131 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/gsl_dist/gsl_Extension.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     5202 2023-04-05 13:01:41.000000 pygsl_lite-0.1.5/gsl_dist/gsl_Location.py
--rwxr-xr-x   0 sossokine  (2188) cluster   (1111)     3817 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/gsl_dist/swig_extension.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2535 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/gsl_packages.py
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:12.000000 pygsl_lite-0.1.5/pygsl_lite/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4803 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/__init__.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2107 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/_block.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2113 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/_callback.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1440 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/_generic_solver.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)       76 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/_numobj.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      160 2023-04-05 13:04:10.000000 pygsl_lite-0.1.5/pygsl_lite/_version.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3055 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/block.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    11319 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/errors.py
--rwxr-xr-x   0 sossokine  (2188) cluster   (1111)     4359 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/gsl_function.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    16828 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/gslwrap.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     6672 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/interpolation.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      439 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/math.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    15822 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/odeiv.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2149 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/odeiv2.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     9980 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/roots.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     5085 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/spline.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2885 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/pygsl_lite/vector.py
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:12.000000 pygsl_lite-0.1.5/pygsl_lite.egg-info/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1662 2023-04-05 13:04:10.000000 pygsl_lite-0.1.5/pygsl_lite.egg-info/PKG-INFO
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3002 2023-04-05 13:04:11.000000 pygsl_lite-0.1.5/pygsl_lite.egg-info/SOURCES.txt
--rw-r--r--   0 sossokine  (2188) cluster   (1111)        1 2023-04-05 13:04:10.000000 pygsl_lite-0.1.5/pygsl_lite.egg-info/dependency_links.txt
--rw-r--r--   0 sossokine  (2188) cluster   (1111)       14 2023-04-05 13:04:10.000000 pygsl_lite-0.1.5/pygsl_lite.egg-info/requires.txt
--rw-r--r--   0 sossokine  (2188) cluster   (1111)       77 2023-04-05 13:04:10.000000 pygsl_lite-0.1.5/pygsl_lite.egg-info/top_level.txt
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      625 2023-03-28 18:50:07.000000 pygsl_lite-0.1.5/pyproject.toml
--rw-r--r--   0 sossokine  (2188) cluster   (1111)       38 2023-04-05 13:04:13.000000 pygsl_lite-0.1.5/setup.cfg
--rwxr-xr-x   0 sossokine  (2188) cluster   (1111)     3040 2023-03-27 21:08:00.000000 pygsl_lite-0.1.5/setup.py
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:12.000000 pygsl_lite-0.1.5/src/
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:12.000000 pygsl_lite-0.1.5/src/block/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1861 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4489 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_char.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4816 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_complex.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     5422 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_complex_float.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4692 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_double.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4590 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_float.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3970 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_generic.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     5157 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_generic_typed.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4388 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_int.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4489 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_long.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4591 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/block/gsl_block_short.i
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:09.542778 pygsl_lite-0.1.5/src/callback/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1037 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/chars.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    29753 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/function_helpers.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1483 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/gsl_callback.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2260 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/gsl_function_test.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3455 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/gsl_multiroots.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3022 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/gsl_odeiv.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    26533 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/gsl_odeiv2.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2316 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/gsl_roots.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    23992 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/odeiv.ic
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3799 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/callback/odeiv_func2.ic
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     6083 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/errortestmodule.c
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:09.570779 pygsl_lite-0.1.5/src/gslwrap/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1322 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/gslwrap/gsl_gslwrap.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    18669 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/gslwrap/interpolation.i
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:09.754782 pygsl_lite-0.1.5/src/init/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    25772 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/block_helpers.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     5521 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/block_helpers_numpy.ic
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2028 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/complex_helpers.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    17120 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/error_helpers.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     3970 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/errorno.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2330 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/function_helpers.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     8719 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/general_helpers.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    15186 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/initmodule.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     5582 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/inittestmodule.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     1586 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/profile.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      914 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/src/init/rng_helpers.c
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:10.010787 pygsl_lite-0.1.5/swig_src/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2107 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/_block.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2113 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/_callback.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)   640394 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/block_wrap.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)   257223 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/callback_wrap.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    16828 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/gslwrap.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)   230587 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/gslwrap_wrap.c
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2149 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/odeiv2.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)   288839 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/swig_src/odeiv2_wrap.c
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:10.026787 pygsl_lite-0.1.5/test/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      405 2023-04-05 13:02:12.000000 pygsl_lite-0.1.5/test/test_spline.py
-drwxr-xr-x   0 sossokine  (2188) cluster   (1111)        0 2023-04-05 13:04:10.182790 pygsl_lite-0.1.5/typemaps/
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     6395 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/block_conversion_functions.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     6965 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/c.py
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      384 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/callable.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    43953 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/convert_block_description.h
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      644 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/error.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2311 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/file_typemaps.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2313 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/gsl_block_special_typemaps.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)    15915 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/gsl_block_typemaps.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     4306 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/gsl_complex_typemap.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     2488 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/gsl_error_typemap.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)     9481 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/gsl_function_typemaps.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      102 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/gsl_permutations_typemaps.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      305 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/gsl_rng_typemaps.i
--rw-r--r--   0 sossokine  (2188) cluster   (1111)      496 2023-03-27 20:49:30.000000 pygsl_lite-0.1.5/typemaps/misc_typemaps.i
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.700537 pygsl_lite-0.1.6/
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.677832 pygsl_lite-0.1.6/.github/
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.680046 pygsl_lite-0.1.6/.github/workflows/
+-rw-r--r--   0 raffi      (502) admin       (80)     2071 2024-05-03 15:11:10.000000 pygsl_lite-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0 raffi      (502) admin       (80)       43 2024-05-03 15:11:10.000000 pygsl_lite-0.1.6/.gitignore
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.677974 pygsl_lite-0.1.6/Include/
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.683781 pygsl_lite-0.1.6/Include/pygsl_lite/
+-rw-r--r--   0 raffi      (502) admin       (80)       96 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/arrayobject.h
+-rw-r--r--   0 raffi      (502) admin       (80)    17048 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/block_helpers.h
+-rw-r--r--   0 raffi      (502) admin       (80)      737 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/block_helpers_numpy.h
+-rw-r--r--   0 raffi      (502) admin       (80)     3408 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/capsuletrunk.h
+-rw-r--r--   0 raffi      (502) admin       (80)      222 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/compilers.h
+-rw-r--r--   0 raffi      (502) admin       (80)     2808 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/complex_helpers.h
+-rw-r--r--   0 raffi      (502) admin       (80)     4028 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/error_helpers.h
+-rw-r--r--   0 raffi      (502) admin       (80)      792 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/errorno.h
+-rw-r--r--   0 raffi      (502) admin       (80)     8213 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/function_helpers.h
+-rw-r--r--   0 raffi      (502) admin       (80)     5742 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/general_helpers.h
+-rw-r--r--   0 raffi      (502) admin       (80)     8846 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/intern.h
+-rw-r--r--   0 raffi      (502) admin       (80)      376 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/old_numpy_compat.h
+-rw-r--r--   0 raffi      (502) admin       (80)     2624 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/profile.h
+-rw-r--r--   0 raffi      (502) admin       (80)      207 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/pygsl.h
+-rw-r--r--   0 raffi      (502) admin       (80)      427 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/pygsl_features.h
+-rw-r--r--   0 raffi      (502) admin       (80)    21150 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/pygsl_features_config.h
+-rw-r--r--   0 raffi      (502) admin       (80)     1612 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/rng.h
+-rw-r--r--   0 raffi      (502) admin       (80)     4824 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/rng_helpers.h
+-rw-r--r--   0 raffi      (502) admin       (80)    10961 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/solver.h
+-rw-r--r--   0 raffi      (502) admin       (80)      700 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/string_helpers.h
+-rw-r--r--   0 raffi      (502) admin       (80)      783 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/transition.h
+-rw-r--r--   0 raffi      (502) admin       (80)     1855 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/Include/pygsl_lite/utils.h
+-rw-r--r--   0 raffi      (502) admin       (80)    17992 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/LICENSE
+-rw-r--r--   0 raffi      (502) admin       (80)     1684 2024-05-03 15:12:50.700325 pygsl_lite-0.1.6/PKG-INFO
+-rw-r--r--   0 raffi      (502) admin       (80)     1357 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/README.rst
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.684437 pygsl_lite-0.1.6/gsl_dist/
+-rw-r--r--   0 raffi      (502) admin       (80)       51 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/gsl_dist/__init__.py
+-rw-r--r--   0 raffi      (502) admin       (80)       92 2024-05-03 15:11:10.000000 pygsl_lite-0.1.6/gsl_dist/array_includes.py
+-rw-r--r--   0 raffi      (502) admin       (80)     5990 2024-05-03 15:11:10.000000 pygsl_lite-0.1.6/gsl_dist/gsl_Extension.py
+-rw-r--r--   0 raffi      (502) admin       (80)     5202 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/gsl_dist/gsl_Location.py
+-rwxr-xr-x   0 raffi      (502) admin       (80)     3817 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/gsl_dist/swig_extension.py
+-rw-r--r--   0 raffi      (502) admin       (80)     2535 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/gsl_packages.py
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.686767 pygsl_lite-0.1.6/pygsl_lite/
+-rw-r--r--   0 raffi      (502) admin       (80)     4803 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/__init__.py
+-rw-r--r--   0 raffi      (502) admin       (80)     2107 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/_block.py
+-rw-r--r--   0 raffi      (502) admin       (80)     2113 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/_callback.py
+-rw-r--r--   0 raffi      (502) admin       (80)     1440 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/_generic_solver.py
+-rw-r--r--   0 raffi      (502) admin       (80)       76 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/_numobj.py
+-rw-r--r--   0 raffi      (502) admin       (80)      411 2024-05-03 15:12:50.000000 pygsl_lite-0.1.6/pygsl_lite/_version.py
+-rw-r--r--   0 raffi      (502) admin       (80)     3055 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/block.py
+-rw-r--r--   0 raffi      (502) admin       (80)    11319 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/errors.py
+-rwxr-xr-x   0 raffi      (502) admin       (80)     4359 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/gsl_function.py
+-rw-r--r--   0 raffi      (502) admin       (80)    16828 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/gslwrap.py
+-rw-r--r--   0 raffi      (502) admin       (80)     6672 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/interpolation.py
+-rw-r--r--   0 raffi      (502) admin       (80)      439 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/math.py
+-rw-r--r--   0 raffi      (502) admin       (80)    15822 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/odeiv.py
+-rw-r--r--   0 raffi      (502) admin       (80)     2149 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/odeiv2.py
+-rw-r--r--   0 raffi      (502) admin       (80)     9980 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/roots.py
+-rw-r--r--   0 raffi      (502) admin       (80)     5085 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/spline.py
+-rw-r--r--   0 raffi      (502) admin       (80)     2885 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/pygsl_lite/vector.py
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.700071 pygsl_lite-0.1.6/pygsl_lite.egg-info/
+-rw-r--r--   0 raffi      (502) admin       (80)     1684 2024-05-03 15:12:50.000000 pygsl_lite-0.1.6/pygsl_lite.egg-info/PKG-INFO
+-rw-r--r--   0 raffi      (502) admin       (80)     3046 2024-05-03 15:12:50.000000 pygsl_lite-0.1.6/pygsl_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 raffi      (502) admin       (80)        1 2024-05-03 15:12:50.000000 pygsl_lite-0.1.6/pygsl_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 raffi      (502) admin       (80)       14 2024-05-03 15:12:50.000000 pygsl_lite-0.1.6/pygsl_lite.egg-info/requires.txt
+-rw-r--r--   0 raffi      (502) admin       (80)       77 2024-05-03 15:12:50.000000 pygsl_lite-0.1.6/pygsl_lite.egg-info/top_level.txt
+-rw-r--r--   0 raffi      (502) admin       (80)      707 2024-05-03 15:11:10.000000 pygsl_lite-0.1.6/pyproject.toml
+-rw-r--r--   0 raffi      (502) admin       (80)       38 2024-05-03 15:12:50.700570 pygsl_lite-0.1.6/setup.cfg
+-rwxr-xr-x   0 raffi      (502) admin       (80)     3040 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/setup.py
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.687451 pygsl_lite-0.1.6/src/
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.688876 pygsl_lite-0.1.6/src/block/
+-rw-r--r--   0 raffi      (502) admin       (80)     1861 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4489 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_char.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4816 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_complex.i
+-rw-r--r--   0 raffi      (502) admin       (80)     5422 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_complex_float.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4692 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_double.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4590 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_float.i
+-rw-r--r--   0 raffi      (502) admin       (80)     3970 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_generic.i
+-rw-r--r--   0 raffi      (502) admin       (80)     5157 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_generic_typed.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4388 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_int.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4489 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_long.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4591 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/block/gsl_block_short.i
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.690356 pygsl_lite-0.1.6/src/callback/
+-rw-r--r--   0 raffi      (502) admin       (80)     1037 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/chars.c
+-rw-r--r--   0 raffi      (502) admin       (80)    29753 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/function_helpers.c
+-rw-r--r--   0 raffi      (502) admin       (80)     1483 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/gsl_callback.i
+-rw-r--r--   0 raffi      (502) admin       (80)     2260 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/gsl_function_test.i
+-rw-r--r--   0 raffi      (502) admin       (80)     3455 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/gsl_multiroots.i
+-rw-r--r--   0 raffi      (502) admin       (80)     3022 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/gsl_odeiv.i
+-rw-r--r--   0 raffi      (502) admin       (80)    26533 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/gsl_odeiv2.i
+-rw-r--r--   0 raffi      (502) admin       (80)     2316 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/gsl_roots.i
+-rw-r--r--   0 raffi      (502) admin       (80)    23992 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/odeiv.ic
+-rw-r--r--   0 raffi      (502) admin       (80)     3799 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/callback/odeiv_func2.ic
+-rw-r--r--   0 raffi      (502) admin       (80)     6083 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/errortestmodule.c
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.690624 pygsl_lite-0.1.6/src/gslwrap/
+-rw-r--r--   0 raffi      (502) admin       (80)     1322 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/gslwrap/gsl_gslwrap.i
+-rw-r--r--   0 raffi      (502) admin       (80)    18669 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/gslwrap/interpolation.i
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.692623 pygsl_lite-0.1.6/src/init/
+-rw-r--r--   0 raffi      (502) admin       (80)    25772 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/block_helpers.c
+-rw-r--r--   0 raffi      (502) admin       (80)     5521 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/block_helpers_numpy.ic
+-rw-r--r--   0 raffi      (502) admin       (80)     2028 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/complex_helpers.c
+-rw-r--r--   0 raffi      (502) admin       (80)    17120 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/error_helpers.c
+-rw-r--r--   0 raffi      (502) admin       (80)     3970 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/errorno.c
+-rw-r--r--   0 raffi      (502) admin       (80)     2330 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/function_helpers.c
+-rw-r--r--   0 raffi      (502) admin       (80)     8719 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/general_helpers.c
+-rw-r--r--   0 raffi      (502) admin       (80)    15186 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/initmodule.c
+-rw-r--r--   0 raffi      (502) admin       (80)     5582 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/inittestmodule.c
+-rw-r--r--   0 raffi      (502) admin       (80)     1586 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/profile.c
+-rw-r--r--   0 raffi      (502) admin       (80)      914 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/src/init/rng_helpers.c
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.697113 pygsl_lite-0.1.6/swig_src/
+-rw-r--r--   0 raffi      (502) admin       (80)     2107 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/_block.py
+-rw-r--r--   0 raffi      (502) admin       (80)     2113 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/_callback.py
+-rw-r--r--   0 raffi      (502) admin       (80)   640394 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/block_wrap.c
+-rw-r--r--   0 raffi      (502) admin       (80)   257223 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/callback_wrap.c
+-rw-r--r--   0 raffi      (502) admin       (80)    16828 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/gslwrap.py
+-rw-r--r--   0 raffi      (502) admin       (80)   230587 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/gslwrap_wrap.c
+-rw-r--r--   0 raffi      (502) admin       (80)     2149 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/odeiv2.py
+-rw-r--r--   0 raffi      (502) admin       (80)   288839 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/swig_src/odeiv2_wrap.c
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.697473 pygsl_lite-0.1.6/test/
+-rw-r--r--   0 raffi      (502) admin       (80)      405 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/test/test_spline.py
+-rw-r--r--   0 raffi      (502) admin       (80)      294 2024-05-03 15:11:10.000000 pygsl_lite-0.1.6/tox.ini
+drwxr-xr-x   0 raffi      (502) admin       (80)        0 2024-05-03 15:12:50.699864 pygsl_lite-0.1.6/typemaps/
+-rw-r--r--   0 raffi      (502) admin       (80)     6395 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/block_conversion_functions.h
+-rw-r--r--   0 raffi      (502) admin       (80)     6965 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/c.py
+-rw-r--r--   0 raffi      (502) admin       (80)      384 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/callable.i
+-rw-r--r--   0 raffi      (502) admin       (80)    43953 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/convert_block_description.h
+-rw-r--r--   0 raffi      (502) admin       (80)      644 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/error.i
+-rw-r--r--   0 raffi      (502) admin       (80)     2311 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/file_typemaps.i
+-rw-r--r--   0 raffi      (502) admin       (80)     2313 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/gsl_block_special_typemaps.i
+-rw-r--r--   0 raffi      (502) admin       (80)    15915 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/gsl_block_typemaps.i
+-rw-r--r--   0 raffi      (502) admin       (80)     4306 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/gsl_complex_typemap.i
+-rw-r--r--   0 raffi      (502) admin       (80)     2488 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/gsl_error_typemap.i
+-rw-r--r--   0 raffi      (502) admin       (80)     9481 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/gsl_function_typemaps.i
+-rw-r--r--   0 raffi      (502) admin       (80)      102 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/gsl_permutations_typemaps.i
+-rw-r--r--   0 raffi      (502) admin       (80)      305 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/gsl_rng_typemaps.i
+-rw-r--r--   0 raffi      (502) admin       (80)      496 2023-08-31 08:27:23.000000 pygsl_lite-0.1.6/typemaps/misc_typemaps.i
```

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/block_helpers.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/block_helpers.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/block_helpers_numpy.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/block_helpers_numpy.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/capsuletrunk.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/capsuletrunk.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/complex_helpers.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/complex_helpers.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/error_helpers.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/error_helpers.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/errorno.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/errorno.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/function_helpers.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/function_helpers.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/general_helpers.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/general_helpers.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/intern.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/intern.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/profile.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/profile.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/pygsl_features_config.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/pygsl_features_config.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/rng.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/rng.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/rng_helpers.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/rng_helpers.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/solver.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/solver.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/string_helpers.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/string_helpers.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/transition.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/transition.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/Include/pygsl_lite/utils.h` & `pygsl_lite-0.1.6/Include/pygsl_lite/utils.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/LICENSE` & `pygsl_lite-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/PKG-INFO` & `pygsl_lite-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pygsl_lite
-Version: 0.1.5
+Version: 0.1.6
 Summary: Minimal GNU Scientific Library Interface
 Author: Sergei Ossokine
 License: GPL-2.0-or-later
-Project-URL: homepage, https://github.com/SergeiOssokine/pygsl_lite
+Project-URL: homepage, https://github.com/AEI-ACR/pygsl_lite
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy>=1.23.0
 
 PyGSL_Lite
 ============
 
 This package provides a very minimal wrapper for ``GSL``, based on the `pygsl library <https://github.com/pygsl/pygsl>`_ .
 This is done to drastically reduce complexity. In particular,  the following features are supported as they provide performance
 advantages useful for physics simulations.
```

### Comparing `pygsl_lite-0.1.5/README.rst` & `pygsl_lite-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/gsl_dist/gsl_Extension.py` & `pygsl_lite-0.1.6/gsl_dist/gsl_Extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from distutils.dep_util import newer_group
 
 import os
 import os.path
 import re
 import string
 import types
-import imp
 from sys import argv,version_info
 
 from gsl_Location import gsl_Location
 
 try:
         from array_includes import array_include_dirs        
 except ImportError:
@@ -104,20 +103,15 @@
 	    if libraries is None: libraries=[]
 	    #libraries.append('pygsl_lite')
 	    libraries.extend(gsl_Location.get_gsl_lib_list())
 
 	    # test if Numeric module is available
 	    if define_macros is None:
 		    define_macros=[]
-	    try:
-		    imp.find_module("Numeric")
-		    define_macros = define_macros + [("NUMERIC",1),]
-	    except ImportError:	    
-		    define_macros = define_macros + [("NUMERIC",0), ]
-
+	    define_macros = define_macros + [("NUMERIC",0), ]
 	    if undef_macros == None:
 		    undef_macros = []
 	    if 'NDEBUG' not in undef_macros:
 		    undef_macros.append('NDEBUG')
 	    tmp = map(lambda x: x[0], define_macros)
 
 	    # Now config will test of GSL_MAJOR_VERSION and GSL_MINOR_VERSION is defined
```

### Comparing `pygsl_lite-0.1.5/gsl_dist/gsl_Location.py` & `pygsl_lite-0.1.6/gsl_dist/gsl_Location.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/gsl_dist/swig_extension.py` & `pygsl_lite-0.1.6/gsl_dist/swig_extension.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/gsl_packages.py` & `pygsl_lite-0.1.6/gsl_packages.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/__init__.py` & `pygsl_lite-0.1.6/pygsl_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/_block.py` & `pygsl_lite-0.1.6/pygsl_lite/_block.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/_callback.py` & `pygsl_lite-0.1.6/pygsl_lite/_callback.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/_generic_solver.py` & `pygsl_lite-0.1.6/pygsl_lite/_generic_solver.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/block.py` & `pygsl_lite-0.1.6/pygsl_lite/block.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/errors.py` & `pygsl_lite-0.1.6/pygsl_lite/errors.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/gsl_function.py` & `pygsl_lite-0.1.6/pygsl_lite/gsl_function.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/gslwrap.py` & `pygsl_lite-0.1.6/pygsl_lite/gslwrap.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/interpolation.py` & `pygsl_lite-0.1.6/pygsl_lite/interpolation.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/odeiv.py` & `pygsl_lite-0.1.6/pygsl_lite/odeiv.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/odeiv2.py` & `pygsl_lite-0.1.6/pygsl_lite/odeiv2.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/roots.py` & `pygsl_lite-0.1.6/pygsl_lite/roots.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/spline.py` & `pygsl_lite-0.1.6/pygsl_lite/spline.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite/vector.py` & `pygsl_lite-0.1.6/pygsl_lite/vector.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/pygsl_lite.egg-info/PKG-INFO` & `pygsl_lite-0.1.6/pygsl_lite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: pygsl-lite
-Version: 0.1.5
+Name: pygsl_lite
+Version: 0.1.6
 Summary: Minimal GNU Scientific Library Interface
 Author: Sergei Ossokine
 License: GPL-2.0-or-later
-Project-URL: homepage, https://github.com/SergeiOssokine/pygsl_lite
+Project-URL: homepage, https://github.com/AEI-ACR/pygsl_lite
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy>=1.23.0
 
 PyGSL_Lite
 ============
 
 This package provides a very minimal wrapper for ``GSL``, based on the `pygsl library <https://github.com/pygsl/pygsl>`_ .
 This is done to drastically reduce complexity. In particular,  the following features are supported as they provide performance
 advantages useful for physics simulations.
```

### Comparing `pygsl_lite-0.1.5/pygsl_lite.egg-info/SOURCES.txt` & `pygsl_lite-0.1.6/pygsl_lite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+.gitignore
 LICENSE
 README.rst
 gsl_packages.py
 pyproject.toml
 setup.py
+tox.ini
+.github/workflows/ci.yml
 Include/pygsl_lite/arrayobject.h
 Include/pygsl_lite/block_helpers.h
 Include/pygsl_lite/block_helpers_numpy.h
 Include/pygsl_lite/capsuletrunk.h
 Include/pygsl_lite/compilers.h
 Include/pygsl_lite/complex_helpers.h
 Include/pygsl_lite/error_helpers.h
```

### Comparing `pygsl_lite-0.1.5/pyproject.toml` & `pygsl_lite-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,17 @@
     requires-python = ">=3.8"
     dependencies = ["numpy>=1.23.0"]
     # dynamic properties set by tools:
     dynamic = ["version"]
 
 
 [project.urls]
-    homepage = "https://github.com/SergeiOssokine/pygsl_lite"
-
+    homepage = "https://github.com/AEI-ACR/pygsl_lite"
 
 [tool.setuptools_scm]
     write_to = "pygsl_lite/_version.py"
+
+[tool.pytest.ini_options]
+    minversion = "6.0"
+    testpaths = [
+        "test",
+    ]
```

### Comparing `pygsl_lite-0.1.5/setup.py` & `pygsl_lite-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block.i` & `pygsl_lite-0.1.6/src/block/gsl_block.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_char.i` & `pygsl_lite-0.1.6/src/block/gsl_block_char.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_complex.i` & `pygsl_lite-0.1.6/src/block/gsl_block_complex.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_complex_float.i` & `pygsl_lite-0.1.6/src/block/gsl_block_complex_float.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_double.i` & `pygsl_lite-0.1.6/src/block/gsl_block_double.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_float.i` & `pygsl_lite-0.1.6/src/block/gsl_block_float.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_generic.i` & `pygsl_lite-0.1.6/src/block/gsl_block_generic.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_generic_typed.i` & `pygsl_lite-0.1.6/src/block/gsl_block_generic_typed.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_int.i` & `pygsl_lite-0.1.6/src/block/gsl_block_int.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_long.i` & `pygsl_lite-0.1.6/src/block/gsl_block_long.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/block/gsl_block_short.i` & `pygsl_lite-0.1.6/src/block/gsl_block_short.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/chars.c` & `pygsl_lite-0.1.6/src/callback/chars.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/function_helpers.c` & `pygsl_lite-0.1.6/src/callback/function_helpers.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/gsl_callback.i` & `pygsl_lite-0.1.6/src/callback/gsl_callback.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/gsl_function_test.i` & `pygsl_lite-0.1.6/src/callback/gsl_function_test.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/gsl_multiroots.i` & `pygsl_lite-0.1.6/src/callback/gsl_multiroots.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/gsl_odeiv.i` & `pygsl_lite-0.1.6/src/callback/gsl_odeiv.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/gsl_odeiv2.i` & `pygsl_lite-0.1.6/src/callback/gsl_odeiv2.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/gsl_roots.i` & `pygsl_lite-0.1.6/src/callback/gsl_roots.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/odeiv.ic` & `pygsl_lite-0.1.6/src/callback/odeiv.ic`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/callback/odeiv_func2.ic` & `pygsl_lite-0.1.6/src/callback/odeiv_func2.ic`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/errortestmodule.c` & `pygsl_lite-0.1.6/src/errortestmodule.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/gslwrap/gsl_gslwrap.i` & `pygsl_lite-0.1.6/src/gslwrap/gsl_gslwrap.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/gslwrap/interpolation.i` & `pygsl_lite-0.1.6/src/gslwrap/interpolation.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/block_helpers.c` & `pygsl_lite-0.1.6/src/init/block_helpers.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/block_helpers_numpy.ic` & `pygsl_lite-0.1.6/src/init/block_helpers_numpy.ic`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/complex_helpers.c` & `pygsl_lite-0.1.6/src/init/complex_helpers.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/error_helpers.c` & `pygsl_lite-0.1.6/src/init/error_helpers.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/errorno.c` & `pygsl_lite-0.1.6/src/init/errorno.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/function_helpers.c` & `pygsl_lite-0.1.6/src/init/function_helpers.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/general_helpers.c` & `pygsl_lite-0.1.6/src/init/general_helpers.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/initmodule.c` & `pygsl_lite-0.1.6/src/init/initmodule.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/inittestmodule.c` & `pygsl_lite-0.1.6/src/init/inittestmodule.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/profile.c` & `pygsl_lite-0.1.6/src/init/profile.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/src/init/rng_helpers.c` & `pygsl_lite-0.1.6/src/init/rng_helpers.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/_block.py` & `pygsl_lite-0.1.6/swig_src/_block.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/_callback.py` & `pygsl_lite-0.1.6/swig_src/_callback.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/block_wrap.c` & `pygsl_lite-0.1.6/swig_src/block_wrap.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/callback_wrap.c` & `pygsl_lite-0.1.6/swig_src/callback_wrap.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/gslwrap.py` & `pygsl_lite-0.1.6/swig_src/gslwrap.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/gslwrap_wrap.c` & `pygsl_lite-0.1.6/swig_src/gslwrap_wrap.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/odeiv2.py` & `pygsl_lite-0.1.6/swig_src/odeiv2.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/swig_src/odeiv2_wrap.c` & `pygsl_lite-0.1.6/swig_src/odeiv2_wrap.c`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/block_conversion_functions.h` & `pygsl_lite-0.1.6/typemaps/block_conversion_functions.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/c.py` & `pygsl_lite-0.1.6/typemaps/c.py`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/convert_block_description.h` & `pygsl_lite-0.1.6/typemaps/convert_block_description.h`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/error.i` & `pygsl_lite-0.1.6/typemaps/error.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/file_typemaps.i` & `pygsl_lite-0.1.6/typemaps/file_typemaps.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/gsl_block_special_typemaps.i` & `pygsl_lite-0.1.6/typemaps/gsl_block_special_typemaps.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/gsl_block_typemaps.i` & `pygsl_lite-0.1.6/typemaps/gsl_block_typemaps.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/gsl_complex_typemap.i` & `pygsl_lite-0.1.6/typemaps/gsl_complex_typemap.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/gsl_error_typemap.i` & `pygsl_lite-0.1.6/typemaps/gsl_error_typemap.i`

 * *Files identical despite different names*

### Comparing `pygsl_lite-0.1.5/typemaps/gsl_function_typemaps.i` & `pygsl_lite-0.1.6/typemaps/gsl_function_typemaps.i`

 * *Files identical despite different names*

