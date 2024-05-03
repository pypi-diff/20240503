# Comparing `tmp/proxyllm-0.1.6.tar.gz` & `tmp/proxyllm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyllm-0.1.6.tar", max compression
+gzip compressed data, was "proxyllm-0.2.0.tar", max compression
```

## Comparing `proxyllm-0.1.6.tar` & `proxyllm-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0     1066 2024-03-10 15:59:37.184771 proxyllm-0.1.6/LICENSE
--rw-r--r--   0        0        0     6318 2024-03-16 17:45:19.889099 proxyllm-0.1.6/README.md
--rw-r--r--   0        0        0       39 2024-03-16 17:45:19.891888 proxyllm-0.1.6/proxyllm/__init__.py
--rw-r--r--   0        0        0      795 2024-03-16 17:45:19.892423 proxyllm-0.1.6/proxyllm/cli.py
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.892491 proxyllm-0.1.6/proxyllm/config/__init__.py
--rw-r--r--   0        0        0     7140 2024-03-16 23:09:51.347233 proxyllm-0.1.6/proxyllm/config/internal_config.py
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.892798 proxyllm-0.1.6/proxyllm/data/__init__.py
--rw-r--r--   0        0        0  1083514 2024-03-16 17:45:19.896757 proxyllm-0.1.6/proxyllm/data/tokenizer-wiki.json
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.896958 proxyllm-0.1.6/proxyllm/provider/__init__.py
--rw-r--r--   0        0        0     1261 2024-03-16 17:45:19.897102 proxyllm-0.1.6/proxyllm/provider/base.py
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897151 proxyllm-0.1.6/proxyllm/provider/cohere/__init__.py
--rw-r--r--   0        0        0     6576 2024-03-16 23:23:38.172676 proxyllm-0.1.6/proxyllm/provider/cohere/cohere.py
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897349 proxyllm-0.1.6/proxyllm/provider/google/__init__.py
--rw-r--r--   0        0        0     6927 2024-03-16 23:09:51.347694 proxyllm-0.1.6/proxyllm/provider/google/vertexai.py
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897524 proxyllm-0.1.6/proxyllm/provider/huggingface/__init__.py
--rw-r--r--   0        0        0    10960 2024-03-16 17:45:19.897657 proxyllm-0.1.6/proxyllm/provider/huggingface/llama2.py
--rw-r--r--   0        0        0     6352 2024-03-16 17:45:19.897755 proxyllm-0.1.6/proxyllm/provider/huggingface/mistral.py
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897802 proxyllm-0.1.6/proxyllm/provider/openai/__init__.py
--rw-r--r--   0        0        0     7972 2024-03-16 23:23:38.173149 proxyllm-0.1.6/proxyllm/provider/openai/chatgpt.py
--rw-r--r--   0        0        0    20994 2024-03-16 23:19:58.938259 proxyllm-0.1.6/proxyllm/proxyllm.py
--rw-r--r--   0        0        0        0 2024-03-16 17:45:19.898161 proxyllm-0.1.6/proxyllm/utils/__init__.py
--rw-r--r--   0        0        0     1406 2024-03-16 17:45:19.898629 proxyllm-0.1.6/proxyllm/utils/categorization.py
--rw-r--r--   0        0        0     1299 2024-03-16 17:45:19.898757 proxyllm-0.1.6/proxyllm/utils/cost.py
--rw-r--r--   0        0        0     1701 2024-03-16 17:45:19.898840 proxyllm-0.1.6/proxyllm/utils/enums.py
--rw-r--r--   0        0        0      184 2024-03-16 17:45:19.899102 proxyllm-0.1.6/proxyllm/utils/exceptions/llmproxy_client.py
--rw-r--r--   0        0        0     1280 2024-03-16 17:45:19.899400 proxyllm-0.1.6/proxyllm/utils/exceptions/provider.py
--rw-r--r--   0        0        0     5881 2024-03-16 17:45:19.899520 proxyllm-0.1.6/proxyllm/utils/logger.py
--rw-r--r--   0        0        0     1382 2024-03-16 17:45:19.899967 proxyllm-0.1.6/proxyllm/utils/sorting.py
--rw-r--r--   0        0        0     3235 2024-03-16 17:45:19.900092 proxyllm-0.1.6/proxyllm/utils/timeout_function.py
--rw-r--r--   0        0        0     1556 2024-03-16 17:45:19.900201 proxyllm-0.1.6/proxyllm/utils/tokenizer.py
--rw-r--r--   0        0        0      918 2024-03-16 23:23:38.173303 proxyllm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7127 1970-01-01 00:00:00.000000 proxyllm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-10 15:59:37.184771 proxyllm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6318 2024-03-16 17:45:19.889099 proxyllm-0.2.0/README.md
+-rw-r--r--   0        0        0       39 2024-04-25 21:49:22.387410 proxyllm-0.2.0/proxyllm/__init__.py
+-rw-r--r--   0        0        0      795 2024-03-16 17:45:19.892423 proxyllm-0.2.0/proxyllm/cli.py
+-rw-r--r--   0        0        0        0 2024-03-16 17:45:19.892491 proxyllm-0.2.0/proxyllm/config/__init__.py
+-rw-r--r--   0        0        0    10342 2024-05-03 15:48:40.170986 proxyllm-0.2.0/proxyllm/config/internal_config.py
+-rw-r--r--   0        0        0        0 2024-03-16 17:45:19.892798 proxyllm-0.2.0/proxyllm/data/__init__.py
+-rw-r--r--   0        0        0  1083514 2024-03-16 17:45:19.896757 proxyllm-0.2.0/proxyllm/data/tokenizer-wiki.json
+-rw-r--r--   0        0        0        0 2024-03-16 17:45:19.896958 proxyllm-0.2.0/proxyllm/provider/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:09:07.068704 proxyllm-0.2.0/proxyllm/provider/anthropic/__init__.py
+-rw-r--r--   0        0        0     8526 2024-05-03 03:11:43.017967 proxyllm-0.2.0/proxyllm/provider/anthropic/claude.py
+-rw-r--r--   0        0        0     1475 2024-04-25 22:52:04.016785 proxyllm-0.2.0/proxyllm/provider/base.py
+-rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897151 proxyllm-0.2.0/proxyllm/provider/cohere/__init__.py
+-rw-r--r--   0        0        0     7911 2024-05-03 03:11:43.018234 proxyllm-0.2.0/proxyllm/provider/cohere/cohere.py
+-rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897349 proxyllm-0.2.0/proxyllm/provider/google/__init__.py
+-rw-r--r--   0        0        0    15887 2024-05-03 03:11:43.018447 proxyllm-0.2.0/proxyllm/provider/google/vertexai.py
+-rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897524 proxyllm-0.2.0/proxyllm/provider/huggingface/__init__.py
+-rw-r--r--   0        0        0    11554 2024-05-03 03:11:43.018618 proxyllm-0.2.0/proxyllm/provider/huggingface/llama2.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:52:04.017500 proxyllm-0.2.0/proxyllm/provider/mistral/__init__.py
+-rw-r--r--   0        0        0     7904 2024-05-03 03:11:43.018906 proxyllm-0.2.0/proxyllm/provider/mistral/mistral.py
+-rw-r--r--   0        0        0        0 2024-03-16 17:45:19.897802 proxyllm-0.2.0/proxyllm/provider/openai/__init__.py
+-rw-r--r--   0        0        0     8744 2024-05-03 03:11:43.019316 proxyllm-0.2.0/proxyllm/provider/openai/chatgpt.py
+-rw-r--r--   0        0        0    26068 2024-05-03 03:11:43.019740 proxyllm-0.2.0/proxyllm/proxyllm.py
+-rw-r--r--   0        0        0        0 2024-04-25 21:49:28.602536 proxyllm-0.2.0/proxyllm/utils/__init__.py
+-rw-r--r--   0        0        0     1424 2024-04-26 02:50:47.168716 proxyllm-0.2.0/proxyllm/utils/categorization.py
+-rw-r--r--   0        0        0     1299 2024-03-16 17:45:19.898757 proxyllm-0.2.0/proxyllm/utils/cost.py
+-rw-r--r--   0        0        0     1701 2024-03-16 17:45:19.898840 proxyllm-0.2.0/proxyllm/utils/enums.py
+-rw-r--r--   0        0        0      234 2024-04-25 22:52:04.018630 proxyllm-0.2.0/proxyllm/utils/exceptions/llmproxy_client.py
+-rw-r--r--   0        0        0     1462 2024-03-31 22:09:07.070612 proxyllm-0.2.0/proxyllm/utils/exceptions/provider.py
+-rw-r--r--   0        0        0     6045 2024-04-26 02:50:47.168896 proxyllm-0.2.0/proxyllm/utils/proxy_logger.py
+-rw-r--r--   0        0        0     1382 2024-03-16 17:45:19.899967 proxyllm-0.2.0/proxyllm/utils/sorting.py
+-rw-r--r--   0        0        0     3235 2024-03-16 17:45:19.900092 proxyllm-0.2.0/proxyllm/utils/timeout_function.py
+-rw-r--r--   0        0        0     1556 2024-03-16 17:45:19.900201 proxyllm-0.2.0/proxyllm/utils/tokenizer.py
+-rw-r--r--   0        0        0      952 2024-05-03 15:49:44.739663 proxyllm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7091 1970-01-01 00:00:00.000000 proxyllm-0.2.0/PKG-INFO
```

### Comparing `proxyllm-0.1.6/LICENSE` & `proxyllm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/README.md` & `proxyllm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/proxyllm/cli.py` & `proxyllm-0.2.0/proxyllm/cli.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/proxyllm/data/tokenizer-wiki.json` & `proxyllm-0.2.0/proxyllm/data/tokenizer-wiki.json`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/proxyllm/provider/base.py` & `proxyllm-0.2.0/proxyllm/provider/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from typing import Any, Dict, List
 
 
 @dataclass
 class TokenizeResponse:
     num_of_input_tokens: int
     num_of_output_tokens: int
 
@@ -11,23 +12,26 @@
 class BaseAdapter(ABC):
     """Abstract base class used to interface with (Language) Models.
     Current only one: Language.
     Likely more to be introduced if more types of LLMs are introduced (Speech, CNNs, Video...)
     """
 
     @abstractmethod
-    def get_completion(self, prompt: str = "") -> str | None:
+    def get_completion(
+        self, prompt: str = "", chat_history: List[Dict[str, str]] | None = None
+    ) -> Dict[str, Any] | None:
         """
         Abstract method to retrieve completion for a given prompt.
 
         Parameters:
         - prompt (str): The prompt for which completion is requested. Defaults to an empty string.
+        - chat_history (List[Dict[str, str]]): The chat history for conversation. Defaults to None.
 
         Returns:
-        - str or None: The completion for the provided prompt, or None if no completion is available.
+        - Dict[str, Any] or None: The model's text response and chat history, or None if an error occurs.
         """
 
     @abstractmethod
     def tokenize(self, prompt="") -> TokenizeResponse:
         pass
 
     @abstractmethod
```

### Comparing `proxyllm-0.1.6/proxyllm/provider/cohere/cohere.py` & `proxyllm-0.2.0/proxyllm/provider/openai/chatgpt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,237 @@
-from tokenizers import Encoding
+from typing import Any, Dict, List
+
+import tiktoken
 
 from proxyllm.provider.base import BaseAdapter, TokenizeResponse
-from proxyllm.utils import logger, tokenizer
-from proxyllm.utils.exceptions.provider import CohereException
+from proxyllm.utils import proxy_logger
+from proxyllm.utils.exceptions.provider import OpenAIException
 
-# Dictionary mapping Cohere model categories to task performance ratings.
-cohere_category_data = {
+# Mapping of OpenAI model categories to their respective task performance ratings.
+open_ai_category_data = {
     "model-categories": {
-        "command": {
+        "gpt-3.5-turbo-1106": {
             "Code Generation Task": 2,
             "Text Generation Task": 1,
             "Translation and Multilingual Applications Task": 2,
             "Natural Language Processing Task": 1,
             "Conversational AI Task": 1,
             "Educational Applications Task": 2,
             "Healthcare and Medical Task": 3,
             "Legal Task": 3,
             "Financial Task": 3,
             "Content Recommendation Task": 2,
         },
-        "command-light": {
-            "Code Generation Task": 3,
-            "Text Generation Task": 2,
-            "Translation and Multilingual Applications Task": 3,
-            "Natural Language Processing Task": 2,
-            "Conversational AI Task": 2,
-            "Educational Applications Task": 3,
-            "Healthcare and Medical Task": 4,
-            "Legal Task": 4,
-            "Financial Task": 4,
-            "Content Recommendation Task": 3,
-        },
-        "command-nightly": {
+        "gpt-3.5-turbo-0125": {
             "Code Generation Task": 2,
             "Text Generation Task": 1,
             "Translation and Multilingual Applications Task": 2,
             "Natural Language Processing Task": 1,
             "Conversational AI Task": 1,
             "Educational Applications Task": 2,
             "Healthcare and Medical Task": 3,
             "Legal Task": 3,
             "Financial Task": 3,
             "Content Recommendation Task": 2,
         },
-        "command-light-nightly": {
-            "Code Generation Task": 3,
-            "Text Generation Task": 2,
-            "Translation and Multilingual Applications Task": 3,
-            "Natural Language Processing Task": 2,
-            "Conversational AI Task": 2,
-            "Educational Applications Task": 3,
-            "Healthcare and Medical Task": 4,
-            "Legal Task": 4,
-            "Financial Task": 4,
-            "Content Recommendation Task": 3,
-        },
-        "command-r": {
+        "gpt-3.5-turbo-instruct": {
             "Code Generation Task": 2,
             "Text Generation Task": 1,
             "Translation and Multilingual Applications Task": 2,
             "Natural Language Processing Task": 1,
             "Conversational AI Task": 1,
             "Educational Applications Task": 2,
             "Healthcare and Medical Task": 3,
             "Legal Task": 3,
             "Financial Task": 3,
             "Content Recommendation Task": 2,
         },
+        "gpt-4": {
+            "Code Generation Task": 1,
+            "Text Generation Task": 1,
+            "Translation and Multilingual Applications Task": 1,
+            "Natural Language Processing Task": 1,
+            "Conversational AI Task": 1,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 2,
+            "Legal Task": 2,
+            "Financial Task": 2,
+            "Content Recommendation Task": 1,
+        },
+        "gpt-4-32k": {
+            "Code Generation Task": 1,
+            "Text Generation Task": 1,
+            "Translation and Multilingual Applications Task": 1,
+            "Natural Language Processing Task": 1,
+            "Conversational AI Task": 1,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 2,
+            "Legal Task": 2,
+            "Financial Task": 2,
+            "Content Recommendation Task": 1,
+        },
+        "gpt-4-0125-preview": {
+            "Code Generation Task": 1,
+            "Text Generation Task": 1,
+            "Translation and Multilingual Applications Task": 1,
+            "Natural Language Processing Task": 1,
+            "Conversational AI Task": 1,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 2,
+            "Legal Task": 2,
+            "Financial Task": 2,
+            "Content Recommendation Task": 1,
+        },
+        "gpt-4-1106-preview": {
+            "Code Generation Task": 1,
+            "Text Generation Task": 1,
+            "Translation and Multilingual Applications Task": 1,
+            "Natural Language Processing Task": 1,
+            "Conversational AI Task": 1,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 2,
+            "Legal Task": 2,
+            "Financial Task": 2,
+            "Content Recommendation Task": 1,
+        },
     }
 }
 
 
-class CohereAdapter(BaseAdapter):
+class OpenAIAdapter(BaseAdapter):
     """
-    Adapter class for the Cohere language model API.
+    Adapter class for interacting with OpenAI's language models.
 
-    This adapter facilitates communication between the LLM Proxy application and the Cohere API,
-    managing API requests and responses, error handling, and cost estimation based on token usage.
+    Facilitates the sending of requests to and the handling of responses from OpenAI's API,
+    including authentication, setting request parameters, and parsing responses. This adapter
+    is part of the LLM Proxy application, enabling seamless integration with OpenAI's services.
 
     Attributes:
-        prompt (str): Default prompt to use for requests.
-        model (str): Model identifier for the Cohere API.
-        temperature (float): Temperature setting for text generation (creativity).
-        api_key (str): API key for authenticating with the Cohere service.
-        max_output_tokens (int | None): Maximum number of tokens for the model response.
-        timeout (int): Timeout for API requests in seconds.
+        prompt (str): Default text prompt for generating responses.
+        model (str): Identifier for the selected OpenAI model.
+        temperature (float): Temperature parameter controlling the creativity of the response.
+        api_key (str): API key for authenticating requests to OpenAI.
+        max_output_tokens (int): Maximum number of tokens for the response.
+        timeout (int): Timeout for the API request in seconds.
     """
 
     def __init__(
         self,
         prompt: str = "",
         model: str = "",
-        temperature: float = 0.0,
+        temperature: float = 0,
         api_key: str = "",
         max_output_tokens: int | None = None,
-        timeout: int = 120,  # default based on Cohere's API
+        timeout: int | None = None,
     ) -> None:
         self.prompt = prompt
         self.model = model
         self.temperature = temperature
         self.api_key = api_key
         self.max_output_tokens = max_output_tokens
         self.timeout = timeout
 
-    def get_completion(self, prompt: str = "") -> str | None:
+    def get_completion(
+        self, prompt: str = "", chat_history: List[Dict[str, str]] | None = None
+    ) -> Dict[str, Any] | None:
         """
-        Requests a text completion from the Cohere model.
+        Requests a text completion from the specified OpenAI model.
 
         Args:
-            prompt (str): Input text prompt for the model.
+            prompt (str): The text prompt for generating completion.
+            chat_history (List[Dict[str, str]]): The chat history for conversation
 
         Returns:
-            str | None: The text completion result from the model, or None if an error occurs.
+            Dict[str, Any] | None: The model's text response and chat history, or None if an error occurs.
 
         Raises:
-            CohereException: If an error occurs during the API request.
+            OpenAIException: If an API or internal error occurs during request processing.
         """
 
-        from cohere import Client, CohereError
+        # Prevent API Connection Error with empty API KEY
+        if self.api_key == "":
+            raise OpenAIException(
+                exception="EMPTY API KEY: API key not provided",
+                error_type="No API Key Provided",
+            )
+
+        if chat_history is None:
+            chat_history = []
+
+        import copy
+
+        from openai import OpenAI, OpenAIError
 
         try:
-            co = Client(api_key=self.api_key, timeout=self.timeout)
-            response = co.chat(
-                max_tokens=self.max_output_tokens,
-                message=prompt or self.prompt,
+            client = OpenAI(api_key=self.api_key)
+
+            openai_chat_history = copy.deepcopy(chat_history)
+            openai_chat_history.append(
+                {"role": "user", "content": prompt or self.prompt}
+            )
+            response = client.chat.completions.create(
+                messages=openai_chat_history,
                 model=self.model,
+                max_tokens=self.max_output_tokens,
                 temperature=self.temperature,
+                timeout=self.timeout,
             )
-            return response.text
-        except CohereError as e:
-            raise CohereException(exception=str(e), error_type="CohereError") from e
+            response_text = response.choices[0].message.content
+
+            chat_history.append({"role": "user", "content": prompt or self.prompt})
+            chat_history.append({"role": "assistant", "content": response_text})
+
+            provider_response = {
+                "response": response_text,
+                "chat_history": chat_history,
+            }
+        except OpenAIError as e:
+            raise OpenAIException(
+                exception=e.args[0], error_type=type(e).__name__
+            ) from e
         except Exception as e:
-            raise CohereException(
-                exception=str(e), error_type="Unknown Cohere Error"
+            raise OpenAIException(
+                exception=e.args[0], error_type="Unknown OpenAI Error"
             ) from e
 
+        return provider_response or None
+
     def tokenize(self, prompt: str = "") -> TokenizeResponse:
         """
         Tokenizes the provided prompt using the tokenizer.
 
         Args:
             prompt (str, optional): The prompt to be tokenized. Defaults to an empty string.
 
         Returns:
             TokenizeResponse: An object containing information about the tokenization process,
                 including the number of input tokens and the maximum number of output tokens.
 
         Note:
             This method currently avoids calculating costs for tokenization.
         """
-        # Note: Avoiding costs for now
-        # tokens = self.co.tokenize(text=prompt or self.prompt).tokens
-        encoding: Encoding = tokenizer.bpe_tokenize_encode(prompt or self.prompt)
+        encoder = tiktoken.encoding_for_model(self.model)
+
+        tokens = encoder.encode(prompt or self.prompt)
 
         return TokenizeResponse(
-            num_of_input_tokens=len(encoding.tokens),
+            num_of_input_tokens=len(tokens),
             num_of_output_tokens=self.max_output_tokens or 256,
         )
 
     def get_category_rank(self, category: str = "") -> int:
         """
         Retrieves the performance rank of the current model for a specified task category.
 
         Args:
-            category (str): The task category to retrieve the rank for.
+            category (str): The task category for which to retrieve the model's rank.
 
         Returns:
-            int: Rank of the model in the specified category.
+            int: The performance rank of the model in the specified category.
         """
-        logger.log(msg=f"MODEL: {self.model}", color="PURPLE")
-        logger.log(msg=f"CATEGORY OF PROMPT: {category}")
+        proxy_logger.log(msg=f"MODEL: {self.model}", color="PURPLE")
 
-        category_rank = cohere_category_data["model-categories"][self.model][category]
+        category_rank = open_ai_category_data["model-categories"][self.model][category]
 
-        logger.log(msg=f"RANK OF PROMPT: {category_rank}", color="BLUE")
+        proxy_logger.log(msg=f"MODEL CATEGORY RANK: {category_rank}", color="BLUE")
 
         return category_rank
```

### Comparing `proxyllm-0.1.6/proxyllm/provider/huggingface/llama2.py` & `proxyllm-0.2.0/proxyllm/provider/huggingface/llama2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import Any, Dict, List
+
 import requests
 from tokenizers import Encoding
 
 from proxyllm.provider.base import BaseAdapter, TokenizeResponse
-from proxyllm.utils import logger, tokenizer
+from proxyllm.utils import proxy_logger, tokenizer
 from proxyllm.utils.exceptions.provider import EmptyPrompt, Llama2Exception
 
 # Mapping of Llama-2 model categories to their respective task performance ratings.
 llama2_category_data = {
     "model-categories": {
         "llama-2-7b-chat-hf": {
             "Code Generation Task": 2,
@@ -188,34 +190,40 @@
         self.prompt = prompt
         self.api_key = api_key
         self.temperature = temperature
         self.model = model
         self.max_output_tokens = max_output_tokens
         self.timeout = timeout
 
-    def get_completion(self, prompt: str = "") -> str | None:
+    def get_completion(
+        self, prompt: str = "", chat_history: List[Dict[str, str]] | None = None
+    ) -> Dict[str, Any] | None:
         """
         Requests a text completion from the specified Llama-2 model.
 
         Args:
             prompt (str): Text prompt for generating completion.
+            chat_history (List[Dict[str, str]]): The chat history for conversation
 
         Returns:
-            str | None: The text completion from the model, or None if an error occurs.
+            Dict[str, Any] | None: The model's text response and chat history, or None if an error occurs.
 
         Raises:
             Llama2Exception: If an API or internal error occurs during request processing.
             EmptyPrompt: If no prompt is provided and the instance has no default prompt.
         """
         if not self.api_key:
             raise Llama2Exception(exception="No API Provided", error_type="ValueError")
 
         if self.prompt == "" and prompt == "":
             raise EmptyPrompt("Empty prompt detected")
 
+        if chat_history is None:
+            chat_history = []
+
         try:
             api_url = (
                 f"https://api-inference.huggingface.co/models/meta-llama/{self.model}"
             )
             headers = {"Authorization": f"Bearer {self.api_key}"}
 
             def query(payload):
@@ -231,22 +239,31 @@
                     "parameters": {
                         "max_length": self.max_output_tokens,
                         "temperature": self.temperature,
                         "max_time": self.timeout,
                     },
                 }
             )
+            output_text = output[0]["generated_text"]
+
+            chat_history.append({"role": "user", "content": self.prompt or prompt})
+            chat_history.append({"role": "assistant", "content": output_text})
+
+            provider_response = {
+                "response": output_text,
+                "chat_history": chat_history,
+            }
 
         except Exception as e:
             raise Llama2Exception(exception=e.args[0], error_type="Llama2Error") from e
 
         if output["error"]:
             raise Llama2Exception(exception=output["error"], error_type="Llama2Error")
 
-        return output[0]["generated_text"]
+        return provider_response or None
 
     def tokenize(self, prompt: str = "") -> TokenizeResponse:
         """
         Tokenizes the provided prompt using the tokenizer.
 
         Args:
             prompt (str, optional): The prompt to be tokenized. Defaults to an empty string.
@@ -271,15 +288,14 @@
 
         Args:
             category (str): Task category for which to retrieve the model's rank.
 
         Returns:
             int: Performance rank of the model in the specified category.
         """
-        logger.log(msg=f"MODEL: {self.model}", color="PURPLE")
-        logger.log(msg=f"CATEGORY OF PROMPT: {category}")
+        proxy_logger.log(msg=f"MODEL: {self.model}", color="PURPLE")
 
         category_rank = llama2_category_data["model-categories"][self.model][category]
 
-        logger.log(msg=f"RANK OF PROMPT: {category_rank}", color="BLUE")
+        proxy_logger.log(msg=f"MODEL CATEGORY RANK: {category_rank}", color="BLUE")
 
         return category_rank
```

### Comparing `proxyllm-0.1.6/proxyllm/provider/huggingface/mistral.py` & `proxyllm-0.2.0/proxyllm/provider/mistral/mistral.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,78 @@
-import requests
-from tokenizers import Encoding
+import copy
+from typing import Any, Dict, List
 
 from proxyllm.provider.base import BaseAdapter, TokenizeResponse
-from proxyllm.utils import logger, tokenizer
+from proxyllm.utils import proxy_logger, tokenizer
 from proxyllm.utils.exceptions.provider import MistralException
 
 # Mapping of Mistral model categories to their task performance ratings.
 mistral_category_data = {
     "model-categories": {
-        "mistral-7b-v0.1": {
+        "open-mistral-7b": {
             "Code Generation Task": 2,
             "Text Generation Task": 1,
             "Translation and Multilingual Applications Task": 2,
-            "Natural Language Processing Task": 1,
-            "Conversational AI Task": 1,
-            "Educational Applications Task": 2,
-            "Healthcare and Medical Task": 3,
-            "Legal Task": 3,
-            "Financial Task": 3,
-            "Content Recommendation Task": 2,
+            "Natural Language Processing Task": 2,
+            "Conversational AI Task": 2,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 1,
+            "Legal Task": 4,
+            "Financial Task": 4,
+            "Content Recommendation Task": 3,
+        },
+        "open-mixtral-8x7b": {
+            "Code Generation Task": 2,
+            "Text Generation Task": 1,
+            "Translation and Multilingual Applications Task": 2,
+            "Natural Language Processing Task": 2,
+            "Conversational AI Task": 2,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 1,
+            "Legal Task": 4,
+            "Financial Task": 4,
+            "Content Recommendation Task": 3,
+        },
+        "mistral-small-latest": {
+            "Code Generation Task": 2,
+            "Text Generation Task": 1,
+            "Translation and Multilingual Applications Task": 2,
+            "Natural Language Processing Task": 2,
+            "Conversational AI Task": 2,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 1,
+            "Legal Task": 4,
+            "Financial Task": 4,
+            "Content Recommendation Task": 3,
         },
-        "mixtral-8x7b-instruct-v0.1": {
+        "mistral-medium-latest": {
             "Code Generation Task": 2,
             "Text Generation Task": 1,
             "Translation and Multilingual Applications Task": 2,
-            "Natural Language Processing Task": 1,
-            "Conversational AI Task": 1,
-            "Educational Applications Task": 2,
-            "Healthcare and Medical Task": 3,
-            "Legal Task": 3,
-            "Financial Task": 3,
-            "Content Recommendation Task": 2,
+            "Natural Language Processing Task": 2,
+            "Conversational AI Task": 2,
+            "Educational Applications Task": 1,
+            "Healthcare and Medical Task": 1,
+            "Legal Task": 4,
+            "Financial Task": 4,
+            "Content Recommendation Task": 3,
         },
-        "mistral-7b-instruct-v0.2": {
+        "mistral-large-latest": {
             "Code Generation Task": 2,
             "Text Generation Task": 1,
             "Translation and Multilingual Applications Task": 2,
             "Natural Language Processing Task": 2,
             "Conversational AI Task": 2,
             "Educational Applications Task": 1,
             "Healthcare and Medical Task": 1,
             "Legal Task": 4,
             "Financial Task": 4,
             "Content Recommendation Task": 3,
         },
-    }
+    },
 }
 
 
 class MistralAdapter(BaseAdapter):
     """
     Adapter class for the Mistral language models API.
 
@@ -76,67 +100,81 @@
         self.prompt = prompt
         self.model = model
         self.api_key = api_key
         self.temperature = temperature
         self.max_output_tokens = max_output_tokens
         self.timeout = timeout
 
-    def get_completion(self, prompt: str = "") -> str:
+    def get_completion(
+        self, prompt: str = "", chat_history: List[Dict[str, str]] | None = None
+    ) -> Dict[str, Any] | None:
         """
         Requests a text completion from the specified Mistral model.
 
         Args:
-            prompt (str): Text prompt for generating completion.
+            prompt (str): The text prompt for generating completion.
+            chat_history (List[Dict[str, str]]): The chat history for conversation
 
         Returns:
-            str: The text completion from the model.
+            Dict[str, Any] | None: The model's text response and chat history, or None if an error occurs.
 
         Raises:
-            MistralException: If an API or internal error occurs during request processing.
-            ValueError: If no API key is provided.
+            MistralAPIStatusException: Returned when Mistral receives a non-200 response from the API.
+            MistralAPIException: Returned when the API responds with an error message.
+            MistralConnectionException: Returned when the SDK can not reach the API server for any reason
         """
         if not self.api_key:
-            raise ValueError("No Hugging Face API Key Provided")
+            raise ValueError("No Mistral API Key Provided")
+
+        if chat_history is None:
+            chat_history = []
+
+        from mistralai.client import MistralClient
+        from mistralai.exceptions import (
+            MistralAPIException,
+            MistralAPIStatusException,
+            MistralConnectionException,
+        )
 
         try:
-            api_url = (
-                f"https://api-inference.huggingface.co/models/mistralai/{self.model}"
+            client = MistralClient(api_key=self.api_key, timeout=self.timeout)
+
+            mistral_chat_history = copy.deepcopy(chat_history)
+            mistral_chat_history.append(
+                {"role": "user", "content": prompt or self.prompt}
             )
-            headers = {"Authorization": f"Bearer {self.api_key}"}
 
-            def query(payload):
-                response = requests.post(api_url, headers=headers, json=payload)
-                return response.json()
-
-            output = query(
-                {
-                    "inputs": prompt or self.prompt,
-                    "parameters": {
-                        "temperature": self.temperature,
-                        "max_length": self.max_output_tokens,
-                        "max_time": self.timeout,
-                    },
-                }
+            output = client.chat(
+                max_tokens=self.max_output_tokens,
+                messages=mistral_chat_history,
+                model=self.model,
+                temperature=self.temperature,
             )
+            response_text = output.choices[0].message.content
 
-        except requests.RequestException as e:
-            raise MistralException(
-                f"Request error: {e}", error_type="RequestError"
-            ) from e
+            chat_history.append({"role": "user", "content": prompt or self.prompt})
+            chat_history.append({"role": "assistant", "content": response_text})
+
+            provider_response = {
+                "response": response_text,
+                "chat_history": chat_history,
+            }
+
+        except (
+            MistralConnectionException,
+            MistralAPIException,
+            MistralAPIStatusException,
+        ) as e:
+            raise MistralException(exception=str(e), error_type="MistralError") from e
         except Exception as e:
             raise MistralException(
-                f"Unknown error: {e}", error_type=" Unknown Mistral Error"
+                exception=str(e), error_type="Unknown Mistral Error"
             ) from e
 
-        # Output will be a dict if there is an error
-        if "error" in output:
-            raise MistralException(f"{output['error']}", error_type="MistralError")
-
-        # Output will be a List[dict] if there is no error
-        return output[0]["generated_text"]
+        return provider_response or None
 
     def tokenize(self, prompt: str = "") -> TokenizeResponse:
         """
         Tokenizes the provided prompt using the tokenizer.
 
         Args:
             prompt (str, optional): The prompt to be tokenized. Defaults to an empty string.
@@ -161,15 +199,14 @@
 
         Args:
             category (str): Task category to retrieve the model's rank.
 
         Returns:
             int: Performance rank of the model in the specified category.
         """
-        logger.log(msg=f"MODEL: {self.model}", color="PURPLE")
-        logger.log(msg=f"CATEGORY OF PROMPT: {category}")
+        proxy_logger.log(msg=f"MODEL: {self.model}", color="PURPLE")
 
         category_rank = mistral_category_data["model-categories"][self.model][category]
 
-        logger.log(msg=f"RANK OF PROMPT: {category_rank}", color="BLUE")
+        proxy_logger.log(msg=f"MODEL CATEGORY RANK: {category_rank}", color="BLUE")
 
         return category_rank
```

### Comparing `proxyllm-0.1.6/proxyllm/proxyllm.py` & `proxyllm-0.2.0/proxyllm/proxyllm.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from typing import Any, Dict, List, Literal
 
 import yaml
 from dotenv import load_dotenv
 
 from proxyllm.config.internal_config import internal_config
 from proxyllm.provider.base import BaseAdapter
-from proxyllm.utils import categorization, logger
+from proxyllm.utils import categorization, proxy_logger
 from proxyllm.utils.cost import calculate_estimated_max_cost
 from proxyllm.utils.enums import BaseEnum
 from proxyllm.utils.exceptions.llmproxy_client import (
     LLMProxyConfigError,
     ModelRequestFailed,
     RequestsFailed,
+    UserChatHistoryError,
     UserConfigError,
 )
 from proxyllm.utils.exceptions.provider import UnsupportedModel
 from proxyllm.utils.sorting import MinHeap
 
 
 @dataclass
@@ -26,32 +27,35 @@
     """
     Data structure to store the response from a model completion request.
 
     Attributes:
         response (str): The response text from the model, if successful; otherwise, an empty string.
         response_model (str): The model that successfully responded to the request.
         errors (List): A list of error messages from models that failed to respond.
+        chat_history (List): A list of chat messages/responses from the user and models.
     """
 
     response: str = ""
     response_model: str = ""
     errors: List = field(default_factory=list)
+    chat_history: List[Dict[str, str]] = field(default_factory=list)
 
 
 class RouteType(str, BaseEnum):
     """
     Enumeration for route types supported by LLM Proxy.
 
     Attributes:
         COST: Route requests based on cost efficiency.
-        CATEGORY: Route requests based on category proficiency.
+        CATEGORY: Route requests based on category elo.
     """
 
     COST = "cost"
     CATEGORY = "category"
+    ELO = "elo"
 
 
 def _get_settings_from_yml(
     path_to_yml: str = "",
 ) -> Dict[str, Any]:
     """
     Load and return settings from a YAML file.
@@ -92,15 +96,14 @@
         # Loop through each provider
         for provider in settings:
             key = provider["provider"].lower()
             import_path = provider["adapter_path"]
 
             # Loop through and aggregate all of the variations of "models" of each provider
             provider_models = set()
-            model_costs = {}
             for model in provider.get("models", []):
                 provider_models.add(model["name"])
 
             module_name, class_name = import_path.rsplit(".", 1)
 
             module = importlib.import_module(module_name)
             model_class = getattr(module, class_name)
@@ -215,56 +218,62 @@
         raise e
     except Exception as e:
         raise UserConfigError(
             f"Unknown error occured during llmproxy.config setup:{e}"
         ) from e
 
 
-def _setup_models_cost_data(settings: List[Dict[str, Any]]) -> Dict[str, Any]:
+def _setup_model_data(settings: List[Dict[str, Any]]) -> Dict[str, Any]:
     """
     Extract and return the cost data for each model from configuration settings.
 
     Args:
         settings (List[Dict[str, Any]]): List of configuration settings for each model.
 
     Returns:
         Dict[str, Any]: A dictionary mapping model names to their cost data.
 
     Raises:
         KeyError: If expected keys are missing from the settings.
     """
     try:
-        models_cost_data = {}
+        model_data = {}
         # Loop through all the providers in settings
         for provider in settings:
             # Loop through the "models" and save the cost data for each model
-            for model_data in provider.get("models", []):
-                model_name, prompt_cost, completion_cost = model_data.values()
-                models_cost_data[model_name] = {
+            for model_yml_data in provider.get("models", []):
+                (
+                    model_name,
+                    prompt_cost,
+                    completion_cost,
+                    model_elo,
+                ) = model_yml_data.values()
+                model_data[model_name] = {
                     "prompt": prompt_cost,
                     "completion": completion_cost,
+                    "elo": model_elo,
                 }
-        return models_cost_data
+        return model_data
     except Exception as e:
         raise e
 
 
 def _get_route_type(
     user_settings: Dict[str, Any] | None,
-    constructor_route_type: Literal["cost", "category"] | None,
-) -> Literal["cost", "category"]:
+    constructor_route_type: Literal["cost", "category", "elo"] | None,
+) -> Literal["cost", "category", "elo"]:
     """
     Determine the routing type based on user settings or constructor arguments.
 
     Args:
         user_settings (Dict[str, Any] | None): Configuration from the user settings.
-        constructor_route_type (Literal["cost", "category"] | None): Routing type specified at object construction.
+        constructor_route_type (Literal["cost", "category", "elo"] | None): Routing type specified at object construction.
 
     Returns:
-        Literal["cost", "category"]: The determined route type.
+        Literal["cost", "category", "elo"]: The determined route type.
 
     Raises:
         UserConfigError: If the route type is not specified or invalid.
     """
     route_type = None
     if constructor_route_type is not None:
         route_type = constructor_route_type
@@ -294,22 +303,22 @@
     This class initializes the proxy with user-defined settings, sets up model adapters,
     and routes requests to the most suitable models based on the selected routing strategy.
 
     Attributes:
         user_models (Dict[str, BaseAdapter]): Models configured by the user, ready for use.
         available_models (Dict[str, Any]): All models available within the proxy.
         route_type (Literal["cost", "category"]): Selected routing strategy.
-        models_cost_data (Dict[str, Any]): Cost data for each model used in cost-based routing.
+        model_data (Dict[str, Any]): Data for each model used in cost-based or elo routing.
     """
 
     def __init__(
         self,
         path_to_user_configuration: str = "llmproxy.config.yml",
         path_to_env_vars: str = ".env",
-        route_type: Literal["cost", "category"] | None = None,
+        route_type: Literal["cost", "category", "elo"] | None = None,
         **kwargs,
     ) -> None:
         """
         Initialize YourClass instance.
 
         Args:
             path_to_user_configuration (str): Path to user configuration YAML file.
@@ -336,40 +345,51 @@
         )
 
         # Setup user cost
         self.route_type = _get_route_type(
             user_settings=user_settings, constructor_route_type=route_type
         )
 
-        if self.route_type == RouteType.COST:
+        if self.route_type == RouteType.COST or RouteType.ELO:
             # Setup the cost data of each model
-            self.models_cost_data = _setup_models_cost_data(settings=internal_config)
+            self.model_data = _setup_model_data(settings=internal_config)
 
     def route(
         self,
         prompt: str = "",
+        chat_history: List[Dict[str, str]] = None,
     ) -> CompletionResponse:
         """
         Routes the request to the appropriate models based on the routing strategy.
 
         Args:
             prompt (str): The input prompt to generate text for.
+            chat_history (List[Dict[str, str]]): The chat history for conversation
 
         Returns:
             CompletionResponse: The generated text response along with any errors encountered.
         """
-        match RouteType(self.route_type):
-            case RouteType.COST:
-                return self._cost_route(prompt=prompt)
-            case RouteType.CATEGORY:
-                return self._category_route(prompt=prompt)
-            case _:
-                raise ValueError("Invalid route type, please try again")
+        if isinstance(chat_history, list) or chat_history is None:
+            match RouteType(self.route_type):
+                case RouteType.COST:
+                    return self._cost_route(prompt=prompt, chat_history=chat_history)
+                case RouteType.CATEGORY:
+                    return self._category_route(
+                        prompt=prompt, chat_history=chat_history
+                    )
+                case RouteType.ELO:
+                    return self._elo_route(prompt=prompt, chat_history=chat_history)
+                case _:
+                    raise ValueError("Invalid route type, please try again")
+        else:
+            raise UserChatHistoryError(
+                "Incorrect format for chat_history: chat_history needs to be a List[Dict[str,str]]."
+            )
 
-    def _cost_route(self, prompt: str):
+    def _cost_route(self, prompt: str, chat_history: List[Dict[str, str]]):
         """
         Routes requests based on cost efficiency.
 
         Args:
             prompt (str): The input prompt for the text generation.
 
         Returns:
@@ -380,189 +400,298 @@
             raise ValueError("No prompt provided.")
 
         min_heap = MinHeap()
         provider_token_data = {}
 
         for model_name, instance in self.user_models.items():
             try:
-                logger.log(msg="========Start Cost Estimation===========")
+                proxy_logger.log(msg="========Start Cost Estimation===========")
 
-                logger.log(msg=f"MODEL: {model_name}", color="PURPLE")
-                logger.log(
-                    msg=f"PROMPT (COST/CHARACTER): {self.models_cost_data[model_name]['prompt']}"
+                proxy_logger.log(msg=f"MODEL: {model_name}", color="PURPLE")
+                proxy_logger.log(
+                    msg=f"PROMPT (COST/CHARACTER): {self.model_data[model_name]['prompt']}"
                 )
-                logger.log(
-                    msg=f"PROMPT (COST/CHARACTER): {self.models_cost_data[model_name]['completion']}"
+                proxy_logger.log(
+                    msg=f"PROMPT (COST/CHARACTER): {self.model_data[model_name]['completion']}"
                 )
 
                 instance_provider = instance.__class__.__name__
 
                 # Save token data per provider
                 if instance_provider not in provider_token_data:
                     provider_token_data[instance_provider] = instance.tokenize(
                         prompt=prompt
                     )
 
                 token_data = provider_token_data[instance_provider]
 
                 cost = calculate_estimated_max_cost(
-                    price_data=self.models_cost_data[model_name],
+                    price_data=self.model_data[model_name],
                     num_of_input_tokens=token_data.num_of_input_tokens,
                     max_output_tokens=token_data.num_of_output_tokens,
                 )
 
                 item = {
                     "name": model_name,
                     "cost": cost,
                     "instance": instance,
                 }
 
                 min_heap.push(cost, item)
 
-                logger.log(msg=f"INPUT TOKENS: {token_data.num_of_input_tokens}")
-                logger.log(msg=f"COMPLETION TOKENS: {token_data.num_of_output_tokens}")
+                proxy_logger.log(msg=f"INPUT TOKENS: {token_data.num_of_input_tokens}")
+                proxy_logger.log(
+                    msg=f"COMPLETION TOKENS: {token_data.num_of_output_tokens}"
+                )
 
-                logger.log(msg=f"COST: {cost}", color="GREEN")
-                logger.log(msg="========End Cost Estimation===========\n")
+                proxy_logger.log(msg=f"COST: {cost}", color="GREEN")
+                proxy_logger.log(msg="========End Cost Estimation===========\n")
             except Exception as e:
-                logger.log(level="ERROR", msg=str(e))
-                logger.log(level="ERROR", msg="(¬_¬)", file_logger_on=False)
-                logger.log(msg="========End Cost Estimation===========\n")
+                proxy_logger.log(level="ERROR", msg=str(e))
+                proxy_logger.log(level="ERROR", msg="(¬_¬)", file_logger_on=False)
+                proxy_logger.log(msg="========End Cost Estimation===========\n")
 
         completion_res = None
         errors = []
         response_model = ""
+
         while not completion_res:
             # Iterate through heap until there are no more options
             min_val_instance = min_heap.pop_min()
             if not min_val_instance:
                 break
 
             instance_data = min_val_instance["data"]
-            logger.log(msg="========START COST ROUTING===========")
-            logger.log(msg=f"Making request to model:{instance_data['name']}")
-            logger.log(msg="ROUTING...")
+            proxy_logger.log(msg="========START COST ROUTING===========")
+            proxy_logger.log(msg=f"Making request to model:{instance_data['name']}")
+            proxy_logger.log(msg="ROUTING...")
 
             try:
-                completion_res = instance_data["instance"].get_completion(prompt=prompt)
+                completion_res = instance_data["instance"].get_completion(
+                    prompt=prompt, chat_history=chat_history
+                )
                 response_model = instance_data["name"]
-                logger.log(
+                proxy_logger.log(
                     msg="==========COST ROUTING COMPLETE! Call to model successful!==========",
                     color="GREEN",
                 )
-                logger.log(msg="(• ◡ •)\n", file_logger_on=False, color="GREEN")
+                proxy_logger.log(msg="(• ◡ •)\n", file_logger_on=False, color="GREEN")
             except Exception as e:
                 errors.append(
                     {
                         "model_name": instance_data["name"],
                         "error_type": e.__class__.__name__,
                         "error": str(e),
                     }
                 )
 
-                logger.log(
+                proxy_logger.log(
                     level="ERROR",
                     msg=f"Request to model {instance_data['name']} failed!",
                 )
-                logger.log(
+                proxy_logger.log(
                     level="ERROR", msg=f"Error when making request to model: {e}"
                 )
-                logger.log(level="ERROR", msg="(•᷄ ∩ •᷅)", file_logger_on=False)
+                proxy_logger.log(level="ERROR", msg="(•᷄ ∩ •᷅)", file_logger_on=False)
 
-                logger.log(
+                proxy_logger.log(
                     level="ERROR",
                     msg="========COST ROUTING FAILED!===========\n",
                 )
 
         # If all model fails raise an Exception to notify user
         if not completion_res:
             raise ModelRequestFailed(
                 "Requests to all models failed! Please check your configuration!"
             )
 
         return CompletionResponse(
-            response=completion_res, response_model=response_model, errors=errors
+            response=completion_res["response"],
+            response_model=response_model,
+            errors=errors,
+            chat_history=completion_res["chat_history"],
         )
 
-    def _category_route(self, prompt: str):
+    def _category_route(self, prompt: str, chat_history: List[Dict[str, str]]):
         """
-        Routes requests based on the category proficiency of available models.
+        Routes requests based on the category elo of available models.
 
         Args:
             prompt (str): The input prompt for the text generation.
 
         Returns:
             CompletionResponse: The response from the model best suited for the prompt's category.
         """
         min_heap = MinHeap()
         best_fit_category = categorization.categorize_text(prompt)
+        proxy_logger.log(msg=f"CATEGORY OF PROMPT: {best_fit_category}")
+
         for model_name, instance in self.user_models.items():
-            logger.log(
-                msg="========Fetching model for category routing===========",
+            proxy_logger.log(
+                msg="========Fetching Model For Category Routing===========",
             )
 
-            logger.log(
-                msg="Sorting fetched models based on proficency...",
-            )
             category_rank = instance.get_category_rank(best_fit_category)
             item = {"name": model_name, "rank": category_rank, "instance": instance}
             min_heap.push(category_rank, item)
 
-            logger.log(
-                msg="========Finished fetching model for category routing=============\n",
+            proxy_logger.log(
+                msg="========Finished Fetching Model For Category Routing=============\n",
             )
 
         completion_res = None
         errors = []
         response_model = ""
+
         while not completion_res:
             # Iterate through heap until there are no more options
             min_val_instance = min_heap.pop_min()
             if not min_val_instance:
                 break
 
             instance_data = min_val_instance["data"]
-            logger.log(
+            proxy_logger.log(msg="========START COST ROUTING===========")
+            proxy_logger.log(
                 msg=f"Making request to model: {instance_data['name']}",
             )
 
             try:
-                completion_res = instance_data["instance"].get_completion(prompt=prompt)
+                completion_res = instance_data["instance"].get_completion(
+                    prompt=prompt, chat_history=chat_history
+                )
                 response_model = instance_data["name"]
-                logger.log(
+                proxy_logger.log(
                     msg="CATEGORY ROUTING COMPLETE! Call to model successful!",
                 )
-                logger.log(msg="(• ◡ •)\n", file_logger_on=False, color="GREEN")
+                proxy_logger.log(msg="(• ◡ •)\n", file_logger_on=False, color="GREEN")
             except Exception as e:
                 errors.append(
                     {
                         "model_name": instance_data["name"],
                         "error_type": e.__class__.__name__,
                         "error": str(e),
                     }
                 )
 
-                logger.log(
+                proxy_logger.log(
                     level="ERROR",
                     msg=f"Request to model {instance_data['name']} failed!",
                 )
 
-                logger.log(
+                proxy_logger.log(
                     level="ERROR",
                     msg=f"Error when making request to model: {e}",
                 )
 
-                logger.log(level="ERROR", msg="(•᷄ ∩ •᷅)", file_logger_on=False)
+                proxy_logger.log(level="ERROR", msg="(•᷄ ∩ •᷅)", file_logger_on=False)
 
-                logger.log(
+                proxy_logger.log(
                     level="ERROR",
                     msg="========CATEGORY ROUTING FAILED!===========\n",
                 )
 
         if not completion_res:
             raise RequestsFailed(
                 "Requests to all models failed! Please check your configuration!"
             )
 
         return CompletionResponse(
-            response=completion_res, response_model=response_model, errors=errors
+            response=completion_res["response"],
+            response_model=response_model,
+            errors=errors,
+            chat_history=completion_res["chat_history"],
+        )
+
+    def _elo_route(self, prompt: str, chat_history: List[Dict[str, str]]):
+        """
+        Routes the request to the appropriate models based on elo elo rating of available models
+
+        Args:
+            prompt (str): The input prompt to generate text for.
+
+        Returns:
+            CompletionResponse: The generated text response along with any errors encountered.
+        """
+
+        min_heap = MinHeap()
+        proxy_logger.log(
+            msg="Sorting fetched models based on elo rating...", color="GREEN"
+        )
+        for model_name, instance in self.user_models.items():
+            proxy_logger.log(
+                msg="========Fetching Models for Elo Routing===========",
+            )
+
+            proxy_logger.log(msg=f"MODEL: {model_name}", color="PURPLE")
+
+            elo_rating = self.model_data[model_name]["elo"]
+
+            proxy_logger.log(msg=f"ELO RATING OF MODEL: {elo_rating}", color="BLUE")
+
+            item = {"name": model_name, "elo": elo_rating, "instance": instance}
+            min_heap.push(-1 * elo_rating, item)
+
+            proxy_logger.log(
+                msg="========Finished Model Fetching For Elo Routing=============\n",
+            )
+
+        completion_res = None
+        errors = []
+        response_model = ""
+        while not completion_res:
+            # Iterate through heap until there are no more options
+            max_val_instance = min_heap.pop_min()
+            if not max_val_instance:
+                break
+
+            instance_data = max_val_instance["data"]
+            proxy_logger.log(msg="========START ELO ROUTING===========")
+            proxy_logger.log(msg=f"Making request to model:{instance_data['name']}")
+            proxy_logger.log(msg="ROUTING...")
+
+            try:
+                completion_res = instance_data["instance"].get_completion(
+                    prompt=prompt, chat_history=chat_history
+                )
+                response_model = instance_data["name"]
+                proxy_logger.log(
+                    msg="==========ELO ROUTING COMPLETE! Call to model successful!==========",
+                    color="GREEN",
+                )
+                proxy_logger.log(msg="(• ◡ •)\n", file_logger_on=False, color="GREEN")
+            except Exception as e:
+                errors.append(
+                    {
+                        "model_name": instance_data["name"],
+                        "error_type": e.__class__.__name__,
+                        "error": str(e),
+                    }
+                )
+
+                proxy_logger.log(
+                    level="ERROR",
+                    msg=f"Request to model {instance_data['name']} failed!",
+                )
+
+                proxy_logger.log(
+                    level="ERROR",
+                    msg=f"Error when making request to model: {e}",
+                )
+
+                proxy_logger.log(level="ERROR", msg="(•᷄ ∩ •᷅)", file_logger_on=False)
+
+                proxy_logger.log(
+                    level="ERROR",
+                    msg="========ELO ROUTING FAILED!===========\n",
+                )
+
+        if not completion_res:
+            raise RequestsFailed(
+                "Requests to all models failed! Please check your configuration!"
+            )
+
+        return CompletionResponse(
+            response=completion_res["response"],
+            response_model=response_model,
+            errors=errors,
+            chat_history=completion_res["chat_history"],
         )
```

### Comparing `proxyllm-0.1.6/proxyllm/utils/categorization.py` & `proxyllm-0.2.0/proxyllm/utils/categorization.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from transformers import pipeline
 
-from proxyllm.utils import logger
+from proxyllm.utils import proxy_logger
 
 
 def categorize_text(prompt: str) -> str:
     """
     Categorizes the given text prompt into predefined categories using a zero-shot classification approach.
 
     Utilizes the 'facebook/bart-large-mnli' model to classify the prompt into one of several predefined task categories.
@@ -26,14 +26,14 @@
         "Conversational AI Task",
         "Educational Applications Task",
         "Healthcare and Medical Task",
         "Legal Task",
         "Financial Task",
         "Content Recommendation Task",
     ]
-    logger.log(msg="Classification model is classifying the user prompt")
+    proxy_logger.log(msg="Classification model is classifying the user prompt")
     classifier = pipeline(task="zero-shot-classification", model=model)
-    logger.log(msg="The prompt has been classified\n")
+    proxy_logger.log(msg="The prompt has been classified\n")
 
     results = classifier(prompt, candidate_labels)
     best_category = results["labels"][0]
     return best_category
```

### Comparing `proxyllm-0.1.6/proxyllm/utils/cost.py` & `proxyllm-0.2.0/proxyllm/utils/cost.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/proxyllm/utils/enums.py` & `proxyllm-0.2.0/proxyllm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/proxyllm/utils/exceptions/provider.py` & `proxyllm-0.2.0/proxyllm/utils/exceptions/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 
 class OpenAIException(Exception):
     def __init__(self, exception: str, error_type: str) -> None:
         super().__init__(f"OpenAI Error: {exception}, Type: {error_type}")
 
 
+class AnthropicException(Exception):
+    def __init__(self, exception: str, error_type: str) -> None:
+        super().__init__(f"Anthropic Error: {exception}, Type: {error_type}")
+
+
 class UnsupportedModel(Exception):
     """
     General Exceptions shared across models
     """
 
     def __init__(self, exception: str, error_type: str) -> None:
         super().__init__(f"Unsupported Model Error: {exception}, Type: {error_type}")
```

### Comparing `proxyllm-0.1.6/proxyllm/utils/logger.py` & `proxyllm-0.2.0/proxyllm/utils/proxy_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime as dt
 import logging
 import sys
+from logging import NullHandler
 from typing import Literal
 
 
 class CustomFormatter(logging.Formatter):
     """
     Custom logging Formatter class that adds color coding to log messages for console output,
     enhancing the visibility and differentiation of log levels.
@@ -115,14 +116,18 @@
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(CustomLogger.file_formatter())
         file_logger.addHandler(file_handler)
         CustomLogger._file_logger = file_logger
         return file_logger
 
 
+# Prevent external loggers from using our custom loggers
+null_handler = NullHandler()
+logging.getLogger().addHandler(null_handler)
+
 file_logger = CustomLogger.get_file_logger()
 console_logger = CustomLogger.get_console_logger()
 
 
 def log(
     level: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "INFO",
     msg: str = "",
```

### Comparing `proxyllm-0.1.6/proxyllm/utils/sorting.py` & `proxyllm-0.2.0/proxyllm/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/proxyllm/utils/timeout_function.py` & `proxyllm-0.2.0/proxyllm/utils/timeout_function.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/proxyllm/utils/tokenizer.py` & `proxyllm-0.2.0/proxyllm/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.1.6/pyproject.toml` & `proxyllm-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "proxyllm"
-version = "0.1.6"
+version = "0.2.0"
 description = "LLM Proxy to reduce cost and complexity of using multiple LLMs"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^1.0.0"
 cohere = "^4.27"
 google-cloud-aiplatform = "^1.35.0"
-pyyaml = "^6.0.1"
-datasets = "^2.14.7"
-evaluate = "^0.4.1"
 openai = "^1.11.1"
+anthropic = "^0.20.0"
 click = "^8.1.7"
-transformers = "^4.38.2"
 torch = "^2.2.1"
+transformers = "^4.38.2" # remove once we depricate classification routing
 tiktoken = "^0.6.0"
+mistralai = "^0.1.8"
 
 [tool.poetry.scripts]
 config = "proxyllm.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
 isort = "^5.13.2"
```

### Comparing `proxyllm-0.1.6/PKG-INFO` & `proxyllm-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: proxyllm
-Version: 0.1.6
+Version: 0.2.0
 Summary: LLM Proxy to reduce cost and complexity of using multiple LLMs
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: anthropic (>=0.20.0,<0.21.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cohere (>=4.27,<5.0)
-Requires-Dist: datasets (>=2.14.7,<3.0.0)
-Requires-Dist: evaluate (>=0.4.1,<0.5.0)
 Requires-Dist: google-cloud-aiplatform (>=1.35.0,<2.0.0)
+Requires-Dist: mistralai (>=0.1.8,<0.2.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: torch (>=2.2.1,<3.0.0)
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: proxyllm Version: 0.1.6 Summary: LLM Proxy to
+Metadata-Version: 2.1 Name: proxyllm Version: 0.2.0 Summary: LLM Proxy to
 reduce cost and complexity of using multiple LLMs Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: cohere (>=4.27,<5.0)
-Requires-Dist: datasets (>=2.14.7,<3.0.0) Requires-Dist: evaluate
-(>=0.4.1,<0.5.0) Requires-Dist: google-cloud-aiplatform (>=1.35.0,<2.0.0)
+Requires-Dist: anthropic (>=0.20.0,<0.21.0) Requires-Dist: click
+(>=8.1.7,<9.0.0) Requires-Dist: cohere (>=4.27,<5.0) Requires-Dist: google-
+cloud-aiplatform (>=1.35.0,<2.0.0) Requires-Dist: mistralai (>=0.1.8,<0.2.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0) Requires-Dist: python-dotenv
-(>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: tiktoken
-(>=0.6.0,<0.7.0) Requires-Dist: torch (>=2.2.1,<3.0.0) Requires-Dist:
-transformers (>=4.38.2,<5.0.0) Description-Content-Type: text/markdown
+(>=1.0.0,<2.0.0) Requires-Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist: torch
+(>=2.2.1,<3.0.0) Requires-Dist: transformers (>=4.38.2,<5.0.0) Description-
+Content-Type: text/markdown
                               ******** LLLLMM PPrrooxxyy ********
    A low-code solution to efficiently manage multiple large language models
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
```

