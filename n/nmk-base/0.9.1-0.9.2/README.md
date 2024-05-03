# Comparing `tmp/nmk-base-0.9.1.tar.gz` & `tmp/nmk-base-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-base-0.9.1.tar", last modified: Fri Jan  6 17:39:37 2023, max compression
+gzip compressed data, was "nmk-base-0.9.2.tar", last modified: Sun Jan 15 15:14:58 2023, max compression
```

## Comparing `nmk-base-0.9.1.tar` & `nmk-base-0.9.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:39:37.887275 nmk-base-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-06 17:39:18.000000 nmk-base-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-01-06 17:39:37.887275 nmk-base-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-06 17:39:36.000000 nmk-base-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-01-06 17:39:37.887275 nmk-base-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-06 17:39:36.000000 nmk-base-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:39:37.883275 nmk-base-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:39:37.887275 nmk-base-0.9.1/src/nmk_base/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/git.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/helpers.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/loadme.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/loadme.yml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/output.yml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/tasks.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:39:37.887275 nmk-base-0.9.1/src/nmk_base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/templates/gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/templates/loadme.sh
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/templates/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/venv.yml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-06 17:39:18.000000 nmk-base-0.9.1/src/nmk_base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:39:37.887275 nmk-base-0.9.1/src/nmk_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-01-06 17:39:37.000000 nmk-base-0.9.1/src/nmk_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-06 17:39:37.000000 nmk-base-0.9.1/src/nmk_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 17:39:37.000000 nmk-base-0.9.1/src/nmk_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-06 17:39:37.000000 nmk-base-0.9.1/src/nmk_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-06 17:39:37.000000 nmk-base-0.9.1/src/nmk_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 15:14:58.839691 nmk-base-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-15 15:14:38.000000 nmk-base-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-01-15 15:14:58.839691 nmk-base-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-01-15 15:14:57.000000 nmk-base-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-15 15:14:58.839691 nmk-base-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-15 15:14:57.000000 nmk-base-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 15:14:58.835691 nmk-base-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 15:14:58.839691 nmk-base-0.9.2/src/nmk_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/git.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/helpers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/loadme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/loadme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/output.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/tasks.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 15:14:58.839691 nmk-base-0.9.2/src/nmk_base/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/templates/gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/templates/loadme.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/templates/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/venv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-15 15:14:38.000000 nmk-base-0.9.2/src/nmk_base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 15:14:58.839691 nmk-base-0.9.2/src/nmk_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-01-15 15:14:58.000000 nmk-base-0.9.2/src/nmk_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-15 15:14:58.000000 nmk-base-0.9.2/src/nmk_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 15:14:58.000000 nmk-base-0.9.2/src/nmk_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-15 15:14:58.000000 nmk-base-0.9.2/src/nmk_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-15 15:14:58.000000 nmk-base-0.9.2/src/nmk_base.egg-info/top_level.txt
```

### Comparing `nmk-base-0.9.1/LICENSE` & `nmk-base-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/PKG-INFO` & `nmk-base-0.9.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-Metadata-Version: 2.1
-Name: nmk-base
-Version: 0.9.1
-Summary: Base plugin for nmk build system
-Home-page: https://github.com/dynod/nmk-base
-Author: The dynod project
-Maintainer: The dynod project
-License: Mozilla Public License Version 2.0
-Description: # nmk-base
-        Base plugin for nmk build system
-        
-        <!-- NMK-BADGES-BEGIN -->
-        [![License: MPL](https://img.shields.io/github/license/dynod/nmk-base)](https://github.com/dynod/nmk-base/blob/main/LICENSE)
-        [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-base/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-base/actions?query=branch%3Amain)
-        [![PyPI](https://img.shields.io/pypi/v/nmk-base)](https://pypi.org/project/nmk-base/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        <!-- NMK-BADGES-END -->
-        
-        ## Usage
-        
-        To use this plugin in your **`nmk`** project, insert this reference:
-        ```
-        refs:
-            - pip://nmk-base!plugin.yml
-        ```
-        
-        ## Documentation
-        
-        This plugin documentation is available [here](https://github.com/dynod/nmk/wiki/nmk-base-plugin)
-        
-        ## Issues
-        
-        Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:base** label.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
+# nmk-base
+Base plugin for nmk build system
+
+<!-- NMK-BADGES-BEGIN -->
+[![License: MPL](https://img.shields.io/github/license/dynod/nmk-base)](https://github.com/dynod/nmk-base/blob/main/LICENSE)
+[![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-base/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-base/actions?query=branch%3Amain)
+[![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Abase)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Abase)
+[![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
+[![PyPI](https://img.shields.io/pypi/v/nmk-base)](https://pypi.org/project/nmk-base/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+[![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-base)](https://app.codecov.io/gh/dynod/nmk-base)
+<!-- NMK-BADGES-END -->
+
+This plugin provides base features for **`nmk`** build, which by design don't need to be part of the **`nmk`** core implementation.
+
+## Usage
+
+To use this plugin in your **`nmk`** project, insert this reference:
+```
+refs:
+    - pip://nmk-base!plugin.yml
+```
+
+## Documentation
+
+This plugin documentation is available [here](https://github.com/dynod/nmk/wiki/nmk-base-plugin)
+
+## Issues
+
+Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:base** label.
```

### Comparing `nmk-base-0.9.1/setup.cfg` & `nmk-base-0.9.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 ignore = E203,E501,B902,W503
 jobs = auto
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk-base
-version = 0.9.1
+version = 0.9.2
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 author = The dynod project
 maintainer = The dynod project
 url = https://github.com/dynod/nmk-base
 description = Base plugin for nmk build system
 
 [options]
 package_dir = =src
```

### Comparing `nmk-base-0.9.1/src/nmk_base/__init__.py` & `nmk-base-0.9.2/src/nmk_base/__init__.py`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/common.py` & `nmk-base-0.9.2/src/nmk_base/common.py`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/git.py` & `nmk-base-0.9.2/src/nmk_base/git.py`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/git.yml` & `nmk-base-0.9.2/src/nmk_base/git.yml`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/helpers.py` & `nmk-base-0.9.2/src/nmk_base/helpers.py`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/helpers.yml` & `nmk-base-0.9.2/src/nmk_base/helpers.yml`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/loadme.py` & `nmk-base-0.9.2/src/nmk_base/loadme.py`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/loadme.yml` & `nmk-base-0.9.2/src/nmk_base/loadme.yml`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/output.py` & `nmk-base-0.9.2/src/nmk_base/output.py`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/output.yml` & `nmk-base-0.9.2/src/nmk_base/output.yml`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/tasks.yml` & `nmk-base-0.9.2/src/nmk_base/tasks.yml`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/templates/loadme.sh` & `nmk-base-0.9.2/src/nmk_base/templates/loadme.sh`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/venv.py` & `nmk-base-0.9.2/src/nmk_base/venv.py`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base/venv.yml` & `nmk-base-0.9.2/src/nmk_base/venv.yml`

 * *Files identical despite different names*

### Comparing `nmk-base-0.9.1/src/nmk_base.egg-info/PKG-INFO` & `nmk-base-0.9.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: nmk-base
-Version: 0.9.1
+Version: 0.9.2
 Summary: Base plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-base
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Description: # nmk-base
         Base plugin for nmk build system
         
         <!-- NMK-BADGES-BEGIN -->
         [![License: MPL](https://img.shields.io/github/license/dynod/nmk-base)](https://github.com/dynod/nmk-base/blob/main/LICENSE)
         [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-base/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-base/actions?query=branch%3Amain)
+        [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Abase)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Abase)
+        [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
         [![PyPI](https://img.shields.io/pypi/v/nmk-base)](https://pypi.org/project/nmk-base/)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+        [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+        [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-base)](https://app.codecov.io/gh/dynod/nmk-base)
         <!-- NMK-BADGES-END -->
         
+        This plugin provides base features for **`nmk`** build, which by design don't need to be part of the **`nmk`** core implementation.
+        
         ## Usage
         
         To use this plugin in your **`nmk`** project, insert this reference:
         ```
         refs:
             - pip://nmk-base!plugin.yml
         ```
@@ -32,8 +38,9 @@
         
         Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:base** label.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `nmk-base-0.9.1/src/nmk_base.egg-info/SOURCES.txt` & `nmk-base-0.9.2/src/nmk_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

