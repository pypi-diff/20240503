# Comparing `tmp/martian_adapters-4.1.2.tar.gz` & `tmp/martian_adapters-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-4.1.2.tar", max compression
+gzip compressed data, was "martian_adapters-4.2.0.tar", max compression
```

## Comparing `martian_adapters-4.1.2.tar` & `martian_adapters-4.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    35149 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/LICENSE
--rw-r--r--   0        0        0     3452 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/README.md
--rw-r--r--   0        0        0      725 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     3347 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2386 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0     3419 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5816 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     5812 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3429 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0      942 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9225 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4102 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2053 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1203 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1663 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4444 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1425 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2307 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    10017 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/rate_limiter.py
--rw-r--r--   0        0        0      335 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/requirements.txt
--rw-r--r--   0        0        0     6903 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/types.py
--rw-r--r--   0        0        0        0 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1170 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 martian_adapters-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/LICENSE
+-rw-r--r--   0        0        0     3452 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/README.md
+-rw-r--r--   0        0        0      725 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     3347 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2386 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0     3419 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5816 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     5812 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3429 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0      942 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9225 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4102 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2412 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2384 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1836 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1757 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1331 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4444 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2450 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2604 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    10017 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      335 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/requirements.txt
+-rw-r--r--   0        0        0     6903 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1170 2024-05-03 19:23:19.519366 martian_adapters-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 martian_adapters-4.2.0/PKG-INFO
```

### Comparing `martian_adapters-4.1.2/LICENSE` & `martian_adapters-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/README.md` & `martian_adapters-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/__init__.py` & `martian_adapters-4.2.0/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-4.2.0/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-4.2.0/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-4.2.0/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-4.2.0/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-4.2.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-4.2.0/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-4.2.0/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/adapter_factory.py` & `martian_adapters-4.2.0/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-4.2.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/__init__.py` & `martian_adapters-4.2.0/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,26 @@
 class DeepInfraModel(Model):
     supports_streaming: bool = True
     provider_name: str = PROVIDER_NAME
 
 
 MODELS = [
     DeepInfraModel(
+        name="gemma-1.1-7b-it",
+        cost=Cost(prompt=0.07e-6, completion=0.07e-6),
+        context_length=8192,
+        vendor_name="google",
+    ),
+    DeepInfraModel(
+        name="Mistral-7B-Instruct-v0.2",
+        cost=Cost(prompt=0.07e-6, completion=0.07e-6),
+        context_length=32768,
+        vendor_name="mistralai",
+    ),
+    DeepInfraModel(
         name="Mixtral-8x7B-Instruct-v0.1",
         cost=Cost(prompt=0.27e-6, completion=0.27e-6),
         context_length=32000,
         vendor_name="mistralai",
     ),
     DeepInfraModel(
         name="Mixtral-8x22B-Instruct-v0.1",
```

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import re
 from typing import Pattern
 
 from adapters.abstract_adapters.openai_sdk_chat_adapter import OpenAISDKChatAdapter
 from adapters.abstract_adapters.provider_adapter_mixin import ProviderAdapterMixin
 from adapters.types import Cost, Model
 
-PROVIDER_NAME = "fireworks"
-BASE_URL = "https://api.fireworks.ai/inference/v1"
-API_KEY_NAME = "FIREWORKS_API_KEY"
+PROVIDER_NAME = "octoai"
+BASE_URL = "https://text.octoai.run/v1"
+API_KEY_NAME = "OCTOAI_API_KEY"
 API_KEY_PATTERN = re.compile(r".*")
 
 
-class FireworksModel(Model):
+class OctoaiModel(Model):
     supports_streaming: bool = True
     provider_name: str = PROVIDER_NAME
 
 
 MODELS = [
-    FireworksModel(
-        name="llama-v3-8b-instruct",
-        cost=Cost(prompt=0.2e-6, completion=0.2e-6),
+    OctoaiModel(
+        name="meta-llama-3-8b-instruct",
+        cost=Cost(prompt=0.1e-6, completion=0.25e-6),
         context_length=8192,
-        vendor_name="accounts/fireworks/models",
+        vendor_name="meta-llama",
     )
 ]
 
 
-class FireworksSDKChatProviderAdapter(ProviderAdapterMixin, OpenAISDKChatAdapter):
+class OctoaiSDKChatProviderAdapter(ProviderAdapterMixin, OpenAISDKChatAdapter):
     @staticmethod
     def get_supported_models():
         return MODELS
 
     @staticmethod
     def get_provider_name() -> str:
         return PROVIDER_NAME
@@ -42,7 +42,12 @@
     @staticmethod
     def get_api_key_name() -> str:
         return API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
+
+    def get_model_name(self) -> str:
+        if self._current_model is None:
+            raise ValueError("Model not set")
+        return self._current_model.name
```

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,23 @@
     GroqModel(
         name="mixtral-8x7b-32768",
         cost=Cost(prompt=0.27e-6, completion=0.27e-6),
         context_length=32768,
         vendor_name="mistralai",
     ),
     GroqModel(
-        name="llama2-70b-4096",
-        cost=Cost(prompt=0.7e-6, completion=0.8e-6),
-        context_length=4096,
+        name="llama3-70b-8192",
+        cost=Cost(prompt=0.59e-6, completion=0.79e-6),
+        context_length=8192,
+        vendor_name="meta-llama",
+    ),
+    GroqModel(
+        name="llama3-8b-8192",
+        cost=Cost(prompt=0.05e-6, completion=0.10e-6),
+        context_length=8192,
         vendor_name="meta-llama",
     ),
     GroqModel(
         name="gemma-7b-it",
         cost=Cost(prompt=0.1e-6, completion=0.1e-6),
         context_length=8192,
         vendor_name="google",
```

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,24 @@
     supports_streaming: bool = True
     vendor_name: str = PROVIDER_NAME
     provider_name: str = PROVIDER_NAME
 
 
 MODELS = [
     PerplexityModel(
+        name="llama-3-70b-instruct",
+        cost=Cost(prompt=0.20e-6, completion=0.20e-6),
+        context_length=8192,
+    ),
+    PerplexityModel(
+        name="llama-3-8b-instruct",
+        cost=Cost(prompt=0.20e-6, completion=0.20e-6),
+        context_length=8192,
+    ),
+    PerplexityModel(
         name="sonar-small-chat",
         cost=Cost(prompt=0.2e-6, completion=0.2e-6),
         context_length=16384,
     ),
     PerplexityModel(
         name="sonar-small-online",
         cost=Cost(prompt=0.2e-6, completion=0.2e-6, request=0.005),
```

### Comparing `martian_adapters-4.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/rate_limiter.py` & `martian_adapters-4.2.0/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/types.py` & `martian_adapters-4.2.0/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/utils/general_utils.py` & `martian_adapters-4.2.0/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/utils/network_utils.py` & `martian_adapters-4.2.0/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/adapters/utils/openai_client_factory.py` & `martian_adapters-4.2.0/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.2/pyproject.toml` & `martian_adapters-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "4.1.2"
+version = "4.2.0"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `martian_adapters-4.1.2/PKG-INFO` & `martian_adapters-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 4.1.2
+Version: 4.2.0
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
```

