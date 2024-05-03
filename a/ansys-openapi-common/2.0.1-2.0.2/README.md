# Comparing `tmp/ansys_openapi_common-2.0.1.tar.gz` & `tmp/ansys_openapi_common-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_openapi_common-2.0.1.tar", max compression
+gzip compressed data, was "ansys_openapi_common-2.0.2.tar", max compression
```

## Comparing `ansys_openapi_common-2.0.1.tar` & `ansys_openapi_common-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      618 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/AUTHORS.md
--rw-r--r--   0        0        0     1098 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/LICENSE
--rw-r--r--   0        0        0     6139 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/README.rst
--rw-r--r--   0        0        0     3761 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2021 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/__init__.py
--rw-r--r--   0        0        0    34351 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_api_client.py
--rw-r--r--   0        0        0     1176 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_base/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_base/_types.py
--rw-r--r--   0        0        0     5063 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_exceptions.py
--rw-r--r--   0        0        0     1262 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_logger.py
--rw-r--r--   0        0        0    14146 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_oidc.py
--rw-r--r--   0        0        0    20665 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_session.py
--rw-r--r--   0        0        0    16120 2024-05-02 15:06:22.753483 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_util.py
--rw-r--r--   0        0        0        0 2024-05-02 15:06:22.753483 ansys_openapi_common-2.0.1/src/ansys/openapi/common/py.typed
--rw-r--r--   0        0        0     7817 1970-01-01 00:00:00.000000 ansys_openapi_common-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      618 2024-05-03 15:21:56.730176 ansys_openapi_common-2.0.2/AUTHORS.md
+-rw-r--r--   0        0        0     1098 2024-05-03 15:21:56.730176 ansys_openapi_common-2.0.2/LICENSE
+-rw-r--r--   0        0        0     6139 2024-05-03 15:21:56.730176 ansys_openapi_common-2.0.2/README.rst
+-rw-r--r--   0        0        0     3867 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2021 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/__init__.py
+-rw-r--r--   0        0        0    34351 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_api_client.py
+-rw-r--r--   0        0        0     1176 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_base/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_base/_types.py
+-rw-r--r--   0        0        0     5063 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_exceptions.py
+-rw-r--r--   0        0        0     1262 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_logger.py
+-rw-r--r--   0        0        0    14146 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_oidc.py
+-rw-r--r--   0        0        0    20665 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_session.py
+-rw-r--r--   0        0        0    16120 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/_util.py
+-rw-r--r--   0        0        0        0 2024-05-03 15:21:56.734176 ansys_openapi_common-2.0.2/src/ansys/openapi/common/py.typed
+-rw-r--r--   0        0        0     7817 1970-01-01 00:00:00.000000 ansys_openapi_common-2.0.2/PKG-INFO
```

### Comparing `ansys_openapi_common-2.0.1/AUTHORS.md` & `ansys_openapi_common-2.0.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/LICENSE` & `ansys_openapi_common-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/README.rst` & `ansys_openapi_common-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/pyproject.toml` & `ansys_openapi_common-2.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ansys-openapi-common"
 description = "Provides a helper to create sessions for use with Ansys OpenAPI clients."
-version = "2.0.1"
+version = "2.0.2"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 repository = "https://github.com/pyansys/openapi-common"
 documentation = "https://openapi.docs.pyansys.com"
 readme = "README.rst"
 keywords = [
@@ -58,25 +58,30 @@
 pytest-cov = { version = "*" }
 uvicorn = { version = "*" }
 fastapi = { version = "*" }
 pydantic = { version = "*" }
 requests-mock = { version = "*" }
 pytest-mock = { version = "*" }
 covertable = { version = "*" }
-asgi_gssapi = { version = "*", markers = "sys_platform == 'linux'" }
 mypy = "^1.8.0"
 types-requests = { version = "*" }
 types-python-dateutil = { version = "*" }
 requests_auth = { version = "*" }
 keyring = { version = "*" }
 
-[tool.poetry.group.docs]
+[tool.poetry.group.dev-linux]
+optional = true
+
+[tool.poetry.group.dev-linux.dependencies]
+asgi_gssapi = { version = "*", markers = "sys_platform == 'linux'" }
+
+[tool.poetry.group.doc]
 optional = true
 
-[tool.poetry.group.docs.dependencies]
+[tool.poetry.group.doc.dependencies]
 # Doc packages
 ansys-sphinx-theme = { version = "0.14.0" }
 numpydoc = { version = "1.6.0" }
 sphinx = { version = "7.2.6" }
 sphinx-notfound-page = { version = "1.0.0" }
 sphinx-copybutton = { version = "0.5.2" }
 
@@ -104,15 +109,15 @@
     3.10: py310
     3.11: py311
     3.12: py312
 
 [testenv]
 whitelist_externals = poetry
 commands_pre =
-    poetry install --no-root --extras "oidc linux-kerberos"
+    poetry install --no-root --with dev-linux --extras "oidc linux-kerberos"
 extras =
     oidc
     linux-kerberos
 commands = poetry run pytest --cov=ansys.openapi.common --cov-report=xml {posargs}
 """
 
 [tool.black]
```

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/__init__.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_api_client.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_api_client.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_base/__init__.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_base/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_base/_types.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_base/_types.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_exceptions.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_exceptions.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_logger.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_logger.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_oidc.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_oidc.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_session.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_session.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_util.py` & `ansys_openapi_common-2.0.2/src/ansys/openapi/common/_util.py`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.1/PKG-INFO` & `ansys_openapi_common-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-openapi-common
-Version: 2.0.1
+Version: 2.0.2
 Summary: Provides a helper to create sessions for use with Ansys OpenAPI clients.
 Home-page: https://github.com/pyansys/openapi-common
 License: MIT
 Keywords: Ansys,OpenAPI
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
```

