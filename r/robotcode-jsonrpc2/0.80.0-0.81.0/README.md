# Comparing `tmp/robotcode_jsonrpc2-0.80.0.tar.gz` & `tmp/robotcode_jsonrpc2-0.81.0.tar.gz`

## Comparing `robotcode_jsonrpc2-0.80.0.tar` & `robotcode_jsonrpc2-0.81.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/src/robotcode/jsonrpc2/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/src/robotcode/jsonrpc2/__version__.py
--rw-r--r--   0        0        0    30048 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/src/robotcode/jsonrpc2/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/src/robotcode/jsonrpc2/py.typed
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/src/robotcode/jsonrpc2/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/LICENSE.txt
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/README.md
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/pyproject.toml
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/src/robotcode/jsonrpc2/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/src/robotcode/jsonrpc2/__version__.py
+-rw-r--r--   0        0        0    30048 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/src/robotcode/jsonrpc2/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/src/robotcode/jsonrpc2/py.typed
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/src/robotcode/jsonrpc2/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/LICENSE.txt
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/README.md
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.81.0/PKG-INFO
```

### Comparing `robotcode_jsonrpc2-0.80.0/src/robotcode/jsonrpc2/protocol.py` & `robotcode_jsonrpc2-0.81.0/src/robotcode/jsonrpc2/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.80.0/src/robotcode/jsonrpc2/server.py` & `robotcode_jsonrpc2-0.81.0/src/robotcode/jsonrpc2/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.80.0/.gitignore` & `robotcode_jsonrpc2-0.81.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.80.0/LICENSE.txt` & `robotcode_jsonrpc2-0.81.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.80.0/README.md` & `robotcode_jsonrpc2-0.81.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.80.0/pyproject.toml` & `robotcode_jsonrpc2-0.81.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,20 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotcode-core==0.80.0"]
+dependencies = ["robotcode-core==0.81.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
-Donate = "https://github.com/sponsors/d-biehl"
+Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
 Changelog = "https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md"
 Issues = "https://github.com/robotcodedev/robotcode/issues"
 Source = "https://github.com/robotcodedev/robotcode"
 
 [tool.hatch.version]
 path = "src/robotcode/jsonrpc2/__version__.py"
```

### Comparing `robotcode_jsonrpc2-0.80.0/PKG-INFO` & `robotcode_jsonrpc2-0.81.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: robotcode-jsonrpc2
-Version: 0.80.0
+Version: 0.81.0
 Summary: JSONRPC Server for RobotCode
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
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.80.0
+Requires-Dist: robotcode-core==0.81.0
 Description-Content-Type: text/markdown
 
 # robotcode-jsonrpc2
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![License](https://img.shields.io/github/license/robotcodedev/robotcode?style=flat&logo=apache)](https://github.com/robotcodedev/robotcode/blob/master/LICENSE.txt)
```

