# Comparing `tmp/sag-py-logging-logstash-2.3.8.tar.gz` & `tmp/sag_py_logging_logstash-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-logging-logstash-2.3.8.tar", last modified: Tue Feb  6 14:00:37 2024, max compression
+gzip compressed data, was "sag_py_logging_logstash-2.3.9.tar", last modified: Fri May  3 07:57:49 2024, max compression
```

## Comparing `sag-py-logging-logstash-2.3.8.tar` & `sag_py_logging_logstash-2.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:00:37.297373 sag-py-logging-logstash-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-02-06 14:00:37.297373 sag-py-logging-logstash-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:00:37.297373 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/memory_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:00:37.297373 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-02-06 14:00:37.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-06 14:00:37.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 14:00:37.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-06 14:00:37.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-06 14:00:37.000000 sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-06 14:00:37.301373 sag-py-logging-logstash-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-06 14:00:30.000000 sag-py-logging-logstash-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:57:49.554679 sag_py_logging_logstash-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-03 07:57:49.554679 sag_py_logging_logstash-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:57:49.550679 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/memory_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:57:49.554679 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-03 07:57:49.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-03 07:57:49.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:57:49.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 07:57:49.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 07:57:49.000000 sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 07:57:49.554679 sag_py_logging_logstash-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-03 07:57:43.000000 sag_py_logging_logstash-2.3.9/setup.py
```

### Comparing `sag-py-logging-logstash-2.3.8/LICENSE.txt` & `sag_py_logging_logstash-2.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/PKG-INFO` & `sag_py_logging_logstash-2.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging-logstash
-Version: 2.3.8
+Version: 2.3.9
 Summary: Python logging logstash handler
 Home-page: https://github.com/SamhammerAG/sag_py_logging_logstash
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging_logstash
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging_logstash/issues
@@ -16,26 +16,27 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: limits
-Requires-Dist: requests
+Requires-Dist: limits>=3.11.0
+Requires-Dist: requests>=2.31.0
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: coverage-lcov; extra == "dev"
-Requires-Dist: mock; extra == "dev"
-Requires-Dist: types-mock; extra == "dev"
+Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: mypy>=1.10.0; extra == "dev"
+Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio>=0.23.6; extra == "dev"
+Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
+Requires-Dist: coverage-lcov==0.2.4; extra == "dev"
+Requires-Dist: toml>=0.10.2; extra == "dev"
+Requires-Dist: mock>=5.1.0; extra == "dev"
+Requires-Dist: types-mock>=5.1.0.20240425; extra == "dev"
 
 # sag_py_logging_logstash
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_logging_logstash/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_logging_logstash)
 
@@ -111,7 +112,15 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_logging_logstash==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-logging-logstash-2.3.8/README.md` & `sag_py_logging_logstash-2.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -76,7 +76,15 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_logging_logstash==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/cache.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/cache.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/constants.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/constants.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/formatter.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/handler.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/handler.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/memory_cache.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/memory_cache.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/transport.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/transport.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/utils.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/utils.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash/worker.py` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash/worker.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/PKG-INFO` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging-logstash
-Version: 2.3.8
+Version: 2.3.9
 Summary: Python logging logstash handler
 Home-page: https://github.com/SamhammerAG/sag_py_logging_logstash
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging_logstash
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging_logstash/issues
@@ -16,26 +16,27 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: limits
-Requires-Dist: requests
+Requires-Dist: limits>=3.11.0
+Requires-Dist: requests>=2.31.0
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: coverage-lcov; extra == "dev"
-Requires-Dist: mock; extra == "dev"
-Requires-Dist: types-mock; extra == "dev"
+Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: mypy>=1.10.0; extra == "dev"
+Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio>=0.23.6; extra == "dev"
+Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
+Requires-Dist: coverage-lcov==0.2.4; extra == "dev"
+Requires-Dist: toml>=0.10.2; extra == "dev"
+Requires-Dist: mock>=5.1.0; extra == "dev"
+Requires-Dist: types-mock>=5.1.0.20240425; extra == "dev"
 
 # sag_py_logging_logstash
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_logging_logstash/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_logging_logstash)
 
@@ -111,7 +112,15 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_logging_logstash==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-logging-logstash-2.3.8/sag_py_logging_logstash.egg-info/SOURCES.txt` & `sag_py_logging_logstash-2.3.9/sag_py_logging_logstash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-logstash-2.3.8/setup.py` & `sag_py_logging_logstash-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-logging-logstash",
-    version="2.3.8",
+    version="2.3.9",
     description="Python logging logstash handler",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_logging_logstash",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

