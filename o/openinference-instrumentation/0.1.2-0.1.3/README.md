# Comparing `tmp/openinference_instrumentation-0.1.2.tar.gz` & `tmp/openinference_instrumentation-0.1.3.tar.gz`

## Comparing `openinference_instrumentation-0.1.2.tar` & `openinference_instrumentation-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/src/openinference/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/src/openinference/instrumentation/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/src/openinference/instrumentation/version.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/LICENSE
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/README.md
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/src/openinference/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/src/openinference/instrumentation/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/src/openinference/instrumentation/version.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/LICENSE
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/README.md
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.3/PKG-INFO
```

### Comparing `openinference_instrumentation-0.1.2/src/openinference/instrumentation/__init__.py` & `openinference_instrumentation-0.1.3/src/openinference/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.2/LICENSE` & `openinference_instrumentation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.2/pyproject.toml` & `openinference_instrumentation-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "opentelemetry-api",
-  "openinference-semantic-conventions",
+  "openinference-semantic-conventions>=0.1.6",
 ]
 
 [project.optional-dependencies]
 test = [
   "opentelemetry-sdk",
 ]
```

### Comparing `openinference_instrumentation-0.1.2/PKG-INFO` & `openinference_instrumentation-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenInference instrumentation utilities
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/openinference-instrumentation
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
-Requires-Dist: openinference-semantic-conventions
+Requires-Dist: openinference-semantic-conventions>=0.1.6
 Requires-Dist: opentelemetry-api
 Provides-Extra: test
 Requires-Dist: opentelemetry-sdk; extra == 'test'
 Description-Content-Type: text/markdown
 
 # OpenInference Mistral AI Instrumentation
 [![PyPI Version](https://img.shields.io/pypi/v/openinference-instrumentation-mistralai.svg)](https://pypi.python.org/pypi/openinference-instrumentation-mistralai)
```

