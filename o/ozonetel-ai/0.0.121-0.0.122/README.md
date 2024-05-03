# Comparing `tmp/ozonetel-ai-0.0.121.tar.gz` & `tmp/ozonetel-ai-0.0.122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozonetel-ai-0.0.121.tar", last modified: Fri May  3 05:55:47 2024, max compression
+gzip compressed data, was "ozonetel-ai-0.0.122.tar", last modified: Fri May  3 08:58:22 2024, max compression
```

## Comparing `ozonetel-ai-0.0.121.tar` & `ozonetel-ai-0.0.122.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/ozoneai/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/ozoneai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 05:55:47.000000 ozonetel-ai-0.0.121/ozonetel_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:55:47.101814 ozonetel-ai-0.0.121/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-03 05:54:05.000000 ozonetel-ai-0.0.121/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:58:22.990476 ozonetel-ai-0.0.122/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-03 08:58:22.990476 ozonetel-ai-0.0.122/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:58:22.986476 ozonetel-ai-0.0.122/ozoneai/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/ozoneai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/ozoneai/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/ozoneai/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/ozoneai/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/ozoneai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:58:22.990476 ozonetel-ai-0.0.122/ozonetel_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-03 08:58:22.000000 ozonetel-ai-0.0.122/ozonetel_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 08:58:22.000000 ozonetel-ai-0.0.122/ozonetel_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:58:22.000000 ozonetel-ai-0.0.122/ozonetel_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 08:58:22.000000 ozonetel-ai-0.0.122/ozonetel_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 08:58:22.000000 ozonetel-ai-0.0.122/ozonetel_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 08:58:22.990476 ozonetel-ai-0.0.122/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-03 08:54:43.000000 ozonetel-ai-0.0.122/setup.py
```

### Comparing `ozonetel-ai-0.0.121/LICENSE` & `ozonetel-ai-0.0.122/LICENSE`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.121/PKG-INFO` & `ozonetel-ai-0.0.122/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.121
+Version: 0.0.122
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
@@ -19,43 +19,46 @@
 
 ## Features
 - Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
 ## Getting Started
 To get started with the Ozonetel AI project, follow the steps below:
 
-1. Set Credentials:
+1. Installation
+   ```bash
+   pip install ozonetel-ai
+   ```
+2. Set Credentials:
     Before using the text embedding feature, set your credentials by importing the os module and setting the `OZAI_API_CREDENTIALS` environment variable to point to your credentials file.
     
     Example:
     
     ```python
     import os
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
 3. Text Embedding Extraction
-    Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `QuantizeSentenceEmbedding` quantizes base embeddings and represents in bits.
+    Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `BinarizeSentenceEmbedding` binarizes base embeddings and represents in bits.
 
    Example:
     ```python
-    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
-    from ozoneai.embeddings import QuantizeSentenceEmbedding
+    # Import `BinarizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
+    from ozoneai.embeddings import BinarizeSentenceEmbedding
     
-    # Extract Embeddings: Use the `quantize` method to obtain quantised embeddings for given texts .
+    # Extract Embeddings: Use the `binarize` method to obtain binarized embeddings for given texts .
     # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
     # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
-    with QuantizeSentenceEmbedding(
+    with BinarizeSentenceEmbedding(
         endcoder_modelid="BAAI/bge-m3") as embedder:
         emb = embedder.encode(["Try me Out"])
-        emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
+        emb_binarized = embedder.binarize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
-    
-    # Get bit representation
-    embeddings = emb_quantised.embedding
+    # Get binary representation
+    embeddings = emb_binarized.embedding
 
     ```
 
     If you want to check available embeddings you can do it as follows
     ```python
     from ozoneai.embeddings import list_models
 
@@ -66,18 +69,22 @@
 ## Examples
 
 ### Search And Index:
 
 ```python
 
 import numpy as np, os
-from ozoneai.embeddings import QuantizeSentenceEmbedding
+from ozoneai.embeddings import BinarizeEmbedding
+
+from sentence_transformers import SentenceTransformer
+base_model = SentenceTransformer("BAAI/bge-m3")
 
 # define credentials
-os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+# os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+credential = {"username":"", "bearer_token":""}
 
 # Documents to be Indexed
 docs = [
     "The cat sits outside",
     "A man is playing guitar",
     "I love pasta",
     "The new movie is awesome",
@@ -90,41 +97,49 @@
     "Language moodel has lot of impact on artifical intelligence",
     "Artifical intelligence is reigning in industry",
     "ROI is one the useful measure for any investors",
     "Understand before you invest"
 ]
 
 # Extract Embeddings for documents to be indexed
-with QuantizeSentenceEmbedding(
-    endcoder_modelid="BAAI/bge-m3"
+docs_emb = base_model.encode(docs)
+
+# Binarise embeedings
+with BinarizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3",
+    credential=credential
 ) as encoder:
-    docs_emb = encoder.encode(docs)
-    docs_emb_quantised = encoder.quantize(docs_emb, model="sieve-bge-m3-en-aug-v1")
+    docs_emb_binarized = encoder.binarize(docs_emb, model="sieve-bge-m3-en-aug-v1")
 
 # Searching
 
 # query_text = "the girl was sitting in the park"
 query_text = "I love Artifical Intellegence"
 # query_text = "Artifical intellegence helps optimising software"
 # query_text = "what is machine learning"
 
 # Extract Embeddings query
-with QuantizeSentenceEmbedding(
-    endcoder_modelid="BAAI/bge-m3"
-) as encoder:
-    query_emb = encoder.encode([query_text])
-    query_emb_quantised = encoder.quantize(query_emb, model="sieve-bge-m3-en-aug-v1")
+
+# Compute sentence embedding using SentenceTransformers (i.e. bge-m3 or paraphrase-multilingual-mpnet-base-v2)
+query_emb = base_model.encode([query_text])
+
+# Binarise embeedings
+with BinarizeEmbedding(
+    endcoder_modelid="BAAI/bge-m3",
+    credential=credential
+) as encoder:    
+    query_emb_binarized = encoder.binarize(query_emb, model="sieve-bge-m3-en-aug-v1")
 
 # compute distance of docs from query
 topn = 5
-dist_pbit = np.bitwise_xor(docs_emb_quantised.embedding, query_emb_quantised.embedding)
+dist_pbit = np.bitwise_xor(docs_emb_binarized.embedding, query_emb_binarized.embedding)
 dist_bit = np.unpackbits(dist_pbit, axis=1)
 dist = np.sum(dist_bit, axis=1)
 topn_indices = np.argsort(dist)[:topn]
-scores = (1 - (dist/(query_emb_quantised.embedding.shape[1]*8))).round(3)
+scores = (1 - (dist/(query_emb_binarized.embedding.shape[1]*8))).round(3)
 
 # Print search result in order
 for i, doci in enumerate(topn_indices):
     print(f"{i}. {docs[doci]} [{doci}] ({scores[doci]})")
 
 
 ```
```

### Comparing `ozonetel-ai-0.0.121/README.md` & `ozonetel-ai-0.0.122/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,43 +4,46 @@
 
 ## Features
 - Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
 ## Getting Started
 To get started with the Ozonetel AI project, follow the steps below:
 
-1. Set Credentials:
+1. Installation
+   ```bash
+   pip install ozonetel-ai
+   ```
+2. Set Credentials:
     Before using the text embedding feature, set your credentials by importing the os module and setting the `OZAI_API_CREDENTIALS` environment variable to point to your credentials file.
     
     Example:
     
     ```python
     import os
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
 3. Text Embedding Extraction
-    Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `QuantizeSentenceEmbedding` quantizes base embeddings and represents in bits.
+    Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `BinarizeSentenceEmbedding` binarizes base embeddings and represents in bits.
 
    Example:
     ```python
-    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
-    from ozoneai.embeddings import QuantizeSentenceEmbedding
+    # Import `BinarizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
+    from ozoneai.embeddings import BinarizeSentenceEmbedding
     
-    # Extract Embeddings: Use the `quantize` method to obtain quantised embeddings for given texts .
+    # Extract Embeddings: Use the `binarize` method to obtain binarized embeddings for given texts .
     # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
     # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
-    with QuantizeSentenceEmbedding(
+    with BinarizeSentenceEmbedding(
         endcoder_modelid="BAAI/bge-m3") as embedder:
         emb = embedder.encode(["Try me Out"])
-        emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
+        emb_binarized = embedder.binarize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
-    
-    # Get bit representation
-    embeddings = emb_quantised.embedding
+    # Get binary representation
+    embeddings = emb_binarized.embedding
 
     ```
 
     If you want to check available embeddings you can do it as follows
     ```python
     from ozoneai.embeddings import list_models
 
@@ -51,18 +54,22 @@
 ## Examples
 
 ### Search And Index:
 
 ```python
 
 import numpy as np, os
-from ozoneai.embeddings import QuantizeSentenceEmbedding
+from ozoneai.embeddings import BinarizeEmbedding
+
+from sentence_transformers import SentenceTransformer
+base_model = SentenceTransformer("BAAI/bge-m3")
 
 # define credentials
-os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+# os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+credential = {"username":"", "bearer_token":""}
 
 # Documents to be Indexed
 docs = [
     "The cat sits outside",
     "A man is playing guitar",
     "I love pasta",
     "The new movie is awesome",
@@ -75,41 +82,49 @@
     "Language moodel has lot of impact on artifical intelligence",
     "Artifical intelligence is reigning in industry",
     "ROI is one the useful measure for any investors",
     "Understand before you invest"
 ]
 
 # Extract Embeddings for documents to be indexed
-with QuantizeSentenceEmbedding(
-    endcoder_modelid="BAAI/bge-m3"
+docs_emb = base_model.encode(docs)
+
+# Binarise embeedings
+with BinarizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3",
+    credential=credential
 ) as encoder:
-    docs_emb = encoder.encode(docs)
-    docs_emb_quantised = encoder.quantize(docs_emb, model="sieve-bge-m3-en-aug-v1")
+    docs_emb_binarized = encoder.binarize(docs_emb, model="sieve-bge-m3-en-aug-v1")
 
 # Searching
 
 # query_text = "the girl was sitting in the park"
 query_text = "I love Artifical Intellegence"
 # query_text = "Artifical intellegence helps optimising software"
 # query_text = "what is machine learning"
 
 # Extract Embeddings query
-with QuantizeSentenceEmbedding(
-    endcoder_modelid="BAAI/bge-m3"
-) as encoder:
-    query_emb = encoder.encode([query_text])
-    query_emb_quantised = encoder.quantize(query_emb, model="sieve-bge-m3-en-aug-v1")
+
+# Compute sentence embedding using SentenceTransformers (i.e. bge-m3 or paraphrase-multilingual-mpnet-base-v2)
+query_emb = base_model.encode([query_text])
+
+# Binarise embeedings
+with BinarizeEmbedding(
+    endcoder_modelid="BAAI/bge-m3",
+    credential=credential
+) as encoder:    
+    query_emb_binarized = encoder.binarize(query_emb, model="sieve-bge-m3-en-aug-v1")
 
 # compute distance of docs from query
 topn = 5
-dist_pbit = np.bitwise_xor(docs_emb_quantised.embedding, query_emb_quantised.embedding)
+dist_pbit = np.bitwise_xor(docs_emb_binarized.embedding, query_emb_binarized.embedding)
 dist_bit = np.unpackbits(dist_pbit, axis=1)
 dist = np.sum(dist_bit, axis=1)
 topn_indices = np.argsort(dist)[:topn]
-scores = (1 - (dist/(query_emb_quantised.embedding.shape[1]*8))).round(3)
+scores = (1 - (dist/(query_emb_binarized.embedding.shape[1]*8))).round(3)
 
 # Print search result in order
 for i, doci in enumerate(topn_indices):
     print(f"{i}. {docs[doci]} [{doci}] ({scores[doci]})")
 
 
 ```
```

### Comparing `ozonetel-ai-0.0.121/ozoneai/connector.py` & `ozonetel-ai-0.0.122/ozoneai/connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 
 from .exception import AuthenticationError
 
 class EmbeddingEndpoints:
     baseurl = "https://speech-kws.ozonetel.com"
     root = urljoin(baseurl, "embeddings/")
     get_embedding = urljoin(root, "text/embedding/get/")
-    quantize = urljoin(root, "text/embedding/quantize/")
+    binarize = urljoin(root, "text/embedding/quantize/")
     url_details = parse_url(baseurl)
     max_retries = 3
     backoff_factor = 0.3
 
 # Embedder Client
 class EmbeddingConnector(object):
     """Ozone Embedder Client Application"""
-    def __init__(self) -> None:
+    def __init__(self, credential=None) -> None:
         super(EmbeddingConnector, self).__init__()
-        credfile = os.environ.get('OZAI_API_CREDENTIALS')
-        if not credfile:
-            raise AuthenticationError(f"No credentials found!\nexport `OZAI_API_CREDENTIALS` before importing the module.")
-        if not os.path.exists(credfile):
-            raise AuthenticationError(f"Invalid credentials found!\n check if `OZAI_API_CREDENTIALS` valid!")
         
-        with open(credfile) as fp:
-            credential = json.load(fp)
-            if not "username" in credential:
-                raise AuthenticationError(f"`username` missing in credentials!")
-            if not "bearer_token" in credential:
-                raise AuthenticationError(f"`bearer_token` missing in credentials!")
+        if not credential:
+            credfile = os.environ.get('OZAI_API_CREDENTIALS')
+            if not credfile:
+                raise AuthenticationError(f"No credentials found!\nexport `OZAI_API_CREDENTIALS` before importing the module.")
+            if not os.path.exists(credfile):
+                raise AuthenticationError(f"Invalid credentials found!\n check if `OZAI_API_CREDENTIALS` valid!")
+            
+            with open(credfile) as fp:
+                credential = json.load(fp)
+                if not "username" in credential:
+                    raise AuthenticationError(f"`username` missing in credentials!")
+                if not "bearer_token" in credential:
+                    raise AuthenticationError(f"`bearer_token` missing in credentials!")
         
         self.username = credential["username"]
         self.bearer_token = credential["bearer_token"]
         self.endpoints = EmbeddingEndpoints
         self.url_details = self.endpoints.url_details
         self.max_retries = self.endpoints.max_retries
         self.backoff_factor = self.endpoints.backoff_factor
```

### Comparing `ozonetel-ai-0.0.121/ozoneai/embeddings.py` & `ozonetel-ai-0.0.122/ozoneai/embeddings.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     
     def ubinary(self):
         return self.embedding
     
     def binary(self):
         return (self.embedding - 128).astype(np.int8)
     
-class QuantizedEmbeddings(object):
+class BinarizedEmbeddings(object):
     def __init__(self, model) -> None:
         self.name = model
         
     def parse(self, response):
         if not "is_error" in response:
             raise AssertionError("API Error!")
 
@@ -67,17 +67,17 @@
     
     def binary(self):
         return (self.embedding - 128).astype(np.int8)
         
 
 class TextEmbedding(object):
     """Ozone Embedder Client Application"""
-    def __init__(self) -> None:
+    def __init__(self, credential=None) -> None:
         super(TextEmbedding, self).__init__()
-        self.connector = EmbeddingConnector()
+        self.connector = EmbeddingConnector(credential)
         self.models = EmbeddingModels.models
 
     def connect(self):
         self.connector.connect()
 
     def close(self):
         self.connector.close()
@@ -119,21 +119,22 @@
             headers=headers, 
             json=data
         )
         embeddings = Embeddings(model)
         r = response.json()
         return embeddings.parse(r)
     
-class QuantizeEmbedding(object):
+class BinarizeEmbedding(object):
     """Ozone Embedder Client Application"""
-    def __init__(self, endcoder_modelid:str = "sieve-bge-m3-en-aug-v1") -> None:
-        super(QuantizeEmbedding, self).__init__()
-        self.connector = EmbeddingConnector()
+    def __init__(self, endcoder_modelid:str = "sieve-bge-m3-en-aug-v1", credential=None) -> None:
+        super(BinarizeEmbedding, self).__init__()
+        self.connector = EmbeddingConnector(credential)
         self.models = EmbeddingModels.models
         self.allowed_encoders = EmbeddingModels.encoders
+        self.model_maps = EmbeddingModels
         self.encoder_name = os.path.basename(endcoder_modelid.rstrip("/"))
         
         if not self.encoder_name in self.allowed_encoders:
             raise NotImplementedError(f"""Encoder provided is not supported! choose one of {self.allowed_encoders} .""")
         
     def connect(self):
         self.connector.connect()
@@ -147,21 +148,21 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
         
     def __del__(self):
         self.close()
 
-    def quantize(self, embedding: np.ndarray, model:str):
+    def binarize(self, embedding: np.ndarray, model:str):
         f"""
         embedding: text embeddings [ no_of_tokens * embeddings_dim ]
         model: {"or, ".join(self.models)}
         """
-        if not model in self.models:
-            raise ValueError("invalid model input!\nselect one from {self.models}")
+        if not model in self.model_maps.encoders_model_map[self.encoder_name]:
+            raise ValueError(f"invalid model input!\n {model} is not type of {self.encoder_name}")
         
         if len(embedding.shape) == 1:
             embedding = np.array([embedding])
         
         headers = {
             "accept": "application/json",
             "Authorization": f"Bearer {self.connector.bearer_token}",
@@ -171,26 +172,26 @@
         data = json.dumps({
             "vectors": embedding.astype(str).tolist(),
             "embedder_name": model,
             "base_model": self.encoder_name
         })
 
         response = self.connector.connection.post(
-            self.connector.endpoints.quantize,
+            self.connector.endpoints.binarize,
             headers=headers, 
             data=data
         )
-        embeddings = QuantizedEmbeddings(model)
+        embeddings = BinarizedEmbeddings(model)
         return embeddings.parse(response.json())
 
-class QuantizeSentenceEmbedding(object):
+class BinarizeSentenceEmbedding(object):
     """Ozone Embedder Client Application"""
-    def __init__(self, endcoder_modelid:str ="", device:str ="cpu") -> None:
-        super(QuantizeSentenceEmbedding, self).__init__()
-        self.connector = EmbeddingConnector()
+    def __init__(self, endcoder_modelid:str ="", device:str ="cpu", credential=None) -> None:
+        super(BinarizeSentenceEmbedding, self).__init__()
+        self.connector = EmbeddingConnector(credential)
         self.models = EmbeddingModels.models
         self.allowed_encoders = EmbeddingModels.encoders
         self.model_maps = EmbeddingModels
         
         self.encoder_name = os.path.basename(endcoder_modelid.rstrip("/"))
         
         if not self.encoder_name in self.allowed_encoders:
@@ -224,15 +225,15 @@
             verbose (bool, optional): _description_. Defaults to False.
 
         Returns:
             _type_: _description_
         """
         return self.embedder.encode(texts, batch_size=batch_size, show_progress_bar=verbose)
         
-    def quantize(self, embedding: np.ndarray, model:str):
+    def binarize(self, embedding: np.ndarray, model:str):
         f"""
         embedding: text embeddings [ no_of_tokens * embeddings_dim ]
         model: {"or, ".join(self.models)}
         """
         if not model in self.model_maps.encoders_model_map[self.encoder_name]:
             raise ValueError(f"invalid model input!\n {model} is not type of {self.encoder_name}")
         
@@ -251,15 +252,15 @@
         data = json.dumps({
             "vectors": embedding.astype(str).tolist(),
             "embedder_name": model,
             "base_model": self.encoder_name
         })
 
         response = self.connector.connection.post(
-            self.connector.endpoints.quantize,
+            self.connector.endpoints.binarize,
             headers=headers, 
             data=data
         )
 
-        embeddings = QuantizedEmbeddings(model)
+        embeddings = BinarizedEmbeddings(model)
         r = response.json()
         return embeddings.parse(r)
```

### Comparing `ozonetel-ai-0.0.121/ozoneai/exception.py` & `ozonetel-ai-0.0.122/ozoneai/exception.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.121/ozoneai/models.py` & `ozonetel-ai-0.0.122/ozoneai/models.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.121/ozonetel_ai.egg-info/PKG-INFO` & `ozonetel-ai-0.0.122/ozonetel_ai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.121
+Version: 0.0.122
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
@@ -19,43 +19,46 @@
 
 ## Features
 - Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
 ## Getting Started
 To get started with the Ozonetel AI project, follow the steps below:
 
-1. Set Credentials:
+1. Installation
+   ```bash
+   pip install ozonetel-ai
+   ```
+2. Set Credentials:
     Before using the text embedding feature, set your credentials by importing the os module and setting the `OZAI_API_CREDENTIALS` environment variable to point to your credentials file.
     
     Example:
     
     ```python
     import os
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
 3. Text Embedding Extraction
-    Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `QuantizeSentenceEmbedding` quantizes base embeddings and represents in bits.
+    Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `BinarizeSentenceEmbedding` binarizes base embeddings and represents in bits.
 
    Example:
     ```python
-    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
-    from ozoneai.embeddings import QuantizeSentenceEmbedding
+    # Import `BinarizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
+    from ozoneai.embeddings import BinarizeSentenceEmbedding
     
-    # Extract Embeddings: Use the `quantize` method to obtain quantised embeddings for given texts .
+    # Extract Embeddings: Use the `binarize` method to obtain binarized embeddings for given texts .
     # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
     # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
-    with QuantizeSentenceEmbedding(
+    with BinarizeSentenceEmbedding(
         endcoder_modelid="BAAI/bge-m3") as embedder:
         emb = embedder.encode(["Try me Out"])
-        emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
+        emb_binarized = embedder.binarize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
-    
-    # Get bit representation
-    embeddings = emb_quantised.embedding
+    # Get binary representation
+    embeddings = emb_binarized.embedding
 
     ```
 
     If you want to check available embeddings you can do it as follows
     ```python
     from ozoneai.embeddings import list_models
 
@@ -66,18 +69,22 @@
 ## Examples
 
 ### Search And Index:
 
 ```python
 
 import numpy as np, os
-from ozoneai.embeddings import QuantizeSentenceEmbedding
+from ozoneai.embeddings import BinarizeEmbedding
+
+from sentence_transformers import SentenceTransformer
+base_model = SentenceTransformer("BAAI/bge-m3")
 
 # define credentials
-os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+# os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
+credential = {"username":"", "bearer_token":""}
 
 # Documents to be Indexed
 docs = [
     "The cat sits outside",
     "A man is playing guitar",
     "I love pasta",
     "The new movie is awesome",
@@ -90,41 +97,49 @@
     "Language moodel has lot of impact on artifical intelligence",
     "Artifical intelligence is reigning in industry",
     "ROI is one the useful measure for any investors",
     "Understand before you invest"
 ]
 
 # Extract Embeddings for documents to be indexed
-with QuantizeSentenceEmbedding(
-    endcoder_modelid="BAAI/bge-m3"
+docs_emb = base_model.encode(docs)
+
+# Binarise embeedings
+with BinarizeSentenceEmbedding(
+    endcoder_modelid="BAAI/bge-m3",
+    credential=credential
 ) as encoder:
-    docs_emb = encoder.encode(docs)
-    docs_emb_quantised = encoder.quantize(docs_emb, model="sieve-bge-m3-en-aug-v1")
+    docs_emb_binarized = encoder.binarize(docs_emb, model="sieve-bge-m3-en-aug-v1")
 
 # Searching
 
 # query_text = "the girl was sitting in the park"
 query_text = "I love Artifical Intellegence"
 # query_text = "Artifical intellegence helps optimising software"
 # query_text = "what is machine learning"
 
 # Extract Embeddings query
-with QuantizeSentenceEmbedding(
-    endcoder_modelid="BAAI/bge-m3"
-) as encoder:
-    query_emb = encoder.encode([query_text])
-    query_emb_quantised = encoder.quantize(query_emb, model="sieve-bge-m3-en-aug-v1")
+
+# Compute sentence embedding using SentenceTransformers (i.e. bge-m3 or paraphrase-multilingual-mpnet-base-v2)
+query_emb = base_model.encode([query_text])
+
+# Binarise embeedings
+with BinarizeEmbedding(
+    endcoder_modelid="BAAI/bge-m3",
+    credential=credential
+) as encoder:    
+    query_emb_binarized = encoder.binarize(query_emb, model="sieve-bge-m3-en-aug-v1")
 
 # compute distance of docs from query
 topn = 5
-dist_pbit = np.bitwise_xor(docs_emb_quantised.embedding, query_emb_quantised.embedding)
+dist_pbit = np.bitwise_xor(docs_emb_binarized.embedding, query_emb_binarized.embedding)
 dist_bit = np.unpackbits(dist_pbit, axis=1)
 dist = np.sum(dist_bit, axis=1)
 topn_indices = np.argsort(dist)[:topn]
-scores = (1 - (dist/(query_emb_quantised.embedding.shape[1]*8))).round(3)
+scores = (1 - (dist/(query_emb_binarized.embedding.shape[1]*8))).round(3)
 
 # Print search result in order
 for i, doci in enumerate(topn_indices):
     print(f"{i}. {docs[doci]} [{doci}] ({scores[doci]})")
 
 
 ```
```

### Comparing `ozonetel-ai-0.0.121/setup.py` & `ozonetel-ai-0.0.122/setup.py`

 * *Files identical despite different names*

