# Comparing `tmp/llama_index_callbacks_argilla-0.1.3.tar.gz` & `tmp/llama_index_callbacks_argilla-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_callbacks_argilla-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_callbacks_argilla-0.1.4.tar", max compression
```

## Comparing `llama_index_callbacks_argilla-0.1.3.tar` & `llama_index_callbacks_argilla-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-02-13 13:53:01.586244 llama_index_callbacks_argilla-0.1.3/README.md
--rw-r--r--   0        0        0      112 2024-02-13 13:53:01.586483 llama_index_callbacks_argilla-0.1.3/llama_index/callbacks/argilla/__init__.py
--rw-r--r--   0        0        0      407 2024-02-13 13:53:01.586569 llama_index_callbacks_argilla-0.1.3/llama_index/callbacks/argilla/base.py
--rw-r--r--   0        0        0     1484 2024-02-21 16:10:05.851081 llama_index_callbacks_argilla-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 llama_index_callbacks_argilla-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4130 2024-05-03 15:14:55.201685 llama_index_callbacks_argilla-0.1.4/README.md
+-rw-r--r--   0        0        0      112 2024-05-03 15:14:55.201685 llama_index_callbacks_argilla-0.1.4/llama_index/callbacks/argilla/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-03 15:14:55.201685 llama_index_callbacks_argilla-0.1.4/llama_index/callbacks/argilla/base.py
+-rw-r--r--   0        0        0     1517 2024-05-03 15:14:55.201685 llama_index_callbacks_argilla-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 llama_index_callbacks_argilla-0.1.4/PKG-INFO
```

### Comparing `llama_index_callbacks_argilla-0.1.3/pyproject.toml` & `llama_index_callbacks_argilla-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index callbacks argilla integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-callbacks-argilla"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 llama-index-core = "^0.10.11.post1"
-argilla = "^1.22.0"
+argilla = ">=1.22.0"
+argilla-llama-index = ">=1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

