# Comparing `tmp/nmk-python-0.8.3.tar.gz` & `tmp/nmk-python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-python-0.8.3.tar", last modified: Sun Dec  4 15:07:10 2022, max compression
+gzip compressed data, was "nmk-python-0.9.0.tar", last modified: Thu Jan  5 07:45:23 2023, max compression
```

## Comparing `nmk-python-0.8.3.tar` & `nmk-python-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:07:10.388234 nmk-python-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2022-12-04 15:06:42.000000 nmk-python-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2022-12-04 15:07:10.388234 nmk-python-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2022-12-04 15:06:42.000000 nmk-python-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2022-12-04 15:07:10.388234 nmk-python-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-04 15:07:08.000000 nmk-python-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:07:10.384234 nmk-python-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:07:10.388234 nmk-python-0.8.3/src/nmk_python/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/files.yml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/flake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/flake.yml
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/plugin-defs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/setup.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:07:10.388234 nmk-python-0.8.3/src/nmk_python/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/build.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/flake.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/pytest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/python-settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/python-test-debug-launch.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/templates/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2022-12-04 15:06:42.000000 nmk-python-0.8.3/src/nmk_python/version.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:07:10.388234 nmk-python-0.8.3/src/nmk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2022-12-04 15:07:10.000000 nmk-python-0.8.3/src/nmk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-04 15:07:10.000000 nmk-python-0.8.3/src/nmk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 15:07:10.000000 nmk-python-0.8.3/src/nmk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-04 15:07:10.000000 nmk-python-0.8.3/src/nmk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-04 15:07:10.000000 nmk-python-0.8.3/src/nmk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:45:23.552417 nmk-python-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-05 07:44:50.000000 nmk-python-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-01-05 07:45:23.552417 nmk-python-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-01-05 07:45:21.000000 nmk-python-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-05 07:45:23.552417 nmk-python-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-05 07:45:21.000000 nmk-python-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:45:23.548417 nmk-python-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:45:23.548417 nmk-python-0.9.0/src/nmk_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/badges.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/files.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/flake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/flake.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/plugin-defs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/setup.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:45:23.552417 nmk-python-0.9.0/src/nmk_python/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/build.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/flake.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/pytest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/python-settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/python-test-debug-launch.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/templates/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-05 07:44:50.000000 nmk-python-0.9.0/src/nmk_python/version.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:45:23.552417 nmk-python-0.9.0/src/nmk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-01-05 07:45:23.000000 nmk-python-0.9.0/src/nmk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-05 07:45:23.000000 nmk-python-0.9.0/src/nmk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 07:45:23.000000 nmk-python-0.9.0/src/nmk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-05 07:45:23.000000 nmk-python-0.9.0/src/nmk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-05 07:45:23.000000 nmk-python-0.9.0/src/nmk_python.egg-info/top_level.txt
```

### Comparing `nmk-python-0.8.3/LICENSE` & `nmk-python-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/PKG-INFO` & `nmk-python-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: nmk-python
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-python
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Description: # nmk-python
         Python plugin for nmk build system
         
+        <!-- NMK-BADGES-BEGIN -->
         [![License: MPL](https://img.shields.io/github/license/dynod/nmk-python)](https://github.com/dynod/nmk-python/blob/main/LICENSE)
-        [![Checks](https://img.shields.io/github/workflow/status/dynod/nmk-python/Build/main?label=build%20%26%20u.t.)](https://github.com/dynod/nmk-python/actions?query=branch%3Amain)
+        [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-python/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-python/actions?query=branch%3Amain)
         [![PyPI](https://img.shields.io/pypi/v/nmk-python)](https://pypi.org/project/nmk-python/)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+        <!-- NMK-BADGES-END -->
         
         This plugin adds support for Python development in an **`nmk`** project:
         * setup file generation
         * code format with [black](https://github.com/psf/black)
         * import sorting with [isort](https://github.com/PyCQA/isort)
         * code analysis with [flake8](https://flake8.pycqa.org/)
         * python wheel build
         * test with [pytest](https://pytest.org)
         * VSCode settings generation (if [**`nmk-vscode`**](https://github.com/dynod/nmk-vscode) plugin is also used)
+        * README badges generation (link to pypi.org + used tools; only if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used)
         
         ## Usage
         
         To use this plugin in your **`nmk`** project, insert this reference:
         ```
         refs:
             - pip://nmk-python!plugin.yml
```

### Comparing `nmk-python-0.8.3/README.md` & `nmk-python-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # nmk-python
 Python plugin for nmk build system
 
+<!-- NMK-BADGES-BEGIN -->
 [![License: MPL](https://img.shields.io/github/license/dynod/nmk-python)](https://github.com/dynod/nmk-python/blob/main/LICENSE)
-[![Checks](https://img.shields.io/github/workflow/status/dynod/nmk-python/Build/main?label=build%20%26%20u.t.)](https://github.com/dynod/nmk-python/actions?query=branch%3Amain)
+[![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-python/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-python/actions?query=branch%3Amain)
 [![PyPI](https://img.shields.io/pypi/v/nmk-python)](https://pypi.org/project/nmk-python/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+<!-- NMK-BADGES-END -->
 
 This plugin adds support for Python development in an **`nmk`** project:
 * setup file generation
 * code format with [black](https://github.com/psf/black)
 * import sorting with [isort](https://github.com/PyCQA/isort)
 * code analysis with [flake8](https://flake8.pycqa.org/)
 * python wheel build
 * test with [pytest](https://pytest.org)
 * VSCode settings generation (if [**`nmk-vscode`**](https://github.com/dynod/nmk-vscode) plugin is also used)
+* README badges generation (link to pypi.org + used tools; only if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used)
 
 ## Usage
 
 To use this plugin in your **`nmk`** project, insert this reference:
 ```
 refs:
     - pip://nmk-python!plugin.yml
```

### Comparing `nmk-python-0.8.3/setup.cfg` & `nmk-python-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ignore = E203,E501,B902,W503
 jobs = auto
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk-python
-version = 0.8.3
+version = 0.9.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `nmk-python-0.8.3/src/nmk_python/__init__.py` & `nmk-python-0.9.0/src/nmk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/build.py` & `nmk-python-0.9.0/src/nmk_python/build.py`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/build.yml` & `nmk-python-0.9.0/src/nmk_python/build.yml`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/files.py` & `nmk-python-0.9.0/src/nmk_python/files.py`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/files.yml` & `nmk-python-0.9.0/src/nmk_python/files.yml`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/flake.yml` & `nmk-python-0.9.0/src/nmk_python/flake.yml`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/format.py` & `nmk-python-0.9.0/src/nmk_python/format.py`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/format.yml` & `nmk-python-0.9.0/src/nmk_python/format.yml`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/plugin-defs.yml` & `nmk-python-0.9.0/src/nmk_python/plugin-defs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     - files.yml     # Look for python source files
     - version.yml   # Python version contribution
     - setup.yml     # Python setup files generation
     - format.yml    # Python code format (with black/isort)
     - flake.yml     # Python code analysis (with flake8)
     - build.yml     # Python module build/install
     - tests.yml     # Python automated tests
+    - badges.yml    # Python badges
 
 config:
     # Plugin version
     nmkPythonPluginVersion:
         __resolver__: nmk_python.NmkPythonVersionResolver
 
     # Plugin versions dict
```

### Comparing `nmk-python-0.8.3/src/nmk_python/setup.py` & `nmk-python-0.9.0/src/nmk_python/setup.py`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/setup.yml` & `nmk-python-0.9.0/src/nmk_python/setup.yml`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/templates/build.cfg` & `nmk-python-0.9.0/src/nmk_python/templates/build.cfg`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/templates/pytest.cfg` & `nmk-python-0.9.0/src/nmk_python/templates/pytest.cfg`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/templates/python-settings.json` & `nmk-python-0.9.0/src/nmk_python/templates/python-settings.json`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/tests.py` & `nmk-python-0.9.0/src/nmk_python/tests.py`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/tests.yml` & `nmk-python-0.9.0/src/nmk_python/tests.yml`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/version.py` & `nmk-python-0.9.0/src/nmk_python/version.py`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python/version.yml` & `nmk-python-0.9.0/src/nmk_python/version.yml`

 * *Files identical despite different names*

### Comparing `nmk-python-0.8.3/src/nmk_python.egg-info/PKG-INFO` & `nmk-python-0.9.0/src/nmk_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: nmk-python
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-python
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Description: # nmk-python
         Python plugin for nmk build system
         
+        <!-- NMK-BADGES-BEGIN -->
         [![License: MPL](https://img.shields.io/github/license/dynod/nmk-python)](https://github.com/dynod/nmk-python/blob/main/LICENSE)
-        [![Checks](https://img.shields.io/github/workflow/status/dynod/nmk-python/Build/main?label=build%20%26%20u.t.)](https://github.com/dynod/nmk-python/actions?query=branch%3Amain)
+        [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-python/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-python/actions?query=branch%3Amain)
         [![PyPI](https://img.shields.io/pypi/v/nmk-python)](https://pypi.org/project/nmk-python/)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+        <!-- NMK-BADGES-END -->
         
         This plugin adds support for Python development in an **`nmk`** project:
         * setup file generation
         * code format with [black](https://github.com/psf/black)
         * import sorting with [isort](https://github.com/PyCQA/isort)
         * code analysis with [flake8](https://flake8.pycqa.org/)
         * python wheel build
         * test with [pytest](https://pytest.org)
         * VSCode settings generation (if [**`nmk-vscode`**](https://github.com/dynod/nmk-vscode) plugin is also used)
+        * README badges generation (link to pypi.org + used tools; only if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used)
         
         ## Usage
         
         To use this plugin in your **`nmk`** project, insert this reference:
         ```
         refs:
             - pip://nmk-python!plugin.yml
```

### Comparing `nmk-python-0.8.3/src/nmk_python.egg-info/SOURCES.txt` & `nmk-python-0.9.0/src/nmk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/nmk_python/__init__.py
+src/nmk_python/badges.yml
 src/nmk_python/build.py
 src/nmk_python/build.yml
 src/nmk_python/files.py
 src/nmk_python/files.yml
 src/nmk_python/flake.py
 src/nmk_python/flake.yml
 src/nmk_python/format.py
```

