# Comparing `tmp/knowledgeai_client-0.5.1.tar.gz` & `tmp/knowledgeai_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgeai_client-0.5.1.tar", max compression
+gzip compressed data, was "knowledgeai_client-0.6.0.tar", max compression
```

## Comparing `knowledgeai_client-0.5.1.tar` & `knowledgeai_client-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1080 2024-02-12 12:45:05.000000 knowledgeai_client-0.5.1/LICENSE
--rw-r--r--   0        0        0     7385 2024-04-28 11:41:59.000000 knowledgeai_client-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-02-12 12:45:05.000000 knowledgeai_client-0.5.1/knowledgeai/__init__.py
--rw-r--r--   0        0        0      392 2024-04-28 11:41:59.000000 knowledgeai_client-0.5.1/knowledgeai/client/__init__.py
--rw-r--r--   0        0        0     5208 2024-04-22 07:11:20.000000 knowledgeai_client-0.5.1/knowledgeai/client/admin.py
--rw-r--r--   0        0        0    13271 2024-04-28 11:29:35.000000 knowledgeai_client-0.5.1/knowledgeai/client/client.py
--rw-r--r--   0        0        0     2044 2024-04-19 15:19:14.000000 knowledgeai_client-0.5.1/knowledgeai/client/schema.py
--rw-r--r--   0        0        0     4252 2024-04-28 11:41:59.000000 knowledgeai_client-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     8212 1970-01-01 00:00:00.000000 knowledgeai_client-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-02-12 12:45:05.581822 knowledgeai_client-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8299 2024-05-03 13:30:46.094584 knowledgeai_client-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-12 12:45:05.582349 knowledgeai_client-0.6.0/knowledgeai/__init__.py
+-rw-r--r--   0        0        0      392 2024-05-03 13:30:46.093735 knowledgeai_client-0.6.0/knowledgeai/client/__init__.py
+-rw-r--r--   0        0        0     5929 2024-05-03 12:23:23.809674 knowledgeai_client-0.6.0/knowledgeai/client/admin.py
+-rw-r--r--   0        0        0    15766 2024-05-03 13:11:24.310541 knowledgeai_client-0.6.0/knowledgeai/client/client.py
+-rw-r--r--   0        0        0     2044 2024-04-19 15:19:14.290191 knowledgeai_client-0.6.0/knowledgeai/client/schema.py
+-rw-r--r--   0        0        0     4252 2024-05-03 13:30:46.066456 knowledgeai_client-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9126 1970-01-01 00:00:00.000000 knowledgeai_client-0.6.0/PKG-INFO
```

### Comparing `knowledgeai_client-0.5.1/LICENSE` & `knowledgeai_client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledgeai_client-0.5.1/README.md` & `knowledgeai_client-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.5.1, (c) 2024 Arvato Systems
+Version: 0.6.0, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
@@ -31,15 +31,15 @@
 
 # Lists all projects
 projects = client.list_projects()
 for project in projects:
     print(project.name)
 
 # Gets the project with the specified ID
-project = client.get_project(project_id=1)
+project = client.get_project(project_id=1, with_documents=True)
 print(project.name)
 
 # Creates a new project with the specified name
 project = client.create_project(project_name="New Project", prompt="x", language=IsoLanguage.ENGLISH, llm=LLM.OPENAI)
 print(project.name)
 
 # Updates the specified project
@@ -54,14 +54,24 @@
 response = client.ask(project_id=1, question="What is the capital of Germany?")
 print(response.answer)
 
 # Retrieves documents for the specified project
 references = client.retrieve(project_id=1, query="What is the capital of Germany?", retrieval_type=Retriever.default)
 for reference in references:
     print(reference.content)
+
+# Delete document from project
+client.delete_document(project_id=1, document_id=1)
+
+# Delete all documents of a project
+client.delete_all_documents(project_id=1)
+
+# Delete project
+client.delete_project(project_id=1)
+
 ```
 
 ## Documentation
 
 The `KnowledgeAIClient` facilitates seamless communication with the Avvia Intelligence KnowledgeAI service, allowing users to manage projects, upload documents, and perform various other tasks programmatically. It provides an intuitive interface to interact with the KnowledgeAI platform, enabling easy integration into Python applications.
 
 ### Class: KnowledgeAIClient
@@ -173,14 +183,33 @@
 - `project_id` (int): The ID of the project to retrieve documents from.
 - `query` (str): The query to retrieve documents for.
 - `retrieval_type` (Retriever, optional): The type of retrieval to use.
 
 Returns:
 - `List[RetrievedDocument]`: The retrieved documents.
 
+#### Method: `delete_project(project_id: int) -> None`
+
+This method is used to delete a specific project.
+
+- `project_id` (int): The ID of the project to be deleted.
+
+#### Method: `delete_document(project_id: int, document_id: int) -> None`
+
+This method is used to delete a specific document from a project.
+
+- `project_id` (int): The ID of the project from which the document will be deleted.
+- `document_id` (int): The ID of the document to be deleted.
+
+#### Method: `delete_all_documents(project_id: int) -> None`
+
+This method is used to delete all documents from a specific project.
+
+- `project_id` (int): The ID of the project from which all documents will be deleted.
+
 
 ### Schema Description
 
 Before diving into the usage of `KnowledgeAIClient`, it's important to understand the schema used in the API. Here are the key classes and enums used:
 
 #### ProjectConfigKey (Enum)
```

### Comparing `knowledgeai_client-0.5.1/knowledgeai/client/admin.py` & `knowledgeai_client-0.6.0/knowledgeai/client/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -169,7 +169,30 @@
         }
 
         response: Response = requests.put(
             url, headers=headers, data=data, timeout=self.timeout
         )
         response.raise_for_status()
         return User(**response.json())
+
+    def delete_user(self, api_key: str) -> None:
+        """
+        Method to delete a user.
+
+        Args:
+            api_key (str): The API key of the user.
+
+        Raises:
+            HTTPError: If the HTTP request returned an unsuccessful status code.
+
+        Example:
+            >>> client.delete_user("put key here")
+        """
+
+        url: str = self.url + "/admin/user/" + api_key
+        headers: dict[str, str] = {
+            "accept": "application/json",
+            "Authorization": self.api_key,
+        }
+        response: Response = requests.delete(url, headers=headers, timeout=self.timeout)
+        response.raise_for_status()
+        log.info("User with API key %s has been deleted.", api_key)
```

### Comparing `knowledgeai_client-0.5.1/knowledgeai/client/client.py` & `knowledgeai_client-0.6.0/knowledgeai/client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,17 +79,20 @@
     def upload_directory(
         self, project_id: int, directory: str, roles: str = "user"
     ) -> None:
         """
         Convenience method to upload all files in a directory to the specified project.
 
         Args:
-            project_id (str): The ID of the project to upload the documents to.
-            directory (str): The path to the directory containing the files to upload.
-            roles (str, optional): The roles to assign to the uploaded documents.
+            project_id (str):
+                The ID of the project to upload the documents to.
+            directory (str):
+                The path to the directory containing the files to upload.
+            roles (str, optional):
+                The roles to assign to the uploaded documents.
                 Comma separated list, defaults to "user".
 
         Returns:
             None
 
         Raises:
             requests.exceptions.RequestException: If an error occurs while uploading
@@ -168,16 +171,18 @@
     def index_urls(
         self, project_id: int, index_urls: list[str], roles: str | None
     ) -> None:
         """
         Indexes the specified URL to the specified project.
 
         Args:
-            project_id (str): The ID of the project to index the URL to.
-            url (str): The URLs to index.
+            project_id (str):
+                The ID of the project to index the URL to.
+            url (str):
+                The URLs to index.
             roles (str, optional): The roles to assign to the indexed document.
                 Comma separated list, defaults to "user".
 
         Returns:
             None
 
         Raises:
@@ -186,14 +191,69 @@
         Example:
           >>> client.index_url("project_id", "https://www.example.com", roles="user")
         """
         url = "/index/urls"
         data = {"project_id": project_id, "urls": index_urls, "roles": roles}
         self._api_call(HttpMethod.POST, url, data=data)
 
+    def delete_document(self, project_id: int, document_id: int) -> None:
+        """
+        Deletes the document with the specified ID by making a DELETE request to the
+        KnowledgeAI API. The `project_id` parameter specifies the ID of the project the
+        document belongs to, and the `document_id` parameter specifies the ID of the
+        document to delete.
+
+        If the deletion is successful, no value is returned. If an error occurs during
+        the API call, a `requests.exceptions.RequestException` is raised.
+
+        Args:
+            project_id (int):
+                The ID of the project the document belongs to.
+            document_id (int):
+                The ID of the document to delete.
+
+        Returns:
+            None
+
+        Raises:
+            requests.exceptions.RequestException: If an error occurs.
+
+        Example usage:
+        ```
+        client = KnowledgeAIClient()
+        client.delete_document(project_id=1, document_id=1)
+        ```
+        """
+        url: str = "/index/document"
+        data = {"project_id": project_id, "document_id": document_id}
+        self._api_call(HttpMethod.DELETE, url, params=data)
+        log.info("Document %s deleted", document_id)
+
+    def delete_all_documents(self, project_id: int) -> None:
+        """
+        Deletes all documents for the specified project.
+
+        Args:
+            project_id (int):
+                The ID of the project to delete all documents for.
+
+        Returns:
+            None
+
+        Raises:
+            requests.exceptions.RequestException: If an error occurs.
+
+        Example:
+            >>> client.delete_all_documents(project_id=1)
+        """
+        url: str = "/index/document/all"
+        data = {"project_id": project_id}
+        self._api_call(HttpMethod.DELETE, url, data=data)
+        log.info("All documents deleted for project %s", project_id)
+
     def list_projects(self) -> list[Project]:
         """
         Lists all projects.
 
         Returns:
             List[Project]: A list of projects.
 
@@ -338,14 +398,34 @@
 
         url: str = "/project/" + str(project_id) + "/configuration/" + key.value
         data: dict[str, str] = {"value": value}
         response: Response = self._api_call(HttpMethod.PUT, url, data=data)
 
         return Project(**response.json())
 
+    def delete_project(self, project_id: int) -> None:
+        """Deletes the project with the specified ID.
+
+        Args:
+            project_id (int): The ID of the project to delete.
+
+        Returns:
+            None
+
+        Raises:
+            requests.exceptions.RequestException: If an error occurs.
+
+        Example:
+            >>> client.delete_project(1)
+        """
+
+        url: str = "/project/" + str(project_id)
+        self._api_call(HttpMethod.DELETE, url)
+        log.info("Project %s deleted", project_id)
+
     def ask(self, project_id: int, question: str) -> AskResponse:
         """Asks a question to the specified project.
 
         Args:
             project_id (int): The ID of the project to ask the question to.
             question (str): The question to ask.
```

### Comparing `knowledgeai_client-0.5.1/knowledgeai/client/schema.py` & `knowledgeai_client-0.6.0/knowledgeai/client/schema.py`

 * *Files identical despite different names*

### Comparing `knowledgeai_client-0.5.1/pyproject.toml` & `knowledgeai_client-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "A python client for the Avvia Intelligence - Knowledge AI Rest API"
 homepage    = "https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client"
 keywords    = ["AI", "Knowledge Retrieval", "arvato systems", "avvia intelligence", "knowledgeai"]
 license     = "MIT"
 name        = "knowledgeai-client"
 packages    = [{ include = "knowledgeai", from = "." }]
 readme      = "README.md"
-version     = "0.5.1"
+version     = "0.6.0"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 
 httpx             = "0.27.0"
 pydantic          = "2.7.0"
 pydantic-settings = "2.2.1"
```

### Comparing `knowledgeai_client-0.5.1/PKG-INFO` & `knowledgeai_client-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgeai-client
-Version: 0.5.1
+Version: 0.6.0
 Summary: A python client for the Avvia Intelligence - Knowledge AI Rest API
 Home-page: https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client
 License: MIT
 Keywords: AI,Knowledge Retrieval,arvato systems,avvia intelligence,knowledgeai
 Author: Arvato Systems
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Dist: python-magic (==0.4.27)
 Requires-Dist: tqdm (==4.66.2)
 Description-Content-Type: text/markdown
 
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.5.1, (c) 2024 Arvato Systems
+Version: 0.6.0, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
@@ -52,15 +52,15 @@
 
 # Lists all projects
 projects = client.list_projects()
 for project in projects:
     print(project.name)
 
 # Gets the project with the specified ID
-project = client.get_project(project_id=1)
+project = client.get_project(project_id=1, with_documents=True)
 print(project.name)
 
 # Creates a new project with the specified name
 project = client.create_project(project_name="New Project", prompt="x", language=IsoLanguage.ENGLISH, llm=LLM.OPENAI)
 print(project.name)
 
 # Updates the specified project
@@ -75,14 +75,24 @@
 response = client.ask(project_id=1, question="What is the capital of Germany?")
 print(response.answer)
 
 # Retrieves documents for the specified project
 references = client.retrieve(project_id=1, query="What is the capital of Germany?", retrieval_type=Retriever.default)
 for reference in references:
     print(reference.content)
+
+# Delete document from project
+client.delete_document(project_id=1, document_id=1)
+
+# Delete all documents of a project
+client.delete_all_documents(project_id=1)
+
+# Delete project
+client.delete_project(project_id=1)
+
 ```
 
 ## Documentation
 
 The `KnowledgeAIClient` facilitates seamless communication with the Avvia Intelligence KnowledgeAI service, allowing users to manage projects, upload documents, and perform various other tasks programmatically. It provides an intuitive interface to interact with the KnowledgeAI platform, enabling easy integration into Python applications.
 
 ### Class: KnowledgeAIClient
@@ -194,14 +204,33 @@
 - `project_id` (int): The ID of the project to retrieve documents from.
 - `query` (str): The query to retrieve documents for.
 - `retrieval_type` (Retriever, optional): The type of retrieval to use.
 
 Returns:
 - `List[RetrievedDocument]`: The retrieved documents.
 
+#### Method: `delete_project(project_id: int) -> None`
+
+This method is used to delete a specific project.
+
+- `project_id` (int): The ID of the project to be deleted.
+
+#### Method: `delete_document(project_id: int, document_id: int) -> None`
+
+This method is used to delete a specific document from a project.
+
+- `project_id` (int): The ID of the project from which the document will be deleted.
+- `document_id` (int): The ID of the document to be deleted.
+
+#### Method: `delete_all_documents(project_id: int) -> None`
+
+This method is used to delete all documents from a specific project.
+
+- `project_id` (int): The ID of the project from which all documents will be deleted.
+
 
 ### Schema Description
 
 Before diving into the usage of `KnowledgeAIClient`, it's important to understand the schema used in the API. Here are the key classes and enums used:
 
 #### ProjectConfigKey (Enum)
```

