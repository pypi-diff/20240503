# Comparing `tmp/cohere_haystack-0.7.0.tar.gz` & `tmp/cohere_haystack-1.0.0.tar.gz`

## Comparing `cohere_haystack-0.7.0.tar` & `cohere_haystack-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/examples/cohere_ranker_in_a_pipeline.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/pydoc/config.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/__init__.py
--rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
--rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/utils.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/__init__.py
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
--rw-r--r--   0        0        0    10087 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/rankers/cohere/__init__.py
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/rankers/cohere/ranker.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_cohere_chat_generator.py
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_cohere_generators.py
--rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_cohere_ranker.py
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_document_embedder.py
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/README.md
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/examples/cohere_ranker_in_a_pipeline.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/pydoc/config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/__init__.py
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/utils.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/__init__.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/rankers/cohere/__init__.py
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/rankers/cohere/ranker.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_cohere_chat_generator.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_cohere_generators.py
+-rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_cohere_ranker.py
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_document_embedder.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/README.md
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/PKG-INFO
```

### Comparing `cohere_haystack-0.7.0/examples/cohere_ranker_in_a_pipeline.py` & `cohere_haystack-1.0.0/examples/cohere_ranker_in_a_pipeline.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/pydoc/config.yml` & `cohere_haystack-1.0.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py` & `cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         self,
         api_key: Secret = Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"]),
         model: str = "embed-english-v2.0",
         input_type: str = "search_document",
         api_base_url: str = "https://api.cohere.com",
         truncate: str = "END",
         use_async_client: bool = False,
-        max_retries: int = 3,
         timeout: int = 120,
         batch_size: int = 32,
         progress_bar: bool = True,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
     ):
         """
@@ -63,30 +62,28 @@
         :param api_base_url: the Cohere API Base url.
         :param truncate: truncate embeddings that are too long from start or end, ("NONE"|"START"|"END").
             Passing "START" will discard the start of the input. "END" will discard the end of the input. In both
             cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
             If "NONE" is selected, when the input exceeds the maximum input token length an error will be returned.
         :param use_async_client: flag to select the AsyncClient. It is recommended to use
             AsyncClient for applications with many concurrent calls.
-        :param max_retries: maximal number of retries for requests.
         :param timeout: request timeout in seconds.
         :param batch_size: number of Documents to encode at once.
         :param progress_bar: whether to show a progress bar or not. Can be helpful to disable in production deployments
                              to keep the logs clean.
         :param meta_fields_to_embed: list of meta fields that should be embedded along with the Document text.
         :param embedding_separator: separator used to concatenate the meta fields to the Document text.
         """
 
         self.api_key = api_key
         self.model = model
         self.input_type = input_type
         self.api_base_url = api_base_url
         self.truncate = truncate
         self.use_async_client = use_async_client
-        self.max_retries = max_retries
         self.timeout = timeout
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
 
     def to_dict(self) -> Dict[str, Any]:
@@ -100,15 +97,14 @@
             self,
             api_key=self.api_key.to_dict(),
             model=self.model,
             input_type=self.input_type,
             api_base_url=self.api_base_url,
             truncate=self.truncate,
             use_async_client=self.use_async_client,
-            max_retries=self.max_retries,
             timeout=self.timeout,
             batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             meta_fields_to_embed=self.meta_fields_to_embed,
             embedding_separator=self.embedding_separator,
         )
 
@@ -166,26 +162,24 @@
         api_key = self.api_key.resolve_value()
         assert api_key is not None
 
         if self.use_async_client:
             cohere_client = AsyncClient(
                 api_key,
                 base_url=self.api_base_url,
-                max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             all_embeddings, metadata = asyncio.run(
                 get_async_response(cohere_client, texts_to_embed, self.model, self.input_type, self.truncate)
             )
         else:
             cohere_client = Client(
                 api_key,
                 base_url=self.api_base_url,
-                max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             all_embeddings, metadata = get_response(
                 cohere_client,
                 texts_to_embed,
                 self.model,
```

### Comparing `cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py` & `cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         self,
         api_key: Secret = Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"]),
         model: str = "embed-english-v2.0",
         input_type: str = "search_query",
         api_base_url: str = "https://api.cohere.com",
         truncate: str = "END",
         use_async_client: bool = False,
-        max_retries: int = 3,
         timeout: int = 120,
     ):
         """
         :param api_key: the Cohere API key.
         :param model: the name of the model to use. Supported Models are:
             `"embed-english-v3.0"`, `"embed-english-light-v3.0"`, `"embed-multilingual-v3.0"`,
             `"embed-multilingual-light-v3.0"`, `"embed-english-v2.0"`, `"embed-english-light-v2.0"`,
@@ -56,25 +55,23 @@
         :param api_base_url: the Cohere API Base url.
         :param truncate: truncate embeddings that are too long from start or end, ("NONE"|"START"|"END").
             Passing "START" will discard the start of the input. "END" will discard the end of the input. In both
             cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
             If "NONE" is selected, when the input exceeds the maximum input token length an error will be returned.
         :param use_async_client: flag to select the AsyncClient. It is recommended to use
             AsyncClient for applications with many concurrent calls.
-        :param max_retries: maximum number of retries for requests.
         :param timeout: request timeout in seconds.
         """
 
         self.api_key = api_key
         self.model = model
         self.input_type = input_type
         self.api_base_url = api_base_url
         self.truncate = truncate
         self.use_async_client = use_async_client
-        self.max_retries = max_retries
         self.timeout = timeout
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
@@ -84,15 +81,14 @@
             self,
             api_key=self.api_key.to_dict(),
             model=self.model,
             input_type=self.input_type,
             api_base_url=self.api_base_url,
             truncate=self.truncate,
             use_async_client=self.use_async_client,
-            max_retries=self.max_retries,
             timeout=self.timeout,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "CohereTextEmbedder":
         """
         Deserializes the component from a dictionary.
@@ -128,25 +124,23 @@
         api_key = self.api_key.resolve_value()
         assert api_key is not None
 
         if self.use_async_client:
             cohere_client = AsyncClient(
                 api_key,
                 base_url=self.api_base_url,
-                max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             embedding, metadata = asyncio.run(
                 get_async_response(cohere_client, [text], self.model, self.input_type, self.truncate)
             )
         else:
             cohere_client = Client(
                 api_key,
                 base_url=self.api_base_url,
-                max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             embedding, metadata = get_response(cohere_client, [text], self.model, self.input_type, self.truncate)
 
         return {"embedding": embedding[0], "meta": metadata}
```

### Comparing `cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/utils.py` & `cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,14 @@
 
     for i in tqdm(
         range(0, len(texts), batch_size),
         disable=not progress_bar,
         desc="Calculating embeddings",
     ):
         batch = texts[i : i + batch_size]
-        response = cohere_client.embed(batch, model=model_name, input_type=input_type, truncate=truncate)
+        response = cohere_client.embed(texts=batch, model=model_name, input_type=input_type, truncate=truncate)
         for emb in response.embeddings:
             all_embeddings.append(emb)
         if response.meta is not None:
             metadata = response.meta
 
     return all_embeddings, metadata
```

### Comparing `cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/generator.py` & `cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import logging
-from typing import Any, Callable, Dict, List, Optional, cast
+from typing import Any, Callable, Dict, List, Optional
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.components.generators.utils import deserialize_callback_handler, serialize_callback_handler
 from haystack.dataclasses import StreamingChunk
 from haystack.utils import Secret, deserialize_secrets_inplace
 
-from cohere import Client, Generation
+from cohere import Client
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class CohereGenerator:
     """LLM Generator compatible with Cohere's generate endpoint.
@@ -71,14 +71,18 @@
                 repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied
                 equally to all tokens that have already appeared, regardless of their exact frequencies.
             - 'return_likelihoods': One of GENERATION|ALL|NONE to specify how and if the token likelihoods are returned
                 with the response. Defaults to NONE.
             - 'logit_bias': Used to prevent the model from generating unwanted tokens or to incentivize it to include
                 desired tokens. The format is {token_id: bias} where bias is a float between -10 and 10.
         """
+        logger.warning(
+            "The 'generate' API is marked as Legacy and is no longer maintained by Cohere. "
+            "We recommend to use the CohereChatGenerator instead."
+        )
         if not api_base_url:
             api_base_url = "https://api.cohere.com"
 
         self.api_key = api_key
         self.model = model
         self.streaming_callback = streaming_callback
         self.api_base_url = api_base_url
@@ -128,42 +132,39 @@
         :returns: A dictionary with the following keys:
             - `replies`: the list of replies generated by the model.
             - `meta`: metadata about the request.
         """
         if self.streaming_callback:
             response = self.client.generate_stream(model=self.model, prompt=prompt, **self.model_parameters)
             metadata_dict: Dict[str, Any] = {}
-            for chunk in response:
-                stream_chunk = self._build_chunk(chunk)
-                self.streaming_callback(stream_chunk)
-            replies = response.texts
-            metadata_dict["finish_reason"] = response.finish_reason
-            metadata = [metadata_dict]
-            self._check_truncated_answers(metadata)
-            return {"replies": replies, "meta": metadata}
+            generated_text = ""
+            for event in response:
+                if event.event_type == "text-generation":
+                    generated_text += event.text
+                    stream_chunk = self._build_chunk(event)
+                    self.streaming_callback(stream_chunk)
+                elif event.event_type == "stream-end":
+                    metadata_dict["finish_reason"] = event.finish_reason
+                    if event.finish_reason == "MAX_TOKENS":
+                        logger.warning(
+                            "Responses have been truncated before reaching a natural stopping point. "
+                            "Increase the max_tokens parameter to allow for longer completions."
+                        )
+            return {"replies": [generated_text], "meta": [metadata_dict]}
 
         response = self.client.generate(model=self.model, prompt=prompt, **self.model_parameters)
-        metadata = [{"finish_reason": resp.finish_reason} for resp in cast(Generation, response)]
-        replies = [resp.text for resp in response]
-        self._check_truncated_answers(metadata)
-        return {"replies": replies, "meta": metadata}
+        metadata = {"finish_reason": response.finish_reason}
+        if response.finish_reason == "MAX_TOKENS":
+            logger.warning(
+                "Responses have been truncated before reaching a natural stopping point. "
+                "Increase the max_tokens parameter to allow for longer completions."
+            )
+        return {"replies": [response.text], "meta": [metadata]}
 
     def _build_chunk(self, chunk) -> StreamingChunk:
         """
         Converts the response from the Cohere API to a StreamingChunk.
         :param chunk: The chunk returned by the OpenAI API.
         :returns: The StreamingChunk.
         """
         streaming_chunk = StreamingChunk(content=chunk.text, meta={"index": chunk.index})
         return streaming_chunk
-
-    def _check_truncated_answers(self, metadata: List[Dict[str, Any]]):
-        """
-        Check the `finish_reason` returned with the Cohere response.
-        If the `finish_reason` is `MAX_TOKEN`, log a warning to the user.
-        :param metadata: The metadata returned by the Cohere API.
-        """
-        if metadata[0]["finish_reason"] == "MAX_TOKENS":
-            logger.warning(
-                "Responses have been truncated before reaching a natural stopping point. "
-                "Increase the max_tokens parameter to allow for longer completions."
-            )
```

### Comparing `cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py` & `cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,29 +159,40 @@
         if self.streaming_callback:
             response = self.client.chat_stream(
                 message=messages[-1].content,
                 model=self.model,
                 chat_history=chat_history,
                 **generation_kwargs,
             )
-            for chunk in response:
-                if chunk.event_type == "text-generation":
-                    stream_chunk = self._build_chunk(chunk)
+
+            response_text = ""
+            finish_response = None
+            for event in response:
+                if event.event_type == "text-generation":
+                    stream_chunk = self._build_chunk(event)
                     self.streaming_callback(stream_chunk)
-            chat_message = ChatMessage.from_assistant(content=response.texts)
-            chat_message.meta.update(
-                {
-                    "model": self.model,
-                    "usage": response.token_count,
-                    "index": 0,
-                    "finish_reason": response.finish_reason,
-                    "documents": response.documents,
-                    "citations": response.citations,
-                }
-            )
+                    response_text += event.text
+                elif event.event_type == "stream-end":
+                    finish_response = event.response
+            chat_message = ChatMessage.from_assistant(content=response_text)
+
+            if finish_response and finish_response.meta:
+                if finish_response.meta.billed_units:
+                    tokens_in = finish_response.meta.billed_units.input_tokens or -1
+                    tokens_out = finish_response.meta.billed_units.output_tokens or -1
+                    chat_message.meta["usage"] = tokens_in + tokens_out
+                chat_message.meta.update(
+                    {
+                        "model": self.model,
+                        "index": 0,
+                        "finish_reason": finish_response.finish_reason,
+                        "documents": finish_response.documents,
+                        "citations": finish_response.citations,
+                    }
+                )
         else:
             response = self.client.chat(
                 message=messages[-1].content,
                 model=self.model,
                 chat_history=chat_history,
                 **generation_kwargs,
             )
@@ -191,29 +202,31 @@
     def _build_chunk(self, chunk) -> StreamingChunk:
         """
         Converts the response from the Cohere API to a StreamingChunk.
         :param chunk: The chunk returned by the OpenAI API.
         :param choice: The choice returned by the OpenAI API.
         :returns: The StreamingChunk.
         """
-        chat_message = StreamingChunk(content=chunk.text, meta={"index": chunk.index, "event_type": chunk.event_type})
+        chat_message = StreamingChunk(content=chunk.text, meta={"event_type": chunk.event_type})
         return chat_message
 
     def _build_message(self, cohere_response):
         """
         Converts the non-streaming response from the Cohere API to a ChatMessage.
         :param cohere_response: The completion returned by the Cohere API.
         :returns: The ChatMessage.
         """
         content = cohere_response.text
         message = ChatMessage.from_assistant(content=content)
+
+        total_tokens = cohere_response.meta.billed_units.input_tokens + cohere_response.meta.billed_units.output_tokens
         message.meta.update(
             {
                 "model": self.model,
-                "usage": cohere_response.token_count,
+                "usage": total_tokens,
                 "index": 0,
                 "finish_reason": None,
                 "documents": cohere_response.documents,
                 "citations": cohere_response.citations,
             }
         )
         return message
```

### Comparing `cohere_haystack-0.7.0/src/haystack_integrations/components/rankers/cohere/ranker.py` & `cohere_haystack-1.0.0/src/haystack_integrations/components/rankers/cohere/ranker.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/tests/test_cohere_chat_generator.py` & `cohere_haystack-1.0.0/tests/test_cohere_chat_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,20 @@
 import os
-from unittest.mock import Mock, patch
+from unittest.mock import Mock
 
-import cohere
 import pytest
+from cohere.core import ApiError
 from haystack.components.generators.utils import print_streaming_chunk
 from haystack.dataclasses import ChatMessage, ChatRole, StreamingChunk
 from haystack.utils import Secret
 from haystack_integrations.components.generators.cohere import CohereChatGenerator
 
 pytestmark = pytest.mark.chat_generators
 
 
-@pytest.fixture
-def mock_chat_response():
-    """
-    Mock the Cohere API response and reuse it for tests
-    """
-    with patch("cohere.Client.chat", autospec=True) as mock_chat_response:
-        # mimic the response from the Cohere API
-
-        mock_response = Mock()
-        mock_response.text = "I'm fine, thanks."
-        mock_response.token_count = {
-            "prompt_tokens": 66,
-            "response_tokens": 78,
-            "total_tokens": 144,
-            "billed_tokens": 133,
-        }
-        mock_response.meta = {
-            "api_version": {"version": "1"},
-            "billed_units": {"input_tokens": 55, "output_tokens": 78},
-        }
-        mock_chat_response.return_value = mock_response
-        yield mock_chat_response
-
-
-@pytest.fixture
-def mock_chat_streaming_response():
-    with patch("cohere.Client.chat_stream", autospec=True) as mock_chat_stream_response:
-        # mimic the response from the Cohere API
-
-        mock_response = Mock()
-        mock_response.text = "I'm fine, thanks."
-        mock_response.token_count = {
-            "prompt_tokens": 66,
-            "response_tokens": 78,
-            "total_tokens": 144,
-            "billed_tokens": 133,
-        }
-        mock_response.meta = {
-            "api_version": {"version": "1"},
-            "billed_units": {"input_tokens": 55, "output_tokens": 78},
-        }
-        mock_chat_stream_response.return_value = mock_response
-        yield mock_chat_stream_response
-
-
 def streaming_chunk(text: str):
     """
     Mock chunks of streaming responses from the Cohere API
     """
     # mimic the chunk response from the OpenAI API
     mock_chunks = Mock()
     mock_chunks.index = 0
@@ -192,81 +147,19 @@
                 "streaming_callback": "haystack.components.generators.utils.print_streaming_chunk",
                 "generation_kwargs": {"max_tokens": 10, "some_test_param": "test-params"},
             },
         }
         with pytest.raises(ValueError):
             CohereChatGenerator.from_dict(data)
 
-    def test_run(self, chat_messages, mock_chat_response):  # noqa: ARG002
-        component = CohereChatGenerator(api_key=Secret.from_token("test-api-key"))
-        response = component.run(chat_messages)
-
-        # check that the component returns the correct ChatMessage response
-        assert isinstance(response, dict)
-        assert "replies" in response
-        assert isinstance(response["replies"], list)
-        assert len(response["replies"]) == 1
-        assert [isinstance(reply, ChatMessage) for reply in response["replies"]]
-
     def test_message_to_dict(self, chat_messages):
         obj = CohereChatGenerator(api_key=Secret.from_token("test-api-key"))
         dictionary = [obj._message_to_dict(message) for message in chat_messages]
         assert dictionary == [{"user_name": "Chatbot", "text": "What's the capital of France"}]
 
-    def test_run_with_params(self, chat_messages, mock_chat_response):
-        component = CohereChatGenerator(
-            api_key=Secret.from_token("test-api-key"), generation_kwargs={"max_tokens": 10, "temperature": 0.5}
-        )
-        response = component.run(chat_messages)
-
-        # check that the component calls the Cohere API with the correct parameters
-        _, kwargs = mock_chat_response.call_args
-        assert kwargs["max_tokens"] == 10
-        assert kwargs["temperature"] == 0.5
-
-        # check that the component returns the correct response
-        assert isinstance(response, dict)
-        assert "replies" in response
-        assert isinstance(response["replies"], list)
-        assert len(response["replies"]) == 1
-        assert [isinstance(reply, ChatMessage) for reply in response["replies"]]
-
-    def test_run_streaming(self, chat_messages, mock_chat_streaming_response):
-        streaming_call_count = 0
-
-        # Define the streaming callback function and assert that it is called with StreamingChunk objects
-        def streaming_callback_fn(chunk: StreamingChunk):
-            nonlocal streaming_call_count
-            streaming_call_count += 1
-            assert isinstance(chunk, StreamingChunk)
-
-        generator = CohereChatGenerator(
-            api_key=Secret.from_token("test-api-key"), streaming_callback=streaming_callback_fn
-        )
-
-        # Create a fake streamed response
-        # self needed here, don't remove
-        def mock_iter(self):  # noqa: ARG001
-            yield streaming_chunk("Hello")
-            yield streaming_chunk("How are you?")
-
-        mock_response = Mock(**{"__iter__": mock_iter})
-        mock_chat_streaming_response.return_value = mock_response
-
-        response = generator.run(chat_messages)
-
-        # Assert that the streaming callback was called twice
-        assert streaming_call_count == 2
-
-        # Assert that the response contains the generated replies
-        assert "replies" in response
-        assert isinstance(response["replies"], list)
-        assert len(response["replies"]) > 0
-        assert [isinstance(reply, ChatMessage) for reply in response["replies"]]
-
     @pytest.mark.skipif(
         not os.environ.get("COHERE_API_KEY", None) and not os.environ.get("CO_API_KEY", None),
         reason="Export an env var called COHERE_API_KEY/CO_API_KEY containing the Cohere API key to run this test.",
     )
     @pytest.mark.integration
     def test_live_run(self):
         chat_messages = [ChatMessage(content="What's the capital of France", role=ChatRole.USER, name="", meta={})]
@@ -279,15 +172,15 @@
     @pytest.mark.skipif(
         not os.environ.get("COHERE_API_KEY", None) and not os.environ.get("CO_API_KEY", None),
         reason="Export an env var called COHERE_API_KEY/CO_API_KEY containing the Cohere API key to run this test.",
     )
     @pytest.mark.integration
     def test_live_run_wrong_model(self, chat_messages):
         component = CohereChatGenerator(model="something-obviously-wrong")
-        with pytest.raises(cohere.CohereAPIError):
+        with pytest.raises(ApiError):
             component.run(chat_messages)
 
     @pytest.mark.skipif(
         not os.environ.get("COHERE_API_KEY", None) and not os.environ.get("CO_API_KEY", None),
         reason="Export an env var called COHERE_API_KEY/CO_API_KEY containing the Cohere API key to run this test.",
     )
     @pytest.mark.integration
@@ -305,15 +198,15 @@
         component = CohereChatGenerator(streaming_callback=callback)
         results = component.run(
             [ChatMessage(content="What's the capital of France? answer in a word", role=ChatRole.USER, name=None)]
         )
 
         assert len(results["replies"]) == 1
         message: ChatMessage = results["replies"][0]
-        assert "Paris" in message.content[0]
+        assert "Paris" in message.content
 
         assert message.meta["finish_reason"] == "COMPLETE"
 
         assert callback.counter > 1
         assert "Paris" in callback.responses
 
     @pytest.mark.skipif(
@@ -349,15 +242,15 @@
         callback = Callback()
         chat_messages = [ChatMessage(content="What's the capital of France? answer in a word", role=None, name=None)]
         component = CohereChatGenerator(streaming_callback=callback)
         results = component.run(chat_messages, generation_kwargs={"connectors": [{"id": "web-search"}]})
 
         assert len(results["replies"]) == 1
         message: ChatMessage = results["replies"][0]
-        assert "Paris" in message.content[0]
+        assert "Paris" in message.content
 
         assert message.meta["finish_reason"] == "COMPLETE"
 
         assert "Paris" in callback.responses
 
         assert message.meta["documents"] is not None
         assert message.meta["citations"] is not None
```

### Comparing `cohere_haystack-0.7.0/tests/test_cohere_generators.py` & `cohere_haystack-1.0.0/tests/test_cohere_generators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import os
 
 import pytest
+from cohere.core import ApiError
 from haystack.components.generators.utils import print_streaming_chunk
 from haystack.utils import Secret
 from haystack_integrations.components.generators.cohere import CohereGenerator
 
 pytestmark = pytest.mark.generators
 COHERE_API_URL = "https://api.cohere.com"
 
@@ -115,23 +116,14 @@
         component: CohereGenerator = CohereGenerator.from_dict(data)
         assert component.api_key == Secret.from_env_var("ENV_VAR", strict=False)
         assert component.model == "command"
         assert component.streaming_callback == print_streaming_chunk
         assert component.api_base_url == "test-base-url"
         assert component.model_parameters == {"max_tokens": 10, "some_test_param": "test-params"}
 
-    def test_check_truncated_answers(self, caplog):
-        component = CohereGenerator(api_key=Secret.from_token("test-api-key"))
-        meta = [{"finish_reason": "MAX_TOKENS"}]
-        component._check_truncated_answers(meta)
-        assert caplog.records[0].message == (
-            "Responses have been truncated before reaching a natural stopping point. "
-            "Increase the max_tokens parameter to allow for longer completions."
-        )
-
     @pytest.mark.skipif(
         not os.environ.get("COHERE_API_KEY", None) and not os.environ.get("CO_API_KEY", None),
         reason="Export an env var called COHERE_API_KEY/CO_API_KEY containing the Cohere API key to run this test.",
     )
     @pytest.mark.integration
     def test_cohere_generator_run(self):
         component = CohereGenerator()
@@ -143,18 +135,16 @@
 
     @pytest.mark.skipif(
         not os.environ.get("COHERE_API_KEY", None) and not os.environ.get("CO_API_KEY", None),
         reason="Export an env var called COHERE_API_KEY/CO_API_KEY containing the Cohere API key to run this test.",
     )
     @pytest.mark.integration
     def test_cohere_generator_run_wrong_model(self):
-        import cohere
-
         component = CohereGenerator(model="something-obviously-wrong")
-        with pytest.raises(cohere.CohereAPIError):
+        with pytest.raises(ApiError):
             component.run(prompt="What's the capital of France?")
 
     @pytest.mark.skipif(
         not os.environ.get("COHERE_API_KEY", None) and not os.environ.get("CO_API_KEY", None),
         reason="Export an env var called COHERE_API_KEY/CO_API_KEY containing the Cohere API key to run this test.",
     )
     @pytest.mark.integration
```

### Comparing `cohere_haystack-0.7.0/tests/test_cohere_ranker.py` & `cohere_haystack-1.0.0/tests/test_cohere_ranker.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/tests/test_document_embedder.py` & `cohere_haystack-1.0.0/tests/test_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,43 +17,40 @@
         embedder = CohereDocumentEmbedder()
         assert embedder.api_key == Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"])
         assert embedder.model == "embed-english-v2.0"
         assert embedder.input_type == "search_document"
         assert embedder.api_base_url == COHERE_API_URL
         assert embedder.truncate == "END"
         assert embedder.use_async_client is False
-        assert embedder.max_retries == 3
         assert embedder.timeout == 120
         assert embedder.batch_size == 32
         assert embedder.progress_bar is True
         assert embedder.meta_fields_to_embed == []
         assert embedder.embedding_separator == "\n"
 
     def test_init_with_parameters(self):
         embedder = CohereDocumentEmbedder(
             api_key=Secret.from_token("test-api-key"),
             model="embed-multilingual-v2.0",
             input_type="search_query",
             api_base_url="https://custom-api-base-url.com",
             truncate="START",
             use_async_client=True,
-            max_retries=5,
             timeout=60,
             batch_size=64,
             progress_bar=False,
             meta_fields_to_embed=["test_field"],
             embedding_separator="-",
         )
         assert embedder.api_key == Secret.from_token("test-api-key")
         assert embedder.model == "embed-multilingual-v2.0"
         assert embedder.input_type == "search_query"
         assert embedder.api_base_url == "https://custom-api-base-url.com"
         assert embedder.truncate == "START"
         assert embedder.use_async_client is True
-        assert embedder.max_retries == 5
         assert embedder.timeout == 60
         assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.meta_fields_to_embed == ["test_field"]
         assert embedder.embedding_separator == "-"
 
     def test_to_dict(self):
@@ -64,15 +61,14 @@
             "init_parameters": {
                 "api_key": {"env_vars": ["COHERE_API_KEY", "CO_API_KEY"], "strict": True, "type": "env_var"},
                 "model": "embed-english-v2.0",
                 "input_type": "search_document",
                 "api_base_url": COHERE_API_URL,
                 "truncate": "END",
                 "use_async_client": False,
-                "max_retries": 3,
                 "timeout": 120,
                 "batch_size": 32,
                 "progress_bar": True,
                 "meta_fields_to_embed": [],
                 "embedding_separator": "\n",
             },
         }
@@ -81,15 +77,14 @@
         embedder_component = CohereDocumentEmbedder(
             api_key=Secret.from_env_var("ENV_VAR", strict=False),
             model="embed-multilingual-v2.0",
             input_type="search_query",
             api_base_url="https://custom-api-base-url.com",
             truncate="START",
             use_async_client=True,
-            max_retries=5,
             timeout=60,
             batch_size=64,
             progress_bar=False,
             meta_fields_to_embed=["text_field"],
             embedding_separator="-",
         )
         component_dict = embedder_component.to_dict()
@@ -98,15 +93,14 @@
             "init_parameters": {
                 "api_key": {"env_vars": ["ENV_VAR"], "strict": False, "type": "env_var"},
                 "model": "embed-multilingual-v2.0",
                 "input_type": "search_query",
                 "api_base_url": "https://custom-api-base-url.com",
                 "truncate": "START",
                 "use_async_client": True,
-                "max_retries": 5,
                 "timeout": 60,
                 "batch_size": 64,
                 "progress_bar": False,
                 "meta_fields_to_embed": ["text_field"],
                 "embedding_separator": "-",
             },
         }
```

### Comparing `cohere_haystack-0.7.0/tests/test_text_embedder.py` & `cohere_haystack-1.0.0/tests/test_text_embedder.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,38 +20,35 @@
 
         assert embedder.api_key == Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"])
         assert embedder.model == "embed-english-v2.0"
         assert embedder.input_type == "search_query"
         assert embedder.api_base_url == COHERE_API_URL
         assert embedder.truncate == "END"
         assert embedder.use_async_client is False
-        assert embedder.max_retries == 3
         assert embedder.timeout == 120
 
     def test_init_with_parameters(self):
         """
         Test custom initialization parameters for CohereTextEmbedder.
         """
         embedder = CohereTextEmbedder(
             api_key=Secret.from_token("test-api-key"),
             model="embed-multilingual-v2.0",
             input_type="classification",
             api_base_url="https://custom-api-base-url.com",
             truncate="START",
             use_async_client=True,
-            max_retries=5,
             timeout=60,
         )
         assert embedder.api_key == Secret.from_token("test-api-key")
         assert embedder.model == "embed-multilingual-v2.0"
         assert embedder.input_type == "classification"
         assert embedder.api_base_url == "https://custom-api-base-url.com"
         assert embedder.truncate == "START"
         assert embedder.use_async_client is True
-        assert embedder.max_retries == 5
         assert embedder.timeout == 60
 
     def test_to_dict(self):
         """
         Test serialization of this component to a dictionary, using default initialization parameters.
         """
         embedder_component = CohereTextEmbedder()
@@ -61,15 +58,14 @@
             "init_parameters": {
                 "api_key": {"env_vars": ["COHERE_API_KEY", "CO_API_KEY"], "strict": True, "type": "env_var"},
                 "model": "embed-english-v2.0",
                 "input_type": "search_query",
                 "api_base_url": COHERE_API_URL,
                 "truncate": "END",
                 "use_async_client": False,
-                "max_retries": 3,
                 "timeout": 120,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         """
         Test serialization of this component to a dictionary, using custom initialization parameters.
@@ -77,28 +73,26 @@
         embedder_component = CohereTextEmbedder(
             api_key=Secret.from_env_var("ENV_VAR", strict=False),
             model="embed-multilingual-v2.0",
             input_type="classification",
             api_base_url="https://custom-api-base-url.com",
             truncate="START",
             use_async_client=True,
-            max_retries=5,
             timeout=60,
         )
         component_dict = embedder_component.to_dict()
         assert component_dict == {
             "type": "haystack_integrations.components.embedders.cohere.text_embedder.CohereTextEmbedder",
             "init_parameters": {
                 "api_key": {"env_vars": ["ENV_VAR"], "strict": False, "type": "env_var"},
                 "model": "embed-multilingual-v2.0",
                 "input_type": "classification",
                 "api_base_url": "https://custom-api-base-url.com",
                 "truncate": "START",
                 "use_async_client": True,
-                "max_retries": 5,
                 "timeout": 60,
             },
         }
 
     def test_run_wrong_input_format(self):
         """
         Test for checking incorrect input when creating embedding.
```

### Comparing `cohere_haystack-0.7.0/.gitignore` & `cohere_haystack-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/LICENSE.txt` & `cohere_haystack-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/README.md` & `cohere_haystack-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/pyproject.toml` & `cohere_haystack-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.7.0/PKG-INFO` & `cohere_haystack-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cohere-haystack
-Version: 0.7.0
+Version: 1.0.0
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

