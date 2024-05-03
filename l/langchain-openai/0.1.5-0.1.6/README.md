# Comparing `tmp/langchain_openai-0.1.5.tar.gz` & `tmp/langchain_openai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.5.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.6.tar", max compression
```

## Comparing `langchain_openai-0.1.5.tar` & `langchain_openai-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/LICENSE
--rw-r--r--   0        0        0     1627 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/README.md
--rw-r--r--   0        0        0      371 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10790 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    46599 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    22520 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8354 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24578 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/py.typed
--rw-r--r--   0        0        0     2835 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1627 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/README.md
+-rw-r--r--   0        0        0      371 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10790 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    47309 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    22520 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24578 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2835 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.6/PKG-INFO
```

### Comparing `langchain_openai-0.1.5/LICENSE` & `langchain_openai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.5/README.md` & `langchain_openai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.5/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.6/langchain_openai/chat_models/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.5/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.6/langchain_openai/chat_models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -759,61 +759,78 @@
             **kwargs,
         )
 
     def bind_tools(
         self,
         tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
         *,
-        tool_choice: Optional[Union[dict, str, Literal["auto", "none"], bool]] = None,
+        tool_choice: Optional[
+            Union[dict, str, Literal["auto", "none", "required", "any"], bool]
+        ] = None,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         """Bind tool-like objects to this chat model.
 
         Assumes model is compatible with OpenAI tool-calling API.
 
         Args:
             tools: A list of tool definitions to bind to this chat model.
                 Can be  a dictionary, pydantic model, callable, or BaseTool. Pydantic
                 models, callables, and BaseTools will be automatically converted to
                 their schema dictionary representation.
             tool_choice: Which tool to require the model to call.
-                Must be the name of the single provided function or
-                "auto" to automatically determine which function to call
-                (if any), or a dict of the form:
+                Options are:
+                name of the tool (str): calls corresponding tool;
+                "auto": automatically selects a tool (including no tool);
+                "none": does not call a tool;
+                "any" or "required": force at least one tool to be called;
+                True: forces tool call (requires `tools` be length 1);
+                False: no effect;
+
+                or a dict of the form:
                 {"type": "function", "function": {"name": <<tool_name>>}}.
             **kwargs: Any additional parameters to pass to the
                 :class:`~langchain.runnable.Runnable` constructor.
         """
 
         formatted_tools = [convert_to_openai_tool(tool) for tool in tools]
-        if tool_choice is not None and tool_choice:
-            if len(formatted_tools) != 1:
-                raise ValueError(
-                    "When specifying `tool_choice`, you must provide exactly one "
-                    f"tool. Received {len(formatted_tools)} tools."
-                )
+        if tool_choice:
             if isinstance(tool_choice, str):
-                if tool_choice not in ("auto", "none"):
+                # tool_choice is a tool/function name
+                if tool_choice not in ("auto", "none", "any", "required"):
                     tool_choice = {
                         "type": "function",
                         "function": {"name": tool_choice},
                     }
+                # 'any' is not natively supported by OpenAI API.
+                # We support 'any' since other models use this instead of 'required'.
+                if tool_choice == "any":
+                    tool_choice = "required"
             elif isinstance(tool_choice, bool):
+                if len(tools) > 1:
+                    raise ValueError(
+                        "tool_choice=True can only be used when a single tool is "
+                        f"passed in, received {len(tools)} tools."
+                    )
                 tool_choice = {
                     "type": "function",
                     "function": {"name": formatted_tools[0]["function"]["name"]},
                 }
             elif isinstance(tool_choice, dict):
-                if (
-                    formatted_tools[0]["function"]["name"]
-                    != tool_choice["function"]["name"]
+                tool_names = [
+                    formatted_tool["function"]["name"]
+                    for formatted_tool in formatted_tools
+                ]
+                if not any(
+                    tool_name == tool_choice["function"]["name"]
+                    for tool_name in tool_names
                 ):
                     raise ValueError(
                         f"Tool choice {tool_choice} was specified, but the only "
-                        f"provided tool was {formatted_tools[0]['function']['name']}."
+                        f"provided tools were {tool_names}."
                     )
             else:
                 raise ValueError(
                     f"Unrecognized tool_choice type. Expected str, bool or dict. "
                     f"Received: {tool_choice}"
                 )
             kwargs["tool_choice"] = tool_choice
```

### Comparing `langchain_openai-0.1.5/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.6/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.5/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.6/langchain_openai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.5/langchain_openai/llms/azure.py` & `langchain_openai-0.1.6/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.5/langchain_openai/llms/base.py` & `langchain_openai-0.1.6/langchain_openai/llms/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.5/pyproject.toml` & `langchain_openai-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.5"
+version = "0.1.6"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1.46"
-openai = "^1.10.0"
+openai = "^1.24.0"
 tiktoken = ">=0.5.2,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_openai-0.1.5/PKG-INFO` & `langchain_openai-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.5
+Version: 0.1.6
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain-core (>=0.1.46,<0.2.0)
-Requires-Dist: openai (>=1.10.0,<2.0.0)
+Requires-Dist: openai (>=1.24.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

