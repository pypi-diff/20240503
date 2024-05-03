# Comparing `tmp/lunary-1.0.6.tar.gz` & `tmp/lunary-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunary-1.0.6.tar", max compression
+gzip compressed data, was "lunary-1.0.7.tar", max compression
```

## Comparing `lunary-1.0.6.tar` & `lunary-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.6/README.md
--rw-r--r--   0        0        0    61168 2024-04-24 21:55:02.078632 lunary-1.0.6/lunary/__init__.py
--rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.6/lunary/consumer.py
--rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.6/lunary/event_queue.py
--rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.6/lunary/openai_utils.py
--rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.6/lunary/parent.py
--rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.6/lunary/parsers.py
--rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.6/lunary/project.py
--rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.6/lunary/tags.py
--rw-r--r--   0        0        0     1164 2024-04-17 19:52:13.801396 lunary-1.0.6/lunary/thread.py
--rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.6/lunary/users.py
--rw-r--r--   0        0        0      762 2024-04-24 21:55:13.382162 lunary-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 lunary-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.7/README.md
+-rw-r--r--   0        0        0    61367 2024-05-03 00:55:17.779559 lunary-1.0.7/lunary/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.7/lunary/consumer.py
+-rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.7/lunary/event_queue.py
+-rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.7/lunary/openai_utils.py
+-rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.7/lunary/parent.py
+-rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.7/lunary/parsers.py
+-rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.7/lunary/project.py
+-rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.7/lunary/tags.py
+-rw-r--r--   0        0        0     1164 2024-04-17 19:52:13.801396 lunary-1.0.7/lunary/thread.py
+-rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.7/lunary/users.py
+-rw-r--r--   0        0        0      762 2024-05-03 00:55:32.246630 lunary-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 lunary-1.0.7/PKG-INFO
```

### Comparing `lunary-1.0.6/README.md` & `lunary-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/lunary/__init__.py` & `lunary-1.0.7/lunary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,18 @@
         stream = fn(*args, **kwargs)
 
         choices = []
         tokens = 0
 
         for chunk in stream:
             tokens += 1
+            if not chunk.choices:
+                # Azure
+                continue
+
             choice = chunk.choices[0]
             index = choice.index
 
             content = choice.delta.content
             role = choice.delta.role
             function_call = choice.delta.function_call
             tool_calls = choice.delta.tool_calls
@@ -257,14 +261,18 @@
     stream = await fn(*args, **kwargs)
 
     choices = []
     tokens = 0
 
     async for chunk in stream:
         tokens += 1
+        if not chunk.choices:
+            # Happens with Azure
+            continue
+
         choice = chunk.choices[0]
         index = choice.index
 
         content = choice.delta.content
         role = choice.delta.role
         function_call = choice.delta.function_call
         tool_calls = choice.delta.tool_calls
@@ -563,15 +571,15 @@
                         output_parser=OpenAIUtils.parse_output,
                     )
                 except Exception as e:
                     logging.info(
                         "[Lunary] Please use `lunary.monitor(openai)` or `lunary.monitor(client)` after setting the OpenAI api key"
                     )
 
-            elif name == "AsyncOpenAI":
+            elif name == "AsyncOpenAI" or name == "AsyncAzureOpenAI":
                 object.chat.completions.create = async_wrap(
                     object.chat.completions.create,
                     "llm",
                     input_parser=OpenAIUtils.parse_input,
                     output_parser=OpenAIUtils.parse_output,
                 )
             else:
```

### Comparing `lunary-1.0.6/lunary/consumer.py` & `lunary-1.0.7/lunary/consumer.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/lunary/event_queue.py` & `lunary-1.0.7/lunary/event_queue.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/lunary/openai_utils.py` & `lunary-1.0.7/lunary/openai_utils.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/lunary/parent.py` & `lunary-1.0.7/lunary/parent.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/lunary/parsers.py` & `lunary-1.0.7/lunary/parsers.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/lunary/thread.py` & `lunary-1.0.7/lunary/thread.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/lunary/users.py` & `lunary-1.0.7/lunary/users.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.6/pyproject.toml` & `lunary-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunary"
-version = "1.0.6"
+version = "1.0.7"
 description = "Observability, analytics and evaluations for AI agents and chatbots."
 authors = ["lunary <hello@lunary.ai>"]
 readme = "README.md"
 repository = "https://github.com/lunary-ai/lunary-py"
 documentation = "https://lunary.ai/docs/py"
 keywords = ["Lunary", "lunary.ai", "Langchain", "AI", "Analytics", "Monitoring"]
```

### Comparing `lunary-1.0.6/PKG-INFO` & `lunary-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunary
-Version: 1.0.6
+Version: 1.0.7
 Summary: Observability, analytics and evaluations for AI agents and chatbots.
 Home-page: https://github.com/lunary-ai/lunary-py
 Keywords: Lunary,lunary.ai,Langchain,AI,Analytics,Monitoring
 Author: lunary
 Author-email: hello@lunary.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
```

