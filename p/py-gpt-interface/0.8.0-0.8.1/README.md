# Comparing `tmp/py_gpt_interface-0.8.0.tar.gz` & `tmp/py_gpt_interface-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_gpt_interface-0.8.0.tar", last modified: Wed Feb 28 18:09:39 2024, max compression
+gzip compressed data, was "py_gpt_interface-0.8.1.tar", last modified: Fri May  3 16:25:21 2024, max compression
```

## Comparing `py_gpt_interface-0.8.0.tar` & `py_gpt_interface-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.0/LICENSE
--rw-r--r--   0        0        0    12881 2024-02-28 16:34:19.921626 py_gpt_interface-0.8.0/README.md
--rw-r--r--   0        0        0      614 2024-02-28 18:09:39.572691 py_gpt_interface-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3896 2024-02-28 16:35:52.078466 py_gpt_interface-0.8.0/src/gpt_interface/__init__.py
--rw-r--r--   0        0        0     1551 2023-12-23 07:13:23.000000 py_gpt_interface-0.8.0/src/gpt_interface/calls/call_gpt.py
--rw-r--r--   0        0        0     1033 2024-02-23 01:04:02.290616 py_gpt_interface-0.8.0/src/gpt_interface/calls/legacy_model.py
--rw-r--r--   0        0        0     4218 2023-12-23 07:08:55.000000 py_gpt_interface-0.8.0/src/gpt_interface/calls/modern_model.py
--rw-r--r--   0        0        0      413 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.0/src/gpt_interface/calls/rate_limiter.py
--rw-r--r--   0        0        0     1382 2024-02-23 00:32:20.962341 py_gpt_interface-0.8.0/src/gpt_interface/log/__init__.py
--rw-r--r--   0        0        0     1968 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.0/src/gpt_interface/log/pruning.py
--rw-r--r--   0        0        0     7866 2024-02-23 00:13:35.924109 py_gpt_interface-0.8.0/src/gpt_interface/options/models.py
--rw-r--r--   0        0        0      160 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.0/src/gpt_interface/options/system_message.py
--rw-r--r--   0        0        0      154 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.0/src/gpt_interface/tools/__init__.py
--rw-r--r--   0        0        0     3220 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.0/src/gpt_interface/tools/functions.py
--rw-r--r--   0        0        0    48164 2024-02-23 00:43:23.383016 py_gpt_interface-0.8.0/tests/elephant.webp
--rw-r--r--   0        0        0     3240 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.0/tests/test_function_dict.py
--rw-r--r--   0        0        0    13408 1970-01-01 00:00:00.000000 py_gpt_interface-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.1/LICENSE
+-rw-r--r--   0        0        0    12881 2024-02-28 16:34:19.921626 py_gpt_interface-0.8.1/README.md
+-rw-r--r--   0        0        0      614 2024-05-03 16:25:21.298107 py_gpt_interface-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3896 2024-02-28 16:35:52.078466 py_gpt_interface-0.8.1/src/gpt_interface/__init__.py
+-rw-r--r--   0        0        0     1551 2023-12-23 07:13:23.000000 py_gpt_interface-0.8.1/src/gpt_interface/calls/call_gpt.py
+-rw-r--r--   0        0        0     1033 2024-02-23 01:04:02.290616 py_gpt_interface-0.8.1/src/gpt_interface/calls/legacy_model.py
+-rw-r--r--   0        0        0     4218 2023-12-23 07:08:55.000000 py_gpt_interface-0.8.1/src/gpt_interface/calls/modern_model.py
+-rw-r--r--   0        0        0      413 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.1/src/gpt_interface/calls/rate_limiter.py
+-rw-r--r--   0        0        0     1382 2024-02-23 00:32:20.962341 py_gpt_interface-0.8.1/src/gpt_interface/log/__init__.py
+-rw-r--r--   0        0        0     1968 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.1/src/gpt_interface/log/pruning.py
+-rw-r--r--   0        0        0     8506 2024-05-03 16:24:49.266574 py_gpt_interface-0.8.1/src/gpt_interface/options/models.py
+-rw-r--r--   0        0        0      160 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.1/src/gpt_interface/options/system_message.py
+-rw-r--r--   0        0        0      154 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.1/src/gpt_interface/tools/__init__.py
+-rw-r--r--   0        0        0     3220 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.1/src/gpt_interface/tools/functions.py
+-rw-r--r--   0        0        0    48164 2024-02-23 00:43:23.383016 py_gpt_interface-0.8.1/tests/elephant.webp
+-rw-r--r--   0        0        0     3240 2023-12-23 06:49:46.000000 py_gpt_interface-0.8.1/tests/test_function_dict.py
+-rw-r--r--   0        0        0    13408 1970-01-01 00:00:00.000000 py_gpt_interface-0.8.1/PKG-INFO
```

### Comparing `py_gpt_interface-0.8.0/LICENSE` & `py_gpt_interface-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/README.md` & `py_gpt_interface-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/pyproject.toml` & `py_gpt_interface-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py_gpt_interface"
-version = "0.8.0"
+version = "0.8.1"
 description = "A simple interface for using the GPT API."
 authors = [
     { name = "Matt Zhang", email = "set.stun@gmail.com" },
 ]
 dependencies = [
     "openai>=1.2.4",
     "tiktoken>=0.5.1",
```

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/__init__.py` & `py_gpt_interface-0.8.1/src/gpt_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/calls/call_gpt.py` & `py_gpt_interface-0.8.1/src/gpt_interface/calls/call_gpt.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/calls/legacy_model.py` & `py_gpt_interface-0.8.1/src/gpt_interface/calls/legacy_model.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/calls/modern_model.py` & `py_gpt_interface-0.8.1/src/gpt_interface/calls/modern_model.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/log/__init__.py` & `py_gpt_interface-0.8.1/src/gpt_interface/log/__init__.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/log/pruning.py` & `py_gpt_interface-0.8.1/src/gpt_interface/log/pruning.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/options/models.py` & `py_gpt_interface-0.8.1/src/gpt_interface/options/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,28 @@
 
 
 # from https://platform.openai.com/docs/models
 # TODO: notify when trying to use deprecated model
 # TODO: do something with model description
 known_models = [
     Model(
+        name="gpt-4-turbo",
+        description="GPT-4 Turbo with Vision: The latest GPT-4 Turbo model with vision capabilities. Vision requests can now use JSON mode and function calling. Currently points to gpt-4-turbo-2024-04-09.",
+        max_tokens=128_000,
+        deprecated=False,
+        legacy_chat_api=False,
+    ),
+    Model(
+        name="gpt-4-turbo-2024-04-09",
+        description="GPT-4 Turbo with Vision model. Vision requests can now use JSON mode and function calling. gpt-4-turbo currently points to this version.",
+        max_tokens=128_000,
+        deprecated=False,
+        legacy_chat_api=False,
+    ),
+    Model(
         name="gpt-4-0125-preview",
         description="GPT-4 Turbo: The latest GPT-4 model intended to reduce cases of “laziness” where the model doesn’t complete a task. Returns a maximum of 4,096 output tokens.",
         max_tokens=128_000,
         deprecated=False,
         legacy_chat_api=False,
     ),
     Model(
```

### Comparing `py_gpt_interface-0.8.0/src/gpt_interface/tools/functions.py` & `py_gpt_interface-0.8.1/src/gpt_interface/tools/functions.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/tests/elephant.webp` & `py_gpt_interface-0.8.1/tests/elephant.webp`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/tests/test_function_dict.py` & `py_gpt_interface-0.8.1/tests/test_function_dict.py`

 * *Files identical despite different names*

### Comparing `py_gpt_interface-0.8.0/PKG-INFO` & `py_gpt_interface-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_gpt_interface
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple interface for using the GPT API.
 Author-Email: Matt Zhang <set.stun@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/MattUnderscoreZhang/gpt_interface
 Requires-Python: >=3.8
 Requires-Dist: openai>=1.2.4
 Requires-Dist: tiktoken>=0.5.1
```

