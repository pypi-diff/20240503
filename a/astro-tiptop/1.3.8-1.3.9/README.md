# Comparing `tmp/astro_tiptop-1.3.8.tar.gz` & `tmp/astro_tiptop-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_tiptop-1.3.8.tar", last modified: Tue Apr 16 14:43:20 2024, max compression
+gzip compressed data, was "astro_tiptop-1.3.9.tar", last modified: Fri Apr 19 09:02:59 2024, max compression
```

## Comparing `astro_tiptop-1.3.8.tar` & `astro_tiptop-1.3.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.270354 astro_tiptop-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.214354 astro_tiptop-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.218354 astro_tiptop-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-AST-EXAMPLE.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-AST-GEN-RECARRAY.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-AST-READ.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-EXAMPLE.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-EXAMPLE.py
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/TIPTOP-GUI.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.258354 astro_tiptop-1.3.8/astTest/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISast10.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISast100.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISast1000.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISastMonads.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISastRandom.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/ERISastSingles1.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISast.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISastGenerate.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISastSingles.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/MAVISastTriplets.ini
--rw-r--r--   0 runner    (1001) docker     (127)   204688 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array10.npy
--rw-r--r--   0 runner    (1001) docker     (127)  2685346 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array100.npy
--rw-r--r--   0 runner    (1001) docker     (127) 26962531 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array100_e.npy
--rw-r--r--   0 runner    (1001) docker     (127)  2935683 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/astTest/rec_array10_e.npy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/astro_tiptop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 14:43:20.000000 astro_tiptop-1.3.8/astro_tiptop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.262354 astro_tiptop-1.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.262354 astro_tiptop-1.3.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22546 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/parameterFile.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/docs/source/wishList.rst
--rw-r--r--   0 runner    (1001) docker     (127)   165545 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/main_sphere_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/perfTest/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/ERIS.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/ERIS_LGS.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     7610 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniLTAO_1.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     7496 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniLTAO_2.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     7520 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniLTAO_3.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniSCAO_1.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniSCAO_2.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/HarmoniSCAO_3.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/MAVIS.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/MORFEO.ini
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/SOUL.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest/SPHERE.ini
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/perfTest.sh
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:43:20.270354 astro_tiptop-1.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tests/allTests.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tests/mavisResult0.npy
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tests/mavisResult1.npy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:43:20.266354 astro_tiptop-1.3.8/tiptop/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 14:43:19.000000 astro_tiptop-1.3.8/tiptop/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    40846 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/asterismSimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35034 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/baseSimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1419 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptopCLT.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptopGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-16 14:43:05.000000 astro_tiptop-1.3.8/tiptop/tiptopUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.324242 astro_tiptop-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.268242 astro_tiptop-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.272242 astro_tiptop-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-19 09:02:59.324242 astro_tiptop-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/TIPTOP-AST-EXAMPLE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/TIPTOP-AST-GEN-RECARRAY.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/TIPTOP-AST-READ.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/TIPTOP-EXAMPLE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/TIPTOP-EXAMPLE.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/TIPTOP-GUI.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.312242 astro_tiptop-1.3.9/astTest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/ERISast10.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/ERISast100.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/ERISast1000.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/ERISastMonads.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/ERISastRandom.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/ERISastSingles1.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/MAVISast.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/MAVISastGenerate.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/MAVISastSingles.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/MAVISastTriplets.ini
+-rw-r--r--   0 runner    (1001) docker     (127)   204688 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/rec_array10.npy
+-rw-r--r--   0 runner    (1001) docker     (127)  2685346 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/rec_array100.npy
+-rw-r--r--   0 runner    (1001) docker     (127) 26962531 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/rec_array100_e.npy
+-rw-r--r--   0 runner    (1001) docker     (127)  2935683 2024-04-19 09:02:48.000000 astro_tiptop-1.3.9/astTest/rec_array10_e.npy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.324242 astro_tiptop-1.3.9/astro_tiptop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-19 09:02:59.000000 astro_tiptop-1.3.9/astro_tiptop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-19 09:02:59.000000 astro_tiptop-1.3.9/astro_tiptop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:02:59.000000 astro_tiptop-1.3.9/astro_tiptop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 09:02:59.000000 astro_tiptop-1.3.9/astro_tiptop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 09:02:59.000000 astro_tiptop-1.3.9/astro_tiptop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.316242 astro_tiptop-1.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.316242 astro_tiptop-1.3.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/source/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22546 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/source/parameterFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/docs/source/wishList.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   165545 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/main_sphere_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.320242 astro_tiptop-1.3.9/perfTest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/ERIS.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/ERIS_LGS.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7610 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/HarmoniLTAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7496 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/HarmoniLTAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7520 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/HarmoniLTAO_3.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/HarmoniSCAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/HarmoniSCAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5777 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/HarmoniSCAO_3.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/MAVIS.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/MORFEO.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/SOUL.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest/SPHERE.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/perfTest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:02:59.324242 astro_tiptop-1.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.320242 astro_tiptop-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tests/allTests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tests/mavisResult0.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tests/mavisResult1.npy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:59.324242 astro_tiptop-1.3.9/tiptop/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tiptop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 09:02:59.000000 astro_tiptop-1.3.9/tiptop/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40846 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tiptop/asterismSimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34971 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tiptop/baseSimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tiptop/tiptop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1419 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tiptop/tiptopCLT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tiptop/tiptopGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-19 09:02:49.000000 astro_tiptop-1.3.9/tiptop/tiptopUtils.py
```

### Comparing `astro_tiptop-1.3.8/.github/workflows/publish.yml` & `astro_tiptop-1.3.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/.github/workflows/run_tests.yml` & `astro_tiptop-1.3.9/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/.gitignore` & `astro_tiptop-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/LICENSE` & `astro_tiptop-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/PKG-INFO` & `astro_tiptop-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.3.8
+Version: 1.3.9
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `astro_tiptop-1.3.8/README.md` & `astro_tiptop-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/TIPTOP-AST-EXAMPLE.ipynb` & `astro_tiptop-1.3.9/TIPTOP-AST-EXAMPLE.ipynb`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/TIPTOP-AST-GEN-RECARRAY.ipynb` & `astro_tiptop-1.3.9/TIPTOP-AST-GEN-RECARRAY.ipynb`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/TIPTOP-AST-READ.ipynb` & `astro_tiptop-1.3.9/TIPTOP-AST-READ.ipynb`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/TIPTOP-EXAMPLE.ipynb` & `astro_tiptop-1.3.9/TIPTOP-EXAMPLE.ipynb`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/TIPTOP-GUI.ipynb` & `astro_tiptop-1.3.9/TIPTOP-GUI.ipynb`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/ERISast10.ini` & `astro_tiptop-1.3.9/astTest/ERISast10.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/ERISast100.ini` & `astro_tiptop-1.3.9/astTest/ERISast100.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/ERISast1000.ini` & `astro_tiptop-1.3.9/astTest/ERISast1000.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/ERISastMonads.ini` & `astro_tiptop-1.3.9/astTest/ERISastMonads.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/ERISastRandom.ini` & `astro_tiptop-1.3.9/astTest/ERISastRandom.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/ERISastSingles1.ini` & `astro_tiptop-1.3.9/astTest/ERISastSingles1.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/MAVISast.ini` & `astro_tiptop-1.3.9/astTest/MAVISast.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/MAVISastGenerate.ini` & `astro_tiptop-1.3.9/astTest/MAVISastGenerate.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/MAVISastSingles.ini` & `astro_tiptop-1.3.9/astTest/MAVISastSingles.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/MAVISastTriplets.ini` & `astro_tiptop-1.3.9/astTest/MAVISastTriplets.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/rec_array10.npy` & `astro_tiptop-1.3.9/astTest/rec_array10.npy`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/rec_array100.npy` & `astro_tiptop-1.3.9/astTest/rec_array100.npy`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/rec_array100_e.npy` & `astro_tiptop-1.3.9/astTest/rec_array100_e.npy`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astTest/rec_array10_e.npy` & `astro_tiptop-1.3.9/astTest/rec_array10_e.npy`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/astro_tiptop.egg-info/PKG-INFO` & `astro_tiptop-1.3.9/astro_tiptop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.3.8
+Version: 1.3.9
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `astro_tiptop-1.3.8/astro_tiptop.egg-info/SOURCES.txt` & `astro_tiptop-1.3.9/astro_tiptop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/Makefile` & `astro_tiptop-1.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/make.bat` & `astro_tiptop-1.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/source/conf.py` & `astro_tiptop-1.3.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/source/howto.rst` & `astro_tiptop-1.3.9/docs/source/howto.rst`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/source/index.rst` & `astro_tiptop-1.3.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/source/parameterFile.rst` & `astro_tiptop-1.3.9/docs/source/parameterFile.rst`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/source/usage.rst` & `astro_tiptop-1.3.9/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/docs/source/wishList.rst` & `astro_tiptop-1.3.9/docs/source/wishList.rst`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/main_sphere_test.ipynb` & `astro_tiptop-1.3.9/main_sphere_test.ipynb`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/ERIS.ini` & `astro_tiptop-1.3.9/perfTest/ERIS.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/ERIS_LGS.ini` & `astro_tiptop-1.3.9/perfTest/ERIS_LGS.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/HarmoniLTAO_1.ini` & `astro_tiptop-1.3.9/perfTest/HarmoniLTAO_1.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/HarmoniLTAO_2.ini` & `astro_tiptop-1.3.9/perfTest/HarmoniLTAO_2.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/HarmoniLTAO_3.ini` & `astro_tiptop-1.3.9/perfTest/HarmoniLTAO_3.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/HarmoniSCAO_1.ini` & `astro_tiptop-1.3.9/perfTest/HarmoniSCAO_1.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/HarmoniSCAO_2.ini` & `astro_tiptop-1.3.9/perfTest/HarmoniSCAO_2.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/HarmoniSCAO_3.ini` & `astro_tiptop-1.3.9/perfTest/HarmoniSCAO_3.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/MAVIS.ini` & `astro_tiptop-1.3.9/perfTest/MAVIS.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/MORFEO.ini` & `astro_tiptop-1.3.9/perfTest/MORFEO.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/SOUL.ini` & `astro_tiptop-1.3.9/perfTest/SOUL.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/perfTest/SPHERE.ini` & `astro_tiptop-1.3.9/perfTest/SPHERE.ini`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/pyproject.toml` & `astro_tiptop-1.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/tests/allTests.py` & `astro_tiptop-1.3.9/tests/allTests.py`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/tiptop/asterismSimulation.py` & `astro_tiptop-1.3.9/tiptop/asterismSimulation.py`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/tiptop/baseSimulation.py` & `astro_tiptop-1.3.9/tiptop/baseSimulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,50 +533,53 @@
                     ee_at_radius_fn = interp1d(rr_, ee_, kind='cubic', bounds_error=False)
                     self.NGS_EE_field.append(ee_at_radius_fn(NGS_FWHM_mas[idx]))
                     if self.verbose:
                         print('EE                   :', "%.5f" % ee_at_radius_fn(NGS_FWHM_mas[idx]))
                     idx += 1
                 self.mLO           = MavisLO(self.path, self.parametersFile, verbose=self.verbose)
 
-            if astIndex is None:
-                self.Ctot          = self.mLO.computeTotalResidualMatrix(np.array(self.cartSciencePointingCoords),
-                                                                         self.cartNGSCoords_field, self.NGS_fluxes_field,
-                                                                         self.LO_freqs_field,
-                                                                         self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field, doAll=True)
-                if self.addFocusError:
-                    # compute focus error
-                    self.CtotFocus = self.mLO.computeFocusTotalResidualMatrix(self.cartNGSCoords_field, self.NGS_fluxes_field,
-                                                                         self.LO_freqs_field,
-                                                                         self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field)
-                    # add focus error to PSD using P3 FocusFilter
-                    for PSDho in self.PSD:
-                        FocusFilter = self.fao.FocusFilter()
-                        FocusFilter *= 1/FocusFilter.sum()
-                        PSDho += self.CtotFocus[0] * FocusFilter
 
-            else:
-                self.NGS_SR_asterism = []
-                for iid in self.currentAsterismIndices:
-                    self.NGS_SR_asterism.append(self.NGS_SR_field[iid])
-                self.NGS_FWHM_mas_asterism = []
-                for iid in self.currentAsterismIndices:
-                    self.NGS_FWHM_mas_asterism.append(self.NGS_FWHM_mas_field[iid])
-                if astIndex==0:
-                    self.mLO.computeTotalResidualMatrix(np.array(self.cartSciencePointingCoords),
-                                                        self.cartNGSCoords_field, self.NGS_fluxes_field,
-                                                        self.LO_freqs_field,
-                                                        self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field, doAll=False)
-                self.Ctot          = self.mLO.computeTotalResidualMatrixI(self.currentAsterismIndices,
-                                                                          np.array(self.cartSciencePointingCoords),
-                                                                          np.array(self.cartNGSCoords_asterism), self.NGS_fluxes_asterism,
-                                                                          self.LO_freqs_asterism,
-                                                                          self.NGS_SR_asterism, self.NGS_EE_field, self.NGS_FWHM_mas_asterism)
-                #TODO add self.CtotFocus computation only for the best asterism
-                #if self.addFocusError:
-                #    ...
+        if astIndex is None:
+            self.Ctot          = self.mLO.computeTotalResidualMatrix(np.array(self.cartSciencePointingCoords),
+                                                                     self.cartNGSCoords_field, self.NGS_fluxes_field,
+                                                                     self.LO_freqs_field,
+                                                                     self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field, doAll=True)
+            if self.addFocusError:
+                # compute focus error
+                self.CtotFocus = self.mLO.computeFocusTotalResidualMatrix(self.cartNGSCoords_field, self.NGS_fluxes_field,
+                                                                     self.LO_freqs_field,
+                                                                     self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field)
+                # add focus error to PSD using P3 FocusFilter
+                FocusFilter = self.fao.FocusFilter()
+                FocusFilter *= 1/FocusFilter.sum()
+                for PSDho in self.PSD:
+                    PSDho += self.CtotFocus[0] * FocusFilter
+
+        else:
+            self.NGS_SR_asterism = []
+            for iid in self.currentAsterismIndices:
+                self.NGS_SR_asterism.append(self.NGS_SR_field[iid])
+            self.NGS_FWHM_mas_asterism = []
+            for iid in self.currentAsterismIndices:
+                self.NGS_FWHM_mas_asterism.append(self.NGS_FWHM_mas_field[iid])
+            if astIndex==0:
+                self.mLO.computeTotalResidualMatrix(np.array(self.cartSciencePointingCoords),
+                                                    self.cartNGSCoords_field, self.NGS_fluxes_field,
+                                                    self.LO_freqs_field,
+                                                    self.NGS_SR_field, self.NGS_EE_field, self.NGS_FWHM_mas_field, doAll=False)
+            self.Ctot          = self.mLO.computeTotalResidualMatrixI(self.currentAsterismIndices,
+                                                                      np.array(self.cartSciencePointingCoords),
+                                                                      np.array(self.cartNGSCoords_asterism), self.NGS_fluxes_asterism,
+                                                                      self.LO_freqs_asterism,
+                                                                      self.NGS_SR_asterism, self.NGS_EE_field, self.NGS_FWHM_mas_asterism)
+            print('Asterism:', astIndex)
+            print('self.Ctot:', self.Ctot)
+            #TODO add self.CtotFocus computation only for the best asterism
+            #if self.addFocusError:
+            #    ...
         
         # ------------------------------------------------------------------------
         # HO PSF
         if self.verbose:
             print('******** HO PSF')
         pointings_SR, psdPointingsArray, psfLongExpPointingsArr, pointings_FWHM_mas = self.psdSetToPsfSet(self.N, 
                                                                                                      self.freq_range,
```

### Comparing `astro_tiptop-1.3.8/tiptop/tiptop.py` & `astro_tiptop-1.3.9/tiptop/tiptop.py`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/tiptop/tiptopCLT.py` & `astro_tiptop-1.3.9/tiptop/tiptopCLT.py`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/tiptop/tiptopGUI.py` & `astro_tiptop-1.3.9/tiptop/tiptopGUI.py`

 * *Files identical despite different names*

### Comparing `astro_tiptop-1.3.8/tiptop/tiptopUtils.py` & `astro_tiptop-1.3.9/tiptop/tiptopUtils.py`

 * *Files identical despite different names*

