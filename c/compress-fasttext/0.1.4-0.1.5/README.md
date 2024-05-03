# Comparing `tmp/compress-fasttext-0.1.4.tar.gz` & `tmp/compress-fasttext-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compress-fasttext-0.1.4.tar", last modified: Sat Oct 14 19:59:30 2023, max compression
+gzip compressed data, was "compress-fasttext-0.1.5.tar", last modified: Fri May  3 06:32:10 2024, max compression
```

## Comparing `compress-fasttext-0.1.4.tar` & `compress-fasttext-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-10-14 19:59:30.719013 compress-fasttext-0.1.4/
--rw-rw-rw-   0        0        0     1088 2020-11-22 21:33:18.000000 compress-fasttext-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     7941 2023-10-14 19:59:30.718013 compress-fasttext-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2023-10-14 19:50:49.000000 compress-fasttext-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-10-14 19:59:30.666014 compress-fasttext-0.1.4/compress_fasttext/
--rw-rw-rw-   0        0        0      324 2021-12-16 10:00:50.000000 compress-fasttext-0.1.4/compress_fasttext/__init__.py
--rw-rw-rw-   0        0        0     9182 2021-12-16 10:00:50.000000 compress-fasttext-0.1.4/compress_fasttext/compress.py
--rw-rw-rw-   0        0        0     1164 2022-05-20 11:11:22.000000 compress-fasttext-0.1.4/compress_fasttext/decomposition.py
--rw-rw-rw-   0        0        0     1097 2021-12-16 10:00:50.000000 compress-fasttext-0.1.4/compress_fasttext/evaluation.py
--rw-rw-rw-   0        0        0     1147 2021-12-14 07:03:23.000000 compress-fasttext-0.1.4/compress_fasttext/feature_extraction.py
--rw-rw-rw-   0        0        0      121 2021-12-16 10:00:50.000000 compress-fasttext-0.1.4/compress_fasttext/models.py
--rw-rw-rw-   0        0        0     4646 2022-05-20 11:11:22.000000 compress-fasttext-0.1.4/compress_fasttext/navec_like.py
--rw-rw-rw-   0        0        0     5424 2023-10-14 19:49:35.000000 compress-fasttext-0.1.4/compress_fasttext/pq_encoder_light.py
--rw-rw-rw-   0        0        0     4444 2021-12-12 08:36:40.000000 compress-fasttext-0.1.4/compress_fasttext/prune.py
--rw-rw-rw-   0        0        0     1076 2023-10-14 19:46:17.000000 compress-fasttext-0.1.4/compress_fasttext/quantization.py
--rw-rw-rw-   0        0        0     1190 2021-12-16 10:00:50.000000 compress-fasttext-0.1.4/compress_fasttext/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-14 19:59:30.715023 compress-fasttext-0.1.4/compress_fasttext.egg-info/
--rw-rw-rw-   0        0        0     7941 2023-10-14 19:59:30.000000 compress-fasttext-0.1.4/compress_fasttext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-10-14 19:59:30.000000 compress-fasttext-0.1.4/compress_fasttext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-14 19:59:30.000000 compress-fasttext-0.1.4/compress_fasttext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-10-14 19:59:30.000000 compress-fasttext-0.1.4/compress_fasttext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-10-14 19:59:30.000000 compress-fasttext-0.1.4/compress_fasttext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-14 19:59:30.719013 compress-fasttext-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-10-14 19:46:36.000000 compress-fasttext-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:32:10.908797 compress-fasttext-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2020-11-22 21:33:18.000000 compress-fasttext-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     7941 2024-05-03 06:32:10.899793 compress-fasttext-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2023-10-14 19:50:49.000000 compress-fasttext-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 06:32:10.750794 compress-fasttext-0.1.5/compress_fasttext/
+-rw-rw-rw-   0        0        0      324 2021-12-16 10:00:50.000000 compress-fasttext-0.1.5/compress_fasttext/__init__.py
+-rw-rw-rw-   0        0        0     9182 2021-12-16 10:00:50.000000 compress-fasttext-0.1.5/compress_fasttext/compress.py
+-rw-rw-rw-   0        0        0     1164 2022-05-20 11:11:22.000000 compress-fasttext-0.1.5/compress_fasttext/decomposition.py
+-rw-rw-rw-   0        0        0     1097 2021-12-16 10:00:50.000000 compress-fasttext-0.1.5/compress_fasttext/evaluation.py
+-rw-rw-rw-   0        0        0     1147 2021-12-14 07:03:23.000000 compress-fasttext-0.1.5/compress_fasttext/feature_extraction.py
+-rw-rw-rw-   0        0        0      121 2021-12-16 10:00:50.000000 compress-fasttext-0.1.5/compress_fasttext/models.py
+-rw-rw-rw-   0        0        0     4646 2022-05-20 11:11:22.000000 compress-fasttext-0.1.5/compress_fasttext/navec_like.py
+-rw-rw-rw-   0        0        0     5430 2024-05-03 06:22:30.000000 compress-fasttext-0.1.5/compress_fasttext/pq_encoder_light.py
+-rw-rw-rw-   0        0        0     4444 2021-12-12 08:36:40.000000 compress-fasttext-0.1.5/compress_fasttext/prune.py
+-rw-rw-rw-   0        0        0     1076 2023-10-14 19:46:17.000000 compress-fasttext-0.1.5/compress_fasttext/quantization.py
+-rw-rw-rw-   0        0        0     1190 2021-12-16 10:00:50.000000 compress-fasttext-0.1.5/compress_fasttext/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:32:10.881793 compress-fasttext-0.1.5/compress_fasttext.egg-info/
+-rw-rw-rw-   0        0        0     7941 2024-05-03 06:32:09.000000 compress-fasttext-0.1.5/compress_fasttext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2024-05-03 06:32:09.000000 compress-fasttext-0.1.5/compress_fasttext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 06:32:09.000000 compress-fasttext-0.1.5/compress_fasttext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-03 06:32:09.000000 compress-fasttext-0.1.5/compress_fasttext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-03 06:32:09.000000 compress-fasttext-0.1.5/compress_fasttext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 06:32:10.910794 compress-fasttext-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      932 2024-05-03 06:26:15.000000 compress-fasttext-0.1.5/setup.py
```

### Comparing `compress-fasttext-0.1.4/LICENSE` & `compress-fasttext-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/PKG-INFO` & `compress-fasttext-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compress-fasttext
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of tools to compress gensim fasttext models
 Home-page: https://github.com/avidale/compress-fasttext
 Author: David Dale
 Author-email: dale.david@mail.ru
 License: MIT
 Description: # Compress-fastText
         This Python 3 package allows to compress fastText word embedding models
```

### Comparing `compress-fasttext-0.1.4/README.md` & `compress-fasttext-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/compress.py` & `compress-fasttext-0.1.5/compress_fasttext/compress.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/decomposition.py` & `compress-fasttext-0.1.5/compress_fasttext/decomposition.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/evaluation.py` & `compress-fasttext-0.1.5/compress_fasttext/evaluation.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/feature_extraction.py` & `compress-fasttext-0.1.5/compress_fasttext/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/navec_like.py` & `compress-fasttext-0.1.5/compress_fasttext/navec_like.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/pq_encoder_light.py` & `compress-fasttext-0.1.5/compress_fasttext/pq_encoder_light.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
         assert x_train.ndim == 2
         N, D = x_train.shape
         assert self.Ks < N, "the number of training vector should be more than Ks"
         assert D % self.M == 0, "input dimension must be dividable by M"
         self.Ds = int(D / self.M)
         assert self.trained_encoder is None, "fit must be called only once"
 
-        codewords = numpy.zeros((self.M, self.Ks, self.Ds), dtype=numpy.float)
+        codewords = numpy.zeros((self.M, self.Ks, self.Ds), dtype=numpy.float32)
         for m in range(self.M):
-            x_train_sub = x_train[:, m * self.Ds: (m + 1) * self.Ds].astype(numpy.float)
+            x_train_sub = x_train[:, m * self.Ds: (m + 1) * self.Ds].astype(numpy.float32)
             codewords[m], _ = kmeans2(x_train_sub, self.Ks, iter=self.iteration, minit='points')
         self.trained_encoder = TrainedPQEncoder(codewords, self.code_dtype)
 
     def transform_generator(self, x_test):
         # type: (typing.Iterable[typing.Iterator[float]]) -> Any
         assert self.trained_encoder is not None, "This PQEncoder instance is not fitted yet. " \
                                                  "Call 'fit' with appropriate arguments before using thie method."
@@ -113,11 +113,11 @@
 
     def decode_multi(self, codes):
         codes = numpy.array(codes)
         N, M = codes.shape
         assert M == self.M
         assert codes.dtype == self.code_dtype
 
-        decoded = numpy.empty((N, self.Ds * self.M), dtype=numpy.float)
+        decoded = numpy.empty((N, self.Ds * self.M), dtype=numpy.float32)
         for m in range(self.M):
             decoded[:, m * self.Ds: (m + 1) * self.Ds] = self.codewords[m][codes[:, m], :]
         return decoded
```

### Comparing `compress-fasttext-0.1.4/compress_fasttext/prune.py` & `compress-fasttext-0.1.5/compress_fasttext/prune.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/quantization.py` & `compress-fasttext-0.1.5/compress_fasttext/quantization.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext/utils.py` & `compress-fasttext-0.1.5/compress_fasttext/utils.py`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/compress_fasttext.egg-info/PKG-INFO` & `compress-fasttext-0.1.5/compress_fasttext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compress-fasttext
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of tools to compress gensim fasttext models
 Home-page: https://github.com/avidale/compress-fasttext
 Author: David Dale
 Author-email: dale.david@mail.ru
 License: MIT
 Description: # Compress-fastText
         This Python 3 package allows to compress fastText word embedding models
```

### Comparing `compress-fasttext-0.1.4/compress_fasttext.egg-info/SOURCES.txt` & `compress-fasttext-0.1.5/compress_fasttext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compress-fasttext-0.1.4/setup.py` & `compress-fasttext-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="compress-fasttext",
-    version="0.1.4",
+    version="0.1.5",
     author="David Dale",
     author_email="dale.david@mail.ru",
     description="A set of tools to compress gensim fasttext models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/avidale/compress-fasttext",
     packages=['compress_fasttext'],
```

