# Comparing `tmp/llama_index_embeddings_jinaai-0.1.3.tar.gz` & `tmp/llama_index_embeddings_jinaai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_jinaai-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_embeddings_jinaai-0.1.4.tar", max compression
```

## Comparing `llama_index_embeddings_jinaai-0.1.3.tar` & `llama_index_embeddings_jinaai-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-02-13 13:53:01.621426 llama_index_embeddings_jinaai-0.1.3/README.md
--rw-r--r--   0        0        0       90 2024-02-13 13:53:01.621636 llama_index_embeddings_jinaai-0.1.3/llama_index/embeddings/jinaai/__init__.py
--rw-r--r--   0        0        0     4032 2024-02-20 22:37:41.281414 llama_index_embeddings_jinaai-0.1.3/llama_index/embeddings/jinaai/base.py
--rw-r--r--   0        0        0     1446 2024-02-21 16:28:49.551284 llama_index_embeddings_jinaai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 llama_index_embeddings_jinaai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/README.md
+-rw-r--r--   0        0        0       90 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/llama_index/embeddings/jinaai/__init__.py
+-rw-r--r--   0        0        0     6399 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/llama_index/embeddings/jinaai/base.py
+-rw-r--r--   0        0        0     1446 2024-05-03 18:27:21.554168 llama_index_embeddings_jinaai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 llama_index_embeddings_jinaai-0.1.4/PKG-INFO
```

### Comparing `llama_index_embeddings_jinaai-0.1.3/pyproject.toml` & `llama_index_embeddings_jinaai-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings jinaai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-jinaai"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_embeddings_jinaai-0.1.3/PKG-INFO` & `llama_index_embeddings_jinaai-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-jinaai
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index embeddings jinaai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Embeddings Integration: Jinaai
```

