# Comparing `tmp/nmk-badges-0.2.3.tar.gz` & `tmp/nmk_badges-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-badges-0.2.3.tar", last modified: Sat Nov  4 14:42:50 2023, max compression
+gzip compressed data, was "nmk_badges-0.2.4.tar", last modified: Fri May  3 10:41:45 2024, max compression
```

## Comparing `nmk-badges-0.2.3.tar` & `nmk_badges-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 14:42:50.655965 nmk-badges-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-04 14:42:16.000000 nmk-badges-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2023-11-04 14:42:50.655965 nmk-badges-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-11-04 14:42:50.000000 nmk-badges-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-11-04 14:42:50.659965 nmk-badges-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-04 14:42:49.000000 nmk-badges-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 14:42:50.655965 nmk-badges-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 14:42:50.655965 nmk-badges-0.2.3/src/nmk_badges/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-11-04 14:42:16.000000 nmk-badges-0.2.3/src/nmk_badges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-11-04 14:42:16.000000 nmk-badges-0.2.3/src/nmk_badges/badges.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-11-04 14:42:16.000000 nmk-badges-0.2.3/src/nmk_badges/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-04 14:42:16.000000 nmk-badges-0.2.3/src/nmk_badges/path.yml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-04 14:42:16.000000 nmk-badges-0.2.3/src/nmk_badges/plugin-defs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-04 14:42:16.000000 nmk-badges-0.2.3/src/nmk_badges/plugin.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 14:42:50.655965 nmk-badges-0.2.3/src/nmk_badges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2023-11-04 14:42:50.000000 nmk-badges-0.2.3/src/nmk_badges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-11-04 14:42:50.000000 nmk-badges-0.2.3/src/nmk_badges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-04 14:42:50.000000 nmk-badges-0.2.3/src/nmk_badges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-04 14:42:50.000000 nmk-badges-0.2.3/src/nmk_badges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-04 14:42:50.000000 nmk-badges-0.2.3/src/nmk_badges.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:41:45.908218 nmk_badges-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-03 10:41:17.000000 nmk_badges-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-03 10:41:45.908218 nmk_badges-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-03 10:41:43.000000 nmk_badges-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-03 10:41:45.908218 nmk_badges-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 10:41:43.000000 nmk_badges-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:41:45.908218 nmk_badges-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:41:45.908218 nmk_badges-0.2.4/src/nmk_badges/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 10:41:17.000000 nmk_badges-0.2.4/src/nmk_badges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-03 10:41:17.000000 nmk_badges-0.2.4/src/nmk_badges/badges.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-03 10:41:17.000000 nmk_badges-0.2.4/src/nmk_badges/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-03 10:41:17.000000 nmk_badges-0.2.4/src/nmk_badges/plugin.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:41:45.908218 nmk_badges-0.2.4/src/nmk_badges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-03 10:41:45.000000 nmk_badges-0.2.4/src/nmk_badges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 10:41:45.000000 nmk_badges-0.2.4/src/nmk_badges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:41:45.000000 nmk_badges-0.2.4/src/nmk_badges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 10:41:45.000000 nmk_badges-0.2.4/src/nmk_badges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 10:41:45.000000 nmk_badges-0.2.4/src/nmk_badges.egg-info/top_level.txt
```

### Comparing `nmk-badges-0.2.3/LICENSE` & `nmk_badges-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-badges-0.2.3/PKG-INFO` & `nmk_badges-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: nmk-badges
-Version: 0.2.3
+Version: 0.2.4
 Summary: Readme badges generation plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-badges
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
-Description: # nmk-badges
-        Readme badges generation plugin for nmk build system
-        
-        <!-- NMK-BADGES-BEGIN -->
-        [![License: MPL](https://img.shields.io/github/license/dynod/nmk-badges?color=green)](https://github.com/dynod/nmk-badges/blob/main/LICENSE)
-        [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-badges/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-badges/actions?query=branch%3Amain)
-        [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)
-        [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
-        [![PyPI](https://img.shields.io/pypi/v/nmk-badges)](https://pypi.org/project/nmk-badges/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
-        [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-badges)](https://app.codecov.io/gh/dynod/nmk-badges)
-        [![Documentation Status](https://readthedocs.org/projects/nmk-badges/badge/?version=stable)](https://nmk-badges.readthedocs.io/)
-        <!-- NMK-BADGES-END -->
-        
-        This plugin adds support for README markdown [badges/shields](https://shields.io/) generation.
-        
-        ## Usage
-        
-        To use this plugin in your **`nmk`** project, insert this reference:
-        ```yaml
-        refs:
-            - pip://nmk-badges!plugin.yml
-        ```
-        
-        ## Documentation
-        
-        This plugin documentation is available [here](https://nmk-badges.readthedocs.io/)
-        
-        ## Issues
-        
-        Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:badges** label.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: nmk-base
+
+# nmk-badges
+Readme badges generation plugin for nmk build system
+
+<!-- NMK-BADGES-BEGIN -->
+[![License: MPL](https://img.shields.io/github/license/dynod/nmk-badges?color=green)](https://github.com/dynod/nmk-badges/blob/main/LICENSE)
+[![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-badges/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-badges/actions?query=branch%3Amain)
+[![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)
+[![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
+[![PyPI](https://img.shields.io/pypi/v/nmk-badges)](https://pypi.org/project/nmk-badges/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+[![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-badges)](https://app.codecov.io/gh/dynod/nmk-badges)
+[![Documentation Status](https://readthedocs.org/projects/nmk-badges/badge/?version=stable)](https://nmk-badges.readthedocs.io/)
+<!-- NMK-BADGES-END -->
+
+This plugin adds support for README markdown [badges/shields](https://shields.io/) generation.
+
+## Usage
+
+To use this plugin in your **`nmk`** project, insert this reference:
+```yaml
+refs:
+    - pip://nmk-badges!plugin.yml
+```
+
+## Documentation
+
+This plugin documentation is available [here](https://nmk-badges.readthedocs.io/)
+
+## Issues
+
+Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:badges** label.
```

### Comparing `nmk-badges-0.2.3/README.md` & `nmk_badges-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nmk-badges-0.2.3/setup.cfg` & `nmk_badges-0.2.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk-badges
 author = The dynod project
 maintainer = The dynod project
-version = 0.2.3
+version = 0.2.4
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `nmk-badges-0.2.3/src/nmk_badges/__init__.py` & `nmk_badges-0.2.4/src/nmk_badges/__init__.py`

 * *Files identical despite different names*

### Comparing `nmk-badges-0.2.3/src/nmk_badges/badges.yml` & `nmk_badges-0.2.4/src/nmk_badges/badges.yml`

 * *Files identical despite different names*

### Comparing `nmk-badges-0.2.3/src/nmk_badges/builder.py` & `nmk_badges-0.2.4/src/nmk_badges/builder.py`

 * *Files identical despite different names*

### Comparing `nmk-badges-0.2.3/src/nmk_badges.egg-info/PKG-INFO` & `nmk_badges-0.2.4/src/nmk_badges.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: nmk-badges
-Version: 0.2.3
+Version: 0.2.4
 Summary: Readme badges generation plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-badges
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
-Description: # nmk-badges
-        Readme badges generation plugin for nmk build system
-        
-        <!-- NMK-BADGES-BEGIN -->
-        [![License: MPL](https://img.shields.io/github/license/dynod/nmk-badges?color=green)](https://github.com/dynod/nmk-badges/blob/main/LICENSE)
-        [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-badges/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-badges/actions?query=branch%3Amain)
-        [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)
-        [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
-        [![PyPI](https://img.shields.io/pypi/v/nmk-badges)](https://pypi.org/project/nmk-badges/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
-        [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-badges)](https://app.codecov.io/gh/dynod/nmk-badges)
-        [![Documentation Status](https://readthedocs.org/projects/nmk-badges/badge/?version=stable)](https://nmk-badges.readthedocs.io/)
-        <!-- NMK-BADGES-END -->
-        
-        This plugin adds support for README markdown [badges/shields](https://shields.io/) generation.
-        
-        ## Usage
-        
-        To use this plugin in your **`nmk`** project, insert this reference:
-        ```yaml
-        refs:
-            - pip://nmk-badges!plugin.yml
-        ```
-        
-        ## Documentation
-        
-        This plugin documentation is available [here](https://nmk-badges.readthedocs.io/)
-        
-        ## Issues
-        
-        Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:badges** label.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: nmk-base
+
+# nmk-badges
+Readme badges generation plugin for nmk build system
+
+<!-- NMK-BADGES-BEGIN -->
+[![License: MPL](https://img.shields.io/github/license/dynod/nmk-badges?color=green)](https://github.com/dynod/nmk-badges/blob/main/LICENSE)
+[![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-badges/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-badges/actions?query=branch%3Amain)
+[![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Abadges)
+[![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
+[![PyPI](https://img.shields.io/pypi/v/nmk-badges)](https://pypi.org/project/nmk-badges/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+[![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-badges)](https://app.codecov.io/gh/dynod/nmk-badges)
+[![Documentation Status](https://readthedocs.org/projects/nmk-badges/badge/?version=stable)](https://nmk-badges.readthedocs.io/)
+<!-- NMK-BADGES-END -->
+
+This plugin adds support for README markdown [badges/shields](https://shields.io/) generation.
+
+## Usage
+
+To use this plugin in your **`nmk`** project, insert this reference:
+```yaml
+refs:
+    - pip://nmk-badges!plugin.yml
+```
+
+## Documentation
+
+This plugin documentation is available [here](https://nmk-badges.readthedocs.io/)
+
+## Issues
+
+Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:badges** label.
```

