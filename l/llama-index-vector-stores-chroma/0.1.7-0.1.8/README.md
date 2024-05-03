# Comparing `tmp/llama_index_vector_stores_chroma-0.1.7.tar.gz` & `tmp/llama_index_vector_stores_chroma-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_chroma-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_chroma-0.1.8.tar", max compression
```

## Comparing `llama_index_vector_stores_chroma-0.1.7.tar` & `llama_index_vector_stores_chroma-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       47 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/README.md
--rw-r--r--   0        0        0      101 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/llama_index/vector_stores/chroma/__init__.py
--rw-r--r--   0        0        0    13268 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/llama_index/vector_stores/chroma/base.py
--rw-r--r--   0        0        0     1487 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_chroma-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-05-03 15:23:20.386115 llama_index_vector_stores_chroma-0.1.8/README.md
+-rw-r--r--   0        0        0      101 2024-05-03 15:23:20.386115 llama_index_vector_stores_chroma-0.1.8/llama_index/vector_stores/chroma/__init__.py
+-rw-r--r--   0        0        0    13271 2024-05-03 15:23:20.386115 llama_index_vector_stores_chroma-0.1.8/llama_index/vector_stores/chroma/base.py
+-rw-r--r--   0        0        0     1487 2024-05-03 15:23:20.386115 llama_index_vector_stores_chroma-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_chroma-0.1.8/PKG-INFO
```

### Comparing `llama_index_vector_stores_chroma-0.1.7/llama_index/vector_stores/chroma/base.py` & `llama_index_vector_stores_chroma-0.1.8/llama_index/vector_stores/chroma/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         results = self._collection.query(
             query_embeddings=query_embeddings,
             n_results=n_results,
             where=where,
             **kwargs,
         )
 
-        logger.debug(f"> Top {len(results['documents'])} nodes:")
+        logger.debug(f"> Top {len(results['documents'][0])} nodes:")
         nodes = []
         similarities = []
         ids = []
         for node_id, text, metadata, distance in zip(
             results["ids"][0],
             results["documents"][0],
             results["metadatas"][0],
```

### Comparing `llama_index_vector_stores_chroma-0.1.7/pyproject.toml` & `llama_index_vector_stores_chroma-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores chroma integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-chroma"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 chromadb = ">=0.4.0,<0.6.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_chroma-0.1.7/PKG-INFO` & `llama_index_vector_stores_chroma-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-chroma
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index vector_stores chroma integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

