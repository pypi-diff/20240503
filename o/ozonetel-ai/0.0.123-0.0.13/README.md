# Comparing `tmp/ozonetel-ai-0.0.123.tar.gz` & `tmp/ozonetel-ai-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozonetel-ai-0.0.123.tar", last modified: Fri May  3 09:50:22 2024, max compression
+gzip compressed data, was "ozonetel-ai-0.0.13.tar", last modified: Fri May  3 10:20:02 2024, max compression
```

## Comparing `ozonetel-ai-0.0.123.tar` & `ozonetel-ai-0.0.13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:50:22.697244 ozonetel-ai-0.0.123/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-03 09:50:22.697244 ozonetel-ai-0.0.123/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:50:22.693244 ozonetel-ai-0.0.123/ozoneai/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/ozoneai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/ozoneai/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12516 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/ozoneai/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/ozoneai/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/ozoneai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:50:22.697244 ozonetel-ai-0.0.123/ozonetel_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-03 09:50:22.000000 ozonetel-ai-0.0.123/ozonetel_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 09:50:22.000000 ozonetel-ai-0.0.123/ozonetel_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:50:22.000000 ozonetel-ai-0.0.123/ozonetel_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 09:50:22.000000 ozonetel-ai-0.0.123/ozonetel_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 09:50:22.000000 ozonetel-ai-0.0.123/ozonetel_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:50:22.697244 ozonetel-ai-0.0.123/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-03 09:48:41.000000 ozonetel-ai-0.0.123/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:20:02.152714 ozonetel-ai-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-03 10:20:02.152714 ozonetel-ai-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:20:02.152714 ozonetel-ai-0.0.13/ozoneai/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/ozoneai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/ozoneai/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12516 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/ozoneai/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/ozoneai/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/ozoneai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:20:02.152714 ozonetel-ai-0.0.13/ozonetel_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-03 10:20:02.000000 ozonetel-ai-0.0.13/ozonetel_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 10:20:02.000000 ozonetel-ai-0.0.13/ozonetel_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:20:02.000000 ozonetel-ai-0.0.13/ozonetel_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 10:20:02.000000 ozonetel-ai-0.0.13/ozonetel_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 10:20:02.000000 ozonetel-ai-0.0.13/ozonetel_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:20:02.152714 ozonetel-ai-0.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-03 10:18:20.000000 ozonetel-ai-0.0.13/setup.py
```

### Comparing `ozonetel-ai-0.0.123/LICENSE` & `ozonetel-ai-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.123/PKG-INFO` & `ozonetel-ai-0.0.13/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.123
+Version: 0.0.13
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
@@ -32,29 +32,35 @@
     
     Example:
     
     ```python
     import os
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
+    or,
+    ``` python
+    credential = {"username":"", "bearer_token":""}
+    ```
 3. Text Embedding Extraction
     Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `BinarizeSentenceEmbedding` binarizes base embeddings and represents in bits.
 
    Example:
     ```python
     # Import `BinarizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
     from ozoneai.embeddings import BinarizeSentenceEmbedding
     
     # Extract Embeddings: Use the `binarize` method to obtain binarized embeddings for given texts .
     # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
     # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
-    with BinarizeSentenceEmbedding(
-        endcoder_modelid="BAAI/bge-m3") as embedder:
-        emb = embedder.encode(["Try me Out"])
-        emb_binarized = embedder.binarize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
+    
+    # Note: for safest use `OZAI_API_CREDENTIALS`. In that case `credential` argument can be ignored. if `credential` is not defined `OZAI_API_CREDENTIALS` will be considered.
+    binary_encoder = BinarizeSentenceEmbedding(endcoder_modelid="BAAI/bge-m3", credential = credential)
+
+    emb = binary_encoder.encode(["Try me Out"])
+    emb_binarized = binary_encoder.get_binary_embeddings(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     # Get binary representation
     embeddings = emb_binarized.embedding
 
     ```
```

### Comparing `ozonetel-ai-0.0.123/README.md` & `ozonetel-ai-0.0.13/ozonetel_ai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: ozonetel-ai
+Version: 0.0.13
+Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
+Home-page: 
+Author: Biswajit Satapathy
+Author-email: biswajit@ozonetel.com
+License: MIT License
+Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Ozonetel AI
 ## Overview
 The Ozonetel AI project is designed to provide a user-friendly interface for software development using Ozonetel's in-house AI libraries, models, and software solutions. It offers seamless integration with Ozonetel's advanced AI capabilities, allowing developers to harness the power of AI to enhance their applications.
 
 ## Features
 - Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
@@ -17,29 +32,35 @@
     
     Example:
     
     ```python
     import os
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
+    or,
+    ``` python
+    credential = {"username":"", "bearer_token":""}
+    ```
 3. Text Embedding Extraction
     Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `BinarizeSentenceEmbedding` binarizes base embeddings and represents in bits.
 
    Example:
     ```python
     # Import `BinarizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
     from ozoneai.embeddings import BinarizeSentenceEmbedding
     
     # Extract Embeddings: Use the `binarize` method to obtain binarized embeddings for given texts .
     # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
     # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
-    with BinarizeSentenceEmbedding(
-        endcoder_modelid="BAAI/bge-m3") as embedder:
-        emb = embedder.encode(["Try me Out"])
-        emb_binarized = embedder.binarize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
+    
+    # Note: for safest use `OZAI_API_CREDENTIALS`. In that case `credential` argument can be ignored. if `credential` is not defined `OZAI_API_CREDENTIALS` will be considered.
+    binary_encoder = BinarizeSentenceEmbedding(endcoder_modelid="BAAI/bge-m3", credential = credential)
+
+    emb = binary_encoder.encode(["Try me Out"])
+    emb_binarized = binary_encoder.get_binary_embeddings(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     # Get binary representation
     embeddings = emb_binarized.embedding
 
     ```
```

### Comparing `ozonetel-ai-0.0.123/ozoneai/connector.py` & `ozonetel-ai-0.0.13/ozoneai/connector.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.123/ozoneai/embeddings.py` & `ozonetel-ai-0.0.13/ozoneai/embeddings.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.123/ozoneai/exception.py` & `ozonetel-ai-0.0.13/ozoneai/exception.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.123/ozoneai/models.py` & `ozonetel-ai-0.0.13/ozoneai/models.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.123/ozonetel_ai.egg-info/PKG-INFO` & `ozonetel-ai-0.0.13/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ozonetel-ai
-Version: 0.0.123
-Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
-Home-page: 
-Author: Biswajit Satapathy
-Author-email: biswajit@ozonetel.com
-License: MIT License
-Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ozonetel AI
 ## Overview
 The Ozonetel AI project is designed to provide a user-friendly interface for software development using Ozonetel's in-house AI libraries, models, and software solutions. It offers seamless integration with Ozonetel's advanced AI capabilities, allowing developers to harness the power of AI to enhance their applications.
 
 ## Features
 - Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
@@ -32,29 +17,35 @@
     
     Example:
     
     ```python
     import os
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
+    or,
+    ``` python
+    credential = {"username":"", "bearer_token":""}
+    ```
 3. Text Embedding Extraction
     Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `BinarizeSentenceEmbedding` binarizes base embeddings and represents in bits.
 
    Example:
     ```python
     # Import `BinarizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
     from ozoneai.embeddings import BinarizeSentenceEmbedding
     
     # Extract Embeddings: Use the `binarize` method to obtain binarized embeddings for given texts .
     # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
     # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
-    with BinarizeSentenceEmbedding(
-        endcoder_modelid="BAAI/bge-m3") as embedder:
-        emb = embedder.encode(["Try me Out"])
-        emb_binarized = embedder.binarize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
+    
+    # Note: for safest use `OZAI_API_CREDENTIALS`. In that case `credential` argument can be ignored. if `credential` is not defined `OZAI_API_CREDENTIALS` will be considered.
+    binary_encoder = BinarizeSentenceEmbedding(endcoder_modelid="BAAI/bge-m3", credential = credential)
+
+    emb = binary_encoder.encode(["Try me Out"])
+    emb_binarized = binary_encoder.get_binary_embeddings(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     # Get binary representation
     embeddings = emb_binarized.embedding
 
     ```
```

### Comparing `ozonetel-ai-0.0.123/setup.py` & `ozonetel-ai-0.0.13/setup.py`

 * *Files identical despite different names*

