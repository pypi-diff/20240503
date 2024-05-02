# Comparing `tmp/langchain_google_cloud_sql_pg-0.4.0-py3-none-any.whl.zip` & `tmp/langchain_google_cloud_sql_pg-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29727 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1034 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/__init__.py
--rw-r--r--  2.0 unx     4964 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/chat_message_history.py
--rw-r--r--  2.0 unx    14672 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/engine.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/indexes.py
--rw-r--r--  2.0 unx    17740 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/py.typed
--rw-r--r--  2.0 unx    29570 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/vectorstore.py
--rw-r--r--  2.0 unx      622 b- defN 24-Apr-03 17:52 langchain_google_cloud_sql_pg/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-03 17:54 langchain_google_cloud_sql_pg-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    20296 b- defN 24-Apr-03 17:54 langchain_google_cloud_sql_pg-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 17:54 langchain_google_cloud_sql_pg-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       30 b- defN 24-Apr-03 17:54 langchain_google_cloud_sql_pg-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1287 b- defN 24-Apr-03 17:54 langchain_google_cloud_sql_pg-0.4.0.dist-info/RECORD
-13 files, 104245 bytes uncompressed, 27511 bytes compressed:  73.6%
+Zip file size: 29746 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/__init__.py
+-rw-r--r--  2.0 unx     4964 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/chat_message_history.py
+-rw-r--r--  2.0 unx    14707 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/engine.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/indexes.py
+-rw-r--r--  2.0 unx    17740 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/py.typed
+-rw-r--r--  2.0 unx    29576 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/vectorstore.py
+-rw-r--r--  2.0 unx      622 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20359 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       30 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1287 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD
+13 files, 104349 bytes uncompressed, 27530 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_cloud_sql_pg/vectorstore.py
 Comment: 
 
 Filename: langchain_google_cloud_sql_pg/version.py
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.0.dist-info/LICENSE
+Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.0.dist-info/METADATA
+Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.0.dist-info/WHEEL
+Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.0.dist-info/top_level.txt
+Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.0.dist-info/RECORD
+Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_cloud_sql_pg/engine.py

```diff
@@ -55,15 +55,15 @@
             The email address associated with the current authenticated IAM
             principal.
     """
     if not credentials.valid:
         request = google.auth.transport.requests.Request()
         credentials.refresh(request)
     if hasattr(credentials, "_service_account_email"):
-        email = credentials._service_account_email
+        return credentials._service_account_email.replace(".gserviceaccount.com", "")
     # call OAuth2 api to get IAM principal email associated with OAuth2 token
     url = f"https://oauth2.googleapis.com/tokeninfo?access_token={credentials.token}"
     async with aiohttp.ClientSession() as client:
         response = await client.get(url, raise_for_status=True)
         response_json: Dict = await response.json()
         email = response_json.get("email")
     if email is None:
```

## langchain_google_cloud_sql_pg/vectorstore.py

```diff
@@ -457,15 +457,15 @@
         filter: Optional[str] = None,
     ) -> List[Any]:
         k = k if k else self.k
         operator = self.distance_strategy.operator
         search_function = self.distance_strategy.search_function
 
         filter = f"WHERE {filter}" if filter else ""
-        stmt = f"SELECT *, {search_function}({self.embedding_column}, '{embedding}') as distance FROM {self.table_name} {filter} ORDER BY {self.embedding_column} {operator} '{embedding}' LIMIT {k};"
+        stmt = f"SELECT *, {search_function}({self.embedding_column}, '{embedding}') as distance FROM \"{self.table_name}\" {filter} ORDER BY {self.embedding_column} {operator} '{embedding}' LIMIT {k};"
         if self.index_query_options:
             await self.engine._aexecute(
                 f"SET LOCAL {self.index_query_options.to_string()};"
             )
         results = await self.engine._afetch(stmt)
         return results
 
@@ -738,15 +738,15 @@
             await self.adrop_vector_index()
             return
 
         filter = f"WHERE ({index.partial_indexes})" if index.partial_indexes else ""
         params = "WITH " + index.index_options()
         function = index.distance_strategy.index_function
         name = name or index.name
-        stmt = f"CREATE INDEX {'CONCURRENTLY' if concurrently else ''} {name} ON {self.table_name} USING {index.index_type} ({self.embedding_column} {function}) {params} {filter};"
+        stmt = f'CREATE INDEX {"CONCURRENTLY" if concurrently else ""} {name} ON "{self.table_name}" USING {index.index_type} ({self.embedding_column} {function}) {params} {filter};'
         if concurrently:
             await self.engine._aexecute_outside_tx(stmt)
         else:
             await self.engine._aexecute(stmt)
 
     async def areindex(self, index_name: str = DEFAULT_INDEX_NAME) -> None:
         query = f"REINDEX INDEX {index_name};"
```

## langchain_google_cloud_sql_pg/version.py

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

## Comparing `langchain_google_cloud_sql_pg-0.4.0.dist-info/LICENSE` & `langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_cloud_sql_pg-0.4.0.dist-info/METADATA` & `langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-cloud-sql-pg
-Version: 0.4.0
+Version: 0.4.1
 Summary: LangChain integrations for Google Cloud SQL for PostgreSQL
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -223,15 +223,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: cloud-sql-python-connector[asyncpg] <2.0.0,>=1.7.0
 Requires-Dist: langchain-core <2.0.0,>=0.1.1
 Requires-Dist: langchain-community <0.1.0,>=0.0.18
 Requires-Dist: numpy <2.0.0,>=1.24.4
 Requires-Dist: pgvector <1.0.0,>=0.2.5
-Requires-Dist: SQLAlchemy <3.0.0,>=2.0.25
+Requires-Dist: SQLAlchemy[asyncio] <3.0.0,>=2.0.25
 Provides-Extra: test
 Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
 Requires-Dist: mypy ==1.9.0 ; extra == 'test'
 Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
 
@@ -291,26 +291,26 @@
 ^^^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-bigquery
+    <your-env>/bin/pip install langchain-google-cloud-sql-pg
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
     <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-bigquery
+    <your-env>\Scripts\pip.exe install langchain-google-cloud-sql-pg
 
 
 Example Usage
 -------------
 
 Code samples and snippets live in the `samples/`_ folder.
 
@@ -329,15 +329,15 @@
 
 
         engine = PostgresEngine.from_instance("project-id", "region", "my-instance", "my-database")
         engine.init_vectorstore_table(
             table_name="my-table",
             vector_size=768,  # Vector size for `VertexAIEmbeddings()`
         )
-        embeddings_service = VertexAIEmbeddings()
+        embeddings_service = VertexAIEmbeddings(model_name="textembedding-gecko@003")
         vectorstore = PostgresVectorStore.create_sync(
             engine,
             table_name="my-table",
             embeddings=embedding_service
         )
 
 See the full `Vector Store`_ tutorial.
@@ -383,16 +383,16 @@
             session_id="my-session_id"
         )
 
 See the full `Chat Message History`_ tutorial.
 
 .. _`Chat Message History`: https://github.com/googleapis/langchain-google-cloud-sql-pg-python/tree/main/docs/chat_message_history.ipynb
 
-Contributing
-~~~~~~~~~~~~
+Contributions
+~~~~~~~~~~~~~
 
 Contributions to this library are always welcome and highly encouraged.
 
 See `CONTRIBUTING`_ for more information how to get started.
 
 Please note that this project is released with a Contributor Code of Conduct. By participating in
 this project you agree to abide by its terms. See `Code of Conduct`_ for more
```

## Comparing `langchain_google_cloud_sql_pg-0.4.0.dist-info/RECORD` & `langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 langchain_google_cloud_sql_pg/__init__.py,sha256=7sz60HhKzCg_1f3mrLbyYgnAkjvhMo3xKt9S_bm1A0A,1034
 langchain_google_cloud_sql_pg/chat_message_history.py,sha256=P5tDXVUF7o_yLNAMQ7VTzmKmIBR74FDs6DTI-Jh7BEg,4964
-langchain_google_cloud_sql_pg/engine.py,sha256=YvYOuGJMLyhhMvIqvjAN4oHr1IkuXj5t2l-B2GgRVpI,14672
+langchain_google_cloud_sql_pg/engine.py,sha256=BAQQbsIlUQ2IxMMsO1_YtBmgYpTJfjTCE4lmbV0wmvk,14707
 langchain_google_cloud_sql_pg/indexes.py,sha256=UYbXMcZXBvaU7FFa7IjhXvBvCuDdxr0Tq2pgyQrKVtU,2580
 langchain_google_cloud_sql_pg/loader.py,sha256=G2yI3QiS2mHxYSUgVIQPDhgCBw1-ARlCvLZJrEQt-HM,17740
 langchain_google_cloud_sql_pg/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_cloud_sql_pg/vectorstore.py,sha256=hF0aCvflIdf1fX4qhqh4VZl3LbOTnbN89i48ojP40ZU,29570
-langchain_google_cloud_sql_pg/version.py,sha256=4bSA5dHz2_cH6tUofCfR5Womm5Lr6yEUsIN6hLlJIeo,622
-langchain_google_cloud_sql_pg-0.4.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_cloud_sql_pg-0.4.0.dist-info/METADATA,sha256=F3uMqvll0s1m5Bd_o_VY0RhrGH4nwJtF4wgPhCu2bg0,20296
-langchain_google_cloud_sql_pg-0.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_cloud_sql_pg-0.4.0.dist-info/top_level.txt,sha256=B0E28f-0MRQQTiqWKALorDWbFG2scm-DwzRuYdQHOOA,30
-langchain_google_cloud_sql_pg-0.4.0.dist-info/RECORD,,
+langchain_google_cloud_sql_pg/vectorstore.py,sha256=-zKkgpoAGTfF7y3tbS0AxihF6UW_uDjd5Rzoxp2KD3g,29576
+langchain_google_cloud_sql_pg/version.py,sha256=lyhj8ZqCp_c181C39EsQQ0JVsjJhyv5RVg17Lp_sKdg,622
+langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA,sha256=vUCL_7shfxeje30eNUxid_OkcU3pnAOc4LkDvuePxek,20359
+langchain_google_cloud_sql_pg-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_cloud_sql_pg-0.4.1.dist-info/top_level.txt,sha256=B0E28f-0MRQQTiqWKALorDWbFG2scm-DwzRuYdQHOOA,30
+langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD,,
```

