# Comparing `tmp/llmsmith-0.3.0.tar.gz` & `tmp/llmsmith-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.3.0.tar", max compression
+gzip compressed data, was "llmsmith-0.4.0.tar", max compression
```

## Comparing `llmsmith-0.3.0.tar` & `llmsmith-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.3.0/LICENSE
--rw-r--r--   0        0        0     1506 2024-04-30 06:58:37.514663 llmsmith-0.3.0/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.3.0/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.3.0/llmsmith/agent/__init__.py
--rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.3.0/llmsmith/agent/errors.py
--rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.3.0/llmsmith/agent/function/__init__.py
--rw-r--r--   0        0        0     5934 2024-04-29 11:21:40.340274 llmsmith-0.3.0/llmsmith/agent/function/gemini.py
--rw-r--r--   0        0        0     8897 2024-04-30 06:33:06.377475 llmsmith-0.3.0/llmsmith/agent/function/openai.py
--rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.3.0/llmsmith/agent/function/options/__init__.py
--rw-r--r--   0        0        0     1996 2024-04-30 04:53:53.672366 llmsmith-0.3.0/llmsmith/agent/function/options/openai.py
--rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.3.0/llmsmith/agent/tool/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-18 12:17:09.379744 llmsmith-0.3.0/llmsmith/agent/tool/gemini.py
--rw-r--r--   0        0        0     2001 2024-04-29 11:21:40.340139 llmsmith-0.3.0/llmsmith/agent/tool/openai.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.3.0/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.3.0/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.3.0/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.3.0/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.3.0/llmsmith/task/base.py
--rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.3.0/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.3.0/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.3.0/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0      147 2024-04-09 10:26:53.708807 llmsmith-0.3.0/llmsmith/task/retrieval/vector/base.py
--rw-r--r--   0        0        0     3667 2024-04-10 05:44:39.948855 llmsmith-0.3.0/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/__init__.py
--rw-r--r--   0        0        0      906 2024-04-10 13:01:55.980002 llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/chromadb.py
--rw-r--r--   0        0        0     1325 2024-04-10 05:42:08.573365 llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/qdrant.py
--rw-r--r--   0        0        0     4316 2024-04-11 04:01:18.457684 llmsmith-0.3.0/llmsmith/task/retrieval/vector/qdrant.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.3.0/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.3.0/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.3.0/llmsmith/task/textgen/errors.py
--rw-r--r--   0        0        0     7108 2024-04-29 11:21:40.339852 llmsmith-0.3.0/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     6447 2024-04-29 11:21:40.339843 llmsmith-0.3.0/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.3.0/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.3.0/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     1346 2024-04-18 07:13:19.756541 llmsmith-0.3.0/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     1890 2024-04-22 08:24:34.750821 llmsmith-0.3.0/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     1845 2024-04-30 10:42:49.875910 llmsmith-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 llmsmith-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1506 2024-04-30 06:58:37.514663 llmsmith-0.4.0/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.4.0/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.4.0/llmsmith/agent/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.4.0/llmsmith/agent/errors.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.4.0/llmsmith/agent/function/__init__.py
+-rw-r--r--   0        0        0     5934 2024-04-29 11:21:40.340274 llmsmith-0.4.0/llmsmith/agent/function/gemini.py
+-rw-r--r--   0        0        0     8897 2024-04-30 06:33:06.377475 llmsmith-0.4.0/llmsmith/agent/function/openai.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.4.0/llmsmith/agent/function/options/__init__.py
+-rw-r--r--   0        0        0     1996 2024-04-30 04:53:53.672366 llmsmith-0.4.0/llmsmith/agent/function/options/openai.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.4.0/llmsmith/agent/tool/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-18 12:17:09.379744 llmsmith-0.4.0/llmsmith/agent/tool/gemini.py
+-rw-r--r--   0        0        0     2001 2024-04-29 11:21:40.340139 llmsmith-0.4.0/llmsmith/agent/tool/openai.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.4.0/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.4.0/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.4.0/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-04-30 12:02:50.437340 llmsmith-0.4.0/llmsmith/reranker/__init__.py
+-rw-r--r--   0        0        0      575 2024-05-02 04:19:45.995736 llmsmith-0.4.0/llmsmith/reranker/base.py
+-rw-r--r--   0        0        0     2848 2024-05-02 05:39:34.864251 llmsmith-0.4.0/llmsmith/reranker/cohere.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:46:41.851482 llmsmith-0.4.0/llmsmith/reranker/options/__init__.py
+-rw-r--r--   0        0        0     1088 2024-05-02 04:19:45.995262 llmsmith-0.4.0/llmsmith/reranker/options/cohere.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.4.0/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.4.0/llmsmith/task/base.py
+-rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.4.0/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.4.0/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.4.0/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-01 10:16:21.291906 llmsmith-0.4.0/llmsmith/task/retrieval/vector/base.py
+-rw-r--r--   0        0        0     3724 2024-05-01 10:16:21.291224 llmsmith-0.4.0/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/__init__.py
+-rw-r--r--   0        0        0      906 2024-04-10 13:01:55.980002 llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/chromadb.py
+-rw-r--r--   0        0        0     1325 2024-04-10 05:42:08.573365 llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/qdrant.py
+-rw-r--r--   0        0        0     4304 2024-05-01 10:31:04.487709 llmsmith-0.4.0/llmsmith/task/retrieval/vector/qdrant.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.4.0/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.4.0/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.4.0/llmsmith/task/textgen/errors.py
+-rw-r--r--   0        0        0     7108 2024-04-29 11:21:40.339852 llmsmith-0.4.0/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     6447 2024-04-29 11:21:40.339843 llmsmith-0.4.0/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.4.0/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.4.0/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     1346 2024-04-18 07:13:19.756541 llmsmith-0.4.0/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     1890 2024-04-22 08:24:34.750821 llmsmith-0.4.0/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     1922 2024-05-03 11:25:28.691081 llmsmith-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 llmsmith-0.4.0/PKG-INFO
```

### Comparing `llmsmith-0.3.0/LICENSE` & `llmsmith-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/README.md` & `llmsmith-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/agent/function/gemini.py` & `llmsmith-0.4.0/llmsmith/agent/function/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/agent/function/openai.py` & `llmsmith-0.4.0/llmsmith/agent/function/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/agent/function/options/openai.py` & `llmsmith-0.4.0/llmsmith/agent/function/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/agent/tool/gemini.py` & `llmsmith-0.4.0/llmsmith/agent/tool/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/agent/tool/openai.py` & `llmsmith-0.4.0/llmsmith/agent/tool/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/job/base.py` & `llmsmith-0.4.0/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/job/job.py` & `llmsmith-0.4.0/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/base.py` & `llmsmith-0.4.0/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/retrieval/vector/chromadb.py` & `llmsmith-0.4.0/llmsmith/task/retrieval/vector/chromadb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
-from typing import Callable
+from typing import Callable, List
 
+from llmsmith.reranker.base import Reranker
 from llmsmith.task.base import Task
 from llmsmith.task.models import TaskInput, TaskOutput
-from llmsmith.task.retrieval.vector.base import EmbeddingFunc
+from llmsmith.task.retrieval.vector.base import EmbeddingFunc, default_doc_processor
 from llmsmith.task.retrieval.vector.options.chromadb import (
     ChromaDBQueryOptions,
     _query_options_dict,
 )
 
 
 try:
@@ -20,69 +21,51 @@
 
 log = logging.getLogger(__name__)
 
 # Default options for querying a Qdrant collection.
 default_options: ChromaDBQueryOptions = ChromaDBQueryOptions(n_results=10)
 
 
-def default_doc_processor(res: QueryResult) -> str:
-    """
-    Formats the retrieved chromadb documents into below format.
-
-    ``
-    [0] document-0-content
-
-    [1] document-1-content
-
-    ...
-
-    [n] document-n-content
-    ``
-    """
-
-    processed_docs = []
-    for idx, doc in enumerate(res["documents"][0]):
-        processed_docs.append(f"[{idx}] {doc}")
-
-    return "\n\n".join(processed_docs)
-
-
 class ChromaDBRetriever(Task[str, str]):
     """
     Task for retrieving documents from a collection in ChromaDB.
 
     :param name: The name of the task.
     :type name: str
     :param collection: The collection to retrieve documents from.
     :type collection: :class:`chromadb.Collection`
     :param embedding_func: Embedding function
     :type embedding_func: :class:`llmsmith.task.retrieval.vector.base.EmbeddingFunc`
-    :param doc_processing_func: The function to process the query result, defaults to `llmsmith.task.retrieval.vector.chromadb.default_doc_processor`.
-    :type doc_processing_func: Callable[[QueryResult], str], optional
+    :param doc_processing_func: The function to process the query result, defaults to `llmsmith.task.retrieval.vector.base.default_doc_processor`.
+    :type doc_processing_func: Callable[[List[str]], str], optional
     :param query_options: A dictionary of options to pass to the ChromaDB collection client for querying.
     :type query_options: :class:`llmsmith.task.retrieval.vector.options.chromadb.ChromaDBQueryOptions`, optional
+    :param reranker: Rerank the documents based on the query used to retrieve the documents.
+    :type reranker: :class:`llmsmith.reranker.base.Reranker`, optional
     """
 
     def __init__(
         self,
         name: str,
         collection: Collection,
         embedding_func: EmbeddingFunc,
-        doc_processing_func: Callable[[QueryResult], str] = default_doc_processor,
+        doc_processing_func: Callable[[List[str]], str] = default_doc_processor,
         query_options: ChromaDBQueryOptions = default_options,
+        reranker: Reranker = None,
     ) -> None:
         super().__init__(name)
 
         if not embedding_func:
             raise ValueError("Embedding function ('embedding_func') is required")
 
         self.collection = collection
         self.embedding_func = embedding_func
         self.doc_processing_func = doc_processing_func
         self.query_options = query_options
+        self._reranker = reranker
 
     async def execute(self, task_input: TaskInput[str]) -> TaskOutput[str]:
         """
         Executes the task of retrieving documents from the chromadb collection.
 
         :param task_input: The input for the task.
         :type task_input: :class:`llmsmith.task.models.TaskInput[str]`
@@ -99,9 +82,13 @@
 
         res: QueryResult = self.collection.query(
             query_embeddings=embeddings,
             include=["metadatas", "documents", "distances"],
             **query_options,
         )
 
-        processed_res: str = self.doc_processing_func(res)
+        docs = [doc for doc in res["documents"][0]]
+        if self._reranker:
+            docs = await self._reranker.rerank(query=task_input.content, docs=docs)
+
+        processed_res: str = self.doc_processing_func(docs)
         return TaskOutput(content=processed_res, raw_output=res)
```

### Comparing `llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/chromadb.py` & `llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/qdrant.py` & `llmsmith-0.4.0/llmsmith/task/retrieval/vector/options/qdrant.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/retrieval/vector/qdrant.py` & `llmsmith-0.4.0/llmsmith/task/retrieval/vector/qdrant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
-from typing import Callable, List, Union
+from typing import Callable, List
 
+from llmsmith.reranker.base import Reranker
 from llmsmith.task.base import Task
 from llmsmith.task.models import TaskInput, TaskOutput
-from llmsmith.task.retrieval.vector.base import EmbeddingFunc
+from llmsmith.task.retrieval.vector.base import EmbeddingFunc, default_doc_processor
 from llmsmith.task.retrieval.vector.options.qdrant import (
     QdrantQueryOptions,
     _query_options_dict,
 )
 
-
 try:
     from qdrant_client import AsyncQdrantClient
     from qdrant_client.conversions.common_types import ScoredPoint
 except ImportError:
     raise ImportError(
         "The 'qdrant-client' library is required to use QdrantRetriever. You can install it with `pip install \"llmsmith[qdrant]\"`"
     )
@@ -21,82 +21,61 @@
 
 log = logging.getLogger(__name__)
 
 # Default options for querying a Qdrant collection.
 default_options: QdrantQueryOptions = QdrantQueryOptions(limit=10, with_vectors=False)
 
 
-def default_doc_processor_func(field: str):
-    def default_doc_processor(res: List[ScoredPoint]) -> str:
-        """
-        Formats the retrieved qdrant documents into below format.
-
-        ``
-        [0] document-0-content
-
-        [1] document-1-content
-
-        ...
-
-        [n] document-n-content
-        ``
-        """
-
-        processed_docs = []
-        for idx, doc in enumerate(res):
-            processed_docs.append(f"[{idx}] {doc.payload.get(field, '')}")
-
-        return "\n\n".join(processed_docs)
-
-    return default_doc_processor
-
-
 class QdrantRetriever(Task[str, str]):
     """
     Task for retrieving documents from a collection in Qdrant.
 
     :param name: The name of the task.
     :type name: str
     :param client: Qdrant client.
     :type client: :class:`qdrant_client.AsyncQdrantClient`
     :param collection_name: Qdrant collection name.
     :type collection_name: str
     :param embedding_func: Embedding function
     :type embedding_func: :class:`llmsmith.task.retrieval.vector.base.EmbeddingFunc`
     :param embedded_field_name: name of the field in the document on which embeddedings are created while uploading data to the Qdrant collection
     :type embedded_field_name: str
-    :param doc_processing_func: The function to process the query result.
-    :type doc_processing_func: Callable[[List[ScoredPoint]], str], optional
+    :param doc_processing_func: The function to process the query result, defaults to `llmsmith.task.retrieval.vector.base.default_doc_processor`.
+    :type doc_processing_func: Callable[[List[str]], str], optional
     :param query_options: A dictionary of options to pass to the Qdrant client for querying.
     :type query_options: :class:`llmsmith.task.retrieval.vector.options.qdrant.QdrantQueryOptions`, optional
+    :param reranker: Rerank the documents based on the query used to retrieve the documents.
+    :type reranker: :class:`llmsmith.reranker.base.Reranker`, optional
     """
 
     def __init__(
         self,
         name: str,
         client: AsyncQdrantClient,
         collection_name: str,
         embedding_func: EmbeddingFunc,
         embedded_field_name: str,
-        doc_processing_func: Union[Callable[[List[ScoredPoint]], str], None] = None,
+        doc_processing_func: Callable[[List[str]], str] = default_doc_processor,
         query_options: QdrantQueryOptions = default_options,
+        reranker: Reranker = None,
     ) -> None:
         super().__init__(name)
 
         if not embedding_func:
             raise ValueError("Embedding function ('embedding_func') is required")
 
         self.client = client
         self.collection_name = collection_name
         self.embedding_func = embedding_func
         self.embedded_field_name = embedded_field_name
         self.query_options = query_options
+        self._reranker = reranker
 
         if not doc_processing_func:
-            self.doc_processing_func = default_doc_processor_func(embedded_field_name)
+            self.doc_processing_func = default_doc_processor
         else:
             self.doc_processing_func = doc_processing_func
 
     async def execute(self, task_input: TaskInput[str]) -> TaskOutput[str]:
         """
         Executes the task of retrieving documents from the qdrant collection.
 
@@ -109,15 +88,21 @@
         query_options: dict = _query_options_dict(self.query_options)
 
         log.debug(
             f"Qdrant query request: input string: {task_input.content}\n OPTIONS: {query_options}"
         )
         embeddings = self.embedding_func([task_input.content])
 
-        res = await self.client.search(
+        res: List[ScoredPoint] = await self.client.search(
             collection_name=self.collection_name,
             query_vector=embeddings[0],
             **query_options,
         )
-        processed_res: str = self.doc_processing_func(res)
+
+        docs = [doc.payload.get(self.embedded_field_name, "") for doc in res]
+
+        if self._reranker:
+            docs = await self._reranker.rerank(query=task_input.content, docs=docs)
+
+        processed_res: str = self.doc_processing_func(docs)
 
         return TaskOutput(content=processed_res, raw_output=res)
```

### Comparing `llmsmith-0.3.0/llmsmith/task/textgen/claude.py` & `llmsmith-0.4.0/llmsmith/task/textgen/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/textgen/errors.py` & `llmsmith-0.4.0/llmsmith/task/textgen/errors.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/textgen/gemini.py` & `llmsmith-0.4.0/llmsmith/task/textgen/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/textgen/openai.py` & `llmsmith-0.4.0/llmsmith/task/textgen/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.4.0/llmsmith/task/textgen/options/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.4.0/llmsmith/task/textgen/options/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/llmsmith/task/textgen/options/openai.py` & `llmsmith-0.4.0/llmsmith/task/textgen/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.3.0/pyproject.toml` & `llmsmith-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.3.0"
+version = "0.4.0"
 description = "Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)"
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -19,22 +19,24 @@
 google-generativeai = {version = "^0.4.0", optional = true}
 chromadb-client = {version = "^0.4.25.dev0", optional = true}
 onnxruntime = {version = "^1.17.1", optional = true}
 protobuf = {version = "3.20.3", optional = true}
 tokenizers = {version = "^0.15.2", optional = true}
 python-dotenv = "^1.0.1"
 qdrant-client = {version = "^1.8.2", optional = true}
+cohere = {version = "^5.3.2", optional = true}
 
 [tool.poetry.extras]
 openai = ["openai"]
 claude = ["anthropic"]
 gemini = ["google-generativeai"]
 chromadb = ["chromadb-client", "onnxruntime", "protobuf", "tokenizers"]
 qdrant = ["qdrant-client"]
-all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers", "qdrant-client"]
+cohere = ["cohere"]
+all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers", "qdrant-client", "cohere"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.2"
 black = "^24.2.0"
```

### Comparing `llmsmith-0.3.0/PKG-INFO` & `llmsmith-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMSmith
-Version: 0.3.0
+Version: 0.4.0
 Summary: Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)
 Author: Dheeraj Gopinath
 Author-email: dheeraj.gopinath@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,19 +14,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: chromadb
 Provides-Extra: claude
+Provides-Extra: cohere
 Provides-Extra: gemini
 Provides-Extra: openai
 Provides-Extra: qdrant
 Requires-Dist: anthropic (>=0.19.2,<0.20.0) ; extra == "claude" or extra == "all"
 Requires-Dist: chromadb-client (>=0.4.25.dev0,<0.5.0) ; extra == "chromadb" or extra == "all"
+Requires-Dist: cohere (>=5.3.2,<6.0.0) ; extra == "cohere" or extra == "all"
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
 Requires-Dist: onnxruntime (>=1.17.1,<2.0.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: openai (>=1.23.2,<2.0.0) ; extra == "openai" or extra == "all"
 Requires-Dist: protobuf (==3.20.3) ; extra == "chromadb" or extra == "all"
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: qdrant-client (>=1.8.2,<2.0.0) ; extra == "qdrant" or extra == "all"
 Requires-Dist: tokenizers (>=0.15.2,<0.16.0) ; extra == "chromadb" or extra == "all"
```

