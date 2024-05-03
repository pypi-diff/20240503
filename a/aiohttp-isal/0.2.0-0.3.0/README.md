# Comparing `tmp/aiohttp_isal-0.2.0.tar.gz` & `tmp/aiohttp_isal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_isal-0.2.0.tar", max compression
+gzip compressed data, was "aiohttp_isal-0.3.0.tar", max compression
```

## Comparing `aiohttp_isal-0.2.0.tar` & `aiohttp_isal-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11345 2024-04-17 17:17:13.391355 aiohttp_isal-0.2.0/LICENSE
--rw-r--r--   0        0        0     4241 2024-04-17 17:17:13.391355 aiohttp_isal-0.2.0/README.md
--rw-r--r--   0        0        0     3558 2024-04-17 17:17:14.351352 aiohttp_isal-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      782 2024-04-17 17:17:14.351352 aiohttp_isal-0.2.0/src/aiohttp_isal/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 17:17:13.391355 aiohttp_isal-0.2.0/src/aiohttp_isal/py.typed
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 aiohttp_isal-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-03 18:00:19.770156 aiohttp_isal-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4241 2024-05-03 18:00:19.770156 aiohttp_isal-0.3.0/README.md
+-rw-r--r--   0        0        0     3558 2024-05-03 18:00:20.546159 aiohttp_isal-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1087 2024-05-03 18:00:20.546159 aiohttp_isal-0.3.0/src/aiohttp_isal/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 18:00:19.774156 aiohttp_isal-0.3.0/src/aiohttp_isal/py.typed
+-rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 aiohttp_isal-0.3.0/PKG-INFO
```

### Comparing `aiohttp_isal-0.2.0/LICENSE` & `aiohttp_isal-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_isal-0.2.0/README.md` & `aiohttp_isal-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_isal-0.2.0/pyproject.toml` & `aiohttp_isal-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohttp-isal"
-version = "0.2.0"
+version = "0.3.0"
 description = "isal support for aiohttp"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/aiohttp-isal"
 documentation = "https://aiohttp-isal.readthedocs.io"
 classifiers = [
```

### Comparing `aiohttp_isal-0.2.0/PKG-INFO` & `aiohttp_isal-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-isal
-Version: 0.2.0
+Version: 0.3.0
 Summary: isal support for aiohttp
 Home-page: https://github.com/bdraco/aiohttp-isal
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiohttp-isal Version: 0.2.0 Summary: isal support
+Metadata-Version: 2.1 Name: aiohttp-isal Version: 0.3.0 Summary: isal support
 for aiohttp Home-page: https://github.com/bdraco/aiohttp-isal License: Apache
 Software License 2.0 Author: J. Nick Koston Author-email: nick@koston.org
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

