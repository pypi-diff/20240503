# Comparing `tmp/aigents-0.5.0.tar.gz` & `tmp/aigents-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.5.0.tar", max compression
+gzip compressed data, was "aigents-0.6.0.tar", max compression
```

## Comparing `aigents-0.5.0.tar` & `aigents-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.5.0/LICENSE
--rw-r--r--   0        0        0     4545 2024-03-20 10:12:52.420736 aigents-0.5.0/README.md
--rw-r--r--   0        0        0      975 2024-03-14 11:18:40.948668 aigents-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      525 2024-03-13 18:32:05.073594 aigents-0.5.0/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.5.0/src/aigents/base.py
--rw-r--r--   0        0        0     1083 2024-02-29 13:08:28.249354 aigents-0.5.0/src/aigents/constants.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.5.0/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.5.0/src/aigents/data.py
--rw-r--r--   0        0        0        0 2024-02-25 12:10:44.226527 aigents-0.5.0/src/aigents/embeddings.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.5.0/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.5.0/src/aigents/prompts.py
--rw-r--r--   0        0        0     2350 2024-02-25 18:23:33.244701 aigents-0.5.0/src/aigents/settings.py
--rw-r--r--   0        0        0     6096 2024-02-29 14:36:13.930172 aigents-0.5.0/src/aigents/utils.py
--rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 aigents-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4545 2024-03-20 10:12:52.420736 aigents-0.6.0/README.md
+-rw-r--r--   0        0        0     1028 2024-05-03 19:31:33.640604 aigents-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      525 2024-03-13 18:32:05.073594 aigents-0.6.0/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.6.0/src/aigents/base.py
+-rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/constants.py
+-rw-r--r--   0        0        0      309 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2018 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/base.py
+-rw-r--r--   0        0        0    11688 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-03 19:35:36.280050 aigents-0.6.0/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    14367 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     2502 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.6.0/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.6.0/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.6.0/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.6.0/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2350 2024-02-25 18:23:33.244701 aigents-0.6.0/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/utils.py
+-rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 aigents-0.6.0/PKG-INFO
```

### Comparing `aigents-0.5.0/LICENSE` & `aigents-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/README.md` & `aigents-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/pyproject.toml` & `aigents-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.5.0"
+version = "0.6.0"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -19,14 +19,17 @@
 openai = "^1.12.0"
 tiktoken = "^0.6.0"
 python-dotenv = "^1.0.1"
 google-generativeai = "^0.3.2"
 tomlkit = "^0.12.4"
 pillow = "^10.2.0"
 g4f = {extras = ["all"], version = "^0.2.4.1"}
+spacy = "^3.7.4"
+pandas = "^2.2.2"
+scipy = "^1.13.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.22.1"
 ipykernel = "^6.29.2"
 tomlkit = "^0.12.3"
 
 [build-system]
```

### Comparing `aigents-0.5.0/src/aigents/__init__.py` & `aigents-0.6.0/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/src/aigents/base.py` & `aigents-0.6.0/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/src/aigents/constants.py` & `aigents-0.6.0/src/aigents/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 """Constants for embeddings operations"""
 
 MODELS_EMBEDDING = (
     'text-embedding-3-small',
     'text-embedding-3-large',
     'text-embedding-ada-002',
+    'models/embedding-001',
+    'models/text-embedding-004',
 )
 
 TOKENIZER = (
     'cl100k_base',
 )
 
 EMBEDDINGS_COLUMNS = ('chunks', 'n_tokens', 'embeddings',)
```

### Comparing `aigents-0.5.0/src/aigents/core.py` & `aigents-0.6.0/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/src/aigents/errors.py` & `aigents-0.6.0/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/src/aigents/prompts.py` & `aigents-0.6.0/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/src/aigents/settings.py` & `aigents-0.6.0/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.5.0/src/aigents/utils.py` & `aigents-0.6.0/src/aigents/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
-from functools import wraps
+import logging
 from pathlib import Path
 from typing import Dict
 
 import tiktoken
-from openai import AsyncOpenAI
 
 from .constants import TOKENIZER
 
+logger = logging.getLogger('standard')
+
 def code_to_str(path: str | Path, comments: str = '#{}'):
     filepath = Path(path)
     code = comments.format(filepath.name) + '\n'
     with open(path, 'r', encoding='utf-8') as file_:
         code += file_.read()
     return code
 
@@ -168,14 +169,35 @@
     raise NotImplementedError(  # TODO choose another error
         f"number_of_tokens() is not presently implemented for model {model}. "
         "See https://github.com/openai/openai-python/blob/main/chatml.md for "
         "information on how messages are converted to tokens."
         ""
     )
 
+def run_async(coro, *args, **kwargs):
+    task = None
+    try:
+        loop = asyncio.get_running_loop()
+        task = loop.create_task(coro(*args, **kwargs))
+    except RuntimeError:
+        task = coro(*args, **kwargs)
+    try:
+        asyncio.run(task)
+    except RuntimeError:
+        try:
+            # NOTE: this allows running in jupyter without using 'await'
+            import nest_asyncio  # pylint --disable=import-outside-toplevel
+            nest_asyncio.apply()
+            asyncio.run(task)
+        except (ImportError, ModuleNotFoundError) as err:
+            logger.error(err)
+            logger.warning("Must install nest_asyncio for running in Jupyter")
+            raise err
+    return task.result()
+
 class Message:
     def __init__(self, content: str = None) -> None:
         self.content: str = content
 
 class Choices:
     def __init__(self, ) -> None:
         self.message = Message()
```

### Comparing `aigents-0.5.0/PKG-INFO` & `aigents-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.5.0
+Version: 0.6.0
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,16 +14,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: g4f[all] (>=0.2.4.1,<0.3.0.0)
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: spacy (>=3.7.4,<4.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: tomlkit (>=0.12.4,<0.13.0)
 Project-URL: Repository, https://github.com/bessavagner/aigents.git
 Description-Content-Type: text/markdown
 
 # aigents
```

