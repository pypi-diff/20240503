# Comparing `tmp/answerrocket-client-0.1.9.tar.gz` & `tmp/answerrocket_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket-client-0.1.9.tar", last modified: Mon Dec 11 17:34:12 2023, max compression
+gzip compressed data, was "answerrocket_client-0.2.0.tar", last modified: Fri May  3 17:14:37 2024, max compression
```

## Comparing `answerrocket-client-0.1.9.tar` & `answerrocket_client-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.430043 answerrocket-client-0.1.9/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22240 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.170405 answerrocket_client-0.2.0/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12592 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45437 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/sdk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/test/test_client.py
```

### Comparing `answerrocket-client-0.1.9/PKG-INFO` & `answerrocket_client-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # AnswerRocket Skill API Client
-This is a client library for interacting with an AnswerRocket instance.  Its purpose is to enable the development of skills (custom AnswerRocket extensions) without the need for AnswerRocket to be running locally.
+This is a client library for interacting with an AnswerRocket instance.
 
 ## Installation
 
 `pip install answerrocket-client`
 
 ## Use
```

### Comparing `answerrocket-client-0.1.9/answer_rocket/auth.py` & `answerrocket_client-0.2.0/answer_rocket/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,19 +18,26 @@
 		pass
 
 
 @dataclass
 class ExternalAuthHelper(AuthHelper):
 	url: str
 	token: str
+	tenant: str
+	user: str
 
 	def headers(self) -> dict:
-		return {
+		headers = {
 			'Authorization': f'Bearer {self.token}'
 		}
+		if self.user:
+			headers['Max-User'] = self.user
+		if self.tenant:
+			headers['Max-Tenant'] = self.tenant
+		return headers
 	
 
 @dataclass
 class InternalAuthHelper(AuthHelper):
 	url: str
 	tenant: str
 	user: str | None
@@ -44,14 +51,14 @@
 			headers['Max-User'] = self.user
 		return headers
 	
 
 def init_auth_helper(url: Optional[str], token: Optional[str]) -> AuthHelper:
 	token = token or os.getenv('AR_TOKEN')
 	url = url or os.getenv('AR_URL')
+	tenant = os.getenv('AR_TENANT_ID')
+	user = os.getenv('AR_USER_ID')
 	if not url:
 		raise AnswerRocketClientError('No AnswerRocket url provided')
 	if token:
-		return ExternalAuthHelper(url=url, token=token)
-	tenant = os.getenv('AR_TENANT_ID')
-	user = os.getenv('AR_USER_ID')
-	return InternalAuthHelper(url=url, tenant=tenant, user=user)
+		return ExternalAuthHelper(url=url, token=token, user=user, tenant=tenant)
+	return InternalAuthHelper(url=url, tenant=tenant, user=user)
```

### Comparing `answerrocket-client-0.1.9/answer_rocket/chat.py` & `answerrocket_client-0.2.0/answer_rocket/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import logging
-from datetime import date, datetime, timedelta, timezone
+from datetime import datetime
 from typing import Literal, Callable, Optional
 
 import openai
-from sgqlc.types import Variable, non_null, String, Arg
+from sgqlc.types import Variable, non_null, String, Arg, Boolean, list_of
 from sgqlc.operation import Fragment
 
 from answer_rocket.auth import AuthHelper
 from answer_rocket.graphql.client import GraphQlClient
 from answer_rocket.graphql.schema import (LLMApiConfig, AzureOpenaiCompletionLLMApiConfig,
                                           AzureOpenaiEmbeddingLLMApiConfig, OpenaiCompletionLLMApiConfig,
-                                          OpenaiEmbeddingLLMApiConfig, UUID, Int, DateTime)
+                                          OpenaiEmbeddingLLMApiConfig, UUID, Int, DateTime, ChatDryRunType)
+from answer_rocket.graphql.sdk_operations import Operations
+
 
 logger = logging.getLogger(__name__)
 
-ModelType = Literal['GPT3_5', 'GPT4', 'Embedding']
+ModelType = Literal['COMPLETION', 'EMBEDDING']
 ApiType = Literal['AZURE', 'OPENAI']
 
 LLMConfigType = LLMApiConfig | AzureOpenaiEmbeddingLLMApiConfig | AzureOpenaiCompletionLLMApiConfig | \
                 OpenaiCompletionLLMApiConfig | OpenaiEmbeddingLLMApiConfig
 
 
 class Chat:
@@ -50,30 +52,38 @@
 
         try:
             result = self.gql_client.submit(operation, llm_config_query_args)
             return result.llmapi_config_for_sdk
         except Exception as e:
             logger.error("failed to get LLM config", exc_info=True)
 
-    def completion(self, model_type: ModelType = 'GPT3_5', stream_callback: Optional[Callable] = None, **kwargs):
+    def completion(self, model_type: ModelType = 'COMPLETION', stream_callback: Optional[Callable] = None, **kwargs):
         """
         Wrapper for the OpenAI chat completion API. This will attempt to retry requests.
         See here for documentation on the wrapped call: https://platform.openai.com/docs/api-reference/chat/create
-        :param model_type: LLM model type to use. One of GPT3_5, GPT4, Embedding
+        :param model_type: LLM model type to use. One of COMPLETION, EMBEDDING
         :param stream_callback: if provided, a function that will be called with the stream response each time one is
             received
 
         :param kwargs: any other arguments to pass to the underlying Completion call. Note that this method will attempt
             to fetch the appropriate config from the remote AnswerRocket instance, but you can override them by
             providing explicit arguments. It will __not__ fetch the API key. When running locally, you must provide this
             yourself in the OPENAI_API_KEY env var that the openai sdk expects you to set.
             Note that kwarg "messages" can be a string for simple completion or a list of role/content message objects for a full conversation history
 
         :return: success indicator (true/false), and a result which is an error string if success is false, or the assistant's reply object if success is true
         """
+
+        # Fall back to completion for old cases where model_type could be a different value such as GPT_4, etc.
+        # This is for backwards compatibility... hopefully this block does not need to be used much in the future
+        if model_type == 'Embedding':
+            model_type: ModelType = 'EMBEDDING'
+        elif model_type not in ['COMPLETION', 'EMBEDDING']:
+            model_type: ModelType = 'COMPLETION'
+
         llm_api_config = self._get_llm_config(model_type=model_type)
         mapped_api_args = _map_llm_api_config_parameters(llm_api_config=llm_api_config, model_type=model_type)
 
         args = {
             **mapped_api_args,
             **kwargs
         }
@@ -135,42 +145,37 @@
             except Exception as e:
                 time.sleep(retry_sleep_time)
                 last_error = e
                 retry_sleep_time *= error_backoff_multiplier
 
         return False, str(last_error)
 
-    def ask_question(self, copilot_id: str, question: str, thread_id: str = None):
+
+    def ask_question(self, copilot_id: str, question: str, thread_id: str = None, skip_report_cache: bool = False, dry_run_type: str = None):
         """
         Calls the Max chat pipeline to answer a natural language question and receive analysis and insights
         in response.
         :param copilot_id: the ID of the copilot to run the question against
         :param question: The natural language question to ask the engine.
         :param thread_id: (optional) ID of the thread/conversation to run the question on. The question and answer will
          be added to the bottom of the thread.
+        :param skip_report_cache: Should the report cache be skipped for this question?
+        :param dry_run_type: If provided, run a dry run at the specified level: 'SKIP_SKILL_EXEC', 'SKIP_SKILL_NLG'
         :return: the ChatEntry response object associate with the answer from the pipeline
         """
         ask_question_query_args = {
             'copilotId': UUID(copilot_id),
             'question': question,
             'threadId': UUID(thread_id) if thread_id else None,
+            'skipReportCache': skip_report_cache,
+            'dryRunType': ChatDryRunType(dry_run_type) if dry_run_type else None
         }
-        ask_question_query_vars = {
-            'copilot_id': Arg(non_null(UUID)),
-            'question': Arg(non_null(String)),
-            'thread_id': Arg(UUID),
-        }
-        operation = self.gql_client.mutation(variables=ask_question_query_vars)
-        ask_question_query = operation.ask_chat_question(
-            copilot_id=Variable('copilot_id'),
-            question=Variable('question'),
-            thread_id=Variable('thread_id'),
-        )
 
-        result = self.gql_client.submit(operation, ask_question_query_args)
+        op = Operations.mutation.ask_chat_question
+        result = self.gql_client.submit(op, ask_question_query_args)
 
         return result.ask_chat_question
 
     def get_threads(self, copilot_id: str, start_date: datetime = None, end_date: datetime = None):
         """
         Fetches all threads for a given copilot and date range.
         :param copilot_id: the ID of the copilot to fetch threads for
@@ -229,14 +234,40 @@
             offset=Variable('offset'),
             limit=Variable('limit'),
         )
 
         result = self.gql_client.submit(operation, get_entries_query_args)
 
         return result.user_chat_entries
+    
+    def evaluate_entry(self, entry_id: str, evals: list[str]):
+        """
+        Runs and fetches the inputted evaluations for a given entry.
+        :param entry_id: the ID of the entry to fetch evaluation for
+        :param evals: a list of strings containing the evaluations to run on the entry
+        :return: a ChatEntryEvaluation object
+        """
+        evaluate_entry_mutation_args = {
+            'entryId': UUID(entry_id),
+            'evals': evals,
+        }
+        evaluate_entry_mutation_vars = {
+            'entry_id': Arg(non_null(UUID)),
+            'evals': Arg(non_null(list_of(non_null(String)))),
+        }
+        operation = self.gql_client.mutation(variables=evaluate_entry_mutation_vars)
+        evaluate_entry_query = operation.evaluate_chat_question(
+            entry_id=Variable('entry_id'),
+            evals=Variable('evals'),
+        )
+
+        result = self.gql_client.submit(operation, evaluate_entry_mutation_args)
+
+        return result.evaluate_chat_question
+
 
 
 def _create_llm_config_fragments():
     azure_completion_fragment = Fragment(AzureOpenaiCompletionLLMApiConfig, 'AzureCompletionFragment')
     azure_completion_fragment.__fields__(__exclude__=['id', 'api_type', 'model_type', 'model_name'])
 
     azure_embedding_fragment = Fragment(AzureOpenaiEmbeddingLLMApiConfig, 'AzureEmbeddingFragment')
@@ -252,15 +283,15 @@
         azure_completion_fragment,
         azure_embedding_fragment,
         openai_embedding_fragment,
         openai_completion_fragment
     ]
 
 
-def _map_llm_api_config_parameters(llm_api_config: LLMConfigType, model_type: ModelType = 'GPT3_5'):
+def _map_llm_api_config_parameters(llm_api_config: LLMConfigType, model_type: ModelType = 'COMPLETION'):
     """
     Maps the LLM Api config to the parameters for openai calls.
     """
     kwargs = {
         "api_key": os.getenv('OPENAI_API_KEY')
     }
 
@@ -275,18 +306,18 @@
         kwargs.update({
             "model": llm_api_config.model_name,
             "organization": llm_api_config.organization
         })
     else:
         raise Exception("Invalid LLM config: Unknown api_type")
 
-    if model_type == 'GPT3_5' or model_type == 'GPT4':
+    if model_type == 'COMPLETION':
         kwargs.update({
             "max_tokens": llm_api_config.max_tokens_content_generation,
             "temperature": llm_api_config.temperature,
             "top_p": llm_api_config.top_p,
             "frequency_penalty": llm_api_config.frequency_penalty,
             "presence_penalty": llm_api_config.presence_penalty,
-            "stop": llm_api_config.stop_sequence,
+            "stop": "** DONE **",
         })
 
     return kwargs
```

### Comparing `answerrocket-client-0.1.9/answer_rocket/client.py` & `answerrocket_client-0.2.0/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.9/answer_rocket/data.py` & `answerrocket_client-0.2.0/answer_rocket/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import os
 from typing import Optional
 from uuid import UUID
 
 import pandas as pd
 from sgqlc.operation import Fragment
 from sgqlc.types import Variable, Arg, non_null, String, Int
 
 from answer_rocket.auth import AuthHelper
 from answer_rocket.graphql.client import GraphQlClient
 from answer_rocket.graphql.schema import UUID as GQL_UUID, MaxMetricAttribute, MaxDomainObject, \
     MaxDimensionEntity, MaxFactEntity, MaxNormalAttribute, \
-    MaxPrimaryAttribute, MaxReferenceAttribute, MaxCalculatedMetric
+    MaxPrimaryAttribute, MaxReferenceAttribute, MaxCalculatedMetric, MaxDataset, MaxCalculatedAttribute
 from answer_rocket.types import MaxResult, RESULT_EXCEPTION_CODE
 
 
 class ExecuteSqlQueryResult(MaxResult):
     df = None
 
 
@@ -29,40 +30,49 @@
     """
     Helper for accessing data from the server.
     """
 
     def __init__(self, auth_helper: AuthHelper, gql_client: GraphQlClient) -> None:
         self._auth_helper = auth_helper
         self._gql_client = gql_client
+        self.copilot_id = os.getenv('AR_COPILOT_ID')
+        self.copilot_skill_id = os.getenv('AR_COPILOT_SKILL_ID')
 
-    def execute_sql_query(self, database_id: UUID, sql_query: str, row_limit: Optional[int] = None) -> ExecuteSqlQueryResult:
+    def execute_sql_query(self, database_id: UUID, sql_query: str, row_limit: Optional[int] = None, copilot_id: Optional[UUID] = None, copilot_skill_id: Optional[UUID] = None) -> ExecuteSqlQueryResult:
         try:
             """
             database_id: the database_id of the connection to execute against.
             sql_query: the SQL query to execute.
             row_limit: the optional row limit of the query results.
+            copilot_id: the optional copilot ID.
             """
             query_args = {
                 'databaseId': database_id,
                 'sqlQuery': sql_query,
                 'rowLimit': row_limit,
+                'copilotId': copilot_id or self.copilot_id,
+                'copilotSkillId': copilot_skill_id or self.copilot_skill_id,
             }
 
             query_vars = {
                 'database_id': Arg(non_null(GQL_UUID)),
                 'sql_query': Arg(non_null(String)),
                 'row_limit': Arg(Int),
+                'copilot_id': Arg(GQL_UUID),
+                'copilot_skill_id': Arg(GQL_UUID),
             }
 
             operation = self._gql_client.query(variables=query_vars)
 
             execute_sql_query = operation.execute_sql_query(
                 database_id=Variable('database_id'),
                 sql_query=Variable('sql_query'),
                 row_limit=Variable('row_limit'),
+                copilot_id=Variable('copilot_id'),
+                copilot_skill_id=Variable('copilot_skill_id'),
             )
 
             execute_sql_query.success()
             execute_sql_query.code()
             execute_sql_query.error()
             execute_sql_query.data()
 
@@ -76,15 +86,15 @@
             execute_sql_query_result.error = execute_sql_query_response.error
             execute_sql_query_result.code = execute_sql_query_response.code
 
             if execute_sql_query_response.success:
                 data = execute_sql_query_response.data
 
                 columns = [column["name"] for column in data["columns"]]
-                rows = [row["data"] for row in data["rows"]]
+                rows = [row["data"] for row in data["rows"]] if "rows" in data else []
 
                 df = pd.DataFrame(rows, columns=columns)
 
                 execute_sql_query_result.df = df
 
             return execute_sql_query_result
         except Exception as e:
@@ -92,35 +102,47 @@
 
             execute_sql_query_result.success = False
             execute_sql_query_result.error = e
             execute_sql_query_result.code = RESULT_EXCEPTION_CODE
 
             return execute_sql_query_result
 
-    def execute_rql_query(self, dataset_id: UUID, rql_query: str) -> ExecuteRqlQueryResult:
+    def execute_rql_query(self, dataset_id: UUID, rql_query: str, row_limit: Optional[int] = None, copilot_id: Optional[UUID] = None, copilot_skill_id: Optional[UUID] = None) -> ExecuteRqlQueryResult:
         try:
             """
             dataset_id: the dataset_id of the dataset to execute against.
             rql_query: the RQL query to execute.
+            row_limit: the optional row limit of the query results.
+            copilot_id: the optional copilot ID.
+            
             """
             query_args = {
                 'datasetId': dataset_id,
-                'rqlQuery': rql_query
+                'rqlQuery': rql_query,
+                'rowLimit': row_limit,
+                'copilotId': copilot_id or self.copilot_id,
+                'copilotSkillId': copilot_skill_id or self.copilot_skill_id,
             }
 
             query_vars = {
                 'dataset_id': Arg(non_null(GQL_UUID)),
-                'rql_query': Arg(non_null(String))
+                'rql_query': Arg(non_null(String)),
+                'row_limit': Arg(Int),
+                'copilot_id': Arg(GQL_UUID),
+                'copilot_skill_id': Arg(GQL_UUID),
             }
 
             operation = self._gql_client.query(variables=query_vars)
 
             execute_rql_query = operation.execute_rql_query(
                 dataset_id=Variable('dataset_id'),
-                rql_query=Variable('rql_query')
+                rql_query=Variable('rql_query'),
+                row_limit=Variable('row_limit'),
+                copilot_id=Variable('copilot_id'),
+                copilot_skill_id=Variable('copilot_skill_id'),
             )
 
             execute_rql_query.success()
             execute_rql_query.code()
             execute_rql_query.error()
             execute_rql_query.data()
             execute_rql_query.process_rql_script_response()
@@ -186,14 +208,76 @@
 
             execute_sql_query_result.success = False
             execute_sql_query_result.error = e
             execute_sql_query_result.code = RESULT_EXCEPTION_CODE
 
             return execute_sql_query_result
 
+    def get_dataset(self, dataset_id: UUID, copilot_id: Optional[UUID] = None) -> Optional[MaxDataset]:
+        try:
+            """
+            dataset_id: the UUID of the dataset
+            """
+            query_args = {
+                'datasetId': str(dataset_id),
+                'copilotId': str(copilot_id) if copilot_id else str(self.copilot_id) if self.copilot_id else None
+            }
+
+            query_vars = {
+                'dataset_id': Arg(non_null(GQL_UUID)),
+                'copilot_id': Arg(GQL_UUID),
+            }
+
+            operation = self._gql_client.query(variables=query_vars)
+
+            gql_query = operation.get_dataset(
+                dataset_id=Variable('dataset_id'),
+                copilot_id=Variable('copilot_id'),
+            )
+
+            gql_query.dataset_id()
+            gql_query.name()
+            gql_query.description()
+            gql_query.misc_info()
+            gql_query.dimension_value_distribution_map()
+            gql_query.date_range_boundary_attribute_id()
+            gql_query.dimension_hierarchies()
+            gql_query.metric_hierarchies()
+            gql_query.domain_attribute_statistics()
+            gql_query.default_performance_metric_id()
+            gql_query.dataset_min_date()
+            gql_query.dataset_max_date()
+            gql_query.query_row_limit()
+
+            database = gql_query.database()
+            database.database_id()
+            database.name()
+            database.dbms()
+            database.schema()
+
+            tables = gql_query.tables()
+            tables.name()
+            columns = tables.columns()
+
+            columns.name()
+            columns.jdbc_type()
+            columns.length()
+            columns.precision()
+            columns.scale()
+
+            self._create_domain_object_query(gql_query.domain_objects())
+
+            result = self._gql_client.submit(operation, query_args)
+
+            dataset = result.get_dataset
+
+            return dataset
+        except Exception as e:
+            return None
+
     def get_domain_object_by_name(self, dataset_id: UUID, rql_name: str) -> DomainObjectResult:
         try:
             """
             dataset_id: the UUID of the dataset
             rql_name: the fully qualified RQL name of the domain object (e.g. transactions.sales, transactions, net_sales)
             """
             query_args = {
@@ -209,15 +293,19 @@
             operation = self._gql_client.query(variables=query_vars)
 
             gql_query = operation.get_domain_object_by_name(
                 dataset_id=Variable('dataset_id'),
                 rql_name=Variable('rql_name'),
             )
 
-            self._create_domain_object_query(gql_query)
+            gql_query.success()
+            gql_query.code()
+            gql_query.error()
+
+            self._create_domain_object_query(gql_query.domain_object())
 
             result = self._gql_client.submit(operation, query_args)
 
             gql_response = result.get_domain_object_by_name
 
             domain_object_result = DomainObjectResult()
 
@@ -255,15 +343,19 @@
             operation = self._gql_client.query(variables=query_vars)
 
             gql_query = operation.get_domain_object(
                 dataset_id=Variable('dataset_id'),
                 domain_object_id=Variable('domain_object_id'),
             )
 
-            self._create_domain_object_query(gql_query)
+            gql_query.success()
+            gql_query.code()
+            gql_query.error()
+
+            self._create_domain_object_query(gql_query.domain_object())
 
             result = self._gql_client.submit(operation, query_args)
 
             gql_response = result.get_domain_object
 
             domain_object_result = DomainObjectResult()
 
@@ -278,38 +370,48 @@
 
             domain_object_result.success = False
             domain_object_result.error = e
             domain_object_result.code = RESULT_EXCEPTION_CODE
 
             return domain_object_result
 
-    def _create_domain_object_query(self, gql_query):
-        gql_query.success()
-        gql_query.code()
-        gql_query.error()
-        domain_object = gql_query.domain_object()
-
+    def _create_domain_object_query(self, domain_object):
         # domain_object_frag = Fragment(MaxDomainObject, 'MaxDomainObjectFragment')
         # gql_query.domain_object.__fragment__(domain_object_frag)
-        domain_object.type()
-        domain_object.id()
-        domain_object.description()
-        domain_object.output_label()
-        domain_object.synonyms()
-        domain_object.output_label_plural()
-        domain_object.hide_from_user()
+
+        self._add_domain_object_fields(domain_object)
 
         fact_entity_frag = Fragment(MaxFactEntity, 'MaxFactEntityFragment')
         self._add_domain_entity_fields(fact_entity_frag)
         domain_object.__fragment__(fact_entity_frag)
 
         dimension_entity_frag = Fragment(MaxDimensionEntity, 'MaxDimensionEntityFragment')
         self._add_domain_entity_fields(dimension_entity_frag)
+        dimension_entity_frag.archetype()
         domain_object.__fragment__(dimension_entity_frag)
 
+        self._add_domain_attribute_fragments(domain_object)
+
+        calc_metric_attribute_frag = Fragment(MaxCalculatedMetric, 'MaxCalculatedMetricFragment')
+        calc_metric_attribute_frag.display_format()
+        calc_metric_attribute_frag.rql()
+        calc_metric_attribute_frag.sql()
+        calc_metric_attribute_frag.agg_method()
+        calc_metric_attribute_frag.is_positive_direction_up()
+        calc_metric_attribute_frag.can_be_averaged()
+        calc_metric_attribute_frag.is_not_additive()
+        calc_metric_attribute_frag.growth_output_format()
+        calc_metric_attribute_frag.hide_percentage_change()
+        calc_metric_attribute_frag.simplified_data_type()
+        calc_metric_attribute_frag.metric_type()
+        domain_object.__fragment__(calc_metric_attribute_frag)
+
+    def _add_domain_attribute_fragments(self, domain_object):
+        self._add_domain_object_fields(domain_object)
+
         normal_attribute_frag = Fragment(MaxNormalAttribute, 'MaxNormalAttributeFragment')
         self._add_domain_attribute_fields(normal_attribute_frag)
         self._add_dimension_attribute_fields(normal_attribute_frag)
         normal_attribute_frag.db_column()
         normal_attribute_frag.db_secondary_column()
         domain_object.__fragment__(normal_attribute_frag)
 
@@ -323,52 +425,61 @@
         reference_attribute_frag = Fragment(MaxReferenceAttribute, 'MaxReferenceAttributeFragment')
         self._add_domain_attribute_fields(reference_attribute_frag)
         self._add_dimension_attribute_fields(reference_attribute_frag)
         reference_attribute_frag.db_foreign_key_columns()
         reference_attribute_frag.referenced_dimension_entity_id()
         domain_object.__fragment__(reference_attribute_frag)
 
+        calculated_attribute_frag = Fragment(MaxCalculatedAttribute, 'MaxCalculatedAttributeFragment')
+        self._add_domain_attribute_fields(calculated_attribute_frag)
+        self._add_dimension_attribute_fields(calculated_attribute_frag)
+        calculated_attribute_frag.rql()
+        domain_object.__fragment__(calculated_attribute_frag)
+
         metric_attribute_frag = Fragment(MaxMetricAttribute, 'MaxMetricAttributeFragment')
         self._add_domain_attribute_fields(metric_attribute_frag)
         metric_attribute_frag.db_metric_column()
         metric_attribute_frag.agg_method()
         metric_attribute_frag.is_row_level_filter()
         metric_attribute_frag.is_positive_direction_up()
         metric_attribute_frag.can_be_averaged()
         metric_attribute_frag.is_not_additive()
         metric_attribute_frag.growth_output_format()
         metric_attribute_frag.hide_percentage_change()
+        metric_attribute_frag.sql_agg_expression()
+        metric_attribute_frag.metric_type()
         domain_object.__fragment__(metric_attribute_frag)
-        
-        calc_metric_attribute_frag = Fragment(MaxCalculatedMetric, 'MaxCalculatedMetricFragment')
-        # self._add_domain_object_fields(calc_metric_attribute_frag)
-        calc_metric_attribute_frag.display_format()
-        calc_metric_attribute_frag.rql()
-        calc_metric_attribute_frag.agg_method()
-        calc_metric_attribute_frag.is_positive_direction_up()
-        calc_metric_attribute_frag.can_be_averaged()
-        calc_metric_attribute_frag.is_not_additive()
-        calc_metric_attribute_frag.growth_output_format()
-        calc_metric_attribute_frag.hide_percentage_change()
-        domain_object.__fragment__(calc_metric_attribute_frag)
 
     def _add_domain_entity_fields(self, fragment: Fragment):
         fragment.db_table()
+        fragment.derived_table_sql()
+
+        attributes = fragment.attributes()
+
+        self._add_domain_attribute_fragments(attributes)
 
     def _add_domain_object_fields(self, domain_object):
         domain_object.type()
         domain_object.id()
         domain_object.name()
         domain_object.description()
         domain_object.output_label()
         domain_object.synonyms()
         domain_object.output_label_plural()
         domain_object.hide_from_user()
+
     def _add_domain_attribute_fields(self, fragment: Fragment):
         fragment.display_format()
         fragment.headline_name()
         fragment.is_favorite()
+        fragment.simplified_data_type()
+        fragment.sql()
+
+        # TODO: we do we want this?
         # fragment.domain_entity()
+        # fragment.domain_entity().id()
+        # fragment.domain_entity().name()
 
     def _add_dimension_attribute_fields(self, fragment: Fragment):
         fragment.default_filter_value()
         fragment.is_required_in_query()
+        fragment.dimension_value_mapping_list()
```

### Comparing `answerrocket-client-0.1.9/answer_rocket/graphql/client.py` & `answerrocket_client-0.2.0/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.9/answer_rocket/graphql/schema.py` & `answerrocket_client-0.2.0/answer_rocket/graphql/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 
 ########################################################################
 # Scalars and Enumerations
 ########################################################################
 Boolean = sgqlc.types.Boolean
 
+class ChatDryRunType(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('SKIP_SKILL_EXEC', 'SKIP_SKILL_NLG')
+
+
 DateTime = sgqlc.types.datetime.DateTime
 
 class DpsAggMethod(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('AVG', 'COUNT', 'CUSTOM', 'MAX', 'MIN', 'NONE', 'SUM')
 
 
@@ -22,114 +27,173 @@
 
 Int = sgqlc.types.Int
 
 class JSON(sgqlc.types.Scalar):
     __schema__ = schema
 
 
+class MetricType(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('BASIC', 'RATIO', 'SHARE')
+
+
+class SimplifiedDataType(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('BOOLEAN', 'DATE', 'NUMBER', 'STRING')
+
+
 String = sgqlc.types.String
 
 class UUID(sgqlc.types.Scalar):
     __schema__ = schema
 
 
 
 ########################################################################
 # Input Objects
 ########################################################################
+class MaxCopilotQuestionInput(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('skill_id', 'nl', 'hint', 'parameters')
+    skill_id = sgqlc.types.Field(UUID, graphql_name='skillId')
+    nl = sgqlc.types.Field(String, graphql_name='nl')
+    hint = sgqlc.types.Field(String, graphql_name='hint')
+    parameters = sgqlc.types.Field(JSON, graphql_name='parameters')
+
+
 
 ########################################################################
 # Output Objects and Interfaces
 ########################################################################
 class LLMApiConfig(sgqlc.types.Interface):
     __schema__ = schema
-    __field_names__ = ('id', 'api_type', 'model_type', 'model_name', 'is_active')
+    __field_names__ = ('id', 'api_type', 'model_type', 'model_name')
     id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
     api_type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='apiType')
     model_type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='modelType')
     model_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='modelName')
-    is_active = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isActive')
 
 
 class MaxDomainObject(sgqlc.types.Interface):
     __schema__ = schema
-    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user')
+    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user', 'misc_info')
     type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='type')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     output_label = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='outputLabel')
     synonyms = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='synonyms')
     output_label_plural = sgqlc.types.Field(String, graphql_name='outputLabelPlural')
     hide_from_user = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hideFromUser')
+    misc_info = sgqlc.types.Field(String, graphql_name='miscInfo')
 
 
 class MaxDomainAttribute(sgqlc.types.Interface):
     __schema__ = schema
-    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user', 'display_format', 'headline_name', 'is_favorite', 'domain_entity')
+    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user', 'misc_info', 'display_format', 'headline_name', 'is_favorite', 'simplified_data_type', 'sql', 'domain_entity')
     type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='type')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     output_label = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='outputLabel')
     synonyms = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='synonyms')
     output_label_plural = sgqlc.types.Field(String, graphql_name='outputLabelPlural')
     hide_from_user = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hideFromUser')
+    misc_info = sgqlc.types.Field(String, graphql_name='miscInfo')
     display_format = sgqlc.types.Field(String, graphql_name='displayFormat')
     headline_name = sgqlc.types.Field(String, graphql_name='headlineName')
-    is_favorite = sgqlc.types.Field(Boolean, graphql_name='isFavorite')
+    is_favorite = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isFavorite')
+    simplified_data_type = sgqlc.types.Field(SimplifiedDataType, graphql_name='simplifiedDataType')
+    sql = sgqlc.types.Field(String, graphql_name='sql')
     domain_entity = sgqlc.types.Field('MaxDomainEntity', graphql_name='domainEntity')
 
 
 class MaxDimensionAttribute(sgqlc.types.Interface):
     __schema__ = schema
-    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user', 'display_format', 'headline_name', 'is_favorite', 'domain_entity', 'default_filter_value', 'is_required_in_query')
+    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user', 'misc_info', 'display_format', 'headline_name', 'is_favorite', 'simplified_data_type', 'sql', 'domain_entity', 'dimension_value_mapping_list', 'default_filter_value', 'is_required_in_query')
     type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='type')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     output_label = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='outputLabel')
     synonyms = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='synonyms')
     output_label_plural = sgqlc.types.Field(String, graphql_name='outputLabelPlural')
     hide_from_user = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hideFromUser')
+    misc_info = sgqlc.types.Field(String, graphql_name='miscInfo')
     display_format = sgqlc.types.Field(String, graphql_name='displayFormat')
     headline_name = sgqlc.types.Field(String, graphql_name='headlineName')
-    is_favorite = sgqlc.types.Field(Boolean, graphql_name='isFavorite')
+    is_favorite = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isFavorite')
+    simplified_data_type = sgqlc.types.Field(SimplifiedDataType, graphql_name='simplifiedDataType')
+    sql = sgqlc.types.Field(String, graphql_name='sql')
     domain_entity = sgqlc.types.Field('MaxDomainEntity', graphql_name='domainEntity')
+    dimension_value_mapping_list = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('DimensionValueMapping'))), graphql_name='dimensionValueMappingList')
     default_filter_value = sgqlc.types.Field(String, graphql_name='defaultFilterValue')
     is_required_in_query = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isRequiredInQuery')
 
 
 class MaxDomainEntity(sgqlc.types.Interface):
     __schema__ = schema
-    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user', 'db_table', 'attributes')
+    __field_names__ = ('type', 'id', 'name', 'description', 'output_label', 'synonyms', 'output_label_plural', 'hide_from_user', 'misc_info', 'db_table', 'derived_table_sql', 'attributes')
     type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='type')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     output_label = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='outputLabel')
     synonyms = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='synonyms')
     output_label_plural = sgqlc.types.Field(String, graphql_name='outputLabelPlural')
     hide_from_user = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hideFromUser')
+    misc_info = sgqlc.types.Field(String, graphql_name='miscInfo')
     db_table = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='dbTable')
-    attributes = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(MaxDomainAttribute)), graphql_name='attributes')
+    derived_table_sql = sgqlc.types.Field(String, graphql_name='derivedTableSql')
+    attributes = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MaxDomainAttribute))), graphql_name='attributes')
+
+
+class ChatEntry(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('id', 'thread_id', 'answer')
+    id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
+    thread_id = sgqlc.types.Field(UUID, graphql_name='threadId')
+    answer = sgqlc.types.Field('ChatResult', graphql_name='answer')
+
+
+class ChatResult(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('answer_id', 'answered_at', 'copilot_skill_id', 'has_finished', 'error', 'is_new_thread', 'message', 'report_results', 'thread_id', 'user_id')
+    answer_id = sgqlc.types.Field(UUID, graphql_name='answerId')
+    answered_at = sgqlc.types.Field(DateTime, graphql_name='answeredAt')
+    copilot_skill_id = sgqlc.types.Field(UUID, graphql_name='copilotSkillId')
+    has_finished = sgqlc.types.Field(Boolean, graphql_name='hasFinished')
+    error = sgqlc.types.Field(String, graphql_name='error')
+    is_new_thread = sgqlc.types.Field(Boolean, graphql_name='isNewThread')
+    message = sgqlc.types.Field(String, graphql_name='message')
+    report_results = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('ReportResult')), graphql_name='reportResults')
+    thread_id = sgqlc.types.Field(UUID, graphql_name='threadId')
+    user_id = sgqlc.types.Field(UUID, graphql_name='userId')
 
 
 class ChatThread(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('id', 'entry_count', 'title', 'pinned_dataset')
     id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
     entry_count = sgqlc.types.Field(Int, graphql_name='entryCount', args=sgqlc.types.ArgDict((
         ('most_recent_entry_inclusive', sgqlc.types.Arg(UUID, graphql_name='mostRecentEntryInclusive', default=None)),
 ))
     )
     title = sgqlc.types.Field(String, graphql_name='title')
     pinned_dataset = sgqlc.types.Field(UUID, graphql_name='pinnedDataset')
 
 
+class ContentBlock(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('id', 'title', 'payload')
+    id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
+    title = sgqlc.types.Field(String, graphql_name='title')
+    payload = sgqlc.types.Field(String, graphql_name='payload')
+
+
 class CopilotSkillArtifact(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('copilot_skill_artifact_id', 'copilot_id', 'copilot_skill_id', 'artifact_path', 'artifact', 'description', 'created_user_id', 'created_utc', 'last_modified_user_id', 'last_modified_utc', 'version', 'is_active', 'is_deleted')
     copilot_skill_artifact_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotSkillArtifactId')
     copilot_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotId')
     copilot_skill_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId')
     artifact_path = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='artifactPath')
@@ -149,23 +213,67 @@
     __field_names__ = ('success', 'code', 'errors', 'data')
     success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
     code = sgqlc.types.Field(String, graphql_name='code')
     errors = sgqlc.types.Field(sgqlc.types.list_of(String), graphql_name='errors')
     data = sgqlc.types.Field(JSON, graphql_name='data')
 
 
+class CostInfo(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('completion_tokens', 'prompt_tokens', 'total_tokens', 'cost_estimate_usd', 'model')
+    completion_tokens = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='completionTokens')
+    prompt_tokens = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='promptTokens')
+    total_tokens = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='totalTokens')
+    cost_estimate_usd = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='costEstimateUsd')
+    model = sgqlc.types.Field(String, graphql_name='model')
+
+
+class CreateMaxCopilotSkillChatQuestionResponse(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('copilot_skill_chat_question_id', 'success', 'code', 'error')
+    copilot_skill_chat_question_id = sgqlc.types.Field(UUID, graphql_name='copilotSkillChatQuestionId')
+    success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
+    code = sgqlc.types.Field(String, graphql_name='code')
+    error = sgqlc.types.Field(String, graphql_name='error')
+
+
+class DimensionValueMapping(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('value', 'mapped_values')
+    value = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='value')
+    mapped_values = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='mappedValues')
+
+
 class DomainObjectResponse(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('success', 'code', 'error', 'domain_object')
     success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
     code = sgqlc.types.Field(String, graphql_name='code')
     error = sgqlc.types.Field(String, graphql_name='error')
     domain_object = sgqlc.types.Field(MaxDomainObject, graphql_name='domainObject')
 
 
+class EvaluateChatQuestionResponse(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('success', 'eval_results')
+    success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
+    eval_results = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('EvaluateChatQuestionResult'))), graphql_name='evalResults')
+
+
+class EvaluateChatQuestionResult(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('eval_type', 'pass_', 'explanation', 'correct_function', 'is_loading', 'cost')
+    eval_type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='evalType')
+    pass_ = sgqlc.types.Field(Boolean, graphql_name='pass')
+    explanation = sgqlc.types.Field(String, graphql_name='explanation')
+    correct_function = sgqlc.types.Field(String, graphql_name='correctFunction')
+    is_loading = sgqlc.types.Field(Boolean, graphql_name='isLoading')
+    cost = sgqlc.types.Field(CostInfo, graphql_name='cost')
+
+
 class ExecuteRqlQueryResponse(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('success', 'code', 'error', 'process_rql_script_response', 'sql', 'data')
     success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
     code = sgqlc.types.Field(String, graphql_name='code')
     error = sgqlc.types.Field(String, graphql_name='error')
     process_rql_script_response = sgqlc.types.Field(JSON, graphql_name='processRqlScriptResponse')
@@ -178,61 +286,268 @@
     __field_names__ = ('success', 'code', 'error', 'data')
     success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
     code = sgqlc.types.Field(String, graphql_name='code')
     error = sgqlc.types.Field(String, graphql_name='error')
     data = sgqlc.types.Field(JSON, graphql_name='data')
 
 
+class MaxColumn(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('name', 'jdbc_type', 'length', 'precision', 'scale')
+    name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
+    jdbc_type = sgqlc.types.Field(String, graphql_name='jdbcType')
+    length = sgqlc.types.Field(Int, graphql_name='length')
+    precision = sgqlc.types.Field(Int, graphql_name='precision')
+    scale = sgqlc.types.Field(Int, graphql_name='scale')
+
+
+class MaxCopilot(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('copilot_id', 'name', 'description', 'system_prompt', 'beta_yaml', 'global_python_code', 'copilot_questions')
+    copilot_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotId')
+    name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
+    description = sgqlc.types.Field(String, graphql_name='description')
+    system_prompt = sgqlc.types.Field(String, graphql_name='systemPrompt')
+    beta_yaml = sgqlc.types.Field(String, graphql_name='betaYaml')
+    global_python_code = sgqlc.types.Field(String, graphql_name='globalPythonCode')
+    copilot_questions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MaxCopilotQuestion'))), graphql_name='copilotQuestions')
+
+
+class MaxCopilotQuestion(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('copilot_question_id', 'nl', 'skill_id', 'parameters', 'is_starter', 'hint', 'created_user_id', 'created_utc', 'last_modified_user_id', 'last_modified_utc', 'version', 'is_deleted')
+    copilot_question_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotQuestionId')
+    nl = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='nl')
+    skill_id = sgqlc.types.Field(UUID, graphql_name='skillId')
+    parameters = sgqlc.types.Field(JSON, graphql_name='parameters')
+    is_starter = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isStarter')
+    hint = sgqlc.types.Field(String, graphql_name='hint')
+    created_user_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='createdUserId')
+    created_utc = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='createdUtc')
+    last_modified_user_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='lastModifiedUserId')
+    last_modified_utc = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='lastModifiedUtc')
+    version = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='version')
+    is_deleted = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isDeleted')
+
+
+class MaxCopilotSkill(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('copilot_skill_id', 'name', 'detailed_name', 'description', 'detailed_description', 'dataset_id', 'skill_chat_questions', 'yaml_code', 'skill_code', 'misc_info', 'scheduling_only')
+    copilot_skill_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId')
+    name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
+    detailed_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='detailedName')
+    description = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='description')
+    detailed_description = sgqlc.types.Field(String, graphql_name='detailedDescription')
+    dataset_id = sgqlc.types.Field(UUID, graphql_name='datasetId')
+    skill_chat_questions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('MaxCopilotSkillChatQuestion')), graphql_name='skillChatQuestions')
+    yaml_code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='yamlCode')
+    skill_code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='skillCode')
+    misc_info = sgqlc.types.Field(JSON, graphql_name='miscInfo')
+    scheduling_only = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='schedulingOnly')
+
+
+class MaxCopilotSkillChatQuestion(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('copilot_skill_chat_question_id', 'question', 'expected_completion_response')
+    copilot_skill_chat_question_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotSkillChatQuestionId')
+    question = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='question')
+    expected_completion_response = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='expectedCompletionResponse')
+
+
+class MaxCreateCopilotQuestionResponse(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('copilot_question_id', 'success', 'code', 'errors')
+    copilot_question_id = sgqlc.types.Field(UUID, graphql_name='copilotQuestionId')
+    success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
+    code = sgqlc.types.Field(String, graphql_name='code')
+    errors = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='errors')
+
+
+class MaxDatabase(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('database_id', 'name', 'dbms', 'schema')
+    database_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='databaseId')
+    name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
+    dbms = sgqlc.types.Field(String, graphql_name='dbms')
+    schema = sgqlc.types.Field(String, graphql_name='schema')
+
+
+class MaxDataset(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('dataset_id', 'name', 'description', 'domain_objects', 'misc_info', 'database', 'tables', 'dimension_value_distribution_map', 'date_range_boundary_attribute_id', 'dimension_hierarchies', 'metric_hierarchies', 'domain_attribute_statistics', 'default_performance_metric_id', 'dataset_min_date', 'dataset_max_date', 'query_row_limit')
+    dataset_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='datasetId')
+    name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
+    description = sgqlc.types.Field(String, graphql_name='description')
+    domain_objects = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MaxDomainObject))), graphql_name='domainObjects')
+    misc_info = sgqlc.types.Field(String, graphql_name='miscInfo')
+    database = sgqlc.types.Field(MaxDatabase, graphql_name='database')
+    tables = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MaxTable'))), graphql_name='tables')
+    dimension_value_distribution_map = sgqlc.types.Field(JSON, graphql_name='dimensionValueDistributionMap')
+    date_range_boundary_attribute_id = sgqlc.types.Field(String, graphql_name='dateRangeBoundaryAttributeId')
+    dimension_hierarchies = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('MaxDimensionHierarchyNode')), graphql_name='dimensionHierarchies')
+    metric_hierarchies = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('MaxMetricHierarchyNode')), graphql_name='metricHierarchies')
+    domain_attribute_statistics = sgqlc.types.Field(JSON, graphql_name='domainAttributeStatistics')
+    default_performance_metric_id = sgqlc.types.Field(String, graphql_name='defaultPerformanceMetricId')
+    dataset_min_date = sgqlc.types.Field(DateTime, graphql_name='datasetMinDate')
+    dataset_max_date = sgqlc.types.Field(DateTime, graphql_name='datasetMaxDate')
+    query_row_limit = sgqlc.types.Field(Int, graphql_name='queryRowLimit')
+
+
+class MaxDimensionHierarchyNode(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('dimension_hierarchy_node_id', 'dimension_attribute_id', 'description', 'children')
+    dimension_hierarchy_node_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='dimensionHierarchyNodeId')
+    dimension_attribute_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='dimensionAttributeId')
+    description = sgqlc.types.Field(String, graphql_name='description')
+    children = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MaxDimensionHierarchyNode'))), graphql_name='children')
+
+
+class MaxDomainAttributeStatisticInfo(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('null_count', 'min_value', 'max_value', 'distinct_count')
+    null_count = sgqlc.types.Field(Int, graphql_name='nullCount')
+    min_value = sgqlc.types.Field(String, graphql_name='minValue')
+    max_value = sgqlc.types.Field(String, graphql_name='maxValue')
+    distinct_count = sgqlc.types.Field(Int, graphql_name='distinctCount')
+
+
+class MaxMetricHierarchyNode(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('metric_hierarchy_node_id', 'metric_id', 'description', 'children')
+    metric_hierarchy_node_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='metricHierarchyNodeId')
+    metric_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='metricId')
+    description = sgqlc.types.Field(String, graphql_name='description')
+    children = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MaxMetricHierarchyNode'))), graphql_name='children')
+
+
+class MaxMutationResponse(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('success', 'code', 'error')
+    success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
+    code = sgqlc.types.Field(String, graphql_name='code')
+    error = sgqlc.types.Field(String, graphql_name='error')
+
+
+class MaxTable(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('name', 'columns')
+    name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
+    columns = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MaxColumn))), graphql_name='columns')
+
+
 class Mutation(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('update_chat_answer_payload', 'ask_chat_question')
+    __field_names__ = ('create_max_copilot_skill_chat_question', 'update_max_copilot_skill_chat_question', 'delete_max_copilot_skill_chat_question', 'create_max_copilot_question', 'update_max_copilot_question', 'delete_max_copilot_question', 'update_chat_answer_payload', 'ask_chat_question', 'evaluate_chat_question')
+    create_max_copilot_skill_chat_question = sgqlc.types.Field(sgqlc.types.non_null(CreateMaxCopilotSkillChatQuestionResponse), graphql_name='createMaxCopilotSkillChatQuestion', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+        ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
+        ('question', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='question', default=None)),
+        ('expected_completion_response', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='expectedCompletionResponse', default=None)),
+))
+    )
+    update_max_copilot_skill_chat_question = sgqlc.types.Field(sgqlc.types.non_null(MaxMutationResponse), graphql_name='updateMaxCopilotSkillChatQuestion', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+        ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
+        ('copilot_skill_chat_question_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillChatQuestionId', default=None)),
+        ('question', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='question', default=None)),
+        ('expected_completion_response', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='expectedCompletionResponse', default=None)),
+))
+    )
+    delete_max_copilot_skill_chat_question = sgqlc.types.Field(sgqlc.types.non_null(MaxMutationResponse), graphql_name='deleteMaxCopilotSkillChatQuestion', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+        ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
+        ('copilot_skill_chat_question_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillChatQuestionId', default=None)),
+))
+    )
+    create_max_copilot_question = sgqlc.types.Field(sgqlc.types.non_null(MaxCreateCopilotQuestionResponse), graphql_name='createMaxCopilotQuestion', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+        ('copilot_question', sgqlc.types.Arg(sgqlc.types.non_null(MaxCopilotQuestionInput), graphql_name='copilotQuestion', default=None)),
+))
+    )
+    update_max_copilot_question = sgqlc.types.Field(sgqlc.types.non_null(MaxMutationResponse), graphql_name='updateMaxCopilotQuestion', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+        ('copilot_question_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotQuestionId', default=None)),
+        ('copilot_question', sgqlc.types.Arg(sgqlc.types.non_null(MaxCopilotQuestionInput), graphql_name='copilotQuestion', default=None)),
+))
+    )
+    delete_max_copilot_question = sgqlc.types.Field(sgqlc.types.non_null(MaxMutationResponse), graphql_name='deleteMaxCopilotQuestion', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+        ('copilot_question_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotQuestionId', default=None)),
+))
+    )
     update_chat_answer_payload = sgqlc.types.Field(JSON, graphql_name='updateChatAnswerPayload', args=sgqlc.types.ArgDict((
         ('answer_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='answerId', default=None)),
         ('payload', sgqlc.types.Arg(sgqlc.types.non_null(JSON), graphql_name='payload', default=None)),
 ))
     )
-    ask_chat_question = sgqlc.types.Field(JSON, graphql_name='askChatQuestion', args=sgqlc.types.ArgDict((
+    ask_chat_question = sgqlc.types.Field(ChatEntry, graphql_name='askChatQuestion', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('question', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='question', default=None)),
         ('thread_id', sgqlc.types.Arg(UUID, graphql_name='threadId', default=None)),
+        ('skip_report_cache', sgqlc.types.Arg(Boolean, graphql_name='skipReportCache', default=None)),
+        ('dry_run_type', sgqlc.types.Arg(ChatDryRunType, graphql_name='dryRunType', default=None)),
+))
+    )
+    evaluate_chat_question = sgqlc.types.Field(sgqlc.types.non_null(EvaluateChatQuestionResponse), graphql_name='evaluateChatQuestion', args=sgqlc.types.ArgDict((
+        ('entry_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='entryId', default=None)),
+        ('evals', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='evals', default=None)),
 ))
     )
 
 
 class Query(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('ping', 'get_copilot_skill_artifact_by_path', 'run_copilot_skill', 'execute_sql_query', 'execute_rql_query', 'get_dataset_id', 'get_domain_object', 'get_domain_object_by_name', 'llmapi_config_for_sdk', 'user_chat_threads', 'user_chat_entries')
+    __field_names__ = ('ping', 'get_copilot_skill_artifact_by_path', 'get_copilot_info', 'get_copilot_skill', 'run_copilot_skill', 'execute_sql_query', 'execute_rql_query', 'get_dataset_id', 'get_dataset', 'get_domain_object', 'get_domain_object_by_name', 'llmapi_config_for_sdk', 'user_chat_threads', 'user_chat_entries')
     ping = sgqlc.types.Field(String, graphql_name='ping')
     get_copilot_skill_artifact_by_path = sgqlc.types.Field(CopilotSkillArtifact, graphql_name='getCopilotSkillArtifactByPath', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
         ('artifact_path', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='artifactPath', default=None)),
 ))
     )
+    get_copilot_info = sgqlc.types.Field(MaxCopilot, graphql_name='getCopilotInfo', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+))
+    )
+    get_copilot_skill = sgqlc.types.Field(MaxCopilotSkill, graphql_name='getCopilotSkill', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+        ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
+))
+    )
     run_copilot_skill = sgqlc.types.Field(CopilotSkillRunResponse, graphql_name='runCopilotSkill', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('skill_name', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='skillName', default=None)),
         ('parameters', sgqlc.types.Arg(JSON, graphql_name='parameters', default=None)),
 ))
     )
     execute_sql_query = sgqlc.types.Field(ExecuteSqlQueryResponse, graphql_name='executeSqlQuery', args=sgqlc.types.ArgDict((
         ('database_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='databaseId', default=None)),
         ('sql_query', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='sqlQuery', default=None)),
         ('row_limit', sgqlc.types.Arg(Int, graphql_name='rowLimit', default=None)),
+        ('copilot_id', sgqlc.types.Arg(UUID, graphql_name='copilotId', default=None)),
+        ('copilot_skill_id', sgqlc.types.Arg(UUID, graphql_name='copilotSkillId', default=None)),
 ))
     )
     execute_rql_query = sgqlc.types.Field(ExecuteRqlQueryResponse, graphql_name='executeRqlQuery', args=sgqlc.types.ArgDict((
         ('dataset_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='datasetId', default=None)),
         ('rql_query', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='rqlQuery', default=None)),
+        ('row_limit', sgqlc.types.Arg(Int, graphql_name='rowLimit', default=None)),
+        ('copilot_id', sgqlc.types.Arg(UUID, graphql_name='copilotId', default=None)),
+        ('copilot_skill_id', sgqlc.types.Arg(UUID, graphql_name='copilotSkillId', default=None)),
 ))
     )
     get_dataset_id = sgqlc.types.Field(UUID, graphql_name='getDatasetId', args=sgqlc.types.ArgDict((
         ('dataset_name', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='datasetName', default=None)),
 ))
     )
+    get_dataset = sgqlc.types.Field(MaxDataset, graphql_name='getDataset', args=sgqlc.types.ArgDict((
+        ('dataset_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='datasetId', default=None)),
+        ('copilot_id', sgqlc.types.Arg(UUID, graphql_name='copilotId', default=None)),
+))
+    )
     get_domain_object = sgqlc.types.Field(DomainObjectResponse, graphql_name='getDomainObject', args=sgqlc.types.ArgDict((
         ('dataset_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='datasetId', default=None)),
         ('domain_object_id', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='domainObjectId', default=None)),
 ))
     )
     get_domain_object_by_name = sgqlc.types.Field(DomainObjectResponse, graphql_name='getDomainObjectByName', args=sgqlc.types.ArgDict((
         ('dataset_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='datasetId', default=None)),
@@ -253,46 +568,75 @@
         ('thread_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='threadId', default=None)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=None)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=None)),
 ))
     )
 
 
+class ReportParamsAndValues(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('key', 'values', 'label', 'type', 'color')
+    key = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='key')
+    values = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='values')
+    label = sgqlc.types.Field(String, graphql_name='label')
+    type = sgqlc.types.Field(String, graphql_name='type')
+    color = sgqlc.types.Field(String, graphql_name='color')
+
+
+class ReportResult(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('id', 'title', 'report_name', 'run_id', 'parameters', 'content_blocks')
+    id = sgqlc.types.Field(UUID, graphql_name='id')
+    title = sgqlc.types.Field(String, graphql_name='title')
+    report_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='reportName')
+    run_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='runId')
+    parameters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ReportParamsAndValues)), graphql_name='parameters')
+    content_blocks = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ContentBlock))), graphql_name='contentBlocks')
+
+
 class AzureOpenaiCompletionLLMApiConfig(sgqlc.types.Type, LLMApiConfig):
     __schema__ = schema
-    __field_names__ = ('api_base_url', 'api_version', 'openai_model_name', 'max_tokens_content_generation', 'temperature', 'top_p', 'presence_penalty', 'frequency_penalty', 'stop_sequence')
+    __field_names__ = ('api_base_url', 'api_version', 'openai_model_name', 'max_tokens_content_generation', 'temperature', 'top_p', 'presence_penalty', 'frequency_penalty')
     api_base_url = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='apiBaseUrl')
     api_version = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='apiVersion')
     openai_model_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='openaiModelName')
     max_tokens_content_generation = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='maxTokensContentGeneration')
     temperature = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='temperature')
     top_p = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='topP')
     presence_penalty = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='presencePenalty')
     frequency_penalty = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='frequencyPenalty')
-    stop_sequence = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='stopSequence')
 
 
 class AzureOpenaiEmbeddingLLMApiConfig(sgqlc.types.Type, LLMApiConfig):
     __schema__ = schema
     __field_names__ = ('api_base_url', 'api_version')
     api_base_url = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='apiBaseUrl')
     api_version = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='apiVersion')
 
 
+class MaxCalculatedAttribute(sgqlc.types.Type, MaxDomainObject, MaxDomainAttribute, MaxDimensionAttribute):
+    __schema__ = schema
+    __field_names__ = ('rql',)
+    rql = sgqlc.types.Field(String, graphql_name='rql')
+
+
 class MaxCalculatedMetric(sgqlc.types.Type, MaxDomainObject):
     __schema__ = schema
-    __field_names__ = ('display_format', 'rql', 'agg_method', 'is_positive_direction_up', 'can_be_averaged', 'is_not_additive', 'growth_output_format', 'hide_percentage_change')
+    __field_names__ = ('display_format', 'rql', 'sql', 'agg_method', 'is_positive_direction_up', 'can_be_averaged', 'is_not_additive', 'growth_output_format', 'hide_percentage_change', 'simplified_data_type', 'metric_type')
     display_format = sgqlc.types.Field(String, graphql_name='displayFormat')
     rql = sgqlc.types.Field(String, graphql_name='rql')
-    agg_method = sgqlc.types.Field(DpsAggMethod, graphql_name='aggMethod')
-    is_positive_direction_up = sgqlc.types.Field(Boolean, graphql_name='isPositiveDirectionUp')
-    can_be_averaged = sgqlc.types.Field(Boolean, graphql_name='canBeAveraged')
-    is_not_additive = sgqlc.types.Field(Boolean, graphql_name='isNotAdditive')
+    sql = sgqlc.types.Field(String, graphql_name='sql')
+    agg_method = sgqlc.types.Field(sgqlc.types.non_null(DpsAggMethod), graphql_name='aggMethod')
+    is_positive_direction_up = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isPositiveDirectionUp')
+    can_be_averaged = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='canBeAveraged')
+    is_not_additive = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isNotAdditive')
     growth_output_format = sgqlc.types.Field(String, graphql_name='growthOutputFormat')
-    hide_percentage_change = sgqlc.types.Field(Boolean, graphql_name='hidePercentageChange')
+    hide_percentage_change = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hidePercentageChange')
+    simplified_data_type = sgqlc.types.Field(SimplifiedDataType, graphql_name='simplifiedDataType')
+    metric_type = sgqlc.types.Field(MetricType, graphql_name='metricType')
 
 
 class MaxDimensionEntity(sgqlc.types.Type, MaxDomainObject, MaxDomainEntity):
     __schema__ = schema
     __field_names__ = ('primary_attribute', 'archetype')
     primary_attribute = sgqlc.types.Field('MaxPrimaryAttribute', graphql_name='primaryAttribute')
     archetype = sgqlc.types.Field(String, graphql_name='archetype')
@@ -301,23 +645,25 @@
 class MaxFactEntity(sgqlc.types.Type, MaxDomainObject, MaxDomainEntity):
     __schema__ = schema
     __field_names__ = ()
 
 
 class MaxMetricAttribute(sgqlc.types.Type, MaxDomainObject, MaxDomainAttribute):
     __schema__ = schema
-    __field_names__ = ('db_metric_column', 'agg_method', 'is_row_level_filter', 'is_positive_direction_up', 'can_be_averaged', 'is_not_additive', 'growth_output_format', 'hide_percentage_change')
-    db_metric_column = sgqlc.types.Field(String, graphql_name='dbMetricColumn')
-    agg_method = sgqlc.types.Field(DpsAggMethod, graphql_name='aggMethod')
-    is_row_level_filter = sgqlc.types.Field(Boolean, graphql_name='isRowLevelFilter')
-    is_positive_direction_up = sgqlc.types.Field(Boolean, graphql_name='isPositiveDirectionUp')
-    can_be_averaged = sgqlc.types.Field(Boolean, graphql_name='canBeAveraged')
-    is_not_additive = sgqlc.types.Field(Boolean, graphql_name='isNotAdditive')
+    __field_names__ = ('db_metric_column', 'agg_method', 'is_row_level_filter', 'is_positive_direction_up', 'can_be_averaged', 'is_not_additive', 'growth_output_format', 'hide_percentage_change', 'sql_agg_expression', 'metric_type')
+    db_metric_column = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='dbMetricColumn')
+    agg_method = sgqlc.types.Field(sgqlc.types.non_null(DpsAggMethod), graphql_name='aggMethod')
+    is_row_level_filter = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isRowLevelFilter')
+    is_positive_direction_up = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isPositiveDirectionUp')
+    can_be_averaged = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='canBeAveraged')
+    is_not_additive = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isNotAdditive')
     growth_output_format = sgqlc.types.Field(String, graphql_name='growthOutputFormat')
-    hide_percentage_change = sgqlc.types.Field(Boolean, graphql_name='hidePercentageChange')
+    hide_percentage_change = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hidePercentageChange')
+    sql_agg_expression = sgqlc.types.Field(String, graphql_name='sqlAggExpression')
+    metric_type = sgqlc.types.Field(MetricType, graphql_name='metricType')
 
 
 class MaxNormalAttribute(sgqlc.types.Type, MaxDomainObject, MaxDomainAttribute, MaxDimensionAttribute):
     __schema__ = schema
     __field_names__ = ('db_column', 'db_secondary_column')
     db_column = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='dbColumn')
     db_secondary_column = sgqlc.types.Field(String, graphql_name='dbSecondaryColumn')
@@ -335,22 +681,21 @@
     __field_names__ = ('db_foreign_key_columns', 'referenced_dimension_entity_id')
     db_foreign_key_columns = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(String)), graphql_name='dbForeignKeyColumns')
     referenced_dimension_entity_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='referencedDimensionEntityId')
 
 
 class OpenaiCompletionLLMApiConfig(sgqlc.types.Type, LLMApiConfig):
     __schema__ = schema
-    __field_names__ = ('organization', 'max_tokens_content_generation', 'temperature', 'top_p', 'presence_penalty', 'frequency_penalty', 'stop_sequence')
+    __field_names__ = ('organization', 'max_tokens_content_generation', 'temperature', 'top_p', 'presence_penalty', 'frequency_penalty')
     organization = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='organization')
     max_tokens_content_generation = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='maxTokensContentGeneration')
     temperature = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='temperature')
     top_p = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='topP')
     presence_penalty = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='presencePenalty')
     frequency_penalty = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='frequencyPenalty')
-    stop_sequence = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='stopSequence')
 
 
 class OpenaiEmbeddingLLMApiConfig(sgqlc.types.Type, LLMApiConfig):
     __schema__ = schema
     __field_names__ = ('organization',)
     organization = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='organization')
```

### Comparing `answerrocket-client-0.1.9/answer_rocket/output.py` & `answerrocket_client-0.2.0/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.9/answer_rocket/skill.py` & `answerrocket_client-0.2.0/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.9/answerrocket_client.egg-info/PKG-INFO` & `answerrocket_client-0.2.0/answerrocket_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # AnswerRocket Skill API Client
-This is a client library for interacting with an AnswerRocket instance.  Its purpose is to enable the development of skills (custom AnswerRocket extensions) without the need for AnswerRocket to be running locally.
+This is a client library for interacting with an AnswerRocket instance.
 
 ## Installation
 
 `pip install answerrocket-client`
 
 ## Use
```

### Comparing `answerrocket-client-0.1.9/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket_client-0.2.0/answerrocket_client.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 answer_rocket/error.py
 answer_rocket/output.py
 answer_rocket/skill.py
 answer_rocket/types.py
 answer_rocket/graphql/__init__.py
 answer_rocket/graphql/client.py
 answer_rocket/graphql/schema.py
+answer_rocket/graphql/sdk_operations.py
 answerrocket_client.egg-info/PKG-INFO
 answerrocket_client.egg-info/SOURCES.txt
 answerrocket_client.egg-info/dependency_links.txt
 answerrocket_client.egg-info/requires.txt
 answerrocket_client.egg-info/top_level.txt
 test/test_client.py
```

### Comparing `answerrocket-client-0.1.9/readme.md` & `answerrocket_client-0.2.0/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # AnswerRocket Skill API Client
-This is a client library for interacting with an AnswerRocket instance.  Its purpose is to enable the development of skills (custom AnswerRocket extensions) without the need for AnswerRocket to be running locally.
+This is a client library for interacting with an AnswerRocket instance.
 
 ## Installation
 
 `pip install answerrocket-client`
 
 ## Use
```

