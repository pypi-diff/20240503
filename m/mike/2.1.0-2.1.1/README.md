# Comparing `tmp/mike-2.1.0.tar.gz` & `tmp/mike-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mike-2.1.0.tar", last modified: Thu May  2 00:49:36 2024, max compression
+gzip compressed data, was "mike-2.1.1.tar", last modified: Fri May  3 19:04:58 2024, max compression
```

## Comparing `mike-2.1.0.tar` & `mike-2.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/
--rw-rw-r--   0 jim       (1000) jim       (1000)     6994 2024-05-02 00:47:02.000000 mike-2.1.0/CHANGES.md
--rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2023-03-02 23:32:07.000000 mike-2.1.0/LICENSE
--rw-rw-r--   0 jim       (1000) jim       (1000)       97 2021-03-01 03:43:15.000000 mike-2.1.0/MANIFEST.in
--rw-rw-r--   0 jim       (1000) jim       (1000)    20375 2024-05-02 00:49:36.269359 mike-2.1.0/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)    16331 2024-02-29 18:47:52.000000 mike-2.1.0/README.md
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.249349 mike-2.1.0/mike/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)       18 2024-05-02 00:49:26.000000 mike-2.1.0/mike/app_version.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1239 2023-11-02 00:12:32.000000 mike-2.1.0/mike/arguments.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    11924 2024-02-29 18:47:52.000000 mike-2.1.0/mike/commands.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    19178 2024-03-01 00:08:45.000000 mike-2.1.0/mike/driver.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    13389 2023-03-13 21:45:58.000000 mike-2.1.0/mike/git_utils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4278 2023-11-02 04:41:55.000000 mike-2.1.0/mike/jsonpath.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2716 2023-07-05 17:42:05.000000 mike-2.1.0/mike/mkdocs_plugin.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3199 2024-04-05 00:45:27.000000 mike-2.1.0/mike/mkdocs_utils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2367 2023-03-02 23:32:07.000000 mike-2.1.0/mike/server.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/templates/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/templates/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      378 2023-03-02 23:32:07.000000 mike-2.1.0/mike/templates/redirect.html
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/mkdocs/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/mkdocs/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/mkdocs/css/
--rw-rw-r--   0 jim       (1000) jim       (1000)      376 2020-02-24 00:26:03.000000 mike-2.1.0/mike/themes/mkdocs/css/version-select.css
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/mkdocs/js/
--rw-rw-r--   0 jim       (1000) jim       (1000)     2475 2023-11-02 00:12:32.000000 mike-2.1.0/mike/themes/mkdocs/js/version-select.js
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/mike/themes/readthedocs/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/readthedocs/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/mike/themes/readthedocs/css/
--rw-rw-r--   0 jim       (1000) jim       (1000)       86 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/readthedocs/css/version-select.css
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/mike/themes/readthedocs/js/
--rw-rw-r--   0 jim       (1000) jim       (1000)     2178 2023-11-02 00:12:32.000000 mike-2.1.0/mike/themes/readthedocs/js/version-select.js
--rw-rw-r--   0 jim       (1000) jim       (1000)     6729 2023-11-02 04:35:40.000000 mike-2.1.0/mike/versions.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike.egg-info/
--rw-rw-r--   0 jim       (1000) jim       (1000)    20375 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)      774 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/SOURCES.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        1 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/dependency_links.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)     1341 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/entry_points.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        1 2017-12-04 03:12:13.000000 mike-2.1.0/mike.egg-info/not-zip-safe
--rw-rw-r--   0 jim       (1000) jim       (1000)      195 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/requires.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        5 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/top_level.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)      423 2024-05-02 00:49:36.269359 mike-2.1.0/setup.cfg
--rw-rw-r--   0 jim       (1000) jim       (1000)     5159 2023-11-02 00:12:32.000000 mike-2.1.0/setup.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7143 2024-05-03 19:03:47.000000 mike-2.1.1/CHANGES.md
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2023-03-02 23:32:07.000000 mike-2.1.1/LICENSE
+-rw-rw-r--   0 jim       (1000) jim       (1000)       97 2021-03-01 03:43:15.000000 mike-2.1.1/MANIFEST.in
+-rw-rw-r--   0 jim       (1000) jim       (1000)    20375 2024-05-03 19:04:58.240369 mike-2.1.1/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)    16331 2024-02-29 18:47:52.000000 mike-2.1.1/README.md
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.236367 mike-2.1.1/mike/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.1/mike/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)       18 2024-05-03 19:03:59.000000 mike-2.1.1/mike/app_version.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1239 2023-11-02 00:12:32.000000 mike-2.1.1/mike/arguments.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    11924 2024-02-29 18:47:52.000000 mike-2.1.1/mike/commands.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    19178 2024-03-01 00:08:45.000000 mike-2.1.1/mike/driver.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    13389 2023-03-13 21:45:58.000000 mike-2.1.1/mike/git_utils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4278 2023-11-02 04:41:55.000000 mike-2.1.1/mike/jsonpath.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2716 2023-07-05 17:42:05.000000 mike-2.1.1/mike/mkdocs_plugin.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3549 2024-05-03 19:03:34.000000 mike-2.1.1/mike/mkdocs_utils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2367 2023-03-02 23:32:07.000000 mike-2.1.1/mike/server.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/templates/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.1/mike/templates/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      378 2023-03-02 23:32:07.000000 mike-2.1.1/mike/templates/redirect.html
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/themes/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.1/mike/themes/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/themes/mkdocs/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.1/mike/themes/mkdocs/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/themes/mkdocs/css/
+-rw-rw-r--   0 jim       (1000) jim       (1000)      376 2020-02-24 00:26:03.000000 mike-2.1.1/mike/themes/mkdocs/css/version-select.css
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/themes/mkdocs/js/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2475 2023-11-02 00:12:32.000000 mike-2.1.1/mike/themes/mkdocs/js/version-select.js
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/themes/readthedocs/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.1/mike/themes/readthedocs/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/themes/readthedocs/css/
+-rw-rw-r--   0 jim       (1000) jim       (1000)       86 2017-12-04 03:10:10.000000 mike-2.1.1/mike/themes/readthedocs/css/version-select.css
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike/themes/readthedocs/js/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2178 2023-11-02 00:12:32.000000 mike-2.1.1/mike/themes/readthedocs/js/version-select.js
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6729 2023-11-02 04:35:40.000000 mike-2.1.1/mike/versions.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-03 19:04:58.240369 mike-2.1.1/mike.egg-info/
+-rw-rw-r--   0 jim       (1000) jim       (1000)    20375 2024-05-03 19:04:57.000000 mike-2.1.1/mike.egg-info/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)      774 2024-05-03 19:04:57.000000 mike-2.1.1/mike.egg-info/SOURCES.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        1 2024-05-03 19:04:57.000000 mike-2.1.1/mike.egg-info/dependency_links.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1341 2024-05-03 19:04:57.000000 mike-2.1.1/mike.egg-info/entry_points.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        1 2017-12-04 03:12:13.000000 mike-2.1.1/mike.egg-info/not-zip-safe
+-rw-rw-r--   0 jim       (1000) jim       (1000)      210 2024-05-03 19:04:57.000000 mike-2.1.1/mike.egg-info/requires.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        5 2024-05-03 19:04:57.000000 mike-2.1.1/mike.egg-info/top_level.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)      423 2024-05-03 19:04:58.240369 mike-2.1.1/setup.cfg
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5177 2024-05-03 19:03:34.000000 mike-2.1.1/setup.py
```

### Comparing `mike-2.1.0/CHANGES.md` & `mike-2.1.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changes
 
+## v2.1.1 (2024-05-03)
+
+### Bug fixes
+- Support using environment variables for `INHERIT` when injecting the `mike`
+  plugin into `mkdocs.yml`
+
+---
+
 ## v2.1.0 (2024-05-01)
 
 ### New features
 - When calling `set-default`, you can now pass `--allow-undefined` to set the
   default to a version that doesn't exist yet
 - Add global-level `-q` / `--quiet` option to suppress warning messages
 - Add support for handling `!relative` in `mkdocs.yml`
```

### Comparing `mike-2.1.0/LICENSE` & `mike-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/PKG-INFO` & `mike-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mike
-Version: 2.1.0
+Version: 2.1.1
 Summary: Manage multiple versions of your MkDocs-powered documentation
 Home-page: https://github.com/jimporter/mike
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
 License: BSD-3-Clause
 Description: # mike
         **mike** is a Python utility that makes it easy to deploy multiple versions of
```

### Comparing `mike-2.1.0/README.md` & `mike-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/arguments.py` & `mike-2.1.1/mike/arguments.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/commands.py` & `mike-2.1.1/mike/commands.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/driver.py` & `mike-2.1.1/mike/driver.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/git_utils.py` & `mike-2.1.1/mike/git_utils.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/jsonpath.py` & `mike-2.1.1/mike/jsonpath.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/mkdocs_plugin.py` & `mike-2.1.1/mike/mkdocs_plugin.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/mkdocs_utils.py` & `mike-2.1.1/mike/mkdocs_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import mkdocs.config
 import mkdocs.plugins
 import mkdocs.utils
 import os
 import re
 import subprocess
 import yaml
+import yaml_env_tag
 from collections.abc import Iterable, Mapping
 from contextlib import contextmanager
 from tempfile import NamedTemporaryFile
 
 docs_version_var = 'MIKE_DOCS_VERSION'
 
 
@@ -28,14 +29,20 @@
         return data.node
 
 
 class RoundTripLoader(yaml.Loader):
     pass
 
 
+# We need to expand environment variables in our round trip loader (making it
+# less of a "round trip"), or else `INHERIT: !ENV ...` will fail when injecting
+# the mike plugin. MkDocs really doesn't make this easy on us...
+yaml.add_constructor('!ENV', yaml_env_tag.construct_env_tag,
+                     Loader=RoundTripLoader)
+
 yaml.add_multi_constructor('!', RoundTrippableTag.constructor,
                            Loader=RoundTripLoader)
 yaml.add_multi_representer(RoundTrippableTag, RoundTrippableTag.representer)
 
 
 def _open_config(config_file=None):
     if config_file is None:
```

### Comparing `mike-2.1.0/mike/server.py` & `mike-2.1.1/mike/server.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/themes/mkdocs/js/version-select.js` & `mike-2.1.1/mike/themes/mkdocs/js/version-select.js`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/themes/readthedocs/js/version-select.js` & `mike-2.1.1/mike/themes/readthedocs/js/version-select.js`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike/versions.py` & `mike-2.1.1/mike/versions.py`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike.egg-info/PKG-INFO` & `mike-2.1.1/mike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mike
-Version: 2.1.0
+Version: 2.1.1
 Summary: Manage multiple versions of your MkDocs-powered documentation
 Home-page: https://github.com/jimporter/mike
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
 License: BSD-3-Clause
 Description: # mike
         **mike** is a Python utility that makes it easy to deploy multiple versions of
```

### Comparing `mike-2.1.0/mike.egg-info/SOURCES.txt` & `mike-2.1.1/mike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/mike.egg-info/entry_points.txt` & `mike-2.1.1/mike.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mike-2.1.0/setup.py` & `mike-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     ],
 
     packages=find_packages(exclude=['test', 'test.*']),
     include_package_data=True,
 
     install_requires=(['importlib_metadata', 'importlib_resources',
                        'jinja2 >= 2.7', 'mkdocs >= 1.0', 'pyparsing >= 3.0',
-                       'pyyaml >= 5.1', 'verspec']),
+                       'pyyaml >= 5.1', 'pyyaml_env_tag', 'verspec']),
     extras_require={
         'dev': ['coverage', 'flake8 >= 3.0', 'flake8-quotes', 'shtab'],
         'test': ['coverage', 'flake8 >= 3.0', 'flake8-quotes', 'shtab'],
     },
 
     entry_points={
         'console_scripts': [
```

