# Comparing `tmp/robotframework-browser-translation-fi-0.4.2.tar.gz` & `tmp/robotframework_browser_translation_fi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-browser-translation-fi-0.4.2.tar", last modified: Fri Apr  5 23:02:59 2024, max compression
+gzip compressed data, was "robotframework_browser_translation_fi-0.5.0.tar", last modified: Fri May  3 19:22:01 2024, max compression
```

## Comparing `robotframework-browser-translation-fi-0.4.2.tar` & `robotframework_browser_translation_fi-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 23:02:08.000000 robotframework-browser-translation-fi-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-05 23:02:08.000000 robotframework-browser-translation-fi-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-05 23:02:55.000000 robotframework-browser-translation-fi-0.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-05 23:02:55.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   256796 2024-04-05 23:02:08.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:02:59.000000 robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:02:59.140919 robotframework-browser-translation-fi-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 19:21:17.000000 robotframework_browser_translation_fi-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-03 19:21:17.000000 robotframework_browser_translation_fi-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-03 19:21:57.000000 robotframework_browser_translation_fi-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-03 19:21:57.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295024 2024-05-03 19:21:17.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:22:01.470982 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:22:01.000000 robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:22:01.474982 robotframework_browser_translation_fi-0.5.0/setup.cfg
```

### Comparing `robotframework-browser-translation-fi-0.4.2/LICENSE` & `robotframework_browser_translation_fi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-browser-translation-fi-0.4.2/PKG-INFO` & `robotframework_browser_translation_fi-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-browser-translation-fi
-Version: 0.4.2
+Version: 0.5.0
 Summary: Robot Framework Browser library translation to Finnish languege
 Author-email: Tatu Aalto <aalto.tatu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,15 +219,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: robotframework-browser>=18.3.0
+Requires-Dist: robotframework-browser>=18.4.0
 
 # Finnish tranlsation for Robot Framework Browser library
 [![Version](https://img.shields.io/pypi/v/robotframework-browser-translation-fi.svg)](https://pypi.python.org/pypi/robotframework-browser-translation-fi)
 ![CI](https://github.com/MarketSquare/robotframework-browser-translation-fi/actions/workflows/on-push.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![All Contributors](https://img.shields.io/github/all-contributors/MarketSquare/robotframework-browser-translation-fi?color=ee8449&style=flat-square)](#contributors)
```

### Comparing `robotframework-browser-translation-fi-0.4.2/README.md` & `robotframework_browser_translation_fi-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-browser-translation-fi-0.4.2/pyproject.toml` & `robotframework_browser_translation_fi-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robotframework-browser-translation-fi"
-version = "0.4.2"
+version = "0.5.0"
 authors = [
   { name="Tatu Aalto", email="aalto.tatu@gmail.com" },
 ]
 license = {file = "LICENSE"}
 description = "Robot Framework Browser library translation to Finnish languege"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 keywords = ["Robot Framework", "Browser"]
 
-dependencies = ["robotframework-browser >= 18.3.0"]
+dependencies = ["robotframework-browser >= 18.4.0"]
 
 [project.urls]
 Homepage = "https://github.com/MarketSquare/robotframework-browser-translation-fi"
 Issues = "https://github.com/MarketSquare/robotframework-browser-translation-fi/issues"
 Changelog = "https://github.com/MarketSquare/robotframework-browser-translation-fi/blob/main/CHANGELOG.md"
 
 [tool.setuptools]
```

### Comparing `robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi/__init__.py` & `robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 from typing import TypedDict
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 
 
 class Language(TypedDict):
     language: str
     path: str
```

### Comparing `robotframework-browser-translation-fi-0.4.2/robotframework_browser_translation_fi.egg-info/PKG-INFO` & `robotframework_browser_translation_fi-0.5.0/robotframework_browser_translation_fi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-browser-translation-fi
-Version: 0.4.2
+Version: 0.5.0
 Summary: Robot Framework Browser library translation to Finnish languege
 Author-email: Tatu Aalto <aalto.tatu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,15 +219,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: robotframework-browser>=18.3.0
+Requires-Dist: robotframework-browser>=18.4.0
 
 # Finnish tranlsation for Robot Framework Browser library
 [![Version](https://img.shields.io/pypi/v/robotframework-browser-translation-fi.svg)](https://pypi.python.org/pypi/robotframework-browser-translation-fi)
 ![CI](https://github.com/MarketSquare/robotframework-browser-translation-fi/actions/workflows/on-push.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![All Contributors](https://img.shields.io/github/all-contributors/MarketSquare/robotframework-browser-translation-fi?color=ee8449&style=flat-square)](#contributors)
```

