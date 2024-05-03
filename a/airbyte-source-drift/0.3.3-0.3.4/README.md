# Comparing `tmp/airbyte_source_drift-0.3.3.tar.gz` & `tmp/airbyte_source_drift-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_drift-0.3.3.tar", max compression
+gzip compressed data, was "airbyte_source_drift-0.3.4.tar", max compression
```

## Comparing `airbyte_source_drift-0.3.3.tar` & `airbyte_source_drift-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4478 2024-05-01 18:38:29.816310 airbyte_source_drift-0.3.3/README.md
--rw-r--r--   0        0        0      712 2024-05-01 18:42:21.056114 airbyte_source_drift-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-01 18:38:29.816310 airbyte_source_drift-0.3.3/source_drift/__init__.py
--rw-r--r--   0        0        0    13121 2024-05-01 18:38:29.816310 airbyte_source_drift-0.3.3/source_drift/manifest.yaml
--rw-r--r--   0        0        0      227 2024-05-01 18:38:29.816310 airbyte_source_drift-0.3.3/source_drift/run.py
--rw-r--r--   0        0        0      474 2024-05-01 18:38:29.816310 airbyte_source_drift-0.3.3/source_drift/source.py
--rw-r--r--   0        0        0     3204 2024-05-01 18:38:29.816310 airbyte_source_drift-0.3.3/source_drift/spec.yaml
--rw-r--r--   0        0        0     5179 1970-01-01 00:00:00.000000 airbyte_source_drift-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     4478 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/README.md
+-rw-r--r--   0        0        0      708 2024-05-03 14:06:02.310621 airbyte_source_drift-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/__init__.py
+-rw-r--r--   0        0        0    13120 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/run.py
+-rw-r--r--   0        0        0      474 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/source.py
+-rw-r--r--   0        0        0     3204 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/spec.yaml
+-rw-r--r--   0        0        0     5177 1970-01-01 00:00:00.000000 airbyte_source_drift-0.3.4/PKG-INFO
```

### Comparing `airbyte_source_drift-0.3.3/README.md` & `airbyte_source_drift-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_drift-0.3.3/pyproject.toml` & `airbyte_source_drift-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.3"
+version = "0.3.4"
 name = "airbyte-source-drift"
 description = "Source implementation for Drift."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_drift" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "^0"
 
 [tool.poetry.scripts]
 source-drift = "source_drift.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_drift-0.3.3/source_drift/manifest.yaml` & `airbyte_source_drift-0.3.4/source_drift/manifest.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     retriever:
       $ref: "#/definitions/retriever"
 
   base_paginator:
     type: "DefaultPaginator"
     pagination_strategy:
       type: "CursorPagination"
-      cursor_value: "{{ last_records['next'] }}"
+      cursor_value: "{{ last_record['next'] }}"
     page_token_option:
       type: "RequestPath"
       field_name: "page_token"
       inject_into: "request_parameter"
 
   accounts_stream:
     $ref: "#/definitions/base_stream"
```

### Comparing `airbyte_source_drift-0.3.3/source_drift/spec.yaml` & `airbyte_source_drift-0.3.4/source_drift/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_drift-0.3.3/PKG-INFO` & `airbyte_source_drift-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-drift
-Version: 0.3.3
+Version: 0.3.4
 Summary: Source implementation for Drift.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/drift
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Drift source connector
```

