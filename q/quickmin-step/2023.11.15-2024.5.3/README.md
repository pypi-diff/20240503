# Comparing `tmp/quickmin_step-2023.11.15.tar.gz` & `tmp/quickmin_step-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickmin_step-2023.11.15.tar", last modified: Wed Nov 15 15:36:05 2023, max compression
+gzip compressed data, was "quickmin_step-2024.5.3.tar", last modified: Fri May  3 20:24:11 2024, max compression
```

## Comparing `quickmin_step-2023.11.15.tar` & `quickmin_step-2024.5.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.352922 quickmin_step-2023.11.15/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.356922 quickmin_step-2023.11.15/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/_static/SEAMM Inverted 288x181.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.356922 quickmin_step-2023.11.15/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/api/quickmin_step.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9544 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.356922 quickmin_step-2023.11.15/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.356922 quickmin_step-2023.11.15/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.356922 quickmin_step-2023.11.15/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/quickmin_step/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/quickmin_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/quickmin_step/data/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    15448 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/quickmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/quickmin_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/quickmin_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/quickmin_step/tk_quickmin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/quickmin_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2023-11-15 15:36:05.000000 quickmin_step-2023.11.15/quickmin_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-11-15 15:36:05.000000 quickmin_step-2023.11.15/quickmin_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 15:36:05.000000 quickmin_step-2023.11.15/quickmin_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-15 15:36:05.000000 quickmin_step-2023.11.15/quickmin_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-15 15:36:05.000000 quickmin_step-2023.11.15/quickmin_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-15 15:36:05.000000 quickmin_step-2023.11.15/quickmin_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 15:35:43.000000 quickmin_step-2023.11.15/quickmin_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 15:36:05.360922 quickmin_step-2023.11.15/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/tests/test_quickmin_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68751 2023-11-15 15:35:39.000000 quickmin_step-2023.11.15/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.503210 quickmin_step-2024.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/SEAMM Inverted 288x181.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/api/quickmin_step.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9544 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/quickmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/quickmin_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/quickmin_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/tk_quickmin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:24:00.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/tests/test_quickmin_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/versioneer.py
```

### Comparing `quickmin_step-2023.11.15/CONTRIBUTING.rst` & `quickmin_step-2024.5.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/HISTORY.rst` & `quickmin_step-2024.5.3/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 =======
 History
 =======
+2024.5.3 -- Added single point energy and Results.json
+    * Added control to allow a single point energy as well as optimization. This
+      supports using QuickMin with e.g energy scans.
+    * Standardized the name of the energy to simply "energy" to better support other
+      plug-ins and codes understanding the results.
+      
 2023.11.15 -- Bugfix: structure handling
     Error putting the coordinates into a newly created configuration.
     
 2023.10.30 -- Enhanced structure handling.
     Switched to standard handling of structures, which adds ability to name with the
     IUPAC name, InCHI, and InChIKey in addition to previous methods.
```

### Comparing `quickmin_step-2023.11.15/LICENSE` & `quickmin_step-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/PKG-INFO` & `quickmin_step-2024.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickmin_step
-Version: 2023.11.15
+Version: 2024.5.3
 Summary: A SEAMM plug-in for simple, quick minimization
 Home-page: https://github.com/molssi-seamm/quickmin_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: seamm
 Requires-Dist: seamm-util
 Requires-Dist: seamm-widgets
+Requires-Dist: numpy
 
 ======================
 SEAMM QuickMin Plug-in
 ======================
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/quickmin_step
    :target: https://github.com/molssi-seamm/quickmin_step/pulls
@@ -109,14 +110,20 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.3 -- Added single point energy and Results.json
+    * Added control to allow a single point energy as well as optimization. This
+      supports using QuickMin with e.g energy scans.
+    * Standardized the name of the energy to simply "energy" to better support other
+      plug-ins and codes understanding the results.
+      
 2023.11.15 -- Bugfix: structure handling
     Error putting the coordinates into a newly created configuration.
     
 2023.10.30 -- Enhanced structure handling.
     Switched to standard handling of structures, which adds ability to name with the
     IUPAC name, InCHI, and InChIKey in addition to previous methods.
```

### Comparing `quickmin_step-2023.11.15/README.rst` & `quickmin_step-2024.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/Makefile` & `quickmin_step-2024.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/_static/SEAMM Inverted 288x181.png` & `quickmin_step-2024.5.3/docs/_static/SEAMM Inverted 288x181.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/_static/SEAMM logo.png` & `quickmin_step-2024.5.3/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/_static/molssi_main_logo.png` & `quickmin_step-2024.5.3/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/_static/molssi_main_logo_inverted_white.png` & `quickmin_step-2024.5.3/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/_static/molssi_square.png` & `quickmin_step-2024.5.3/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/_static/nsf.png` & `quickmin_step-2024.5.3/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/api/quickmin_step.rst` & `quickmin_step-2024.5.3/docs/api/quickmin_step.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/conf.py` & `quickmin_step-2024.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/developer_guide/installation.rst` & `quickmin_step-2024.5.3/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/getting_started/index.rst` & `quickmin_step-2024.5.3/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/index.rst` & `quickmin_step-2024.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/make.bat` & `quickmin_step-2024.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/docs/user_guide/index.rst` & `quickmin_step-2024.5.3/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/quickmin_step/__init__.py` & `quickmin_step-2024.5.3/quickmin_step/__init__.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/quickmin_step/data/references.bib` & `quickmin_step-2024.5.3/quickmin_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/quickmin_step/metadata.py` & `quickmin_step-2024.5.3/quickmin_step/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,15 +62,31 @@
 type : str
     The type of the data: string, integer, or float.
 
 units : str
     Optional units for the result. If present, the value should be in these units.
 """
 metadata["results"] = {
-    "total energy": {
+    "energy": {
         "description": "The total energy",
         "dimensionality": "scalar",
         "property": "total energy#QuickMin#{model}",
         "type": "float",
         "units": "kJ/mol",
     },
+    "gradients": {
+        "description": "The gradients",
+        "dimensionality": "[3, n_atoms]",
+        "type": "float",
+        "units": "kJ/mol/Å",
+    },
+    "forcefield": {
+        "description": "The forcefield used",
+        "dimensionality": "scalar",
+        "type": "string",
+    },
+    "model": {
+        "description": "The model string",
+        "dimensionality": "scalar",
+        "type": "string",
+    },
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quickmin_step-2023.11.15/quickmin_step/quickmin.py` & `quickmin_step-2024.5.3/quickmin_step/quickmin.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import os
 import sys
 import threading
 import time
 
 import logging
+import numpy as np
 from pathlib import Path
 import pkg_resources
 import pprint  # noqa: F401
 import shutil
 import string
 import subprocess
 
@@ -208,29 +209,35 @@
         -------
         str
             A description of the current step.
         """
         if P is None:
             P = self.parameters.values_to_dict()
 
+        calculation = P["calculation"]
         n_steps = P["n_steps"]
         forcefield = P["forcefield"]
         if forcefield == "best available":
             ff_name = "the best available forcefield"
         else:
             ff_name = forcefield.split()[0]
 
-        text = f"Minimizing the structure with {ff_name}, with a maximum of "
-        text += f"{n_steps} steps."
-
-        if P["forcefield"] == "best available":
-            kwargs = {}
+        if calculation == "optimization":
+            text = f"Minimizing the structure with {ff_name}, with a maximum of "
+            text += f"{n_steps} steps."
+
+            if P["forcefield"] == "best available":
+                kwargs = {}
+            else:
+                kwargs = {"forcefield": ff_name}
+            text += seamm.standard_parameters.structure_handling_description(
+                P, **kwargs
+            )
         else:
-            kwargs = {"forcefield": ff_name}
-        text += seamm.standard_parameters.structure_handling_description(P, **kwargs)
+            text = f"Performing a quick energy calculation with {ff_name}."
 
         return self.header + "\n" + __(text, indent=4 * " ").__str__()
 
     def run(self):
         """Run a QuickMin step.
 
         Parameters
@@ -245,14 +252,15 @@
         global OpenBabel_version
 
         next_node = super().run(printer)
         # Get the values of the parameters, dereferencing any variables
         P = self.parameters.current_values_to_dict(
             context=seamm.flowchart_variables._data
         )
+        calculation = P["calculation"]
 
         # Print what we are doing
         printer.important(__(self.description_text(P)))
 
         # Add the citations for Open Babel
         self.references.cite(
             raw=self._bibliography["openbabel"],
@@ -322,14 +330,15 @@
         directory.mkdir(parents=True, exist_ok=True)
 
         # Get the current system and configuration (ignoring the system...)
         system, configuration = self.get_system_configuration(None)
 
         obmol = configuration.to_OBMol()
 
+        gradients = []
         if P["forcefield"] == "best available":
             for ff_name in ("GAFF", "MMFF94s", "Ghemical", "UFF"):
                 obFF = openbabel.OBForceField.FindForceField(ff_name)
 
                 if obFF is None:
                     self.logger.warning(f"Couldn't find forcefield '{ff_name}'")
                     continue
@@ -341,20 +350,37 @@
                 with out:
                     if not obFF.Setup(obmol):
                         if ff_name == "UFF":
                             raise RuntimeError(
                                 "Could not find a forcefield for the molecule"
                             )
                         continue
-                    obFF.ConjugateGradients(P["n_steps"])
+                    if calculation == "optimization":
+                        obFF.ConjugateGradients(P["n_steps"])
 
-                    energy = obFF.Energy(False)
+                    energy = obFF.Energy(True)
                     units = obFF.GetUnit()
 
-                path = Path(self.directory) / "min.out"
+                    # Capture the gradients
+                    factor = Q_(1.0, units).m_as("kJ/mol")
+                    for atom in openbabel.OBMolAtomIter(obmol):
+                        # vector objects have to be de-referenced individually (sigh)
+                        grad = obFF.GetGradient(atom)
+                        gradients.append(
+                            [
+                                factor * grad.GetX(),
+                                factor * grad.GetY(),
+                                factor * grad.GetZ(),
+                            ]
+                        )
+
+                if calculation == "optimization":
+                    path = Path(self.directory) / "min.out"
+                else:
+                    path = Path(self.directory) / "energy.out"
                 path.write_text(out.capturedtext)
                 break
         else:
             ff_name = P["forcefield"].split()[0]
             obFF = openbabel.OBForceField.FindForceField(ff_name)
 
             if obFF is None:
@@ -365,21 +391,38 @@
             # see https://stackoverflow.com/questions/50978464/redirect-logs-to-file-in-pybel  # noqa: E501
             out = OutputGrabber(sys.stderr)
             with out:
                 if not obFF.Setup(obmol):
                     raise RuntimeError(
                         f"Could not assign forcefield {ff_name} to the molecule"
                     )
-                obFF.ConjugateGradients(P["n_steps"])
-                obFF.GetCoordinates(obmol)
+                if calculation == "optimization":
+                    obFF.ConjugateGradients(P["n_steps"])
+                    obFF.GetCoordinates(obmol)
 
-                energy = obFF.Energy(False)
+                energy = obFF.Energy(True)
                 units = obFF.GetUnit()
 
-            path = Path(self.directory) / "min.out"
+                # Capture the gradients
+                factor = Q_(1.0, units).m_as("kJ/mol")
+                for atom in openbabel.OBMolAtomIter(obmol):
+                    # vector objects have to be de-referenced individually (sigh)
+                    grad = obFF.GetGradient(atom)
+                    gradients.append(
+                        [
+                            factor * grad.GetX(),
+                            factor * grad.GetY(),
+                            factor * grad.GetZ(),
+                        ]
+                    )
+
+            if calculation == "optimization":
+                path = Path(self.directory) / "min.out"
+            else:
+                path = Path(self.directory) / "energy.out"
             path.write_text(out.capturedtext)
 
         # Set the model chemistry to the forcefield name.
         self._model = ff_name
 
         # Check for convergence
         lines = out.capturedtext.splitlines()
@@ -389,28 +432,42 @@
         else:
             n_iterations = "unknown"
         converged = "HAS CONVERGED" in lines[-1]
 
         # Set up the results data
         data = {}
         if units == "kJ/mol":
-            data["total energy"] = energy
+            data["energy"] = energy
+            data["gradients"] = gradients
         else:
-            data["total energy"] = Q_(energy, units).m_as("kJ/mol")
-
-        if converged:
-            text = (
-                f"The minimization using {ff_name} converged in {n_iterations} steps "
-                f"to {energy:.3f} {units}. "
-            )
+            data["energy"] = Q_(energy, units).m_as("kJ/mol")
+            tmp = np.array(gradients) * Q_(1.0, units).m_as("kJ/mol")
+            data["gradients"] = tmp.tolist()
+        data["forcefield"] = ff_name
+        data["model"] = self.model
+
+        if calculation == "optimization":
+            if converged:
+                text = (
+                    f"The minimization using {ff_name} converged in {n_iterations} "
+                    f"steps to {energy:.3f} {units}. "
+                )
+            else:
+                text = (
+                    f"The minimization with {ff_name} did not converge in "
+                    f"{n_iterations} steps! The final energy was {energy:.3f} {units}. "
+                )
         else:
-            text = (
-                f"The minimization with {ff_name} did not converge in {n_iterations} "
-                f"steps! The final energy was {energy:.3f} {units}. "
-            )
+            text = f"Calculated the energy and gradients using {ff_name}"
+
+        # Put any requested results into variables or tables
+        self.store_results(
+            configuration=configuration,
+            data=data,
+        )
 
         # Save the structure
         system, configuration = self.get_system_configuration(P)
 
         configuration.coordinates_from_OBMol(obmol)
 
         text += seamm.standard_parameters.set_names(
@@ -451,18 +508,12 @@
                 raw=self._bibliography[ff_name],
                 alias=ff_name,
                 module="quickmin_step",
                 level=1,
                 note=f"The main {ff_name} citation.",
             )
 
-        # Put any requested results into variables or tables
-        self.store_results(
-            configuration=configuration,
-            data=data,
-        )
-
         # Add other citations here or in the appropriate place in the code.
         # Add the bibtex to data/references.bib, and add a self.reference.cite
         # similar to the above to actually add the citation to the references.
 
         return next_node
```

### Comparing `quickmin_step-2023.11.15/quickmin_step/quickmin_parameters.py` & `quickmin_step-2024.5.3/quickmin_step/quickmin_parameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -88,54 +88,34 @@
                 "MMFF94s -- MMFF94s force field for minimization",
                 "UFF -- Universal Force Field",
             ),
             "format_string": "",
             "description": "Forcefield:",
             "help_text": "The forcefield to use.",
         },
+        "calculation": {
+            "default": "optimization",
+            "kind": "enum",
+            "enumeration": (
+                "optimization",
+                "single-point energy",
+            ),
+            "format_string": "",
+            "description": "Calculation:",
+            "help_text": "The type of calculation to perform.",
+        },
         "n_steps": {
             "default": 1000,
             "kind": "integer",
             "default_units": "",
             "enumeration": tuple(),
             "format_string": "",
             "description": "Maximum steps:",
             "help_text": "The maximum number of steps to run.",
         },
-        # Put in the configuration handling options needed
-        # "structure handling": {
-        #     "default": "Create a new configuration",
-        #     "kind": "enum",
-        #     "default_units": "",
-        #     "enumeration": (
-        #         "Overwrite the current configuration",
-        #         "Create a new configuration",
-        #     ),
-        #     "format_string": "s",
-        #     "description": "Configuration handling:",
-        #     "help_text": (
-        #         "Whether to overwrite the current configuration, or create a new "
-        #         "configuration or system and configuration for the new structure"
-        #     ),
-        # },
-        # "configuration name": {
-        #     "default": "optimized with <Forcefield>",
-        #     "kind": "string",
-        #     "default_units": "",
-        #     "enumeration": (
-        #         "optimized with <Forcefield>",
-        #         "keep current name",
-        #         "use SMILES string",
-        #         "use Canonical SMILES string",
-        #         "use configuration number",
-        #     ),
-        #     "format_string": "s",
-        #     "description": "Configuration name:",
-        #     "help_text": "The name for the new configuration",
-        # },
         # Results handling
         "results": {
             "default": {},
             "kind": "dictionary",
             "default_units": "",
             "enumeration": tuple(),
             "format_string": "",
```

### Comparing `quickmin_step-2023.11.15/quickmin_step/quickmin_step.py` & `quickmin_step-2024.5.3/quickmin_step/quickmin_step.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/quickmin_step/tk_quickmin.py` & `quickmin_step-2024.5.3/quickmin_step/tk_quickmin.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,17 @@
                 "results",
                 "extra keywords",
                 "create tables",
                 "subsequent structure handling",
             ):
                 self[key] = P[key].widget(frame)
 
+        # and binding to change as needed
+        self["calculation"].combobox.bind("<<ComboboxSelected>>", self.reset_dialog)
+
         # and lay them out
         self.reset_dialog()
 
     def reset_dialog(self, widget=None):
         """Layout the widgets in the dialog.
 
         The widgets are chosen by default from the information in
@@ -159,28 +162,27 @@
         """
 
         # Remove any widgets previously packed
         frame = self["frame"]
         for slave in frame.grid_slaves():
             slave.grid_forget()
 
-        # Shortcut for parameters
-        P = self.node.parameters
-
         # keep track of the row in a variable, so that the layout is flexible
-        # if e.g. rows are skipped to control such as "method" here
+        # if e.g. rows are skipped to control such as "calculation" here
+        calculation = self["calculation"].get()
+
         row = 0
         widgets = []
-        for key in P:
-            if key[0] != "_" and key not in (
-                "results",
-                "extra keywords",
-                "create tables",
-                "subsequent structure handling",
-            ):
+        for key in ("forcefield", "calculation"):
+            self[key].grid(row=row, column=0, sticky=tk.EW)
+            widgets.append(self[key])
+            row += 1
+
+        if calculation == "optimization":
+            for key in ("n_steps",):
                 self[key].grid(row=row, column=0, sticky=tk.EW)
                 widgets.append(self[key])
                 row += 1
 
         # Align the labels
         sw.align_labels(widgets, sticky=tk.E)
```

### Comparing `quickmin_step-2023.11.15/quickmin_step.egg-info/PKG-INFO` & `quickmin_step-2024.5.3/quickmin_step.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quickmin-step
-Version: 2023.11.15
+Name: quickmin_step
+Version: 2024.5.3
 Summary: A SEAMM plug-in for simple, quick minimization
 Home-page: https://github.com/molssi-seamm/quickmin_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: seamm
 Requires-Dist: seamm-util
 Requires-Dist: seamm-widgets
+Requires-Dist: numpy
 
 ======================
 SEAMM QuickMin Plug-in
 ======================
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/quickmin_step
    :target: https://github.com/molssi-seamm/quickmin_step/pulls
@@ -109,14 +110,20 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.3 -- Added single point energy and Results.json
+    * Added control to allow a single point energy as well as optimization. This
+      supports using QuickMin with e.g energy scans.
+    * Standardized the name of the energy to simply "energy" to better support other
+      plug-ins and codes understanding the results.
+      
 2023.11.15 -- Bugfix: structure handling
     Error putting the coordinates into a newly created configuration.
     
 2023.10.30 -- Enhanced structure handling.
     Switched to standard handling of structures, which adds ability to name with the
     IUPAC name, InCHI, and InChIKey in addition to previous methods.
```

### Comparing `quickmin_step-2023.11.15/quickmin_step.egg-info/SOURCES.txt` & `quickmin_step-2024.5.3/quickmin_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/setup.py` & `quickmin_step-2024.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2023.11.15/versioneer.py` & `quickmin_step-2024.5.3/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -272,15 +273,14 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
-
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,59 +304,54 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = (
-            "Versioneer was unable to run the project root directory. "
-            "Versioneer requires setup.py to be executed from "
-            "its immediate directory (like 'python setup.py COMMAND'), "
-            "or in a way that lets it use sys.argv[0] to find the root "
-            "(like 'python path/to/setup.py COMMAND')."
-        )
+        err = ("Versioneer was unable to run the project root directory. "
+               "Versioneer requires setup.py to be executed from "
+               "its immediate directory (like 'python setup.py COMMAND'), "
+               "or in a way that lets it use sys.argv[0] to find the root "
+               "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print(
-                "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(me), versioneer_py)
-            )
+            print("Warning: build in %s is using versioneer.py from %s"
+                  % (os.path.dirname(me), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
+    parser = configparser.ConfigParser()
     with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+        parser.read_file(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
-
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -373,40 +368,36 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
-
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
-
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen(
-                [c] + args,
-                cwd=cwd,
-                env=env,
-                stdout=subprocess.PIPE,
-                stderr=(subprocess.PIPE if hide_stderr else None),
-            )
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -423,17 +414,15 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY[
-    "git"
-] = '''
+LONG_VERSION_PY['git'] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -1000,86 +989,71 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r"\d", r)])
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix) :]
+            r = ref[len(tag_prefix):]
             if verbose:
                 print("picking %s" % r)
-            return {
-                "version": r,
-                "full-revisionid": keywords["full"].strip(),
-                "dirty": False,
-                "error": None,
-                "date": date,
-            }
+            return {"version": r,
+                    "full-revisionid": keywords["full"].strip(),
+                    "dirty": False, "error": None,
+                    "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {
-        "version": "0+unknown",
-        "full-revisionid": keywords["full"].strip(),
-        "dirty": False,
-        "error": "no suitable tags",
-        "date": None,
-    }
+    return {"version": "0+unknown",
+            "full-revisionid": keywords["full"].strip(),
+            "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(
-        GITS,
-        [
-            "describe",
-            "--tags",
-            "--dirty",
-            "--always",
-            "--long",
-            "--match",
-            "%s*" % tag_prefix,
-        ],
-        cwd=root,
-    )
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%s*" % tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1094,55 +1068,54 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[: git_describe.rindex("-dirty")]
+        git_describe = git_describe[:git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
+        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
+            pieces["error"] = ("unable to parse git-describe output: '%s'"
+                               % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
-                full_tag,
-                tag_prefix,
-            )
+            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
+                               % (full_tag, tag_prefix))
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
+        pieces["closest-tag"] = full_tag[len(tag_prefix):]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
-        0
-    ].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
+                       cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1190,30 +1163,24 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {
-                "version": dirname[len(parentdir_prefix) :],
-                "full-revisionid": None,
-                "dirty": False,
-                "error": None,
-                "date": None,
-            }
+            return {"version": dirname[len(parentdir_prefix):],
+                    "full-revisionid": None,
+                    "dirty": False, "error": None, "date": None}
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print(
-            "Tried directories %s but none started with prefix %s"
-            % (str(rootdirs), parentdir_prefix)
-        )
+        print("Tried directories %s but none started with prefix %s" %
+              (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1234,30 +1201,29 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(
-        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-    )
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+                   contents, re.M | re.S)
     if not mo:
-        mo = re.search(
-            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-        )
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+                       contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True,
+                          indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1281,15 +1247,16 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1395,21 +1362,19 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {
-            "version": "unknown",
-            "full-revisionid": pieces.get("long"),
-            "dirty": None,
-            "error": pieces["error"],
-            "date": None,
-        }
+        return {"version": "unknown",
+                "full-revisionid": pieces.get("long"),
+                "dirty": None,
+                "error": pieces["error"],
+                "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1421,21 +1386,17 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {
-        "version": rendered,
-        "full-revisionid": pieces["long"],
-        "dirty": pieces["dirty"],
-        "error": None,
-        "date": pieces.get("date"),
-    }
+    return {"version": rendered, "full-revisionid": pieces["long"],
+            "dirty": pieces["dirty"], "error": None,
+            "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1450,17 +1411,16 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert (
-        cfg.versionfile_source is not None
-    ), "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, \
+        "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1506,21 +1466,17 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {
-        "version": "0+unknown",
-        "full-revisionid": None,
-        "dirty": None,
-        "error": "unable to compute version",
-        "date": None,
-    }
+    return {"version": "0+unknown", "full-revisionid": None,
+            "dirty": None, "error": "unable to compute version",
+            "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1561,15 +1517,14 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
-
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1594,23 +1549,22 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib,
+                                                  cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
-
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
-
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1623,29 +1577,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if "py2exe" in sys.modules:  # py2exe enabled?
+    if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1656,25 +1606,21 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1693,18 +1639,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(
-                target_versionfile, self._versioneer_generated_versions
-            )
-
+            write_to_version_file(target_versionfile,
+                                  self._versioneer_generated_versions)
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1751,41 +1695,36 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (
-        EnvironmentError,
-        configparser.NoSectionError,
-        configparser.NoOptionError,
-    ) as e:
+    except (EnvironmentError, configparser.NoSectionError,
+            configparser.NoOptionError) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg",
+                  file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(
-            LONG
-            % {
-                "DOLLAR": "$",
-                "STYLE": cfg.style,
-                "TAG_PREFIX": cfg.tag_prefix,
-                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                "VERSIONFILE_SOURCE": cfg.versionfile_source,
-            }
-        )
+        f.write(LONG % {"DOLLAR": "$",
+                        "STYLE": cfg.style,
+                        "TAG_PREFIX": cfg.tag_prefix,
+                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        })
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
+                       "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1819,18 +1758,16 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
+        print(" appending versionfile_source ('%s') to MANIFEST.in" %
+              cfg.versionfile_source)
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

