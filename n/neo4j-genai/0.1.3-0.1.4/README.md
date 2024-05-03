# Comparing `tmp/neo4j_genai-0.1.3.tar.gz` & `tmp/neo4j_genai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j_genai-0.1.3.tar", max compression
+gzip compressed data, was "neo4j_genai-0.1.4.tar", max compression
```

## Comparing `neo4j_genai-0.1.3.tar` & `neo4j_genai-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0    11360 2024-04-24 10:41:46.557163 neo4j_genai-0.1.3/LICENSE.APACHE2.txt
--rw-r--r--   0        0        0     2774 2024-04-24 10:41:46.557163 neo4j_genai-0.1.3/LICENSE.PYTHON.txt
--rw-r--r--   0        0        0      423 2024-04-24 10:41:46.557163 neo4j_genai-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      160 2024-04-24 10:41:46.557163 neo4j_genai-0.1.3/NOTICE.txt
--rw-r--r--   0        0        0     4153 2024-04-24 10:41:46.557163 neo4j_genai-0.1.3/README.md
--rw-r--r--   0        0        0     1529 2024-04-24 10:41:46.561163 neo4j_genai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      750 2024-04-24 10:41:46.561163 neo4j_genai-0.1.3/src/neo4j_genai/__init__.py
--rw-r--r--   0        0        0     1027 2024-04-24 10:41:46.561163 neo4j_genai-0.1.3/src/neo4j_genai/embedder.py
--rw-r--r--   0        0        0     4265 2024-04-24 10:41:46.561163 neo4j_genai-0.1.3/src/neo4j_genai/indexes.py
--rw-r--r--   0        0        0     8701 2024-04-24 10:41:46.561163 neo4j_genai-0.1.3/src/neo4j_genai/retrievers.py
--rw-r--r--   0        0        0     2370 2024-04-24 10:41:46.561163 neo4j_genai-0.1.3/src/neo4j_genai/types.py
--rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 neo4j_genai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11360 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/LICENSE.APACHE2.txt
+-rw-r--r--   0        0        0     2774 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/LICENSE.PYTHON.txt
+-rw-r--r--   0        0        0      423 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      160 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/NOTICE.txt
+-rw-r--r--   0        0        0     5527 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/README.md
+-rw-r--r--   0        0        0     1529 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      889 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/embedder.py
+-rw-r--r--   0        0        0     4276 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/indexes.py
+-rw-r--r--   0        0        0     2496 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/neo4j_queries.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/__init__.py
+-rw-r--r--   0        0        0     1969 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/base.py
+-rw-r--r--   0        0        0     7145 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/hybrid.py
+-rw-r--r--   0        0        0     7059 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/vector.py
+-rw-r--r--   0        0        0     2736 2024-05-03 13:42:59.615292 neo4j_genai-0.1.4/src/neo4j_genai/types.py
+-rw-r--r--   0        0        0     6263 1970-01-01 00:00:00.000000 neo4j_genai-0.1.4/PKG-INFO
```

### Comparing `neo4j_genai-0.1.3/LICENSE.APACHE2.txt` & `neo4j_genai-0.1.4/LICENSE.APACHE2.txt`

 * *Files identical despite different names*

### Comparing `neo4j_genai-0.1.3/LICENSE.PYTHON.txt` & `neo4j_genai-0.1.4/LICENSE.PYTHON.txt`

 * *Files identical despite different names*

### Comparing `neo4j_genai-0.1.3/README.md` & `neo4j_genai-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,131 @@
 # Neo4j GenAI package for Python
 
 This repository contains the official Neo4j GenAI features for Python.
 
+The purpose of this package is to provide a first party package to developers,
+where Neo4j can guarantee long term commitment and maintenance as well as being
+fast to ship new features and high performing patterns and methods.
+
+Docs are coming soon!
+
 # Usage
 
 ## Installation
 
 This package requires Python (>=3.8.1).
 
 To install the latest stable version, use:
 
 ```shell
 pip install neo4j-genai
 ```
 
-## Example
+## Examples
+
+While the library has more retrievers than shown here, the following examples should be able to get you started.
 
-After setting up a Neo4j database instance:
+### Performing a similarity search
+
+Assumption: Neo4j running with populated vector index in place.
 
 ```python
 from neo4j import GraphDatabase
 from neo4j_genai import VectorRetriever
+from langchain_openai import OpenAIEmbeddings
 
-from random import random
+URI = "neo4j://localhost:7687"
+AUTH = ("neo4j", "password")
+
+INDEX_NAME = "embedding-name"
 
+# Connect to Neo4j database
+driver = GraphDatabase.driver(URI, auth=AUTH)
+
+# Create Embedder object
+embedder = OpenAIEmbeddings(model="text-embedding-3-large")
+
+# Initialize the retriever
+retriever = VectorRetriever(driver, INDEX_NAME, embedder)
+
+# Run the similarity search
+query_text = "How do I do similarity search in Neo4j?"
+response = retriever.search(query_text=query_text, top_k=5)
+```
+
+### Creating a vector index
+
+When creating a vector index, make sure you match the number of dimensions in the index with the number of dimensions the embeddings have.
+
+Assumption: Neo4j running
+
+```python
+from neo4j import GraphDatabase
 from neo4j_genai.indexes import create_vector_index
 
 URI = "neo4j://localhost:7687"
 AUTH = ("neo4j", "password")
 
-INDEX_NAME = "embedding-name"
-DIMENSION = 1536
+INDEX_NAME = "chunk-index"
 
 # Connect to Neo4j database
 driver = GraphDatabase.driver(URI, auth=AUTH)
 
 # Creating the index
 create_vector_index(
     driver,
     INDEX_NAME,
     label="Document",
-    property="propertyKey",
-    dimensions=DIMENSION,
+    property="textProperty",
+    dimensions=1536,
     similarity_fn="euclidean",
 )
 
-# Initialize the retriever
-retriever = VectorRetriever(driver, INDEX_NAME)
+```
+
+### Populating the Neo4j Vector Index
+
+This library does not write to the database, that is up to you.
+See below for how to write using Cypher via the Neo4j driver.
+
+Assumption: Neo4j running with a defined vector index
+
+```python
+from neo4j import GraphDatabase
+from random import random
+
+URI = "neo4j://localhost:7687"
+AUTH = ("neo4j", "password")
+
+# Connect to Neo4j database
+driver = GraphDatabase.driver(URI, auth=AUTH)
 
 # Upsert the vector
 vector = [random() for _ in range(DIMENSION)]
 insert_query = (
     "MERGE (n:Document {id: $id})"
     "WITH n "
-    "CALL db.create.setNodeVectorProperty(n, 'propertyKey', $vector)"
+    "CALL db.create.setNodeVectorProperty(n, 'textProperty', $vector)"
     "RETURN n"
 )
 parameters = {
     "id": 0,
     "vector": vector,
 }
 driver.execute_query(insert_query, parameters)
-
-# Perform the similarity search for a vector query
-query_vector = [random() for _ in range(DIMENSION)]
-print(retriever.search(query_vector=query_vector, top_k=5))
-
 ```
 
 # Development
 
 ## Install dependencies
 
 ```bash
 poetry install
 ```
 
-
 ## Getting started
 
 ### Issues
 
 If you have a bug to report or feature to request, first
 [search to see if an issue already exists](https://docs.github.com/en/github/searching-for-information-on-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments).
 If a related issue doesn't exist, please raise a new issue using the relevant
@@ -98,33 +143,32 @@
 2. Install Python and Poetry. For more information, see [the development guide](./docs/contributing/DEVELOPING.md).
 3. Create a working branch from `main` and start with your changes!
 
 ### Pull request
 
 When you're finished with your changes, create a pull request, also known as a PR.
 
-* Ensure that you have [signed the CLA](https://neo4j.com/developer/contributing-code/#sign-cla).
-* Ensure that the base of your PR is set to `main`.
-* Don't forget to [link your PR to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
-if you are solving one.
-* Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
-so that maintainers can make any necessary tweaks and update your branch for merge.
-* Reviewers may ask for changes to be made before a PR can be merged, either using
-[suggested changes](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/incorporating-feedback-in-your-pull-request)
-or normal pull request comments. You can apply suggested changes directly through
-the UI, and any other changes can be made in your fork and committed to the PR branch.
-* As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
-
+-   Ensure that you have [signed the CLA](https://neo4j.com/developer/contributing-code/#sign-cla).
+-   Ensure that the base of your PR is set to `main`.
+-   Don't forget to [link your PR to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
+    if you are solving one.
+-   Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
+    so that maintainers can make any necessary tweaks and update your branch for merge.
+-   Reviewers may ask for changes to be made before a PR can be merged, either using
+    [suggested changes](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/incorporating-feedback-in-your-pull-request)
+    or normal pull request comments. You can apply suggested changes directly through
+    the UI, and any other changes can be made in your fork and committed to the PR branch.
+-   As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
 
 ## Run tests
 
 Open a new virtual environment and then run the tests.
 
 ```bash
 poetry shell
-pytest
+pytest tests/unit
 ```
 
 ## Further information
 
 -   [The official Neo4j Python driver](https://github.com/neo4j/neo4j-python-driver)
 -   [Neo4j GenAI integrations](https://neo4j.com/docs/cypher-manual/current/genai-integrations/)
```

### Comparing `neo4j_genai-0.1.3/pyproject.toml` & `neo4j_genai-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "neo4j-genai"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python package to allow easy integration to Neo4j's GenAI features"
 authors = ["Neo4j, Inc <team-gen-ai@neo4j.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [[tool.poetry.packages]]
 include = "neo4j_genai"
```

### Comparing `neo4j_genai-0.1.3/src/neo4j_genai/__init__.py` & `neo4j_genai-0.1.4/src/neo4j_genai/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,11 +9,16 @@
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .retrievers import VectorRetriever, VectorCypherRetriever
+from .retrievers.vector import VectorRetriever, VectorCypherRetriever
+from .retrievers.hybrid import HybridRetriever, HybridCypherRetriever
 
-
-__all__ = ["VectorRetriever", "VectorCypherRetriever"]
+__all__ = [
+    "VectorRetriever",
+    "VectorCypherRetriever",
+    "HybridRetriever",
+    "HybridCypherRetriever",
+]
```

### Comparing `neo4j_genai-0.1.3/src/neo4j_genai/embedder.py` & `neo4j_genai-0.1.4/src/neo4j_genai/embedder.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import ABC, abstractmethod
-from .types import EmbeddingVector
 
 
 class Embedder(ABC):
     """Interface for embedding models."""
 
     @abstractmethod
-    def embed_query(self, text: str) -> EmbeddingVector:
+    def embed_query(self, text: str) -> list[float]:
         """Embed query text.
 
         Args:
             text (str): Text to convert to vector embedding
 
         Returns:
-            EmbeddingVector: A vector embedding.
+            list[float]: A vector embedding.
         """
```

### Comparing `neo4j_genai-0.1.3/src/neo4j_genai/indexes.py` & `neo4j_genai-0.1.4/src/neo4j_genai/indexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 "node_properties": node_properties,
             }
         )
     except ValidationError as e:
         raise ValueError(f"Error for inputs to create_fulltext_index {str(e)}")
 
     query = (
-        "CREATE FULLTEXT INDEX $name"
+        "CREATE FULLTEXT INDEX $name "
         f"FOR (n:`{label}`) ON EACH "
         f"[{', '.join(['n.`' + prop + '`' for prop in node_properties])}]"
     )
     driver.execute_query(query, {"name": name})
 
 
 def drop_index(driver: Driver, name: str) -> None:
@@ -111,12 +111,12 @@
     to drop a vector index in Neo4j.
     See Cypher manual on [Drop vector indexes](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-drop)
 
     Args:
         driver (Driver): Neo4j Python driver instance.
         name (str): The name of the index to delete.
     """
-    query = "DROP INDEX $name"
+    query = "DROP INDEX $name IF EXISTS"
     parameters = {
         "name": name,
     }
     driver.execute_query(query, parameters)
```

### Comparing `neo4j_genai-0.1.3/src/neo4j_genai/retrievers.py` & `neo4j_genai-0.1.4/src/neo4j_genai/retrievers/hybrid.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,226 +8,154 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from abc import abstractmethod, ABC
 from typing import Optional, Any
-from pydantic import ValidationError
-from neo4j import Driver, Record
-from .embedder import Embedder
-from .types import (
-    SimilaritySearchModel,
-    VectorSearchRecord,
-    VectorCypherSearchModel,
-)
-
-
-class Retriever(ABC):
-    """
-    Abstract class for Neo4j retrievers
-    """
-
-    def __init__(self, driver: Driver):
-        self.driver = driver
-
-    def _verify_version(self) -> None:
-        """
-        Check if the connected Neo4j database version supports vector indexing.
-
-        Queries the Neo4j database to retrieve its version and compares it
-        against a target version (5.18.1) that is known to support vector
-        indexing. Raises a ValueError if the connected Neo4j version is
-        not supported.
-        """
-        records, _, _ = self.driver.execute_query("CALL dbms.components()")
-        version = records[0]["versions"][0]
-
-        if "aura" in version:
-            version_tuple = (
-                *tuple(map(int, version.split("-")[0].split("."))),
-                0,
-            )
-            target_version = (5, 18, 0)
-        else:
-            version_tuple = tuple(map(int, version.split(".")))
-            target_version = (5, 18, 1)
-
-        if version_tuple < target_version:
-            raise ValueError(
-                "This package only supports Neo4j version 5.18.1 or greater"
-            )
 
-    @abstractmethod
-    def search(self, *args, **kwargs) -> Any:
-        pass
+from neo4j import Record, Driver
+from pydantic import ValidationError
 
+from neo4j_genai.embedder import Embedder
+from neo4j_genai.retrievers.base import Retriever
+from neo4j_genai.types import HybridSearchModel, SearchType, HybridCypherSearchModel
+from neo4j_genai.neo4j_queries import get_search_query
 
-class VectorRetriever(Retriever):
-    """
-    Provides retrieval method using vector search over embeddings.
-    If an embedder is provided, it needs to have the required Embedder type.
-    """
 
+class HybridRetriever(Retriever):
     def __init__(
         self,
         driver: Driver,
-        index_name: str,
+        vector_index_name: str,
+        fulltext_index_name: str,
         embedder: Optional[Embedder] = None,
         return_properties: Optional[list[str]] = None,
     ) -> None:
         super().__init__(driver)
-        self._verify_version()
-        self.index_name = index_name
-        self.return_properties = return_properties
+        self.vector_index_name = vector_index_name
+        self.fulltext_index_name = fulltext_index_name
         self.embedder = embedder
+        self.return_properties = return_properties
 
     def search(
         self,
+        query_text: str,
         query_vector: Optional[list[float]] = None,
-        query_text: Optional[str] = None,
         top_k: int = 5,
-    ) -> list[VectorSearchRecord]:
+    ) -> list[Record]:
         """Get the top_k nearest neighbor embeddings for either provided query_vector or query_text.
+        Both query_vector and query_text can be provided.
+        If query_vector is provided, then it will be preferred over the embedded query_text
+        for the vector search.
         See the following documentation for more details:
-
         - [Query a vector index](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-query)
         - [db.index.vector.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_vector_queryNodes)
-
+        - [db.index.fulltext.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_fulltext_querynodes)
         Args:
+            query_text (str): The text to get the closest neighbors of.
             query_vector (Optional[list[float]], optional): The vector embeddings to get the closest neighbors of. Defaults to None.
-            query_text (Optional[str], optional): The text to get the closest neighbors of. Defaults to None.
             top_k (int, optional): The number of neighbors to return. Defaults to 5.
-
         Raises:
             ValueError: If validation of the input arguments fail.
             ValueError: If no embedder is provided.
-
         Returns:
-            list[VectorSearchRecord]: The `top_k` neighbors found in vector search with their nodes and scores.
+            list[Record]: The results of the search query
         """
         try:
-            validated_data = SimilaritySearchModel(
-                index_name=self.index_name,
+            validated_data = HybridSearchModel(
+                vector_index_name=self.vector_index_name,
+                fulltext_index_name=self.fulltext_index_name,
                 top_k=top_k,
                 query_vector=query_vector,
                 query_text=query_text,
             )
         except ValidationError as e:
-            error_details = e.errors()
-            raise ValueError(f"Validation failed: {error_details}")
+            raise ValueError(f"Validation failed: {e.errors()}")
 
         parameters = validated_data.model_dump(exclude_none=True)
 
-        if query_text:
+        if query_text and not query_vector:
             if not self.embedder:
                 raise ValueError("Embedding method required for text query.")
             query_vector = self.embedder.embed_query(query_text)
             parameters["query_vector"] = query_vector
-            del parameters["query_text"]
-
-        db_query_string = """
-        CALL db.index.vector.queryNodes($index_name, $top_k, $query_vector)
-        YIELD node, score
-        """
 
-        if self.return_properties:
-            return_properties_cypher = ", ".join(
-                [f".{prop}" for prop in self.return_properties]
-            )
-            db_query_string += (
-                f"RETURN node {{{return_properties_cypher}}} as node, score"
-            )
-
-        records, _, _ = self.driver.execute_query(db_query_string, parameters)
-
-        try:
-            return [
-                VectorSearchRecord(node=record["node"], score=record["score"])
-                for record in records
-            ]
-        except ValidationError as e:
-            error_details = e.errors()
-            raise ValueError(
-                f"Validation failed while constructing output: {error_details}"
-            )
+        search_query = get_search_query(SearchType.HYBRID, self.return_properties)
 
+        records, _, _ = self.driver.execute_query(search_query, parameters)
+        return records
 
-class VectorCypherRetriever(Retriever):
-    """
-    Provides retrieval method using vector similarity and custom Cypher query.
-    If an embedder is provided, it needs to have the required Embedder type.
-    """
 
+class HybridCypherRetriever(Retriever):
     def __init__(
         self,
         driver: Driver,
-        index_name: str,
+        vector_index_name: str,
+        fulltext_index_name: str,
         retrieval_query: str,
         embedder: Optional[Embedder] = None,
     ) -> None:
         super().__init__(driver)
-        self._verify_version()
-        self.index_name = index_name
+        self.vector_index_name = vector_index_name
+        self.fulltext_index_name = fulltext_index_name
         self.retrieval_query = retrieval_query
         self.embedder = embedder
 
     def search(
         self,
+        query_text: str,
         query_vector: Optional[list[float]] = None,
-        query_text: Optional[str] = None,
         top_k: int = 5,
         query_params: Optional[dict[str, Any]] = None,
     ) -> list[Record]:
         """Get the top_k nearest neighbor embeddings for either provided query_vector or query_text.
+        Both query_vector and query_text can be provided.
+        If query_vector is provided, then it will be preferred over the embedded query_text
+        for the vector search.
         See the following documentation for more details:
-
         - [Query a vector index](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-query)
         - [db.index.vector.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_vector_queryNodes)
-
+        - [db.index.fulltext.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_fulltext_querynodes)
         Args:
+            query_text (str): The text to get the closest neighbors of.
             query_vector (Optional[list[float]], optional): The vector embeddings to get the closest neighbors of. Defaults to None.
-            query_text (Optional[str], optional): The text to get the closest neighbors of. Defaults to None.
             top_k (int, optional): The number of neighbors to return. Defaults to 5.
             query_params (Optional[dict[str, Any]], optional): Parameters for the Cypher query. Defaults to None.
-
         Raises:
             ValueError: If validation of the input arguments fail.
             ValueError: If no embedder is provided.
-
         Returns:
             list[Record]: The results of the search query
         """
         try:
-            validated_data = VectorCypherSearchModel(
-                index_name=self.index_name,
+            validated_data = HybridCypherSearchModel(
+                vector_index_name=self.vector_index_name,
+                fulltext_index_name=self.fulltext_index_name,
                 top_k=top_k,
                 query_vector=query_vector,
                 query_text=query_text,
                 query_params=query_params,
             )
         except ValidationError as e:
             raise ValueError(f"Validation failed: {e.errors()}")
 
         parameters = validated_data.model_dump(exclude_none=True)
 
-        if query_text:
+        if query_text and not query_vector:
             if not self.embedder:
                 raise ValueError("Embedding method required for text query.")
-            parameters["query_vector"] = self.embedder.embed_query(query_text)
-            del parameters["query_text"]
+            query_vector = self.embedder.embed_query(query_text)
+            parameters["query_vector"] = query_vector
 
         if query_params:
             for key, value in query_params.items():
                 if key not in parameters:
                     parameters[key] = value
             del parameters["query_params"]
 
-        query_prefix = """
-                CALL db.index.vector.queryNodes($index_name, $top_k, $query_vector)
-                YIELD node, score
-                """
-        search_query = query_prefix + self.retrieval_query
+        search_query = get_search_query(
+            SearchType.HYBRID, retrieval_query=self.retrieval_query
+        )
         records, _, _ = self.driver.execute_query(search_query, parameters)
         return records
```

### Comparing `neo4j_genai-0.1.3/src/neo4j_genai/types.py` & `neo4j_genai-0.1.4/src/neo4j_genai/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,29 +8,25 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
+from enum import Enum
 from typing import Any, Literal, Optional
 from pydantic import BaseModel, PositiveInt, model_validator, field_validator
 from neo4j import Driver
 
 
 class VectorSearchRecord(BaseModel):
     node: Any
     score: float
 
 
-class EmbeddingVector(BaseModel):
-    vector: list[float]
-
-
 class IndexModel(BaseModel):
     driver: Any
 
     @field_validator("driver")
     def check_driver_is_valid(cls, v):
         if not isinstance(v, Driver):
             raise ValueError("driver must be an instance of neo4j.Driver")
@@ -53,15 +49,15 @@
     @field_validator("node_properties")
     def check_node_properties_not_empty(cls, v):
         if len(v) == 0:
             raise ValueError("node_properties cannot be an empty list")
         return v
 
 
-class SimilaritySearchModel(BaseModel):
+class VectorSearchModel(BaseModel):
     index_name: str
     top_k: PositiveInt = 5
     query_vector: Optional[list[float]] = None
     query_text: Optional[str] = None
 
     @model_validator(mode="before")
     def check_query(cls, values):
@@ -72,9 +68,28 @@
         if not (bool(query_vector) ^ bool(query_text)):
             raise ValueError(
                 "You must provide exactly one of query_vector or query_text."
             )
         return values
 
 
-class VectorCypherSearchModel(SimilaritySearchModel):
+class VectorCypherSearchModel(VectorSearchModel):
     query_params: Optional[dict[str, Any]] = None
+
+
+class HybridSearchModel(BaseModel):
+    vector_index_name: str
+    fulltext_index_name: str
+    query_text: str
+    top_k: PositiveInt = 5
+    query_vector: Optional[list[float]] = None
+
+
+class HybridCypherSearchModel(HybridSearchModel):
+    query_params: Optional[dict[str, Any]] = None
+
+
+class SearchType(str, Enum):
+    """Enumerator of the search strategies."""
+
+    VECTOR = "vector"
+    HYBRID = "hybrid"
```

### Comparing `neo4j_genai-0.1.3/PKG-INFO` & `neo4j_genai-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-genai
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package to allow easy integration to Neo4j's GenAI features
 License: Apache License, Version 2.0
 Author: Neo4j, Inc
 Author-email: team-gen-ai@neo4j.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -17,89 +17,134 @@
 Requires-Dist: types-requests (>=2.31.0.20240218,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 # Neo4j GenAI package for Python
 
 This repository contains the official Neo4j GenAI features for Python.
 
+The purpose of this package is to provide a first party package to developers,
+where Neo4j can guarantee long term commitment and maintenance as well as being
+fast to ship new features and high performing patterns and methods.
+
+Docs are coming soon!
+
 # Usage
 
 ## Installation
 
 This package requires Python (>=3.8.1).
 
 To install the latest stable version, use:
 
 ```shell
 pip install neo4j-genai
 ```
 
-## Example
+## Examples
+
+While the library has more retrievers than shown here, the following examples should be able to get you started.
 
-After setting up a Neo4j database instance:
+### Performing a similarity search
+
+Assumption: Neo4j running with populated vector index in place.
 
 ```python
 from neo4j import GraphDatabase
 from neo4j_genai import VectorRetriever
+from langchain_openai import OpenAIEmbeddings
 
-from random import random
+URI = "neo4j://localhost:7687"
+AUTH = ("neo4j", "password")
+
+INDEX_NAME = "embedding-name"
 
+# Connect to Neo4j database
+driver = GraphDatabase.driver(URI, auth=AUTH)
+
+# Create Embedder object
+embedder = OpenAIEmbeddings(model="text-embedding-3-large")
+
+# Initialize the retriever
+retriever = VectorRetriever(driver, INDEX_NAME, embedder)
+
+# Run the similarity search
+query_text = "How do I do similarity search in Neo4j?"
+response = retriever.search(query_text=query_text, top_k=5)
+```
+
+### Creating a vector index
+
+When creating a vector index, make sure you match the number of dimensions in the index with the number of dimensions the embeddings have.
+
+Assumption: Neo4j running
+
+```python
+from neo4j import GraphDatabase
 from neo4j_genai.indexes import create_vector_index
 
 URI = "neo4j://localhost:7687"
 AUTH = ("neo4j", "password")
 
-INDEX_NAME = "embedding-name"
-DIMENSION = 1536
+INDEX_NAME = "chunk-index"
 
 # Connect to Neo4j database
 driver = GraphDatabase.driver(URI, auth=AUTH)
 
 # Creating the index
 create_vector_index(
     driver,
     INDEX_NAME,
     label="Document",
-    property="propertyKey",
-    dimensions=DIMENSION,
+    property="textProperty",
+    dimensions=1536,
     similarity_fn="euclidean",
 )
 
-# Initialize the retriever
-retriever = VectorRetriever(driver, INDEX_NAME)
+```
+
+### Populating the Neo4j Vector Index
+
+This library does not write to the database, that is up to you.
+See below for how to write using Cypher via the Neo4j driver.
+
+Assumption: Neo4j running with a defined vector index
+
+```python
+from neo4j import GraphDatabase
+from random import random
+
+URI = "neo4j://localhost:7687"
+AUTH = ("neo4j", "password")
+
+# Connect to Neo4j database
+driver = GraphDatabase.driver(URI, auth=AUTH)
 
 # Upsert the vector
 vector = [random() for _ in range(DIMENSION)]
 insert_query = (
     "MERGE (n:Document {id: $id})"
     "WITH n "
-    "CALL db.create.setNodeVectorProperty(n, 'propertyKey', $vector)"
+    "CALL db.create.setNodeVectorProperty(n, 'textProperty', $vector)"
     "RETURN n"
 )
 parameters = {
     "id": 0,
     "vector": vector,
 }
 driver.execute_query(insert_query, parameters)
-
-# Perform the similarity search for a vector query
-query_vector = [random() for _ in range(DIMENSION)]
-print(retriever.search(query_vector=query_vector, top_k=5))
-
 ```
 
 # Development
 
 ## Install dependencies
 
 ```bash
 poetry install
 ```
 
-
 ## Getting started
 
 ### Issues
 
 If you have a bug to report or feature to request, first
 [search to see if an issue already exists](https://docs.github.com/en/github/searching-for-information-on-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments).
 If a related issue doesn't exist, please raise a new issue using the relevant
@@ -117,34 +162,33 @@
 2. Install Python and Poetry. For more information, see [the development guide](./docs/contributing/DEVELOPING.md).
 3. Create a working branch from `main` and start with your changes!
 
 ### Pull request
 
 When you're finished with your changes, create a pull request, also known as a PR.
 
-* Ensure that you have [signed the CLA](https://neo4j.com/developer/contributing-code/#sign-cla).
-* Ensure that the base of your PR is set to `main`.
-* Don't forget to [link your PR to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
-if you are solving one.
-* Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
-so that maintainers can make any necessary tweaks and update your branch for merge.
-* Reviewers may ask for changes to be made before a PR can be merged, either using
-[suggested changes](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/incorporating-feedback-in-your-pull-request)
-or normal pull request comments. You can apply suggested changes directly through
-the UI, and any other changes can be made in your fork and committed to the PR branch.
-* As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
-
+-   Ensure that you have [signed the CLA](https://neo4j.com/developer/contributing-code/#sign-cla).
+-   Ensure that the base of your PR is set to `main`.
+-   Don't forget to [link your PR to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
+    if you are solving one.
+-   Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
+    so that maintainers can make any necessary tweaks and update your branch for merge.
+-   Reviewers may ask for changes to be made before a PR can be merged, either using
+    [suggested changes](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/incorporating-feedback-in-your-pull-request)
+    or normal pull request comments. You can apply suggested changes directly through
+    the UI, and any other changes can be made in your fork and committed to the PR branch.
+-   As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
 
 ## Run tests
 
 Open a new virtual environment and then run the tests.
 
 ```bash
 poetry shell
-pytest
+pytest tests/unit
 ```
 
 ## Further information
 
 -   [The official Neo4j Python driver](https://github.com/neo4j/neo4j-python-driver)
 -   [Neo4j GenAI integrations](https://neo4j.com/docs/cypher-manual/current/genai-integrations/)
```

