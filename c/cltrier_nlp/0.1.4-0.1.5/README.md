# Comparing `tmp/cltrier_nlp-0.1.4.tar.gz` & `tmp/cltrier_nlp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltrier_nlp-0.1.4.tar", max compression
+gzip compressed data, was "cltrier_nlp-0.1.5.tar", max compression
```

## Comparing `cltrier_nlp-0.1.4.tar` & `cltrier_nlp-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      633 2024-04-30 12:36:28.308254 cltrier_nlp-0.1.4/README.md
--rw-r--r--   0        0        0      513 2024-05-02 13:39:38.069285 cltrier_nlp-0.1.4/cltrier_nlp/__init__.py
--rw-r--r--   0        0        0     3357 2024-05-02 13:49:31.124909 cltrier_nlp-0.1.4/cltrier_nlp/corpus/__init__.py
--rw-r--r--   0        0        0     1601 2024-05-02 13:49:44.304304 cltrier_nlp-0.1.4/cltrier_nlp/corpus/sentence.py
--rw-r--r--   0        0        0     3041 2024-05-02 13:39:16.910298 cltrier_nlp-0.1.4/cltrier_nlp/encoder/__init__.py
--rw-r--r--   0        0        0      764 2024-05-02 13:20:39.672728 cltrier_nlp-0.1.4/cltrier_nlp/encoder/batch.py
--rw-r--r--   0        0        0     2556 2024-05-02 13:44:28.872227 cltrier_nlp-0.1.4/cltrier_nlp/encoder/pooler.py
--rw-r--r--   0        0        0      454 2024-05-02 13:42:32.691002 cltrier_nlp-0.1.4/cltrier_nlp/functional/__init__.py
--rw-r--r--   0        0        0      489 2024-05-02 13:21:35.690210 cltrier_nlp-0.1.4/cltrier_nlp/functional/neural.py
--rw-r--r--   0        0        0     1454 2024-05-02 13:21:45.699761 cltrier_nlp-0.1.4/cltrier_nlp/functional/text.py
--rw-r--r--   0        0        0       49 2024-05-02 13:38:50.221580 cltrier_nlp-0.1.4/cltrier_nlp/utility/__init__.py
--rw-r--r--   0        0        0      683 2024-05-02 13:22:04.985564 cltrier_nlp-0.1.4/cltrier_nlp/utility/map.py
--rw-r--r--   0        0        0     1250 2024-05-02 13:53:34.547101 cltrier_nlp-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      633 2024-04-30 12:36:28.308254 cltrier_nlp-0.1.5/README.md
+-rw-r--r--   0        0        0      513 2024-05-02 13:39:38.069285 cltrier_nlp-0.1.5/cltrier_nlp/__init__.py
+-rw-r--r--   0        0        0     3357 2024-05-02 13:49:31.124909 cltrier_nlp-0.1.5/cltrier_nlp/corpus/__init__.py
+-rw-r--r--   0        0        0     1635 2024-05-02 13:56:48.991581 cltrier_nlp-0.1.5/cltrier_nlp/corpus/sentence.py
+-rw-r--r--   0        0        0     3041 2024-05-02 13:39:16.910298 cltrier_nlp-0.1.5/cltrier_nlp/encoder/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-02 13:20:39.672728 cltrier_nlp-0.1.5/cltrier_nlp/encoder/batch.py
+-rw-r--r--   0        0        0     2556 2024-05-02 13:44:28.872227 cltrier_nlp-0.1.5/cltrier_nlp/encoder/pooler.py
+-rw-r--r--   0        0        0      454 2024-05-02 13:42:32.691002 cltrier_nlp-0.1.5/cltrier_nlp/functional/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-02 13:21:35.690210 cltrier_nlp-0.1.5/cltrier_nlp/functional/neural.py
+-rw-r--r--   0        0        0     1454 2024-05-02 13:21:45.699761 cltrier_nlp-0.1.5/cltrier_nlp/functional/text.py
+-rw-r--r--   0        0        0       49 2024-05-02 13:38:50.221580 cltrier_nlp-0.1.5/cltrier_nlp/utility/__init__.py
+-rw-r--r--   0        0        0      683 2024-05-02 13:22:04.985564 cltrier_nlp-0.1.5/cltrier_nlp/utility/map.py
+-rw-r--r--   0        0        0     1250 2024-05-02 15:16:51.312853 cltrier_nlp-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.5/PKG-INFO
```

### Comparing `cltrier_nlp-0.1.4/README.md` & `cltrier_nlp-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/__init__.py` & `cltrier_nlp-0.1.5/cltrier_nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/corpus/__init__.py` & `cltrier_nlp-0.1.5/cltrier_nlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/corpus/sentence.py` & `cltrier_nlp-0.1.5/cltrier_nlp/corpus/sentence.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import typing
 
 import pandas
 import pydantic
 
 from .. import functional
 
+UNK_LANG: str = 'unknown'
+
 
 class Sentence(pydantic.BaseModel):
     """
 
     """
     raw: str
 
-    language: str = 'unknown'
+    language: str = UNK_LANG
     tokens: typing.List[str] = pydantic.Field(default_factory=lambda: [])
 
     def model_post_init(self, __context) -> None:
         """
 
         """
         self.raw = self.raw.replace("\n", " ").strip()
 
-        if not self.language:
+        if self.language == UNK_LANG:
             self.language = functional.text.detect_language(self.raw)
 
         if not self.tokens:
             self.tokens = functional.text.tokenize(self.raw)
 
     @pydantic.computed_field  # type: ignore[misc]
     @property
```

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/encoder/__init__.py` & `cltrier_nlp-0.1.5/cltrier_nlp/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/encoder/batch.py` & `cltrier_nlp-0.1.5/cltrier_nlp/encoder/batch.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/encoder/pooler.py` & `cltrier_nlp-0.1.5/cltrier_nlp/encoder/pooler.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/functional/text.py` & `cltrier_nlp-0.1.5/cltrier_nlp/functional/text.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/cltrier_nlp/utility/map.py` & `cltrier_nlp-0.1.5/cltrier_nlp/utility/map.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.4/pyproject.toml` & `cltrier_nlp-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cltrier_nlp"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Simon Münker <muenker@uni-trier.de>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/simon-muenker/cltrier_nlp"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `cltrier_nlp-0.1.4/PKG-INFO` & `cltrier_nlp-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltrier_nlp
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/simon-muenker/cltrier_nlp
 License: Apache-2.0
 Author: Simon Münker
 Author-email: muenker@uni-trier.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

