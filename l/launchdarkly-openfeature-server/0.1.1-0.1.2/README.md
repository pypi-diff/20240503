# Comparing `tmp/launchdarkly_openfeature_server-0.1.1.tar.gz` & `tmp/launchdarkly_openfeature_server-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchdarkly_openfeature_server-0.1.1.tar", max compression
+gzip compressed data, was "launchdarkly_openfeature_server-0.1.2.tar", max compression
```

## Comparing `launchdarkly_openfeature_server-0.1.1.tar` & `launchdarkly_openfeature_server-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      557 2024-02-12 21:16:26.784329 launchdarkly_openfeature_server-0.1.1/LICENSE
--rw-r--r--   0        0        0     8949 2024-02-12 21:16:26.784329 launchdarkly_openfeature_server-0.1.1/README.md
--rw-r--r--   0        0        0       99 2024-02-12 21:16:26.784329 launchdarkly_openfeature_server-0.1.1/ld_openfeature/__init__.py
--rw-r--r--   0        0        0     4531 2024-02-12 21:16:26.784329 launchdarkly_openfeature_server-0.1.1/ld_openfeature/impl/context_converter.py
--rw-r--r--   0        0        0     2282 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/ld_openfeature/impl/details_converter.py
--rw-r--r--   0        0        0     5134 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/ld_openfeature/provider.py
--rw-r--r--   0        0        0        1 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/ld_openfeature/py.typed
--rw-r--r--   0        0        0     1760 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     6941 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/tests/impl/test_context_converter.py
--rw-r--r--   0        0        0     1962 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/tests/impl/test_details_converter.py
--rw-r--r--   0        0        0     5755 2024-02-12 21:16:26.788329 launchdarkly_openfeature_server-0.1.1/tests/test_provider.py
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 launchdarkly_openfeature_server-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      557 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9131 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/README.md
+-rw-r--r--   0        0        0       99 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/ld_openfeature/__init__.py
+-rw-r--r--   0        0        0     4532 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/ld_openfeature/impl/context_converter.py
+-rw-r--r--   0        0        0     2282 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/ld_openfeature/impl/details_converter.py
+-rw-r--r--   0        0        0     5134 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/ld_openfeature/provider.py
+-rw-r--r--   0        0        0        1 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/ld_openfeature/py.typed
+-rw-r--r--   0        0        0     1765 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     6941 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/tests/impl/test_context_converter.py
+-rw-r--r--   0        0        0     1962 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/tests/impl/test_details_converter.py
+-rw-r--r--   0        0        0     5755 2024-05-03 20:23:41.169269 launchdarkly_openfeature_server-0.1.2/tests/test_provider.py
+-rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 launchdarkly_openfeature_server-0.1.2/PKG-INFO
```

### Comparing `launchdarkly_openfeature_server-0.1.1/LICENSE` & `launchdarkly_openfeature_server-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `launchdarkly_openfeature_server-0.1.1/README.md` & `launchdarkly_openfeature_server-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 [![PyPI](https://img.shields.io/pypi/v/launchdarkly-openfeature-server.svg?maxAge=2592000)](https://pypi.python.org/pypi/launchdarkly-openfeature-server)
 [![PyPI](https://img.shields.io/pypi/pyversions/launchdarkly-openfeature-server.svg)](https://pypi.python.org/pypi/launchdarkly-openfeature-server)
 
 This provider allows for using LaunchDarkly with the OpenFeature SDK for Python.
 
 This provider is designed primarily for use in multi-user systems such as web servers and applications. It follows the server-side LaunchDarkly model for multi-user contexts. It is not intended for use in desktop and embedded systems applications.
 
-This provider is a beta version and should not be considered ready for production use while this message is visible.
+> [!WARNING]
+> This is a beta version. The API is not stabilized and may introduce breaking changes.
+
+> [!NOTE]
+> This OpenFeature provider uses production versions of the LaunchDarkly SDK, which adhere to our standard [versioning policy](https://docs.launchdarkly.com/home/relay-proxy/versioning).
 
 # LaunchDarkly overview
 
 [LaunchDarkly](https://www.launchdarkly.com) is a feature management platform that serves trillions of feature flags daily to help teams build better software, faster. [Get started](https://docs.launchdarkly.com/home/getting-started) using LaunchDarkly today!
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/launchdarkly.svg?style=social&label=Follow&maxAge=2592000)](https://twitter.com/intent/follow?screen_name=launchdarkly)
```

### Comparing `launchdarkly_openfeature_server-0.1.1/ld_openfeature/impl/context_converter.py` & `launchdarkly_openfeature_server-0.1.2/ld_openfeature/impl/context_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from logging import getLogger
 from typing import Any, Dict, List, Optional
 
 from ldclient.context import Context, ContextBuilder, ContextMultiBuilder
-from openfeature.provider.provider import EvaluationContext
+from openfeature.evaluation_context import EvaluationContext
 
 
 logger = getLogger("launchdarkly-openfeature-server")
 
 
 class EvaluationContextConverter:
     def to_ld_context(self, context: EvaluationContext) -> Context:
```

### Comparing `launchdarkly_openfeature_server-0.1.1/ld_openfeature/impl/details_converter.py` & `launchdarkly_openfeature_server-0.1.2/ld_openfeature/impl/details_converter.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_openfeature_server-0.1.1/ld_openfeature/provider.py` & `launchdarkly_openfeature_server-0.1.2/ld_openfeature/provider.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_openfeature_server-0.1.1/pyproject.toml` & `launchdarkly_openfeature_server-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "launchdarkly-openfeature-server"
-version = "0.1.1"
+version = "0.1.2"
 description = "An OpenFeature provider for the LaunchDarkly Python server SDK"
 authors = ["LaunchDarkly <dev@launchdarkly.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/launchdarkly/openfeature-python-server"
 documentation = "https://launchdarkly-openfeature-server.readthedocs.io/en/latest/"
 classifiers = [
@@ -24,15 +24,15 @@
     { include = "ld_openfeature" },
     { include = "tests" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openfeature-sdk = "0.4.2"
+openfeature-sdk = ">=0.4.2,<1"
 launchdarkly-server-sdk = "<10"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=2.8"
 pytest-cov = ">=2.4.0"
 pytest-mypy = "==0.10.3"
```

### Comparing `launchdarkly_openfeature_server-0.1.1/tests/impl/test_context_converter.py` & `launchdarkly_openfeature_server-0.1.2/tests/impl/test_context_converter.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_openfeature_server-0.1.1/tests/impl/test_details_converter.py` & `launchdarkly_openfeature_server-0.1.2/tests/impl/test_details_converter.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_openfeature_server-0.1.1/tests/test_provider.py` & `launchdarkly_openfeature_server-0.1.2/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_openfeature_server-0.1.1/PKG-INFO` & `launchdarkly_openfeature_server-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchdarkly-openfeature-server
-Version: 0.1.1
+Version: 0.1.2
 Summary: An OpenFeature provider for the LaunchDarkly Python server SDK
 Home-page: https://github.com/launchdarkly/openfeature-python-server
 License: Apache-2.0
 Author: LaunchDarkly
 Author-email: dev@launchdarkly.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: launchdarkly-server-sdk (<10)
-Requires-Dist: openfeature-sdk (==0.4.2)
+Requires-Dist: openfeature-sdk (>=0.4.2,<1)
 Project-URL: Documentation, https://launchdarkly-openfeature-server.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/launchdarkly/openfeature-python-server
 Description-Content-Type: text/markdown
 
 # LaunchDarkly OpenFeature provider for the Server-Side SDK for Python
 
 [![Quality control checks](https://github.com/launchdarkly/openfeature-python-server/actions/workflows/ci.yml/badge.svg)](https://github.com/launchdarkly/openfeature-python-server/actions/workflows/ci.yml)
@@ -32,15 +32,19 @@
 [![PyPI](https://img.shields.io/pypi/v/launchdarkly-openfeature-server.svg?maxAge=2592000)](https://pypi.python.org/pypi/launchdarkly-openfeature-server)
 [![PyPI](https://img.shields.io/pypi/pyversions/launchdarkly-openfeature-server.svg)](https://pypi.python.org/pypi/launchdarkly-openfeature-server)
 
 This provider allows for using LaunchDarkly with the OpenFeature SDK for Python.
 
 This provider is designed primarily for use in multi-user systems such as web servers and applications. It follows the server-side LaunchDarkly model for multi-user contexts. It is not intended for use in desktop and embedded systems applications.
 
-This provider is a beta version and should not be considered ready for production use while this message is visible.
+> [!WARNING]
+> This is a beta version. The API is not stabilized and may introduce breaking changes.
+
+> [!NOTE]
+> This OpenFeature provider uses production versions of the LaunchDarkly SDK, which adhere to our standard [versioning policy](https://docs.launchdarkly.com/home/relay-proxy/versioning).
 
 # LaunchDarkly overview
 
 [LaunchDarkly](https://www.launchdarkly.com) is a feature management platform that serves trillions of feature flags daily to help teams build better software, faster. [Get started](https://docs.launchdarkly.com/home/getting-started) using LaunchDarkly today!
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/launchdarkly.svg?style=social&label=Follow&maxAge=2592000)](https://twitter.com/intent/follow?screen_name=launchdarkly)
```

