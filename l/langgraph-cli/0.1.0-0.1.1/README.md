# Comparing `tmp/langgraph_cli-0.1.0.tar.gz` & `tmp/langgraph_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_cli-0.1.0.tar", max compression
+gzip compressed data, was "langgraph_cli-0.1.1.tar", max compression
```

## Comparing `langgraph_cli-0.1.0.tar` & `langgraph_cli-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.0/langgraph_cli/__init__.py
--rw-r--r--   0        0        0     5685 2024-05-02 17:41:43.798531 langgraph_cli-0.1.0/langgraph_cli/cli.py
--rw-r--r--   0        0        0     2738 2024-05-02 00:35:49.773352 langgraph_cli-0.1.0/langgraph_cli/config.py
--rw-r--r--   0        0        0     1616 2024-05-02 00:35:49.773581 langgraph_cli-0.1.0/langgraph_cli/docker.py
--rw-r--r--   0        0        0     1024 2024-05-02 17:42:05.493463 langgraph_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.1/langgraph_cli/__init__.py
+-rw-r--r--   0        0        0     5685 2024-05-02 17:41:43.798531 langgraph_cli-0.1.1/langgraph_cli/cli.py
+-rw-r--r--   0        0        0     2738 2024-05-02 00:35:49.773352 langgraph_cli-0.1.1/langgraph_cli/config.py
+-rw-r--r--   0        0        0     1609 2024-05-02 20:46:38.017185 langgraph_cli-0.1.1/langgraph_cli/docker.py
+-rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.1/langgraph_cli/initdb/init.sql
+-rw-r--r--   0        0        0     1024 2024-05-02 20:47:24.787936 langgraph_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.1/PKG-INFO
```

### Comparing `langgraph_cli-0.1.0/langgraph_cli/cli.py` & `langgraph_cli-0.1.1/langgraph_cli/cli.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.0/langgraph_cli/config.py` & `langgraph_cli-0.1.1/langgraph_cli/config.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.0/langgraph_cli/docker.py` & `langgraph_cli-0.1.1/langgraph_cli/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 from typing import Optional
 
 
-ROOT = pathlib.Path(__file__).parent.parent.resolve()
+ROOT = pathlib.Path(__file__).parent.resolve()
 
 
 DB = f"""
     postgres:
         image: postgres:16
         restart: on-failure
         healthcheck:
```

### Comparing `langgraph_cli-0.1.0/pyproject.toml` & `langgraph_cli-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_cli"}]
 
 [tool.poetry.scripts]
 langgraph = "langgraph_cli.cli:cli"
```

