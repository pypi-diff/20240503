# Comparing `tmp/argilla_llama_index-0.0.1a0.tar.gz` & `tmp/argilla_llama_index-1.0.0.tar.gz`

## Comparing `argilla_llama_index-0.0.1a0.tar` & `argilla_llama_index-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0   342508 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/docs/argilla-ui-dataset-2.png
--rw-r--r--   0        0        0   319798 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/docs/argilla-ui-dataset.png
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/src/argilla_llama_index/__init__.py
--rw-r--r--   0        0        0    28733 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/src/argilla_llama_index/llama_index_handler.py
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/tests/test_llama_index_callback.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/LICENSE
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/LICENSE_HEADER
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 argilla_llama_index-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0    75041 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/data/paul_graham_essay.txt
+-rw-r--r--   0        0        0   102735 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/docs/assets/argilla-ui-dataset.png
+-rw-r--r--   0        0        0    52647 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/docs/examples/usage_example.ipynb
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/src/argilla_llama_index/__init__.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/src/argilla_llama_index/helpers.py
+-rw-r--r--   0        0        0    30479 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/src/argilla_llama_index/llama_index_handler.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/tests/test_llama_index_callback.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/LICENSE
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/PKG-INFO
```

### Comparing `argilla_llama_index-0.0.1a0/src/argilla_llama_index/__init__.py` & `argilla_llama_index-1.0.0/src/argilla_llama_index/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.1-alpha"
+__version__ = "1.0.0"
 
 from argilla_llama_index.llama_index_handler import ArgillaCallbackHandler
 
 __all__ = ["ArgillaCallbackHandler"]
```

### Comparing `argilla_llama_index-0.0.1a0/src/argilla_llama_index/llama_index_handler.py` & `argilla_llama_index-1.0.0/src/argilla_llama_index/llama_index_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,428 +1,455 @@
-from argilla._constants import DEFAULT_API_KEY, DEFAULT_API_URL
-import argilla as rg
-from typing import Any, Dict, List, Optional
+from collections import defaultdict
+from datetime import datetime
+import os
 from packaging.version import parse
+from typing import Any, Dict, List, Optional
 import warnings
-import os
-from datetime import datetime
-from collections import defaultdict
-from contextvars import ContextVar
 
-from llama_index.callbacks.base_handler import BaseCallbackHandler
-from llama_index.callbacks.schema import (
-    BASE_TRACE_EVENT,
+from argilla_llama_index.helpers import _calc_time, _get_time_diff
+
+import argilla as rg
+from argilla._constants import DEFAULT_API_KEY, DEFAULT_API_URL
+from llama_index.core.callbacks.base_handler import BaseCallbackHandler
+from llama_index.core.callbacks.schema import (
     CBEventType,
     EventPayload,
     CBEvent,
 )
 
-global_stack_trace = ContextVar("trace", default=[BASE_TRACE_EVENT])
 
 class ArgillaCallbackHandler(BaseCallbackHandler):
-    """Callback handler for Argilla.
-    
-    Args:
-        dataset_name: The name of the dataset to log the events to. If the dataset does not exist,
-            a new one will be created.
-        number_of_retrievals: The number of retrieved documents to log.
-        workspace_name: The name of the workspace to log the events to.
-        api_url: The URL of the Argilla server.
-        api_key: The API key to use to connect to Argilla.
-        event_starts_to_ignore: A list of event types to ignore when they start.
-        event_ends_to_ignore: A list of event types to ignore when they end.
-        handlers: A list of handlers to run when an event starts or ends.
-    
-    Raises:
-        ImportError: If the `argilla` Python package is not installed or the one installed is not compatible
-        ConnectionError: If the connection to Argilla fails
-        FileNotFoundError: If the retrieval and creation of the `FeedbackDataset` fails
-    
-    Example:
-        >>> from argilla_llama_index import ArgillaCallbackHandler
-        >>> from llama_index import VectorStoreIndex, ServiceContext, SimpleDirectoryReader
-        >>> from llama_index.llms import OpenAI
-        >>> from llama_index import set_global_handler
-        >>> set_global_handler("argilla", dataset_name="query_model")
-        >>> llm = OpenAI(model="gpt-3.5-turbo", temperature=0.8)
-        >>> service_context = ServiceContext.from_defaults(llm=llm)
-        >>> docs = SimpleDirectoryReader("data").load_data()
-        >>> index = VectorStoreIndex.from_documents(docs, service_context=service_context)
-        >>> query_engine = index.as_query_engine()
-        >>> response = query_engine.query("What did the author do growing up dude?")
     """
+    Callback handler that logs predictions to Argilla.
+
+    This handler automatically logs the predictions made with LlamaIndex to Argilla,
+    without the need to create a dataset and log the predictions manually. Events relevant
+    to the predictions are automatically logged to Argilla as well, including timestamps of
+    all the different steps of the retrieval and prediction process.
+
+    Attributes:
+        dataset_name (str): The name of the Argilla dataset.
+        number_of_retrievals (int): The number of retrievals to log.
+        workspace_name (str): The name of the Argilla workspace.
+        api_url (str): Argilla API URL.
+        api_key (str): Argilla API key.
+        event_starts_to_ignore (List[CBEventType]): List of event types to ignore at the start of the trace.
+        event_ends_to_ignore (List[CBEventType]): List of event types to ignore at the end of the trace.
+        handlers (List[BaseCallbackHandler]): List of extra handlers to include.
+
+    Methods:
+        start_trace(trace_id: Optional[str] = None) -> None:
+            Logic to be executed at the beggining of the tracing process.
+
+        end_trace(trace_id: Optional[str] = None, trace_map: Optional[Dict[str, List[str]]] = None) -> None:
+            Logic to be executed at the end of the tracing process.
+
+        on_event_start(event_type: CBEventType, payload: Optional[Dict[str, Any]] = None, event_id: Optional[str] = None, parent_id: str = None) -> str:
+            Store event start data by event type. Executed at the start of an event.
+        
+        on_event_end(event_type: CBEventType, payload: Optional[Dict[str, Any]] = None, event_id: str = None) -> None:
+            Store event end data by event type. Executed at the end of an event.
 
-    REPO_URL: str = "https://github.com/argilla-io/argilla"
-    ISSUES_URL: str = f"{REPO_URL}/issues"
+    Usage:
+    ```python
+    from llama_index.core import VectorStoreIndex, ServiceContext, SimpleDirectoryReader, set_global_handler
+    from llama_index.llms.openai import OpenAI
+
+    set_global_handler("argilla", dataset_name="query_model")
+
+    llm = OpenAI(model="gpt-3.5-turbo", temperature=0.8, openai_api_key=os.getenv("OPENAI_API_KEY"))
+
+    service_context = ServiceContext.from_defaults(llm=llm)
+    docs = SimpleDirectoryReader("../../data").load_data()
+    index = VectorStoreIndex.from_documents(docs, service_context=service_context)
+    query_engine = index.as_query_engine()
+
+    response = query_engine.query("What did the author do growing up?")
+    ```
+    """
 
     def __init__(
         self,
         dataset_name: str,
         number_of_retrievals: int = 0,
         workspace_name: Optional[str] = None,
         api_url: Optional[str] = None,
         api_key: Optional[str] = None,
         event_starts_to_ignore: Optional[List[CBEventType]] = None,
         event_ends_to_ignore: Optional[List[CBEventType]] = None,
         handlers: Optional[List[BaseCallbackHandler]] = None,
     ) -> None:
-        """Initialize the Argilla callback handler.
-        
-        Args:
-            dataset_name: The name of the dataset to log the events to. If the dataset does not exist,
-                a new one will be created.
-            number_of_retrievals: The number of retrieved documents to log.
-            workspace_name: The name of the workspace to log the events to.
-            api_url: The URL of the Argilla server.
-            api_key: The API key to use to connect to Argilla.
-            event_starts_to_ignore: A list of event types to ignore when they start.
-            event_ends_to_ignore: A list of event types to ignore when they end.
-            handlers: A list of handlers to run when an event starts or ends.
-    
-        Raises:
-            ImportError: If the `argilla` Python package is not installed or the one installed is not compatible
-            ConnectionError: If the connection to Argilla fails
-            FileNotFoundError: If the retrieval and creation of the `FeedbackDataset` fails
-        
-        """
-        
+
         self.event_starts_to_ignore = event_starts_to_ignore or []
         self.event_ends_to_ignore = event_ends_to_ignore or []
         self.handlers = handlers or []
         self.number_of_retrievals = number_of_retrievals
 
-        # Import Argilla 
         try:
             import argilla as rg
+
             self.ARGILLA_VERSION = rg.__version__
 
         except ImportError:
             raise ImportError(
                 "To use the Argilla callback manager you need to have the `argilla` "
                 "Python package installed. Please install it with `pip install argilla`"
             )
 
-        # Check whether the Argilla version is compatible
         if parse(self.ARGILLA_VERSION) < parse("1.18.0"):
             raise ImportError(
                 f"The installed `argilla` version is {self.ARGILLA_VERSION} but "
                 "`ArgillaCallbackHandler` requires at least version 1.18.0. Please "
                 "upgrade `argilla` with `pip install --upgrade argilla`."
             )
-        
-        # API_URL and API_KEY
-        # Show a warning message if Argilla will assume the default values will be used
+
+        # Ensure the API URL and API key are set, or assume the default values
         if api_url is None and os.getenv("ARGILLA_API_URL") is None:
             warnings.warn(
                 (
-                    "Since `api_url` is None, and the env var `ARGILLA_API_URL` is not"
+                    "Since `api_url` is None, and the environment var `ARGILLA_API_URL` is not"
                     f" set, it will default to `{DEFAULT_API_URL}`, which is the"
                     " default API URL in Argilla Quickstart."
                 ),
             )
             api_url = DEFAULT_API_URL
 
         if api_key is None and os.getenv("ARGILLA_API_KEY") is None:
             warnings.warn(
                 (
-                    "Since `api_key` is None, and the env var `ARGILLA_API_KEY` is not"
+                    "Since `api_key` is None, and the environment var `ARGILLA_API_KEY` is not"
                     f" set, it will default to `{DEFAULT_API_KEY}`, which is the"
                     " default API key in Argilla Quickstart."
                 ),
             )
             api_key = DEFAULT_API_KEY
-    
-        # Connect to Argilla with the provided credentials, if applicable
-        try:
-            rg.init(
-                api_key=api_key, 
-                api_url=api_url
-            )
-        except Exception as e:
-            raise ConnectionError(
-                f"Could not connect to Argilla with exception: '{e}'.\n"
-                "Please check your `api_key` and `api_url`, and make sure that "
-                "the Argilla server is up and running. If the problem persists "
-                f"please report it to {self.ISSUES_URL} as an `integration` issue."
-            ) from e
+
         
+        rg.init(api_key=api_key, api_url=api_url, workspace=workspace_name or rg.get_workspace())
+
         # Set the Argilla variables
         self.dataset_name = dataset_name
         self.workspace_name = workspace_name or rg.get_workspace()
 
-        # Retrieve the `FeedbackDataset` from Argilla
+        # Either create a new dataset or use an existing one, updating it if necessary
         try:
-            if self.dataset_name in [ds.name for ds in rg.FeedbackDataset.list()]:
-                self.dataset = rg.FeedbackDataset.from_argilla(
-                    name=self.dataset_name,
-                    workspace=self.workspace_name,
-                )
-                self.is_new_dataset_created = False
-
-                if number_of_retrievals > 0:
-                    required_context_fields = self._add_context_fields(number_of_retrievals)
-                    required_context_questions = self._add_context_questions(number_of_retrievals)
-                    existing_fields = [field.to_local() for field in self.dataset.fields]
-                    existing_questions = [question.to_local() for question in self.dataset.questions]
-                    # If the required fields and questions do not match with the existing ones, update the dataset and upload it again with "-updated" added to the name
-                    if all(element in existing_fields for element in required_context_fields) == False or all(element in existing_questions for element in required_context_questions) == False:
-                        local_dataset = self.dataset.pull()
-
-                        fields_to_pop = []
-                        for index, field in enumerate(local_dataset.fields):
-                            if field.name.startswith("retrieved_document_"):
-                                fields_to_pop.append(index)
-                                fields_to_pop.sort(reverse=True)
-                        else:
-                            for index in fields_to_pop:
-                                local_dataset.fields.pop(index)
-                        
-                        questions_to_pop = []
-                        for index, question in enumerate(local_dataset.questions):
-                            if question.name.startswith("rating_retrieved_document_"):
-                                questions_to_pop.append(index)
-                                questions_to_pop.sort(reverse=True)
-                        else:
-                            for index in questions_to_pop:
-                                local_dataset.questions.pop(index)
-
-                        for field in required_context_fields:
-                            local_dataset.fields.append(field)
-                        for question in required_context_questions:
-                            local_dataset.questions.append(question)
-                        self.dataset = local_dataset.push_to_argilla(self.dataset_name+"-updated")
-
-            # If the dataset does not exist, create a new one with the given name
-            else:
+            if self.dataset_name not in [ds.name for ds in rg.FeedbackDataset.list()]:
                 dataset = rg.FeedbackDataset(
                     fields=[
                         rg.TextField(name="prompt", required=True),
                         rg.TextField(name="response", required=False),
-                        rg.TextField(name="time-details", title="Time Details", use_markdown=True)
-                    ] + self._add_context_fields(number_of_retrievals),
+                        rg.TextField(
+                            name="time-details", title="Time Details", use_markdown=True
+                        ),
+                    ]
+                    + self._add_context_fields(number_of_retrievals),
                     questions=[
                         rg.RatingQuestion(
                             name="response-rating",
                             title="Rating for the response",
                             description="How would you rate the quality of the response?",
                             values=[1, 2, 3, 4, 5, 6, 7],
                             required=True,
                         ),
                         rg.TextQuestion(
                             name="response-feedback",
                             title="Feedback for the response",
                             description="What feedback do you have for the response?",
                             required=False,
                         ),
-                    ] + self._add_context_questions(number_of_retrievals),
-                        guidelines="You're asked to rate the quality of the response and provide feedback.",
-                        allow_extra_metadata=True,
+                    ]
+                    + self._add_context_questions(number_of_retrievals),
+                    guidelines="You're asked to rate the quality of the response and provide feedback.",
+                    allow_extra_metadata=True,
                 )
+
                 self.dataset = dataset.push_to_argilla(self.dataset_name)
                 self.is_new_dataset_created = True
                 warnings.warn(
-                (
-                    f"No dataset with the name {self.dataset_name} was found in workspace "
-                    f"{self.workspace_name}. A new dataset with the name {self.dataset_name} "
-                    "has been created with the question fields `prompt` and `response`"
-                    "and the rating question `response-rating` with values 1-7 and text question"
-                    " named `response-feedback`."
-                ),
-            )
+                    (
+                        f"No dataset with the name {self.dataset_name} was found in workspace "
+                        f"{self.workspace_name}. A new dataset with the name {self.dataset_name} "
+                        "has been created with the question fields `prompt` and `response`"
+                        "and the rating question `response-rating` with values 1-7 and text question"
+                        " named `response-feedback`."
+                    ),
+                )
+
+            else:
+                # Update the existing dataset. If the fields and questions do not match, the dataset will be updated using the
+                # -updated flag in the name.
+                if self.dataset_name in [ds.name for ds in rg.FeedbackDataset.list()]:
+                    self.dataset = rg.FeedbackDataset.from_argilla(
+                        name=self.dataset_name,
+                        workspace=self.workspace_name,
+                    )
+
+                    self.is_new_dataset_created = False
+
+                    if number_of_retrievals > 0:
+                        required_context_fields = self._add_context_fields(
+                            number_of_retrievals
+                        )
+                        required_context_questions = self._add_context_questions(
+                            number_of_retrievals
+                        )
+                        existing_fields = [
+                            field.to_local() for field in self.dataset.fields
+                        ]
+                        existing_questions = [
+                            question.to_local() for question in self.dataset.questions
+                        ]
+                        # If the required fields and questions do not match with the existing ones, update the dataset and upload it again with "-updated" added to the name
+                        if not (
+                            all(
+                                element in existing_fields
+                                for element in required_context_fields
+                            )
+                            and all(
+                                element in existing_questions
+                                for element in required_context_questions
+                            )
+                        ):
+                            local_dataset = self.dataset.pull()
+
+                            fields_to_pop = []
+                            for index, field in enumerate(local_dataset.fields):
+                                if field.name.startswith("retrieved_document_"):
+                                    fields_to_pop.append(index)
+                                    fields_to_pop.sort(reverse=True)
+                            else:
+                                for index in fields_to_pop:
+                                    local_dataset.fields.pop(index)
+
+                            questions_to_pop = []
+                            for index, question in enumerate(local_dataset.questions):
+                                if question.name.startswith(
+                                    "rating_retrieved_document_"
+                                ):
+                                    questions_to_pop.append(index)
+                                    questions_to_pop.sort(reverse=True)
+                            else:
+                                for index in questions_to_pop:
+                                    local_dataset.questions.pop(index)
+
+                            for field in required_context_fields:
+                                local_dataset.fields.append(field)
+                            for question in required_context_questions:
+                                local_dataset.questions.append(question)
+                            self.dataset = local_dataset.push_to_argilla(
+                                self.dataset_name + "-updated"
+                            )
 
         except Exception as e:
             raise FileNotFoundError(
                 f"`FeedbackDataset` retrieval and creation both failed with exception `{e}`."
-                f" If the problem persists please report it to {self.ISSUES_URL} "
+                f" If the problem persists please report it to https://github.com/argilla-io/argilla/issues/ "
                 f"as an `integration` issue."
             ) from e
-        
-        supported_context_fields = [f"retrieved_document_{i+1}" for i in range(number_of_retrievals)]
-        supported_fields = ["prompt", "response", "time-details"] + supported_context_fields
+
+        supported_context_fields = [
+            f"retrieved_document_{i+1}" for i in range(number_of_retrievals)
+        ]
+        supported_fields = [
+            "prompt",
+            "response",
+            "time-details",
+        ] + supported_context_fields
         if supported_fields != [field.name for field in self.dataset.fields]:
             raise ValueError(
                 f"`FeedbackDataset` with name={self.dataset_name} in the workspace="
                 f"{self.workspace_name} had fields that are not supported yet for the"
                 f"`llama-index` integration. Supported fields are: {supported_fields},"
                 f" and the current `FeedbackDataset` fields are {[field.name for field in self.dataset.fields]}."
             )
-        
+
         self.events_data: Dict[str, List[CBEvent]] = defaultdict(list)
         self.event_map_id_to_name = {}
         self._ignore_components_in_tree = ["templating"]
         self.components_to_log = set()
         self.event_ids_traced = set()
 
-    def _add_context_fields(
-        self,
-        number_of_retrievals: int
-    ) -> List:
+    def _add_context_fields(self, number_of_retrievals: int) -> List:
         """Create the context fields to be added to the dataset."""
         context_fields = [
             rg.TextField(
                 name="retrieved_document_" + str(doc + 1),
                 title="Retrieved Document " + str(doc + 1),
                 use_markdown=True,
                 required=False,
             )
             for doc in range(number_of_retrievals)
         ]
         return context_fields
-    
-    def _add_context_questions(
-        self,
-        number_of_retrievals: int
-    ) -> List:
+
+    def _add_context_questions(self, number_of_retrievals: int) -> List:
         """Create the context questions to be added to the dataset."""
         rating_questions = [
             rg.RatingQuestion(
                 name="rating_retrieved_document_" + str(doc + 1),
-                title="Rate the relevance of the Retrieved Document " + str(doc + 1) + " (if present)",
+                title="Rate the relevance of the Retrieved Document "
+                + str(doc + 1)
+                + " (if present)",
                 values=list(range(1, 8)),
                 # After https://github.com/argilla-io/argilla/issues/4523 is fixed, we can use the description
-                description=None, #"Rate the relevance of the retrieved document."
+                description=None,  # "Rate the relevance of the retrieved document."
                 required=False,
             )
             for doc in range(number_of_retrievals)
         ]
         return rating_questions
 
-    def _create_root_and_other_nodes(
-        self, 
-        trace_map: Dict[str, List[str]]
-    ) -> None:
+    def _create_root_and_other_nodes(self, trace_map: Dict[str, List[str]]) -> None:
         """Create the root node and the other nodes in the tree."""
         self.root_node = self._get_event_name_by_id(trace_map["root"][0])
         self.event_ids_traced = set(trace_map.keys()) - {"root"}
         self.event_ids_traced.update(*trace_map.values())
         for id in self.event_ids_traced:
             self.components_to_log.add(self._get_event_name_by_id(id))
 
-    def _get_event_name_by_id(
-        self, 
-        event_id: str
-    ) -> str:
+    def _get_event_name_by_id(self, event_id: str) -> str:
         """Get the name of the event by its id."""
         return str(self.events_data[event_id][0].event_type).split(".")[1].lower()
-    
+
         # TODO: If we have a component more than once, properties currently don't account for those after the first one and get overwritten
+
     def _add_missing_metadata_properties(
-        self, 
-        dataset: rg.FeedbackDataset, 
+        self,
+        dataset: rg.FeedbackDataset,
     ) -> None:
         """Add missing metadata properties to the dataset."""
         required_metadata_properties = []
         for property in self.components_to_log:
             metadata_name = f"{property}_time"
             if property == self.root_node:
                 metadata_name = "total_time"
             required_metadata_properties.append(metadata_name)
 
-        existing_metadata_properties = [property.name for property in dataset.metadata_properties]
-        missing_metadata_properties = [property for property in required_metadata_properties if property not in existing_metadata_properties]
+        existing_metadata_properties = [
+            property.name for property in dataset.metadata_properties
+        ]
+        missing_metadata_properties = [
+            property
+            for property in required_metadata_properties
+            if property not in existing_metadata_properties
+        ]
 
         for property in missing_metadata_properties:
-            title= " ".join([word.capitalize() for word in property.split('_')])
+            title = " ".join([word.capitalize() for word in property.split("_")])
             if title == "Llm Time":
                 title = "LLM Time"
             dataset.add_metadata_property(
-                rg.FloatMetadataProperty(name=property, title=title))
+                rg.FloatMetadataProperty(name=property, title=title)
+            )
             if self.is_new_dataset_created == False:
                 warnings.warn(
                     (
                         f"The dataset given was missing some required metadata properties. "
                         f"Missing properties were {missing_metadata_properties}. "
                         f"Properties have been added to the dataset with "
                     ),
                 )
-                
+
     def _check_components_for_tree(
-        self,
-        tree_structure_dict: Dict[str, List[str]]
+        self, tree_structure_dict: Dict[str, List[str]]
     ) -> Dict[str, List[str]]:
         """
         Check whether the components in the tree are in the components to log.
-        Removes components that are not in the components to log so that they are not shown in the tree.  
+        Removes components that are not in the components to log so that they are not shown in the tree.
         """
         final_components_in_tree = self.components_to_log.copy()
         final_components_in_tree.add("root")
         for component in self._ignore_components_in_tree:
             if component in final_components_in_tree:
                 final_components_in_tree.remove(component)
         for key in list(tree_structure_dict.keys()):
             if key.strip("0") not in final_components_in_tree:
                 del tree_structure_dict[key]
         for key, value in tree_structure_dict.items():
             if isinstance(value, list):
-                tree_structure_dict[key] = [element for element in value if element.strip("0") in final_components_in_tree]
+                tree_structure_dict[key] = [
+                    element
+                    for element in value
+                    if element.strip("0") in final_components_in_tree
+                ]
         return tree_structure_dict
-                
+
     def _get_events_map_with_names(
-        self, 
-        events_data: Dict[str, List[CBEvent]],
-        trace_map: Dict[str, List[str]]
+        self, events_data: Dict[str, List[CBEvent]], trace_map: Dict[str, List[str]]
     ) -> Dict[str, List[str]]:
         """
         Returns a dictionary where trace_map is mapped with the event names instead of the event ids.
         Also returns a set of the event ids that were traced.
         """
         self.event_map_id_to_name = {}
         for event_id in self.event_ids_traced:
             event_name = str(events_data[event_id][0].event_type).split(".")[1].lower()
             while event_name in self.event_map_id_to_name.values():
-                event_name = event_name + "0" 
+                event_name = event_name + "0"
             self.event_map_id_to_name[event_id] = event_name
-        events_trace_map = {self.event_map_id_to_name.get(k, k): [self.event_map_id_to_name.get(v, v) for v in values] for k, values in trace_map.items()}
+        events_trace_map = {
+            self.event_map_id_to_name.get(k, k): [
+                self.event_map_id_to_name.get(v, v) for v in values
+            ]
+            for k, values in trace_map.items()
+        }
 
         return events_trace_map
-    
+
     def _extract_and_log_info(
-        self, 
-        events_data: Dict[str, List[CBEvent]],
-        trace_map: Dict[str, List[str]]
+        self, events_data: Dict[str, List[CBEvent]], trace_map: Dict[str, List[str]]
     ) -> None:
         """
         Main function that extracts the information from the events and logs it to Argilla.
         We currently log data if the root node is either "agent_step" or "query".
         Otherwise, we do not log anything.
         If we want to account for more root nodes, we just need to add them to the if statement.
         """
         events_trace_map = self._get_events_map_with_names(events_data, trace_map)
         root_node = trace_map["root"]
         data_to_log = {}
+
         if len(root_node) == 1:
+
             # Create logging data for the root node
             if self.root_node == "agent_step":
                 # Event start
                 event = events_data[root_node[0]][0]
                 data_to_log["query"] = event.payload.get(EventPayload.MESSAGES)[0]
                 query_start_time = event.time
                 # Event end
                 event = events_data[root_node[0]][1]
-                data_to_log["response"] = event.payload.get(EventPayload.RESPONSE).response
+                data_to_log["response"] = event.payload.get(
+                    EventPayload.RESPONSE
+                ).response
                 query_end_time = event.time
-                data_to_log["agent_step_time"] = _get_time_diff(query_start_time, query_end_time)
+                data_to_log["agent_step_time"] = _get_time_diff(
+                    query_start_time, query_end_time
+                )
 
             elif self.root_node == "query":
                 # Event start
                 event = events_data[root_node[0]][0]
                 data_to_log["query"] = event.payload.get(EventPayload.QUERY_STR)
                 query_start_time = event.time
                 # Event end
                 event = events_data[root_node[0]][1]
-                data_to_log["response"] = event.payload.get(EventPayload.RESPONSE).response
+                data_to_log["response"] = event.payload.get(
+                    EventPayload.RESPONSE
+                ).response
                 query_end_time = event.time
-                data_to_log["query_time"] = _get_time_diff(query_start_time, query_end_time)
-            
+                data_to_log["query_time"] = _get_time_diff(
+                    query_start_time, query_end_time
+                )
+
             else:
                 return
-            
+
             # Create logging data for the rest of the components
             self.event_ids_traced.remove(root_node[0])
-
             number_of_components_used = defaultdict(int)
             components_to_log_without_root_node = self.components_to_log.copy()
             components_to_log_without_root_node.remove(self.root_node)
             retrieval_metadata = {}
             for id in self.event_ids_traced:
                 event_name = self.event_map_id_to_name[id]
                 if event_name.endswith("0"):
@@ -432,184 +459,243 @@
                     event_name_reduced = event_name
 
                 for component in components_to_log_without_root_node:
                     if event_name_reduced == component:
                         data_to_log[f"{event_name}_time"] = _calc_time(events_data, id)
 
                 if event_name_reduced == "llm":
-                    data_to_log[f"{event_name}_system_prompt"] = events_data[id][0].payload.get(EventPayload.MESSAGES)[0].content
-                    data_to_log[f"{event_name}_model_name"] = events_data[id][0].payload.get(EventPayload.SERIALIZED)["model"]
+                    data_to_log[f"{event_name}_system_prompt"] = (
+                        events_data[id][0].payload.get(EventPayload.MESSAGES)[0].content
+                    )
+                    data_to_log[f"{event_name}_model_name"] = events_data[id][
+                        0
+                    ].payload.get(EventPayload.SERIALIZED)["model"]
 
                 retrieved_document_counter = 1
                 if event_name_reduced == "retrieve":
-                    for retrieval_node in events_data[id][1].payload.get(EventPayload.NODES):
+                    for retrieval_node in events_data[id][1].payload.get(
+                        EventPayload.NODES
+                    ):
                         retrieve_dict = retrieval_node.to_dict()
-                        retrieval_metadata[f"{event_name}_document_{retrieved_document_counter}_score"] = retrieval_node.score
-                        retrieval_metadata[f"{event_name}_document_{retrieved_document_counter}_filename"] = retrieve_dict["node"]["metadata"]["file_name"]
-                        retrieval_metadata[f"{event_name}_document_{retrieved_document_counter}_text"] = retrieve_dict["node"]["text"]
-                        retrieval_metadata[f"{event_name}_document_{retrieved_document_counter}_start_character"] = retrieve_dict["node"]["start_char_idx"]
-                        retrieval_metadata[f"{event_name}_document_{retrieved_document_counter}_end_character"] = retrieve_dict["node"]["end_char_idx"]
+                        retrieval_metadata[
+                            f"{event_name}_document_{retrieved_document_counter}_score"
+                        ] = retrieval_node.score
+                        retrieval_metadata[
+                            f"{event_name}_document_{retrieved_document_counter}_filename"
+                        ] = retrieve_dict["node"]["metadata"]["file_name"]
+                        retrieval_metadata[
+                            f"{event_name}_document_{retrieved_document_counter}_text"
+                        ] = retrieve_dict["node"]["text"]
+                        retrieval_metadata[
+                            f"{event_name}_document_{retrieved_document_counter}_start_character"
+                        ] = retrieve_dict["node"]["start_char_idx"]
+                        retrieval_metadata[
+                            f"{event_name}_document_{retrieved_document_counter}_end_character"
+                        ] = retrieve_dict["node"]["end_char_idx"]
                         retrieved_document_counter += 1
                         if retrieved_document_counter > self.number_of_retrievals:
                             break
 
             metadata_to_log = {}
 
             for keys in data_to_log.keys():
                 if keys == "query_time" or keys == "agent_step_time":
                     metadata_to_log["total_time"] = data_to_log[keys]
                 elif keys.endswith("_time"):
                     metadata_to_log[keys] = data_to_log[keys]
                 elif keys != "query" and keys != "response":
                     metadata_to_log[keys] = data_to_log[keys]
-                        
+
             if len(number_of_components_used) > 0:
                 for key, value in number_of_components_used.items():
                     metadata_to_log[f"number_of_{key}_used"] = value + 1
-            
+
             metadata_to_log.update(retrieval_metadata)
-            
+
             tree_structure = self._create_tree_structure(events_trace_map, data_to_log)
             tree = self._create_svg(tree_structure)
 
             fields = {
-                "prompt": data_to_log["query"], 
+                "prompt": data_to_log["query"],
                 "response": data_to_log["response"],
-                "time-details": tree
+                "time-details": tree,
             }
 
             if self.number_of_retrievals > 0:
                 for key, value in list(retrieval_metadata.items()):
                     if key.endswith("_text"):
-                        fields[f"retrieved_document_{key[-6]}"] = f"DOCUMENT SCORE: {retrieval_metadata[key[:-5]+'_score']}\n\n" + value
+                        fields[f"retrieved_document_{key[-6]}"] = (
+                            f"DOCUMENT SCORE: {retrieval_metadata[key[:-5]+'_score']}\n\n"
+                            + value
+                        )
                         del metadata_to_log[key]
 
             self.dataset.add_records(
                 records=[
-                    {
-                        "fields": fields,
-                        "metadata": metadata_to_log
-                    },
+                    {"fields": fields, "metadata": metadata_to_log},
                 ]
             )
-    
+
     def _create_tree_structure(
-        self,
-        events_trace_map: Dict[str, List[str]],
-        data_to_log: Dict[str, Any]
+        self, events_trace_map: Dict[str, List[str]], data_to_log: Dict[str, Any]
     ) -> List:
         """Create the tree data to be converted to an SVG."""
         events_trace_map = self._check_components_for_tree(events_trace_map)
         data = []
-        data.append((0, 0, self.root_node.strip("0").upper(), data_to_log[f"{self.root_node}_time"]))
+        data.append(
+            (
+                0,
+                0,
+                self.root_node.strip("0").upper(),
+                data_to_log[f"{self.root_node}_time"],
+            )
+        )
         current_row = 1
         for root_child in events_trace_map[self.root_node]:
-            data.append((current_row, 1, root_child.strip("0").upper(), data_to_log[f"{root_child}_time"]))
+            data.append(
+                (
+                    current_row,
+                    1,
+                    root_child.strip("0").upper(),
+                    data_to_log[f"{root_child}_time"],
+                )
+            )
             current_row += 1
             for child in events_trace_map[root_child]:
-                data.append((current_row, 2, child.strip("0").upper(), data_to_log[f"{child}_time"]))
+                data.append(
+                    (
+                        current_row,
+                        2,
+                        child.strip("0").upper(),
+                        data_to_log[f"{child}_time"],
+                    )
+                )
                 current_row += 1
         return data
-        
-    def _create_svg(
-        self, 
-        data: List
-    ) -> str:
+
+    def _create_svg(self, data: List) -> str:
+        """
+        Create an SVG file from the data.
+
+        Args:
+            data (List): The data to create the SVG file from.
+
+        Returns:
+            str: The SVG file.
+        """
+
         # changing only the box height changes all other values as well
         # others can be adjusted individually if needed
         box_height = 47
         box_width = box_height * 8.65
         row_constant = box_height + 7
         indent_constant = 40
         font_size_node_name = box_height * 0.4188
         font_size_time = font_size_node_name - 4
         text_centering = box_height * 0.6341
         node_name_indent = box_height * 0.35
         time_indent = box_height * 7.15
-        
+
         body = ""
         for each in data:
             row, indent, node_name, node_time = each
             body_raw = f"""
 <g transform="translate({indent*indent_constant}, {row*row_constant})">
 <rect x=".5" y=".5" width="{box_width}" height="{box_height}" rx="8.49" ry="8.49" style="fill: #24272e; stroke: #afdfe5; stroke-miterlimit: 10;"/>
 <text transform="translate({node_name_indent} {text_centering})" style="fill: #fff; font-size: {font_size_node_name}px;"><tspan x="0" y="0">{node_name}</tspan></text>
 <text transform="translate({time_indent} {text_centering})" style="fill: #b7d989; font-size: {font_size_time}px; font-style: italic;"><tspan x="0" y="0">{node_time}</tspan></text>
 </g>
             """
             body += body_raw
-            base = base =f"""
+            base = (
+                base
+            ) = f"""
 <?xml version="1.0" encoding="UTF-8"?>
 <svg id="Layer_1" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 750 {len(data)*row_constant}">
 {body}
 </svg>
             """
             base = base.strip()
         return base
 
-    def start_trace(
-        self, 
-        trace_id: Optional[str] = None
-    ) -> None:
-        """Launch a trace."""
+    # The four methods required by the abstrac class BaseCallbackHandler.
+    # These methods are the one being executed on the different events, by the llama-index
+    # BaseCallbackHandler class.
+
+    def start_trace(self, trace_id: Optional[str] = None) -> None:
+        """
+        Start tracing events.
+
+        Args:
+            trace_id (str, optional): The trace_id to start tracing.
+        """
+
         self._trace_map = defaultdict(list)
         self._cur_trace_id = trace_id
         self._start_time = datetime.now()
+
+        # Clear the events and the components prior to running the query.
+        # They are usually events related to creating the docs and indexing.
         self.events_data.clear()
         self.components_to_log.clear()
 
     def end_trace(
         self,
         trace_id: Optional[str] = None,
         trace_map: Optional[Dict[str, List[str]]] = None,
     ) -> None:
-        """End a trace."""
+        """
+        End tracing events.
+
+        Args:
+            trace_id (str, optional): The trace_id to end tracing.
+            trace_map (Dict[str, List[str]], optional): The trace_map to end. This map has been obtained from the parent class.
+        """
+
         self._trace_map = trace_map or defaultdict(list)
         self._end_time = datetime.now()
         self._create_root_and_other_nodes(trace_map)
         self._add_missing_metadata_properties(self.dataset)
         self._extract_and_log_info(self.events_data, trace_map)
 
     def on_event_start(
         self,
         event_type: CBEventType,
         payload: Optional[Dict[str, Any]] = None,
         event_id: Optional[str] = None,
-        parent_id: Optional[str] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Run handlers when an event starts."""
+        parent_id: str = None,
+    ) -> str:
+        """
+        Store event start data by event type. Executed at the start of an event.
+
+        Args:
+            event_type (CBEventType): The event type to store.
+            payload (Dict[str, Any], optional): The payload to store.
+            event_id (str, optional): The event id to store.
+            parent_id (str, optional): The parent id to store.
+
+        Returns:
+            str: The event id.
+        """
+
         event = CBEvent(event_type, payload=payload, id_=event_id)
         self.events_data[event_id].append(event)
 
+        return event.id_
+
     def on_event_end(
         self,
         event_type: CBEventType,
         payload: Optional[Dict[str, Any]] = None,
-        event_id: Optional[str] = None,
-        **kwargs: Any,
+        event_id: str = None,
     ) -> None:
-        """Run handlers when an event ends."""
+        """
+        Store event end data by event type. Executed at the end of an event.
+
+        Args:
+            event_type (CBEventType): The event type to store.
+            payload (Dict[str, Any], optional): The payload to store.
+            event_id (str, optional): The event id to store.
+        """
+
         event = CBEvent(event_type, payload=payload, id_=event_id)
         self.events_data[event_id].append(event)
-
-def _get_time_diff(
-    event_1_time_str: str, 
-    event_2_time_str: str
-) -> float:
-    """Get the time difference between two events."""
-    time_format = "%m/%d/%Y, %H:%M:%S.%f"
-
-    event_1_time = datetime.strptime(event_1_time_str, time_format)
-    event_2_time = datetime.strptime(event_2_time_str, time_format)
-
-    return round((event_2_time - event_1_time).total_seconds(), 4)
-
-def _calc_time(
-    events_data: Dict[str, List[CBEvent]], 
-    id: str
-) -> float:
-    """Calculate the time difference between the start and end of an event using the events_data."""
-    start_time = events_data[id][0].time
-    end_time = events_data[id][1].time
-    return _get_time_diff(start_time, end_time)
-
```

### Comparing `argilla_llama_index-0.0.1a0/tests/test_llama_index_callback.py` & `argilla_llama_index-1.0.0/tests/test_llama_index_callback.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+from argilla_llama_index.helpers import _calc_time, _get_time_diff
+
 import unittest
 from unittest.mock import patch, MagicMock
-from argilla_llama_index import ArgillaCallbackHandler, _get_time_diff, _calc_time # TODO: correct import
+from argilla_llama_index import ArgillaCallbackHandler
+
 
 class TestArgillaCallbackHandler(unittest.TestCase):
     def setUp(self):
         self.dataset_name = "test_dataset_llama_index"
-        self.workspace_name = "argilla"
+        self.workspace_name = "admin"
         self.api_url = "http://localhost:6900"
-        self.api_key = "argilla.apikey"
+        self.api_key = "admin.apikey"
 
         self.handler = ArgillaCallbackHandler(
             dataset_name=self.dataset_name,
             workspace_name=self.workspace_name,
             api_url=self.api_url,
             api_key=self.api_key,
         )
 
         self.events_data = MagicMock()
         self.data_to_log = MagicMock()
         self.components_to_log = MagicMock()
         self._ignore_components_in_tree = MagicMock()
         self.trace_map = MagicMock()
-       
+
         self.tree_structure_dict = {
             "root": ["query"],
             "query": ["retrieve", "synthesize"],
             "synthesize": ["llm", "grandchild1"],
         }
 
     def test_init(self):
@@ -52,56 +55,45 @@
             ArgillaCallbackHandler(
                 dataset_name=self.dataset_name,
                 workspace_name=self.workspace_name,
                 api_url=self.api_url,
                 api_key=self.api_key,
             )
 
-    def test_add_missing_metadata_properties(self):
-        dataset = self.handler.dataset
-        is_new_dataset_created = True
-        self.handler._add_missing_metadata_properties(dataset, is_new_dataset_created)
-        self.assertEqual(len(dataset.metadata_properties), 6)
-
     def test_check_components_for_tree(self):
         self.handler._check_components_for_tree(self.tree_structure_dict)
 
-    def test_create_tree(self):
-
-        tree = self.handler._create_tree(self.tree_structure_dict, self.data_to_log)
-        self.assertIsInstance(tree, str)
-
     def test_get_events_map_with_names(self):
 
-        trace_map = {
-            "query": ["retrieve"],
-            "llm": []
-        }
-        events_map = self.handler._get_events_map_with_names(self.events_data, trace_map)
-        self.assertIsInstance(events_map, tuple)
+        trace_map = {"query": ["retrieve"], "llm": []}
+        events_map = self.handler._get_events_map_with_names(
+            self.events_data, trace_map
+        )
+        self.assertIsInstance(events_map, dict)
         self.assertEqual(len(events_map), 2)
 
     def test_extract_and_log_info(self):
 
-        tree_structure_dict = self.handler._check_components_for_tree(self.tree_structure_dict)
+        tree_structure_dict = self.handler._check_components_for_tree(
+            self.tree_structure_dict
+        )
         self.handler._extract_and_log_info(self.events_data, tree_structure_dict)
 
     def test_start_trace(self):
         self.handler.start_trace()
 
     # TODO: Create a test for end_trace
 
     def test_on_event_start(self):
         event_type = "event1"
         payload = {}
         event_id = "123"
         parent_id = "456"
         self.handler.on_event_start(event_type, payload, event_id, parent_id)
 
-
     def test_on_event_end(self):
         event_type = "event1"
         payload = {}
         event_id = "123"
         self.handler.on_event_end(event_type, payload, event_id)
 
     def test_get_time_diff(self):
@@ -109,15 +101,19 @@
         event_2_time_str = "01/11/2024, 17:02:07.328523"
         time_diff = _get_time_diff(event_1_time_str, event_2_time_str)
         self.assertIsInstance(time_diff, float)
 
     def test_calc_time(self):
 
         id = "event1"
-        self.events_data.__getitem__().__getitem__().time = "01/11/2024, 17:01:04.328656"
-        self.events_data.__getitem__().__getitem__().time = "01/11/2024, 17:02:07.328523"
+        self.events_data.__getitem__().__getitem__().time = (
+            "01/11/2024, 17:01:04.328656"
+        )
+        self.events_data.__getitem__().__getitem__().time = (
+            "01/11/2024, 17:02:07.328523"
+        )
         time = _calc_time(self.events_data, id)
         self.assertIsInstance(time, float)
 
+
 if __name__ == "__main__":
     unittest.main()
-
```

### Comparing `argilla_llama_index-0.0.1a0/.gitignore` & `argilla_llama_index-1.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
+.DS_Store
+
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `argilla_llama_index-0.0.1a0/LICENSE` & `argilla_llama_index-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-0.0.1a0/LICENSE_HEADER` & `argilla_llama_index-1.0.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-0.0.1a0/README.md` & `argilla_llama_index-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,84 @@
-# Argilla-Llama-Index
+<div align="center">
+  <h1>✨🦙 Argilla's LlamaIndex Integration</h1>
+  <p><em> Argilla integration into the LlamaIndex workflow</em></p>
+</div>
 
-Argilla is an open-source platform for data-centric LLM development. Integrates human and model feedback loops for continuous LLM refinement and oversight.
+> [!TIP]
+> To discuss, get support, or give feedback [join Argilla's Slack Community](https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g) and you will be able to engage with our amazing community and also with the core developers of `argilla` and `distilabel`.
 
-With Argilla's Python SDK and adaptable UI, you can create human and model-in-the-loop workflows for:
 
-- Supervised fine-tuning
-- Preference tuning (RLHF, DPO, RLAIF, and more)
-- Small, specialized NLP models
-- Scalable evaluation.
+This integration allows the user to include the feedback loop that Argilla offers into the LlamaIndex ecosystem. It's based on a callback handler to be run within the LlamaIndex workflow. 
+
+Don't hesitate to check out both [LlamaIndex](https://github.com/run-llama/llama_index) and [Argilla](https://github.com/argilla-io/argilla)
 
 ## Getting Started
 
 You first need to install argilla and argilla-llama-index as follows:
 
 ```bash
 pip install argilla-llama-index
 ```
 
-You will need to an Argilla Server running to monitor the LLM. You can either install the server locally or have it on HuggingFace Spaces. For a complete guide on how to install and initialize the server, you can refer to the [Quickstart Guide](https://docs.argilla.io/en/latest/getting_started/quickstart_installation.html). 
+You will need to an Argilla Server running to monitor the LLM. You can either install the server locally or have it on HuggingFace Spaces. For a complete guide on how to install and initialize the server, you can refer to the [Quickstart Guide](https://docs.argilla.io/en/latest/getting_started/quickstart_installation.html).
 
 ## Usage
 
 It requires just a simple step to log your data into Argilla within your LlamaIndex workflow. We just need to call the handler before starting production with your LLM.
 
 We will use GPT3.5 from OpenAI as our LLM. For this, you will need a valid API key from OpenAI. You can have more info and get one via [this link](https://openai.com/blog/openai-api).
 
-After you get your API key, let us import the key.
+After you get your API key, the easiest way to import it is through an environment variable, or via *getpass()*.
 
 ```python
 import os
 from getpass import getpass
 
 openai_api_key = os.getenv("OPENAI_API_KEY", None) or getpass("Enter OpenAI API key:")
 ```
 
-Let us make the necessary imports.
+Let's now write all the necessary imports
 
 ```python
-from argilla_llama_index import ArgillaCallbackHandler
-from llama_index import VectorStoreIndex, ServiceContext, SimpleDirectoryReader
-from llama_index.llms import OpenAI
-from llama_index import set_global_handler
+from llama_index.core import VectorStoreIndex, ServiceContext, SimpleDirectoryReader, set_global_handler
+from llama_index.llms.openai import OpenAI
 ```
 
-What we need to do is to set Argilla as the global handler as below. Within the handler, we need to provide the dataset name that we will use. If the dataset does not exist, it will be created with the given name. You can also set the API KEY, API URL, and the Workspace name. If you do not provide these, the default values will be used.
+What we need to do is to set Argilla as the global handler as below. Within the handler, we need to provide the dataset name that we will use. If the dataset does not exist, it will be created with the given name. You can also set the API KEY, API URL, and the Workspace name. You can learn more about the variables that controls Argilla initialization [here](https://docs.argilla.io/en/latest/getting_started/installation/configurations/workspace_management.html)
+
+> [!TIP]
+> Remember that the default Argilla workspace name is `admin`. If you want to use a custom Workspace, you'll need to create it and grant access to the desired users. The link above also explains how to do that.
+
 
 ```python
 set_global_handler("argilla", dataset_name="query_model")
 ```
 
-Let us create the LLM.
+Let's now create the llm instance, using GPT-3.5 from OpenAI.
 
 ```python
-llm = OpenAI(model="gpt-3.5-turbo", temperature=0.8)
+llm = OpenAI(model="gpt-3.5-turbo", temperature=0.8, openai_api_key=openai_api_key)
 ```
 
-With the code snippet below, you can create a basic workflow with Llama Index. You will also need a txt file as the data source within a folder named "data". For a sample data file and more info regarding the use of Llama Index, you can refer to the [Llama Index documentation](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html).
-
+With the code snippet below, you can create a basic workflow with LlamaIndex. You will also need a txt file as the data source within a folder named "data". For a sample data file and more info regarding the use of Llama Index, you can refer to the [Llama Index documentation](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html).
 
 ```python
 service_context = ServiceContext.from_defaults(llm=llm)
 docs = SimpleDirectoryReader("data").load_data()
 index = VectorStoreIndex.from_documents(docs, service_context=service_context)
 query_engine = index.as_query_engine()
 ```
 
-Now, let us run the `query_engine` to have a response from the model. 
+Now, let's run the `query_engine` to have a response from the model.
 
 ```python
 response = query_engine.query("What did the author do growing up?")
+response
 ```
 
 ```bash
 The author worked on two main things outside of school before college: writing and programming. They wrote short stories and tried writing programs on an IBM 1401. They later got a microcomputer, built it themselves, and started programming on it.
 ```
 
-The prompt given and the response obtained will be logged in to Argilla server. You can check the data on the Argilla UI.
-
-![Argilla Dataset](docs/argilla-ui-dataset.png)
-
-And we also logged the metadata properties into Argilla. You can check them via the Filters on the upper left and filter your data according to any of them.
-
-![Argilla Dataset](docs/argilla-ui-dataset-2.png)
-
-
-
+The prompt given and the response obtained will be logged in to Argilla server. You can check the data on Argilla's UI:
 
+![Argilla Dataset](docs/assets/argilla-ui-dataset.png)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `argilla_llama_index-0.0.1a0/pyproject.toml` & `argilla_llama_index-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "argilla >= 1.18.0",
-    "llama-index >= 0.9.32",
+    "argilla >= 1.22.0",
+    "llama-index >= 0.10.0",
     "packaging >= 23.2",
     "typing-extensions >= 4.3.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black == 23.10.0", "ruff == 0.1.0", "pre-commit >= 3.5.0"]
```

### Comparing `argilla_llama_index-0.0.1a0/PKG-INFO` & `argilla_llama_index-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: argilla-llama-index
-Version: 0.0.1a0
+Version: 1.0.0
 Summary: Argilla-Llama Index Integration
 Project-URL: Documentation, https://github.com/argilla-io/argilla-llama-index
 Project-URL: Issues, https://github.com/argilla-io/argilla-llama-index/issues
 Project-URL: Source, https://github.com/argilla-io/argilla-llama-index
 Author-email: Argilla <admin@argilla.io>
 License-Expression: MIT
 License-File: LICENSE
@@ -12,107 +12,103 @@
 Keywords: annotation,llm,monitoring
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: argilla>=1.18.0
-Requires-Dist: llama-index>=0.9.32
+Requires-Dist: argilla>=1.22.0
+Requires-Dist: llama-index>=0.10.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: typing-extensions>=4.3.0
 Provides-Extra: dev
 Requires-Dist: black==23.10.0; extra == 'dev'
 Requires-Dist: pre-commit>=3.5.0; extra == 'dev'
 Requires-Dist: ruff==0.1.0; extra == 'dev'
 Provides-Extra: tests
 Requires-Dist: pytest>=7.4.0; extra == 'tests'
 Description-Content-Type: text/markdown
 
-# Argilla-Llama-Index
+<div align="center">
+  <h1>✨🦙 Argilla's LlamaIndex Integration</h1>
+  <p><em> Argilla integration into the LlamaIndex workflow</em></p>
+</div>
 
-Argilla is an open-source platform for data-centric LLM development. Integrates human and model feedback loops for continuous LLM refinement and oversight.
+> [!TIP]
+> To discuss, get support, or give feedback [join Argilla's Slack Community](https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g) and you will be able to engage with our amazing community and also with the core developers of `argilla` and `distilabel`.
 
-With Argilla's Python SDK and adaptable UI, you can create human and model-in-the-loop workflows for:
 
-- Supervised fine-tuning
-- Preference tuning (RLHF, DPO, RLAIF, and more)
-- Small, specialized NLP models
-- Scalable evaluation.
+This integration allows the user to include the feedback loop that Argilla offers into the LlamaIndex ecosystem. It's based on a callback handler to be run within the LlamaIndex workflow. 
+
+Don't hesitate to check out both [LlamaIndex](https://github.com/run-llama/llama_index) and [Argilla](https://github.com/argilla-io/argilla)
 
 ## Getting Started
 
 You first need to install argilla and argilla-llama-index as follows:
 
 ```bash
 pip install argilla-llama-index
 ```
 
-You will need to an Argilla Server running to monitor the LLM. You can either install the server locally or have it on HuggingFace Spaces. For a complete guide on how to install and initialize the server, you can refer to the [Quickstart Guide](https://docs.argilla.io/en/latest/getting_started/quickstart_installation.html). 
+You will need to an Argilla Server running to monitor the LLM. You can either install the server locally or have it on HuggingFace Spaces. For a complete guide on how to install and initialize the server, you can refer to the [Quickstart Guide](https://docs.argilla.io/en/latest/getting_started/quickstart_installation.html).
 
 ## Usage
 
 It requires just a simple step to log your data into Argilla within your LlamaIndex workflow. We just need to call the handler before starting production with your LLM.
 
 We will use GPT3.5 from OpenAI as our LLM. For this, you will need a valid API key from OpenAI. You can have more info and get one via [this link](https://openai.com/blog/openai-api).
 
-After you get your API key, let us import the key.
+After you get your API key, the easiest way to import it is through an environment variable, or via *getpass()*.
 
 ```python
 import os
 from getpass import getpass
 
 openai_api_key = os.getenv("OPENAI_API_KEY", None) or getpass("Enter OpenAI API key:")
 ```
 
-Let us make the necessary imports.
+Let's now write all the necessary imports
 
 ```python
-from argilla_llama_index import ArgillaCallbackHandler
-from llama_index import VectorStoreIndex, ServiceContext, SimpleDirectoryReader
-from llama_index.llms import OpenAI
-from llama_index import set_global_handler
+from llama_index.core import VectorStoreIndex, ServiceContext, SimpleDirectoryReader, set_global_handler
+from llama_index.llms.openai import OpenAI
 ```
 
-What we need to do is to set Argilla as the global handler as below. Within the handler, we need to provide the dataset name that we will use. If the dataset does not exist, it will be created with the given name. You can also set the API KEY, API URL, and the Workspace name. If you do not provide these, the default values will be used.
+What we need to do is to set Argilla as the global handler as below. Within the handler, we need to provide the dataset name that we will use. If the dataset does not exist, it will be created with the given name. You can also set the API KEY, API URL, and the Workspace name. You can learn more about the variables that controls Argilla initialization [here](https://docs.argilla.io/en/latest/getting_started/installation/configurations/workspace_management.html)
+
+> [!TIP]
+> Remember that the default Argilla workspace name is `admin`. If you want to use a custom Workspace, you'll need to create it and grant access to the desired users. The link above also explains how to do that.
+
 
 ```python
 set_global_handler("argilla", dataset_name="query_model")
 ```
 
-Let us create the LLM.
+Let's now create the llm instance, using GPT-3.5 from OpenAI.
 
 ```python
-llm = OpenAI(model="gpt-3.5-turbo", temperature=0.8)
+llm = OpenAI(model="gpt-3.5-turbo", temperature=0.8, openai_api_key=openai_api_key)
 ```
 
-With the code snippet below, you can create a basic workflow with Llama Index. You will also need a txt file as the data source within a folder named "data". For a sample data file and more info regarding the use of Llama Index, you can refer to the [Llama Index documentation](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html).
-
+With the code snippet below, you can create a basic workflow with LlamaIndex. You will also need a txt file as the data source within a folder named "data". For a sample data file and more info regarding the use of Llama Index, you can refer to the [Llama Index documentation](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html).
 
 ```python
 service_context = ServiceContext.from_defaults(llm=llm)
 docs = SimpleDirectoryReader("data").load_data()
 index = VectorStoreIndex.from_documents(docs, service_context=service_context)
 query_engine = index.as_query_engine()
 ```
 
-Now, let us run the `query_engine` to have a response from the model. 
+Now, let's run the `query_engine` to have a response from the model.
 
 ```python
 response = query_engine.query("What did the author do growing up?")
+response
 ```
 
 ```bash
 The author worked on two main things outside of school before college: writing and programming. They wrote short stories and tried writing programs on an IBM 1401. They later got a microcomputer, built it themselves, and started programming on it.
 ```
 
-The prompt given and the response obtained will be logged in to Argilla server. You can check the data on the Argilla UI.
-
-![Argilla Dataset](docs/argilla-ui-dataset.png)
-
-And we also logged the metadata properties into Argilla. You can check them via the Filters on the upper left and filter your data according to any of them.
-
-![Argilla Dataset](docs/argilla-ui-dataset-2.png)
-
-
-
+The prompt given and the response obtained will be logged in to Argilla server. You can check the data on Argilla's UI:
 
+![Argilla Dataset](docs/assets/argilla-ui-dataset.png)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

