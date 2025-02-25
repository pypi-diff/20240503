# Comparing `tmp/robotcode_analyze-0.80.0.tar.gz` & `tmp/robotcode_analyze-0.81.0.tar.gz`

## Comparing `robotcode_analyze-0.80.0.tar` & `robotcode_analyze-0.81.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/src/robotcode/analyze/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/src/robotcode/analyze/__version__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/src/robotcode/analyze/analyzer.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/src/robotcode/analyze/cli.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/src/robotcode/analyze/config.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/src/robotcode/analyze/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/src/robotcode/analyze/py.typed
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/LICENSE.txt
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/README.md
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 robotcode_analyze-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/src/robotcode/analyze/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/src/robotcode/analyze/__version__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/src/robotcode/analyze/analyzer.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/src/robotcode/analyze/cli.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/src/robotcode/analyze/config.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/src/robotcode/analyze/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/src/robotcode/analyze/py.typed
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/LICENSE.txt
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 robotcode_analyze-0.81.0/PKG-INFO
```

### Comparing `robotcode_analyze-0.80.0/src/robotcode/analyze/cli.py` & `robotcode_analyze-0.81.0/src/robotcode/analyze/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.80.0/src/robotcode/analyze/config.py` & `robotcode_analyze-0.81.0/src/robotcode/analyze/config.py`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.80.0/.gitignore` & `robotcode_analyze-0.81.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.80.0/LICENSE.txt` & `robotcode_analyze-0.81.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.80.0/README.md` & `robotcode_analyze-0.81.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.80.0/pyproject.toml` & `robotcode_analyze-0.81.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,26 +23,26 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-plugin==0.80.0",
-  "robotcode-robot==0.80.0",
-  "robotcode==0.80.0",
+  "robotcode-plugin==0.81.0",
+  "robotcode-robot==0.81.0",
+  "robotcode==0.81.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 analyze = "robotcode.analyze.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
-Donate = "https://github.com/sponsors/d-biehl"
+Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
 Changelog = "https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md"
 Issues = "https://github.com/robotcodedev/robotcode/issues"
 Source = "https://github.com/robotcodedev/robotcode"
 
 [tool.hatch.version]
 path = "src/robotcode/analyze/__version__.py"
```

### Comparing `robotcode_analyze-0.80.0/PKG-INFO` & `robotcode_analyze-0.81.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: robotcode-analyze
-Version: 0.80.0
+Version: 0.81.0
 Summary: RobotCode analyze plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
-Project-URL: Donate, https://github.com/sponsors/d-biehl
+Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
 License: Apache-2.0
 License-File: LICENSE.txt
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-plugin==0.80.0
-Requires-Dist: robotcode-robot==0.80.0
-Requires-Dist: robotcode==0.80.0
+Requires-Dist: robotcode-plugin==0.81.0
+Requires-Dist: robotcode-robot==0.81.0
+Requires-Dist: robotcode==0.81.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-analyze
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-analyze.svg)](https://pypi.org/project/robotcode-analyze)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-analyze.svg)](https://pypi.org/project/robotcode-analyze)
```

