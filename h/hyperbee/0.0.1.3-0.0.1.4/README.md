# Comparing `tmp/hyperbee-0.0.1.3.tar.gz` & `tmp/hyperbee-0.0.1.4.tar.gz`

## Comparing `hyperbee-0.0.1.3.tar` & `hyperbee-0.0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/__init__.py
--rw-r--r--   0        0        0    16770 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/_client.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/version.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/__init__.py
--rw-r--r--   0        0        0    29864 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/completions.py
--rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/models.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/chat/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/chat/chat.py
--rw-r--r--   0        0        0    33700 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/chat/completions.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/pipeline/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/pipeline/pipeline.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/.gitignore
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/pyproject.toml
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/__init__.py
+-rw-r--r--   0        0        0    16826 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/_client.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/version.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/__init__.py
+-rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/completions.py
+-rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/models.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/chat/chat.py
+-rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/chat/completions.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/pipeline/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/pipeline/pipeline.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/.gitignore
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/PKG-INFO
```

### Comparing `hyperbee-0.0.1.3/src/hyperbee/__init__.py` & `hyperbee-0.0.1.4/src/hyperbee/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.3/src/hyperbee/_client.py` & `hyperbee-0.0.1.4/src/hyperbee/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         if organization is None:
             organization = os.environ.get("HIVE_ORG_ID")
         self.organization = organization
 
         if base_url is None:
             base_url = os.environ.get("HIVE_BASE_URL")
         if base_url is None:
-            base_url = f"https://api.openai.com/v1"
+            base_url = f"https://api.hyperbee.ai/v1/"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
@@ -302,14 +302,15 @@
         self._default_stream_cls = AsyncStream
 
         self.completions = resources.AsyncCompletions(self)
         self.chat = resources.AsyncChat(self)
         self.models = resources.AsyncModels(self)
         self.with_raw_response = AsyncHiveWithRawResponse(self)
         self.with_streaming_response = AsyncHiveWithStreamedResponse(self)
+        self.pipeline = resources.AsyncPipeline(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
```

### Comparing `hyperbee-0.0.1.3/src/hyperbee/resources/__init__.py` & `hyperbee-0.0.1.4/src/hyperbee/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CompletionsWithRawResponse,
     AsyncCompletionsWithRawResponse,
     CompletionsWithStreamingResponse,
     AsyncCompletionsWithStreamingResponse,
 )
 from .pipeline import (
     Pipeline,
+    AsyncPipeline,
 )
 
 __all__ = [
     "Completions",
     "AsyncCompletions",
     "CompletionsWithRawResponse",
     "AsyncCompletionsWithRawResponse",
@@ -43,9 +44,10 @@
     "AsyncChatWithStreamingResponse",
     "Models",
     "AsyncModels",
     "ModelsWithRawResponse",
     "AsyncModelsWithRawResponse",
     "ModelsWithStreamingResponse",
     "AsyncModelsWithStreamingResponse",
-    "Pipeline"
+    "Pipeline",
+    "AsyncPipeline"
 ]
```

### Comparing `hyperbee-0.0.1.3/src/hyperbee/resources/completions.py` & `hyperbee-0.0.1.4/src/hyperbee/resources/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion:
@@ -80,14 +82,16 @@
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Stream[Completion]:
@@ -112,14 +116,16 @@
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion | Stream[Completion]:
@@ -144,14 +150,16 @@
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion | Stream[Completion]:
@@ -327,14 +335,16 @@
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion:
@@ -359,14 +369,16 @@
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncStream[Completion]:
@@ -391,14 +403,16 @@
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion | AsyncStream[Completion]:
@@ -423,14 +437,16 @@
         seed: Optional[int] | NotGiven = NOT_GIVEN,
         stop: Union[Optional[str], List[str], None] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
         suffix: Optional[str] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion | AsyncStream[Completion]:
```

### Comparing `hyperbee-0.0.1.3/src/hyperbee/resources/models.py` & `hyperbee-0.0.1.4/src/hyperbee/resources/models.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.3/src/hyperbee/resources/chat/__init__.py` & `hyperbee-0.0.1.4/src/hyperbee/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.3/src/hyperbee/resources/chat/chat.py` & `hyperbee-0.0.1.4/src/hyperbee/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.3/src/hyperbee/resources/chat/completions.py` & `hyperbee-0.0.1.4/src/hyperbee/resources/chat/completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ChatCompletion:
@@ -101,14 +103,16 @@
         stop: Union[Optional[str], List[str]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Stream[ChatCompletionChunk]:
@@ -141,26 +145,29 @@
         stop: Union[Optional[str], List[str]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ChatCompletion | Stream[ChatCompletionChunk]:
         """
         
         """
         ...
 
+    
     @required_args(["messages", "model"], ["messages", "model", "stream"])
     def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
         model: Union[
             str,
@@ -181,14 +188,16 @@
         stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ChatCompletion | Stream[ChatCompletionChunk]:
@@ -301,15 +310,24 @@
               means only the tokens comprising the top 10% probability mass are considered.
 
               We generally recommend altering this or `temperature` but not both.
 
           user: A unique identifier representing your end-user, which can help OpenAI to monitor
               and detect abuse.
               [Learn more](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids).
-
+        
+          output_mode: Specifies the desired output format for the model's response.
+              If set to "json", the model will attempt to generate a valid JSON response.
+              Otherwise, the model will generate a regular text response.
+
+          json_schema: Specifies a JSON schema that the model's JSON response should conform to.
+            The schema should be a Python dictionary following the JSON Schema specification (https://json-schema.org/).
+            If not provided, the model will generate a JSON response without enforcing a specific schema.
+  
+    
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds"""
@@ -333,14 +351,16 @@
                     "temperature": temperature,
                     "tool_choice": tool_choice,
                     "tools": tools,
                     "top_logprobs": top_logprobs,
                     "top_p": top_p,
                     "user": user,
                     "optimization": optimization,
+                    "output_mode": output_mode,
+                    "json_schema": json_schema,
                 },
                 completion_create_params.CompletionCreateParams,
             ),
             
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
@@ -366,14 +386,15 @@
         messages: Iterable[ChatCompletionMessageParam],
         model: Union[
             str,
             Literal[
                 "hive",
             ],
         ],
+        optimization: Optional[Literal["cost", "quality", "auto"]] | NotGiven = NOT_GIVEN,
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         response_format: completion_create_params.ResponseFormat | NotGiven = NOT_GIVEN,
@@ -382,14 +403,16 @@
         stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ChatCompletion:
@@ -405,14 +428,15 @@
         model: Union[
             str,
             Literal[
                 "hive",
             ],
         ],
         stream: Literal[True],
+        optimization: Optional[Literal["cost", "quality", "auto"]] | NotGiven = NOT_GIVEN,
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         response_format: completion_create_params.ResponseFormat | NotGiven = NOT_GIVEN,
@@ -420,14 +444,16 @@
         stop: Union[Optional[str], List[str]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncStream[ChatCompletionChunk]:
@@ -444,14 +470,15 @@
         model: Union[
             str,
             Literal[
                 "hive",
             ],
         ],
         stream: bool,
+        optimization: Optional[Literal["cost", "quality", "auto"]] | NotGiven = NOT_GIVEN,
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         response_format: completion_create_params.ResponseFormat | NotGiven = NOT_GIVEN,
@@ -459,14 +486,16 @@
         stop: Union[Optional[str], List[str]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ChatCompletion | AsyncStream[ChatCompletionChunk]:
@@ -482,14 +511,15 @@
         messages: Iterable[ChatCompletionMessageParam],
         model: Union[
             str,
             Literal[
                 "hive",
             ],
         ],
+        optimization: Optional[Literal["cost", "quality", "auto"]] | NotGiven = NOT_GIVEN,
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
         presence_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         response_format: completion_create_params.ResponseFormat | NotGiven = NOT_GIVEN,
@@ -498,14 +528,16 @@
         stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         tool_choice: ChatCompletionToolChoiceOptionParam | NotGiven = NOT_GIVEN,
         tools: Iterable[ChatCompletionToolParam] | NotGiven = NOT_GIVEN,
         top_logprobs: Optional[int] | NotGiven = NOT_GIVEN,
         top_p: Optional[float] | NotGiven = NOT_GIVEN,
         user: str | NotGiven = NOT_GIVEN,
+        output_mode: Optional[str] | NotGiven = NOT_GIVEN,
+        json_schema: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ChatCompletion | AsyncStream[ChatCompletionChunk]:
@@ -514,14 +546,17 @@
         Args:
           messages: A list of messages comprising the conversation so far.
               [Example Python code](https://cookbook.openai.com/examples/how_to_format_inputs_to_chatgpt_models).
 
           model: ID of the model to use. See the
               For now only `hive` is supported.
 
+          optimization: Whether to optimize for `cost` or `quality`. If set to `auto`, 
+              the API will optimize for both cost and quality. The default is `auto`.
+
           frequency_penalty: Number between -2.0 and 2.0. Positive values penalize new tokens based on their
               existing frequency in the text so far, decreasing the model's likelihood to
               repeat the same line verbatim.
 
               [See more information about frequency and presence penalties.](https://platform.openai.com/docs/guides/text-generation/parameter-details)
 
           logit_bias: Modify the likelihood of specified tokens appearing in the completion.
@@ -616,14 +651,22 @@
 
               We generally recommend altering this or `temperature` but not both.
 
           user: A unique identifier representing your end-user, which can help OpenAI to monitor
               and detect abuse.
               [Learn more](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids).
 
+          output_mode: Specifies the desired output format for the model's response.
+              If set to "json", the model will attempt to generate a valid JSON response.
+              Otherwise, the model will generate a regular text response.
+
+          json_schema: Specifies a JSON schema that the model's JSON response should conform to.
+            The schema should be a Python dictionary following the JSON Schema specification (https://json-schema.org/).
+            If not provided, the model will generate a JSON response without enforcing a specific schema.
+  
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds"""
@@ -645,14 +688,17 @@
                     "stream": stream,
                     "temperature": temperature,
                     "tool_choice": tool_choice,
                     "tools": tools,
                     "top_logprobs": top_logprobs,
                     "top_p": top_p,
                     "user": user,
+                    "optimization": optimization,
+                    "output_mode": output_mode,
+                    "json_schema": json_schema,
                 },
                 completion_create_params.CompletionCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ChatCompletion,
```

### Comparing `hyperbee-0.0.1.3/README.md` & `hyperbee-0.0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.3/pyproject.toml` & `hyperbee-0.0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperbee"
-version = "0.0.1.3"
+version = "0.0.1.4"
 description = "The official Python library for the hyperbee API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Hive", email = "support@hyperbee.ai" },
 ]
 dependencies = [
```

### Comparing `hyperbee-0.0.1.3/PKG-INFO` & `hyperbee-0.0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperbee
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: The official Python library for the hyperbee API
 Project-URL: Homepage, https://github.com/HyperbeeAI/hive-python
 Project-URL: Repository, https://github.com/HyperbeeAI/hive-python
 Author-email: Hive <support@hyperbee.ai>
 License-Expression: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

