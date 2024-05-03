# Comparing `tmp/ozonetel-ai-0.0.12.tar.gz` & `tmp/ozonetel-ai-0.0.121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozonetel-ai-0.0.12.tar", last modified: Thu May  2 13:02:55 2024, max compression
+gzip compressed data, was "ozonetel-ai-0.0.121.tar", last modified: Fri May  3 05:55:47 2024, max compression
```

## Comparing `ozonetel-ai-0.0.12.tar` & `ozonetel-ai-0.0.121.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/ozoneai/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/ozoneai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 13:02:55.000000 ozonetel-ai-0.0.12/ozonetel_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:02:55.442077 ozonetel-ai-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-02 13:01:10.000000 ozonetel-ai-0.0.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/ozoneai/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/setup.py
```

### Comparing `ozonetel-ai-0.0.12/LICENSE` & `ozonetel-ai-0.0.121/LICENSE`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.12/PKG-INFO` & `ozonetel-ai-0.0.121/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.12
+Version: 0.0.121
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
@@ -47,33 +47,93 @@
         endcoder_modelid="BAAI/bge-m3") as embedder:
         emb = embedder.encode(["Try me Out"])
         emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     
     # Get bit representation
-    embedding_bits = emb_quantised.bits
-    
-    # Get unsigned binary
-    embedding_ubin = emb_quantised.ubinary()
-    
-    # Get signed binary
-    embedding_bin = emb_quantised.binary()
+    embeddings = emb_quantised.embedding
+
     ```
 
     If you want to check available embeddings you can do it as follows
     ```python
     from ozoneai.embeddings import list_models
 
     list_models()
     ```
 
+
 ## Examples
 
-- [search and index](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/main/examples/search-index/Text%20Indexing%20using%20OzoneAI%20Embeddings%20Faiss.ipynb)
+### Search And Index:
+
+```python
+
+import numpy as np, os
+from ozoneai.embeddings import QuantizeSentenceEmbedding
+
+# define credentials
+os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+
+# Documents to be Indexed
+docs = [
+    "The cat sits outside",
+    "A man is playing guitar",
+    "I love pasta",
+    "The new movie is awesome",
+    "The cat plays in the garden",
+    "A woman watches TV",
+    "The new movie is so great",
+    "Do you like pizza?",
+    "Artifical intelligence is all about enabling computers to simulate human capabilities.",
+    "Artifical intelligence is there to help human",
+    "Language moodel has lot of impact on artifical intelligence",
+    "Artifical intelligence is reigning in industry",
+    "ROI is one the useful measure for any investors",
+    "Understand before you invest"
+]
+
+# Extract Embeddings for documents to be indexed
+with QuantizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3"
+) as encoder:
+    docs_emb = encoder.encode(docs)
+    docs_emb_quantised = encoder.quantize(docs_emb, model="sieve-bge-m3-en-aug-v1")
+
+# Searching
+
+# query_text = "the girl was sitting in the park"
+query_text = "I love Artifical Intellegence"
+# query_text = "Artifical intellegence helps optimising software"
+# query_text = "what is machine learning"
+
+# Extract Embeddings query
+with QuantizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3"
+) as encoder:
+    query_emb = encoder.encode([query_text])
+    query_emb_quantised = encoder.quantize(query_emb, model="sieve-bge-m3-en-aug-v1")
+
+# compute distance of docs from query
+topn = 5
+dist_pbit = np.bitwise_xor(docs_emb_quantised.embedding, query_emb_quantised.embedding)
+dist_bit = np.unpackbits(dist_pbit, axis=1)
+dist = np.sum(dist_bit, axis=1)
+topn_indices = np.argsort(dist)[:topn]
+scores = (1 - (dist/(query_emb_quantised.embedding.shape[1]*8))).round(3)
+
+# Print search result in order
+for i, doci in enumerate(topn_indices):
+    print(f"{i}. {docs[doci]} [{doci}] ({scores[doci]})")
+
+
+```
+    
+[try more..](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/main/examples/search-index/)
 
 ## Benchmarks
 ### Classification
 | S.N | Dataset                                     | paraphrase-multilingual-mpnet-base-v2 | siv-sentence-bitnet-pmbv2-wikid-small | bge-m3 | sieve-bge-m3-en-aug-v0 | sieve-bge-m3-en-aug-v1 |
 |-----|---------------------------------------------|---------------------------------------|----------------------------------------|--------|------------------------|------------------------|
 | 1   | Amazon Counterfactual Classification(en)   | 75.81                                 | 79.06                                  | 75.63  | 79.23                  | 78.28                  |
 | 2   | Amazon Polarity Classification              | 76.41                                 | 70.19                                  | 91.01  | 86.81                  | 85.69                  |
```

### Comparing `ozonetel-ai-0.0.12/README.md` & `ozonetel-ai-0.0.121/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,33 +32,93 @@
         endcoder_modelid="BAAI/bge-m3") as embedder:
         emb = embedder.encode(["Try me Out"])
         emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     
     # Get bit representation
-    embedding_bits = emb_quantised.bits
-    
-    # Get unsigned binary
-    embedding_ubin = emb_quantised.ubinary()
-    
-    # Get signed binary
-    embedding_bin = emb_quantised.binary()
+    embeddings = emb_quantised.embedding
+
     ```
 
     If you want to check available embeddings you can do it as follows
     ```python
     from ozoneai.embeddings import list_models
 
     list_models()
     ```
 
+
 ## Examples
 
-- [search and index](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/main/examples/search-index/Text%20Indexing%20using%20OzoneAI%20Embeddings%20Faiss.ipynb)
+### Search And Index:
+
+```python
+
+import numpy as np, os
+from ozoneai.embeddings import QuantizeSentenceEmbedding
+
+# define credentials
+os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+
+# Documents to be Indexed
+docs = [
+    "The cat sits outside",
+    "A man is playing guitar",
+    "I love pasta",
+    "The new movie is awesome",
+    "The cat plays in the garden",
+    "A woman watches TV",
+    "The new movie is so great",
+    "Do you like pizza?",
+    "Artifical intelligence is all about enabling computers to simulate human capabilities.",
+    "Artifical intelligence is there to help human",
+    "Language moodel has lot of impact on artifical intelligence",
+    "Artifical intelligence is reigning in industry",
+    "ROI is one the useful measure for any investors",
+    "Understand before you invest"
+]
+
+# Extract Embeddings for documents to be indexed
+with QuantizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3"
+) as encoder:
+    docs_emb = encoder.encode(docs)
+    docs_emb_quantised = encoder.quantize(docs_emb, model="sieve-bge-m3-en-aug-v1")
+
+# Searching
+
+# query_text = "the girl was sitting in the park"
+query_text = "I love Artifical Intellegence"
+# query_text = "Artifical intellegence helps optimising software"
+# query_text = "what is machine learning"
+
+# Extract Embeddings query
+with QuantizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3"
+) as encoder:
+    query_emb = encoder.encode([query_text])
+    query_emb_quantised = encoder.quantize(query_emb, model="sieve-bge-m3-en-aug-v1")
+
+# compute distance of docs from query
+topn = 5
+dist_pbit = np.bitwise_xor(docs_emb_quantised.embedding, query_emb_quantised.embedding)
+dist_bit = np.unpackbits(dist_pbit, axis=1)
+dist = np.sum(dist_bit, axis=1)
+topn_indices = np.argsort(dist)[:topn]
+scores = (1 - (dist/(query_emb_quantised.embedding.shape[1]*8))).round(3)
+
+# Print search result in order
+for i, doci in enumerate(topn_indices):
+    print(f"{i}. {docs[doci]} [{doci}] ({scores[doci]})")
+
+
+```
+    
+[try more..](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/main/examples/search-index/)
 
 ## Benchmarks
 ### Classification
 | S.N | Dataset                                     | paraphrase-multilingual-mpnet-base-v2 | siv-sentence-bitnet-pmbv2-wikid-small | bge-m3 | sieve-bge-m3-en-aug-v0 | sieve-bge-m3-en-aug-v1 |
 |-----|---------------------------------------------|---------------------------------------|----------------------------------------|--------|------------------------|------------------------|
 | 1   | Amazon Counterfactual Classification(en)   | 75.81                                 | 79.06                                  | 75.63  | 79.23                  | 78.28                  |
 | 2   | Amazon Polarity Classification              | 76.41                                 | 70.19                                  | 91.01  | 86.81                  | 85.69                  |
```

### Comparing `ozonetel-ai-0.0.12/ozoneai/connector.py` & `ozonetel-ai-0.0.121/ozoneai/connector.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.12/ozoneai/embeddings.py` & `ozonetel-ai-0.0.121/ozoneai/embeddings.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.12/ozoneai/exception.py` & `ozonetel-ai-0.0.121/ozoneai/exception.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.12/ozoneai/models.py` & `ozonetel-ai-0.0.121/ozoneai/models.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.12/ozonetel_ai.egg-info/PKG-INFO` & `ozonetel-ai-0.0.121/ozonetel_ai.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.12
+Version: 0.0.121
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
@@ -47,33 +47,93 @@
         endcoder_modelid="BAAI/bge-m3") as embedder:
         emb = embedder.encode(["Try me Out"])
         emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     
     # Get bit representation
-    embedding_bits = emb_quantised.bits
-    
-    # Get unsigned binary
-    embedding_ubin = emb_quantised.ubinary()
-    
-    # Get signed binary
-    embedding_bin = emb_quantised.binary()
+    embeddings = emb_quantised.embedding
+
     ```
 
     If you want to check available embeddings you can do it as follows
     ```python
     from ozoneai.embeddings import list_models
 
     list_models()
     ```
 
+
 ## Examples
 
-- [search and index](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/main/examples/search-index/Text%20Indexing%20using%20OzoneAI%20Embeddings%20Faiss.ipynb)
+### Search And Index:
+
+```python
+
+import numpy as np, os
+from ozoneai.embeddings import QuantizeSentenceEmbedding
+
+# define credentials
+os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+
+# Documents to be Indexed
+docs = [
+    "The cat sits outside",
+    "A man is playing guitar",
+    "I love pasta",
+    "The new movie is awesome",
+    "The cat plays in the garden",
+    "A woman watches TV",
+    "The new movie is so great",
+    "Do you like pizza?",
+    "Artifical intelligence is all about enabling computers to simulate human capabilities.",
+    "Artifical intelligence is there to help human",
+    "Language moodel has lot of impact on artifical intelligence",
+    "Artifical intelligence is reigning in industry",
+    "ROI is one the useful measure for any investors",
+    "Understand before you invest"
+]
+
+# Extract Embeddings for documents to be indexed
+with QuantizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3"
+) as encoder:
+    docs_emb = encoder.encode(docs)
+    docs_emb_quantised = encoder.quantize(docs_emb, model="sieve-bge-m3-en-aug-v1")
+
+# Searching
+
+# query_text = "the girl was sitting in the park"
+query_text = "I love Artifical Intellegence"
+# query_text = "Artifical intellegence helps optimising software"
+# query_text = "what is machine learning"
+
+# Extract Embeddings query
+with QuantizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3"
+) as encoder:
+    query_emb = encoder.encode([query_text])
+    query_emb_quantised = encoder.quantize(query_emb, model="sieve-bge-m3-en-aug-v1")
+
+# compute distance of docs from query
+topn = 5
+dist_pbit = np.bitwise_xor(docs_emb_quantised.embedding, query_emb_quantised.embedding)
+dist_bit = np.unpackbits(dist_pbit, axis=1)
+dist = np.sum(dist_bit, axis=1)
+topn_indices = np.argsort(dist)[:topn]
+scores = (1 - (dist/(query_emb_quantised.embedding.shape[1]*8))).round(3)
+
+# Print search result in order
+for i, doci in enumerate(topn_indices):
+    print(f"{i}. {docs[doci]} [{doci}] ({scores[doci]})")
+
+
+```
+    
+[try more..](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/main/examples/search-index/)
 
 ## Benchmarks
 ### Classification
 | S.N | Dataset                                     | paraphrase-multilingual-mpnet-base-v2 | siv-sentence-bitnet-pmbv2-wikid-small | bge-m3 | sieve-bge-m3-en-aug-v0 | sieve-bge-m3-en-aug-v1 |
 |-----|---------------------------------------------|---------------------------------------|----------------------------------------|--------|------------------------|------------------------|
 | 1   | Amazon Counterfactual Classification(en)   | 75.81                                 | 79.06                                  | 75.63  | 79.23                  | 78.28                  |
 | 2   | Amazon Polarity Classification              | 76.41                                 | 70.19                                  | 91.01  | 86.81                  | 85.69                  |
```

### Comparing `ozonetel-ai-0.0.12/setup.py` & `ozonetel-ai-0.0.121/setup.py`

 * *Files identical despite different names*

