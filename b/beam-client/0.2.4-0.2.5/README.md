# Comparing `tmp/beam_client-0.2.4.tar.gz` & `tmp/beam_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_client-0.2.4.tar", max compression
+gzip compressed data, was "beam_client-0.2.5.tar", max compression
```

## Comparing `beam_client-0.2.4.tar` & `beam_client-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      735 2024-05-02 22:21:33.348756 beam_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      597 2024-04-17 13:15:05.679787 beam_client-0.2.4/src/beam/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 13:15:05.679851 beam_client-0.2.4/src/beam/cli/__init__.py
--rw-r--r--   0        0        0      438 2024-04-29 21:55:36.161099 beam_client-0.2.4/src/beam/cli/logs.py
--rw-r--r--   0        0        0      405 2024-05-02 22:21:05.937690 beam_client-0.2.4/src/beam/cli/main.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 beam_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      735 2024-05-03 14:57:20.719475 beam_client-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      597 2024-04-17 13:15:05.679787 beam_client-0.2.5/src/beam/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:15:05.679851 beam_client-0.2.5/src/beam/cli/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-29 21:55:36.161099 beam_client-0.2.5/src/beam/cli/logs.py
+-rw-r--r--   0        0        0      405 2024-05-02 22:21:05.937690 beam_client-0.2.5/src/beam/cli/main.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 beam_client-0.2.5/PKG-INFO
```

### Comparing `beam_client-0.2.4/pyproject.toml` & `beam_client-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "beam-client"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beam/**/*.py", from = "src" },
     { include = "beam", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-beta9 = "0.1.13"
+beta9 = "0.1.16"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-env = "^1.1.3"
 ruff = "^0.4.2"
 
 [tool.poetry.scripts]
```

### Comparing `beam_client-0.2.4/src/beam/__init__.py` & `beam_client-0.2.5/src/beam/__init__.py`

 * *Files identical despite different names*

