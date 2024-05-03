# Comparing `tmp/airbyte_source_openweather-0.2.3.tar.gz` & `tmp/airbyte_source_openweather-0.2.3.dev202405030718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_openweather-0.2.3.tar", max compression
+gzip compressed data, was "airbyte_source_openweather-0.2.3.dev202405030718.tar", max compression
```

## Comparing `airbyte_source_openweather-0.2.3.tar` & `airbyte_source_openweather-0.2.3.dev202405030718.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4586 2024-05-01 18:58:59.236318 airbyte_source_openweather-0.2.3/README.md
--rw-r--r--   0        0        0      773 2024-05-01 19:02:46.927499 airbyte_source_openweather-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      134 2024-05-01 18:58:59.236318 airbyte_source_openweather-0.2.3/source_openweather/__init__.py
--rw-r--r--   0        0        0     8090 2024-05-01 18:58:59.236318 airbyte_source_openweather-0.2.3/source_openweather/manifest.yaml
--rw-r--r--   0        0        0      245 2024-05-01 18:58:59.236318 airbyte_source_openweather-0.2.3/source_openweather/run.py
--rw-r--r--   0        0        0      480 2024-05-01 18:58:59.236318 airbyte_source_openweather-0.2.3/source_openweather/source.py
--rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 airbyte_source_openweather-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4586 2024-05-02 19:52:56.000000 airbyte_source_openweather-0.2.3.dev202405030718/README.md
+-rw-r--r--   0        0        0      789 2024-05-03 07:18:26.027802 airbyte_source_openweather-0.2.3.dev202405030718/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-05-02 19:52:56.000000 airbyte_source_openweather-0.2.3.dev202405030718/source_openweather/__init__.py
+-rw-r--r--   0        0        0     8090 2024-05-02 19:52:56.000000 airbyte_source_openweather-0.2.3.dev202405030718/source_openweather/manifest.yaml
+-rw-r--r--   0        0        0      245 2024-05-02 19:52:56.000000 airbyte_source_openweather-0.2.3.dev202405030718/source_openweather/run.py
+-rw-r--r--   0        0        0      480 2024-05-02 19:52:56.000000 airbyte_source_openweather-0.2.3.dev202405030718/source_openweather/source.py
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 airbyte_source_openweather-0.2.3.dev202405030718/PKG-INFO
```

### Comparing `airbyte_source_openweather-0.2.3/README.md` & `airbyte_source_openweather-0.2.3.dev202405030718/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_openweather-0.2.3/pyproject.toml` & `airbyte_source_openweather-0.2.3.dev202405030718/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.3"
+version = "0.2.3.dev202405030718"
 name = "airbyte-source-openweather"
 description = "Source implementation for Openweather."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_openweather-0.2.3/source_openweather/manifest.yaml` & `airbyte_source_openweather-0.2.3.dev202405030718/source_openweather/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_openweather-0.2.3/PKG-INFO` & `airbyte_source_openweather-0.2.3.dev202405030718/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-openweather
-Version: 0.2.3
+Version: 0.2.3.dev202405030718
 Summary: Source implementation for Openweather.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

