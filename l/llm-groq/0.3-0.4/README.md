# Comparing `tmp/llm-groq-0.3.tar.gz` & `tmp/llm_groq-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-groq-0.3.tar", last modified: Tue Mar 12 08:32:25 2024, max compression
+gzip compressed data, was "llm_groq-0.4.tar", last modified: Fri May  3 10:47:22 2024, max compression
```

## Comparing `llm-groq-0.3.tar` & `llm_groq-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:32:25.660122 llm-groq-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-12 08:32:18.000000 llm-groq-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-12 08:32:25.660122 llm-groq-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-12 08:32:18.000000 llm-groq-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:32:25.660122 llm-groq-0.3/llm_groq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-12 08:32:25.000000 llm-groq-0.3/llm_groq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-12 08:32:25.000000 llm-groq-0.3/llm_groq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 08:32:25.000000 llm-groq-0.3/llm_groq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-12 08:32:25.000000 llm-groq-0.3/llm_groq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 08:32:25.000000 llm-groq-0.3/llm_groq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 08:32:25.000000 llm-groq-0.3/llm_groq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-12 08:32:18.000000 llm-groq-0.3/llm_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-12 08:32:18.000000 llm-groq-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 08:32:25.660122 llm-groq-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:47:22.237821 llm_groq-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-03 10:47:13.000000 llm_groq-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-03 10:47:22.237821 llm_groq-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 10:47:13.000000 llm_groq-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:47:22.237821 llm_groq-0.4/llm_groq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-03 10:47:22.000000 llm_groq-0.4/llm_groq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-03 10:47:22.000000 llm_groq-0.4/llm_groq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:47:22.000000 llm_groq-0.4/llm_groq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 10:47:22.000000 llm_groq-0.4/llm_groq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 10:47:22.000000 llm_groq-0.4/llm_groq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 10:47:22.000000 llm_groq-0.4/llm_groq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-03 10:47:13.000000 llm_groq-0.4/llm_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 10:47:13.000000 llm_groq-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:47:22.237821 llm_groq-0.4/setup.cfg
```

### Comparing `llm-groq-0.3/LICENSE` & `llm_groq-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-groq-0.3/PKG-INFO` & `llm_groq-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-groq
-Version: 0.3
+Version: 0.4
 Author: Moritz Angermann
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/angerman/llm-groq
 Project-URL: Changelog, https://github.com/angerman/llm-groq/releases
 Project-URL: Issues, https://github.com/angerman/llm-groq/issues
 Project-URL: CI, https://github.com/angerman/llm-groq/actions
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llm-groq-0.3/README.md` & `llm_groq-0.4/README.md`

 * *Files identical despite different names*

### Comparing `llm-groq-0.3/llm_groq.egg-info/PKG-INFO` & `llm_groq-0.4/llm_groq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-groq
-Version: 0.3
+Version: 0.4
 Author: Moritz Angermann
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/angerman/llm-groq
 Project-URL: Changelog, https://github.com/angerman/llm-groq/releases
 Project-URL: Issues, https://github.com/angerman/llm-groq/issues
 Project-URL: CI, https://github.com/angerman/llm-groq/actions
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llm-groq-0.3/llm_groq.py` & `llm_groq-0.4/llm_groq.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 from groq import Groq
 from pydantic import Field
 from typing import Optional, List, Union
 
 @llm.hookimpl
 def register_models(register):
     register(LLMGroq("groq-llama2"))
+    register(LLMGroq("groq-llama3"))
+    register(LLMGroq("groq-llama3-70b"))
     register(LLMGroq("groq-mixtral"))
     register(LLMGroq("groq-gemma"))
 
 class LLMGroq(llm.Model):
     can_stream = True
 
     model_map: dict = {
+        "groq-gemma": "gemma-7b-it",
         "groq-llama2": "llama2-70b-4096",
+        "groq-llama3": "llama3-8b-8192",
+        "groq-llama3-70b": "llama3-70b-8192",
         "groq-mixtral": "mixtral-8x7b-32768",
-        "groq-gemma": "gemma-7b-it",
     }
 
     class Options(llm.Options):
         temperature: Optional[float] = Field(
             description=(
                 "Controls randomness of responses. A lower temperature leads to"
                 "more predictable outputs while a higher temperature results in"
@@ -108,8 +112,8 @@
             stop=prompt.options.stop
         )
         if stream:
             for chunk in resp:
                 if chunk.choices[0].delta.content:
                     yield from chunk.choices[0].delta.content
         else:
-            yield from resp.choices[0].message.content
+            yield from resp.choices[0].message.content
```

### Comparing `llm-groq-0.3/pyproject.toml` & `llm_groq-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-groq"
-version = "0.3"
+version = "0.4"
 
 readme = "README.md"
 authors = [{name = "Moritz Angermann"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

