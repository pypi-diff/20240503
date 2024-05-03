# Comparing `tmp/nmk-doc-0.5.0.tar.gz` & `tmp/nmk_doc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-doc-0.5.0.tar", last modified: Thu Nov 23 08:09:44 2023, max compression
+gzip compressed data, was "nmk_doc-0.5.1.tar", last modified: Fri May  3 11:34:03 2024, max compression
```

## Comparing `nmk-doc-0.5.0.tar` & `nmk_doc-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:09:44.540390 nmk-doc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-11-23 08:09:44.540390 nmk-doc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-11-23 08:09:44.000000 nmk-doc-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-11-23 08:09:44.544390 nmk-doc-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-23 08:09:43.000000 nmk-doc-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:09:44.540390 nmk-doc-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:09:44.540390 nmk-doc-0.5.0/src/nmk_doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/badges.yml
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/path.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/plugin-defs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:09:44.540390 nmk-doc-0.5.0/src/nmk_doc/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/templates/config.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-11-23 08:09:13.000000 nmk-doc-0.5.0/src/nmk_doc/templates/readthedocs.yaml.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:09:44.540390 nmk-doc-0.5.0/src/nmk_doc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-11-23 08:09:44.000000 nmk-doc-0.5.0/src/nmk_doc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-11-23 08:09:44.000000 nmk-doc-0.5.0/src/nmk_doc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 08:09:44.000000 nmk-doc-0.5.0/src/nmk_doc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-23 08:09:44.000000 nmk-doc-0.5.0/src/nmk_doc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-23 08:09:44.000000 nmk-doc-0.5.0/src/nmk_doc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:34:03.737213 nmk_doc-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-03 11:34:03.737213 nmk_doc-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-03 11:34:01.000000 nmk_doc-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-03 11:34:03.737213 nmk_doc-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 11:34:00.000000 nmk_doc-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:34:03.733213 nmk_doc-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:34:03.737213 nmk_doc-0.5.1/src/nmk_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/badges.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:34:03.737213 nmk_doc-0.5.1/src/nmk_doc/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/templates/config.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-03 11:33:36.000000 nmk_doc-0.5.1/src/nmk_doc/templates/readthedocs.yaml.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:34:03.737213 nmk_doc-0.5.1/src/nmk_doc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-03 11:34:03.000000 nmk_doc-0.5.1/src/nmk_doc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 11:34:03.000000 nmk_doc-0.5.1/src/nmk_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:34:03.000000 nmk_doc-0.5.1/src/nmk_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 11:34:03.000000 nmk_doc-0.5.1/src/nmk_doc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 11:34:03.000000 nmk_doc-0.5.1/src/nmk_doc.egg-info/top_level.txt
```

### Comparing `nmk-doc-0.5.0/LICENSE` & `nmk_doc-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-doc-0.5.0/PKG-INFO` & `nmk_doc-0.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: nmk-doc
-Version: 0.5.0
+Version: 0.5.1
 Summary: Documentation handling plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-doc
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
-Description: # nmk-doc
-        Documentation handling plugin for nmk build system
-        
-        <!-- NMK-BADGES-BEGIN -->
-        [![License: MPL](https://img.shields.io/github/license/dynod/nmk-doc?color=green)](https://github.com/dynod/nmk-doc/blob/main/LICENSE)
-        [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-doc/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-doc/actions?query=branch%3Amain)
-        [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)
-        [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
-        [![PyPI](https://img.shields.io/pypi/v/nmk-doc)](https://pypi.org/project/nmk-doc/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
-        [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-doc)](https://app.codecov.io/gh/dynod/nmk-doc)
-        [![Documentation Status](https://readthedocs.org/projects/nmk-doc/badge/?version=stable)](https://nmk-doc.readthedocs.io/)
-        <!-- NMK-BADGES-END -->
-        
-        This plugin provide tasks to build documentation using the [Sphinx tool](https://www.sphinx-doc.org/).
-        
-        ## Usage
-        
-        To use this plugin in your **`nmk`** project, insert this reference:
-        ```yaml
-        refs:
-            - pip://nmk-doc!plugin.yml
-        ```
-        
-        ## Documentation
-        
-        This plugin documentation is available [here](https://nmk-doc.readthedocs.io/)
-        
-        ## Issues
-        
-        Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:doc** label.
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
+# nmk-doc
+Documentation handling plugin for nmk build system
+
+<!-- NMK-BADGES-BEGIN -->
+[![License: MPL](https://img.shields.io/github/license/dynod/nmk-doc?color=green)](https://github.com/dynod/nmk-doc/blob/main/LICENSE)
+[![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-doc/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-doc/actions?query=branch%3Amain)
+[![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)
+[![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
+[![PyPI](https://img.shields.io/pypi/v/nmk-doc)](https://pypi.org/project/nmk-doc/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+[![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-doc)](https://app.codecov.io/gh/dynod/nmk-doc)
+[![Documentation Status](https://readthedocs.org/projects/nmk-doc/badge/?version=stable)](https://nmk-doc.readthedocs.io/)
+<!-- NMK-BADGES-END -->
+
+This plugin provide tasks to build documentation using the [Sphinx tool](https://www.sphinx-doc.org/).
+
+## Usage
+
+To use this plugin in your **`nmk`** project, insert this reference:
+```yaml
+refs:
+    - pip://nmk-doc!plugin.yml
+```
+
+## Documentation
+
+This plugin documentation is available [here](https://nmk-doc.readthedocs.io/)
+
+## Issues
+
+Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:doc** label.
```

### Comparing `nmk-doc-0.5.0/README.md` & `nmk_doc-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nmk-doc-0.5.0/setup.cfg` & `nmk_doc-0.5.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk-doc
 author = The dynod project
 maintainer = The dynod project
-version = 0.5.0
+version = 0.5.1
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `nmk-doc-0.5.0/src/nmk_doc/__init__.py` & `nmk_doc-0.5.1/src/nmk_doc/__init__.py`

 * *Files identical despite different names*

### Comparing `nmk-doc-0.5.0/src/nmk_doc/builders.py` & `nmk_doc-0.5.1/src/nmk_doc/builders.py`

 * *Files identical despite different names*

### Comparing `nmk-doc-0.5.0/src/nmk_doc/doc.yml` & `nmk_doc-0.5.1/src/nmk_doc/doc.yml`

 * *Files identical despite different names*

### Comparing `nmk-doc-0.5.0/src/nmk_doc/plugin-defs.yml` & `nmk_doc-0.5.1/src/nmk_doc/plugin.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Doc plugin definition
 refs:
-    - path.yml  # Python path contrib
+    - pip://nmk-base!plugin.yml
     - doc.yml   # Doc generation handling
     - badges.yml  # Badges generation logic
 
 # Extra config
 config:
 
     # Plugin version
```

### Comparing `nmk-doc-0.5.0/src/nmk_doc/resolvers.py` & `nmk_doc-0.5.1/src/nmk_doc/resolvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module containing all config item resolvers for **nmk-doc** plugin.
 """
+
 from datetime import date
 
 from nmk.model.resolver import NmkIntConfigResolver
 from nmk_base.resolvers import FilesResolver
 
 
 class NmkDocInputsResolver(FilesResolver):
```

### Comparing `nmk-doc-0.5.0/src/nmk_doc/templates/config.py.jinja` & `nmk_doc-0.5.1/src/nmk_doc/templates/config.py.jinja`

 * *Files identical despite different names*

### Comparing `nmk-doc-0.5.0/src/nmk_doc/templates/readthedocs.yaml.jinja` & `nmk_doc-0.5.1/src/nmk_doc/templates/readthedocs.yaml.jinja`

 * *Files identical despite different names*

### Comparing `nmk-doc-0.5.0/src/nmk_doc.egg-info/PKG-INFO` & `nmk_doc-0.5.1/src/nmk_doc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: nmk-doc
-Version: 0.5.0
+Version: 0.5.1
 Summary: Documentation handling plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-doc
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
-Description: # nmk-doc
-        Documentation handling plugin for nmk build system
-        
-        <!-- NMK-BADGES-BEGIN -->
-        [![License: MPL](https://img.shields.io/github/license/dynod/nmk-doc?color=green)](https://github.com/dynod/nmk-doc/blob/main/LICENSE)
-        [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-doc/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-doc/actions?query=branch%3Amain)
-        [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)
-        [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
-        [![PyPI](https://img.shields.io/pypi/v/nmk-doc)](https://pypi.org/project/nmk-doc/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
-        [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-doc)](https://app.codecov.io/gh/dynod/nmk-doc)
-        [![Documentation Status](https://readthedocs.org/projects/nmk-doc/badge/?version=stable)](https://nmk-doc.readthedocs.io/)
-        <!-- NMK-BADGES-END -->
-        
-        This plugin provide tasks to build documentation using the [Sphinx tool](https://www.sphinx-doc.org/).
-        
-        ## Usage
-        
-        To use this plugin in your **`nmk`** project, insert this reference:
-        ```yaml
-        refs:
-            - pip://nmk-doc!plugin.yml
-        ```
-        
-        ## Documentation
-        
-        This plugin documentation is available [here](https://nmk-doc.readthedocs.io/)
-        
-        ## Issues
-        
-        Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:doc** label.
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
+# nmk-doc
+Documentation handling plugin for nmk build system
+
+<!-- NMK-BADGES-BEGIN -->
+[![License: MPL](https://img.shields.io/github/license/dynod/nmk-doc?color=green)](https://github.com/dynod/nmk-doc/blob/main/LICENSE)
+[![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-doc/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-doc/actions?query=branch%3Amain)
+[![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Adoc)
+[![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
+[![PyPI](https://img.shields.io/pypi/v/nmk-doc)](https://pypi.org/project/nmk-doc/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+[![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-doc)](https://app.codecov.io/gh/dynod/nmk-doc)
+[![Documentation Status](https://readthedocs.org/projects/nmk-doc/badge/?version=stable)](https://nmk-doc.readthedocs.io/)
+<!-- NMK-BADGES-END -->
+
+This plugin provide tasks to build documentation using the [Sphinx tool](https://www.sphinx-doc.org/).
+
+## Usage
+
+To use this plugin in your **`nmk`** project, insert this reference:
+```yaml
+refs:
+    - pip://nmk-doc!plugin.yml
+```
+
+## Documentation
+
+This plugin documentation is available [here](https://nmk-doc.readthedocs.io/)
+
+## Issues
+
+Issues for this plugin shall be reported on the [main  **`nmk`** project](https://github.com/dynod/nmk/issues), using the **plugin:doc** label.
```

