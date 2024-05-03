# Comparing `tmp/bigdata_client-0.1.0.tar.gz` & `tmp/bigdata_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigdata_client-0.1.0.tar", max compression
+gzip compressed data, was "bigdata_client-0.2.0.tar", max compression
```

## Comparing `bigdata_client-0.1.0.tar` & `bigdata_client-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0      358 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/README.md
--rw-r--r--   0        0        0      155 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/__init__.py
--rw-r--r--   0        0        0     6526 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/advanced_search_query.py
--rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/__init__.py
--rw-r--r--   0        0        0      888 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/knowledge_graph.py
--rw-r--r--   0        0        0     8304 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/search.py
--rw-r--r--   0        0        0     2985 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/uploads.py
--rw-r--r--   0        0        0      975 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/watchlist.py
--rw-r--r--   0        0        0     6464 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/auth.py
--rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/__init__.py
--rw-r--r--   0        0        0     2256 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/base_instance.py
--rw-r--r--   0        0        0     4166 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/dev_instance.py
--rw-r--r--   0        0        0     3650 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/production_instance.py
--rw-r--r--   0        0        0      853 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/exceptions.py
--rw-r--r--   0        0        0      245 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/models.py
--rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/__init__.py
--rw-r--r--   0        0        0      243 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/base.py
--rw-r--r--   0        0        0     1008 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/password.py
--rw-r--r--   0        0        0     2510 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/token_manager.py
--rw-r--r--   0        0        0     2040 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/token_manager_factory.py
--rw-r--r--   0        0        0    13702 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/connection.py
--rw-r--r--   0        0        0      475 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/connection_protocol.py
--rw-r--r--   0        0        0      154 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/constants.py
--rw-r--r--   0        0        0     4501 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/daterange.py
--rw-r--r--   0        0        0     1234 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/entity_types.py
--rw-r--r--   0        0        0      664 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/enum_utils.py
--rw-r--r--   0        0        0       82 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/errors.py
--rw-r--r--   0        0        0      196 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/file_status.py
--rw-r--r--   0        0        0      513 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/jwt.py
--rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/__init__.py
--rw-r--r--   0        0        0    21160 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/advanced_search_query.py
--rw-r--r--   0        0        0     1181 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/comentions.py
--rw-r--r--   0        0        0     5961 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/entities.py
--rw-r--r--   0        0        0     1094 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/languages.py
--rw-r--r--   0        0        0     3841 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/parse.py
--rw-r--r--   0        0        0     1710 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/search.py
--rw-r--r--   0        0        0     2280 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/sources.py
--rw-r--r--   0        0        0      855 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/story.py
--rw-r--r--   0        0        0     2180 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/topics.py
--rw-r--r--   0        0        0     6580 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/uploads.py
--rw-r--r--   0        0        0     2820 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/watchlists.py
--rw-r--r--   0        0        0     4773 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/old_auth.py
--rw-r--r--   0        0        0      177 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/pdf_utils.py
--rw-r--r--   0        0        0      970 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/query.py
--rw-r--r--   0        0        0      251 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/query_type.py
--rw-r--r--   0        0        0     7859 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/search.py
--rw-r--r--   0        0        0    15123 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/services.py
--rw-r--r--   0        0        0     1086 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/settings.py
--rw-r--r--   0        0        0    12157 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/simple_search_query.py
--rw-r--r--   0        0        0     2022 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/story.py
--rw-r--r--   0        0        0      465 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/user_agent.py
--rw-r--r--   0        0        0     1359 2024-04-26 08:25:50.395026 bigdata_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      358 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/README.md
+-rw-r--r--   0        0        0      155 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/__init__.py
+-rw-r--r--   0        0        0     6556 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/advanced_search_query.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/knowledge_graph.py
+-rw-r--r--   0        0        0     8329 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/search.py
+-rw-r--r--   0        0        0     2985 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/uploads.py
+-rw-r--r--   0        0        0      975 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/watchlist.py
+-rw-r--r--   0        0        0     6464 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/auth.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/__init__.py
+-rw-r--r--   0        0        0     2256 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/base_instance.py
+-rw-r--r--   0        0        0     4166 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/dev_instance.py
+-rw-r--r--   0        0        0     3650 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/production_instance.py
+-rw-r--r--   0        0        0      853 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/exceptions.py
+-rw-r--r--   0        0        0      245 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/models.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/base.py
+-rw-r--r--   0        0        0     1008 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/password.py
+-rw-r--r--   0        0        0     2510 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/token_manager.py
+-rw-r--r--   0        0        0     2040 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/token_manager_factory.py
+-rw-r--r--   0        0        0    13702 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/connection.py
+-rw-r--r--   0        0        0      475 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/connection_protocol.py
+-rw-r--r--   0        0        0      154 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/constants.py
+-rw-r--r--   0        0        0     4501 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/daterange.py
+-rw-r--r--   0        0        0     1234 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/entity_types.py
+-rw-r--r--   0        0        0      664 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/enum_utils.py
+-rw-r--r--   0        0        0       82 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/errors.py
+-rw-r--r--   0        0        0      196 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/file_status.py
+-rw-r--r--   0        0        0      513 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/jwt.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/__init__.py
+-rw-r--r--   0        0        0    21160 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/advanced_search_query.py
+-rw-r--r--   0        0        0     1181 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/comentions.py
+-rw-r--r--   0        0        0     5961 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/entities.py
+-rw-r--r--   0        0        0     1094 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/languages.py
+-rw-r--r--   0        0        0     3841 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/parse.py
+-rw-r--r--   0        0        0     1710 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/search.py
+-rw-r--r--   0        0        0     2280 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/sources.py
+-rw-r--r--   0        0        0      876 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/story.py
+-rw-r--r--   0        0        0     2180 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/topics.py
+-rw-r--r--   0        0        0     6580 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/uploads.py
+-rw-r--r--   0        0        0     2820 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/watchlists.py
+-rw-r--r--   0        0        0     4773 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/old_auth.py
+-rw-r--r--   0        0        0      177 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/pdf_utils.py
+-rw-r--r--   0        0        0      970 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/query.py
+-rw-r--r--   0        0        0      251 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/query_type.py
+-rw-r--r--   0        0        0     6746 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/search.py
+-rw-r--r--   0        0        0    14376 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/services.py
+-rw-r--r--   0        0        0     1086 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/settings.py
+-rw-r--r--   0        0        0     2091 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/story.py
+-rw-r--r--   0        0        0      465 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/user_agent.py
+-rw-r--r--   0        0        0     1359 2024-05-03 16:46:20.953843 bigdata_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.2.0/PKG-INFO
```

### Comparing `bigdata_client-0.1.0/bigdata/advanced_search_query.py` & `bigdata_client-0.2.0/bigdata/advanced_search_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     scope: FileType = FileType.ALL
 
     def make_copy(self) -> "AdvancedSearchQuery":
         return AdvancedSearchQuery(
             date_range=self.date_range,
             query=self.query.make_copy(),  # TODO: make copy of this too?
             sortby=self.sortby,
+            scope=self.scope,
         )
 
     def to_query_clusters_api_request(self, page: int) -> QueryClustersRequest:
         """
         Used when composing the request to perform a search using the
         /query-clusters endpoint.
         The difference between this method and to_save_search_request is that
```

### Comparing `bigdata_client-0.1.0/bigdata/api/knowledge_graph.py` & `bigdata_client-0.2.0/bigdata/api/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/api/search.py` & `bigdata_client-0.2.0/bigdata/api/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
     source_name: str = Field(validation_alias="srcName")
     source_rank: int
     language: str
 
     class ChunkedStoryResponseSentence(BaseModel):
         text: str
         cnum: int
+        relevance: float
 
         class StoryResponseEntity(BaseModel):
             key: str
             start: int
             end: int
             queryType: QueryType
```

### Comparing `bigdata_client-0.1.0/bigdata/api/uploads.py` & `bigdata_client-0.2.0/bigdata/api/uploads.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/api/watchlist.py` & `bigdata_client-0.2.0/bigdata/api/watchlist.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/auth.py` & `bigdata_client-0.2.0/bigdata/auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/clerk/authenticators/base_instance.py` & `bigdata_client-0.2.0/bigdata/clerk/authenticators/base_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/clerk/authenticators/dev_instance.py` & `bigdata_client-0.2.0/bigdata/clerk/authenticators/dev_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/clerk/authenticators/production_instance.py` & `bigdata_client-0.2.0/bigdata/clerk/authenticators/production_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/clerk/exceptions.py` & `bigdata_client-0.2.0/bigdata/clerk/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/password.py` & `bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/password.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/clerk/token_manager.py` & `bigdata_client-0.2.0/bigdata/clerk/token_manager.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/clerk/token_manager_factory.py` & `bigdata_client-0.2.0/bigdata/clerk/token_manager_factory.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/connection.py` & `bigdata_client-0.2.0/bigdata/connection.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/daterange.py` & `bigdata_client-0.2.0/bigdata/daterange.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/entity_types.py` & `bigdata_client-0.2.0/bigdata/entity_types.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/enum_utils.py` & `bigdata_client-0.2.0/bigdata/enum_utils.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/jwt.py` & `bigdata_client-0.2.0/bigdata/jwt.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/advanced_search_query.py` & `bigdata_client-0.2.0/bigdata/models/advanced_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/comentions.py` & `bigdata_client-0.2.0/bigdata/models/comentions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/entities.py` & `bigdata_client-0.2.0/bigdata/models/entities.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/languages.py` & `bigdata_client-0.2.0/bigdata/models/languages.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/parse.py` & `bigdata_client-0.2.0/bigdata/models/parse.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/search.py` & `bigdata_client-0.2.0/bigdata/models/search.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/sources.py` & `bigdata_client-0.2.0/bigdata/models/sources.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/story.py` & `bigdata_client-0.2.0/bigdata/models/story.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,7 +47,8 @@
     A chunk of text representing a contextual unit within the document
     """
 
     text: str
     chunk: int
     entities: list[StorySentenceEntity]
     sentences: list[StorySentence]
+    relevance: float
```

### Comparing `bigdata_client-0.1.0/bigdata/models/topics.py` & `bigdata_client-0.2.0/bigdata/models/topics.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/uploads.py` & `bigdata_client-0.2.0/bigdata/models/uploads.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/models/watchlists.py` & `bigdata_client-0.2.0/bigdata/models/watchlists.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/old_auth.py` & `bigdata_client-0.2.0/bigdata/old_auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/query.py` & `bigdata_client-0.2.0/bigdata/query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/bigdata/search.py` & `bigdata_client-0.2.0/bigdata/search.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,64 +11,34 @@
 )
 from bigdata.connection import BigdataConnection
 from bigdata.constants import MAX_SEARCH_PAGES
 from bigdata.daterange import AbsoluteDateRange, RollingDateRange
 from bigdata.models.advanced_search_query import QueryComponent
 from bigdata.models.comentions import Comentions
 from bigdata.models.search import FileType, SortBy
-from bigdata.simple_search_query import SimpleSearchQuery
 from bigdata.story import Story
 
 
 class Search:
     """
     Class representing a search, saved or not.
     It allows you to perform searches.
     """
 
     def __init__(
         self,
         api: BigdataConnection,
-        # TODO: Change the type of this to something more generic
-        query: "SimpleSearchQuery",
+        query: AdvancedSearchQuery,
         id: Optional[str] = None,
         name: str = "",
     ):
-        self.api: BigdataConnection = api
+        self._api: BigdataConnection = api
         self.id: Optional[str] = id
         self.name: str = name
-        self.query: SimpleSearchQuery = query or SimpleSearchQuery()
-
-    @classmethod
-    def from_filters(
-        cls,
-        api: "BigdataConnection",
-        date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None,
-        keywords: Optional[list[str]] = None,
-        entities: Optional[list[str]] = None,
-        sources: Optional[list[str]] = None,
-        topics: Optional[list[str]] = None,
-        languages: Optional[list[str]] = None,
-        watchlists: Optional[list[str]] = None,
-        sortby: SortBy = SortBy.RELEVANCE,
-        scope: FileType = FileType.ALL,
-    ) -> "Search":
-        """Create a simplified search with just a set of filters"""
-        rpx_query = SimpleSearchQuery(
-            date_range=date_range,
-            keywords=keywords,
-            entities=entities,
-            sources=sources,
-            topics=topics,
-            languages=languages,
-            watchlists=watchlists,
-            sortby=sortby,
-            scope=scope,
-        )
-        return cls(api=api, query=rpx_query)
+        self.query: AdvancedSearchQuery = query
 
     @classmethod
     def from_query(
         cls,
         api: "BigdataConnection",
         query: QueryComponent,
         date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None,
@@ -81,15 +51,15 @@
         )
         return cls(api=api, query=rpx_query)
 
     @classmethod
     def from_saved_search_response(
         cls, api: BigdataConnection, response: SavedSearchResponse
     ):
-        simple_query = SimpleSearchQuery.from_saved_search_response(response.query)
+        simple_query = AdvancedSearchQuery.from_saved_search_response(response.query)
 
         return cls(
             api=api,
             query=simple_query,
             id=response.id,
             name=response.name,
             # TODO: Add the rest of the parameters like created_at, updated_at,
@@ -98,53 +68,53 @@
 
     def limit_stories(self, limit: int) -> Iterable[Story]:
         """Limit the number of stories returned by this search"""
         new = self.make_copy()
         return SearchResults(new, limit=limit)
 
     def get_comentions(self) -> Comentions:
-        if self.api is None:
+        if self._api is None:
             raise ValueError("The search object must have an API to get comentions.")
         request = self.query.to_discovery_panel_api_request()
-        response = self.api.query_discovery_panel(request)
+        response = self._api.query_discovery_panel(request)
         return Comentions.from_response(response)
 
     def make_copy(self):
         query = self.query.make_copy()
-        return Search(self.api, id=self.id, name=self.name, query=query)
+        return Search(self._api, id=self.id, name=self.name, query=query)
 
     def get_page(self, page: int = 1) -> QueryChunksResponse:
-        if self.api is None:
+        if self._api is None:
             raise ValueError("The search object must have an API to get pages.")
         request = self.query.to_query_chunks_api_request(page)
-        return self.api.query_chunks(request)
+        return self._api.query_chunks(request)
 
     def save(self, name: str):
-        if self.api is None:
+        if self._api is None:
             raise ValueError("The search object must have an API to save.")
         if self.id is None:
             # Create a new search
             request = SaveSearchRequest(
                 name=name, query=self.query.to_save_search_request()
             )
-            response = self.api.save_search(request)
+            response = self._api.save_search(request)
             self.id = response.id
         else:
             # Update an existing search
             request = UpdateSearchRequest(
                 name=name, query=self.query.to_save_search_request()
             )
-            self.api.update_search(request, self.id)
+            self._api.update_search(request, self.id)
 
     def delete(self):
-        if self.api is None:
+        if self._api is None:
             raise ValueError("The search object must have an API to delete.")
         if self.id is None:
             raise ValueError("The search object is not saved.")
-        self.api.delete_search(self.id)
+        self._api.delete_search(self.id)
         self.id = None
 
     @property
     def is_saved(self) -> bool:
         return self.id is not None
```

### Comparing `bigdata_client-0.1.0/bigdata/services.py` & `bigdata_client-0.2.0/bigdata/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     AutosuggestedSavedSearch,
     EntityTypes,
     KnowledgeGraphTypes,
 )
 from bigdata.models.search import FileType, SortBy
 from bigdata.models.sources import Source
 from bigdata.models.topics import Topic
-from bigdata.models.uploads import File, UploadQuota
+from bigdata.models.uploads import File
 from bigdata.models.watchlists import Watchlist
 from bigdata.pdf_utils import is_pdf_file
 from bigdata.query_type import QueryType
 from bigdata.search import Search
 from bigdata.settings import BigdataAuthType, settings
 
 CONCURRENT_AUTOSUGGEST_REQUESTS_LIMIT = 10
@@ -71,42 +71,42 @@
             auth = old_auth.Auth.from_username_and_password(username, password)
 
         if bigdata_api_url is None:
             bigdata_api_url = str(settings.BIGDATA_API_URL)
         if upload_api_url is None:
             upload_api_url = str(settings.UPLOAD_API_URL)
 
-        self.api = BigdataConnection(auth, bigdata_api_url)
-        self.upload_api = UploadsConnection(auth, upload_api_url)
-        self.knowledge_graph = KnowledgeGraph(self.api)
-        self.content_search = ContentSearch(self.api)
-        self.watchlists = Watchlists(self.api)
-        self.uploads = Uploads(self.upload_api)
+        self._api = BigdataConnection(auth, bigdata_api_url)
+        self._upload_api = UploadsConnection(auth, upload_api_url)
+        self.knowledge_graph = KnowledgeGraph(self._api)
+        self.content_search = ContentSearch(self._api)
+        self.watchlists = Watchlists(self._api)
+        self.uploads = Uploads(self._upload_api)
 
 
 class KnowledgeGraph:
     """For finding entities, sources and topics"""
 
     def __init__(self, api_connection: BigdataConnectionProtocol):
-        self.api = api_connection
+        self._api = api_connection
 
     def autosuggest(
         self, values: list[str], /, limit=20
     ) -> dict[str, list[KnowledgeGraphTypes]]:
         """
         Searches for entities, sources, topics, searches and watchlists
         Args:
             values: Searched items
             limit: Upper limit for each result
 
         Returns:
             Dictionary with the searched terms as keys each with a list of results.
         """
 
-        api_response = self.api.autosuggest(
+        api_response = self._api.autosuggest(
             AutosuggestRequests(root=values),
             limit=limit,
         )
 
         # Exclude macros and saved searches from response
         api_response = self._exclude_macros_and_saved_searches(api_response)
 
@@ -141,201 +141,176 @@
         return self._get_by_ids(ids, QueryType.TOPIC)
 
     def get_languages(self, ids: list[str], /) -> list[Optional[Language]]:
         """Retrieve a list of languages by its ids."""
         return self._get_by_ids(ids, QueryType.LANGUAGE)
 
     def _get_by_ids(self, ids: list[str], query_type: QueryType) -> list:
-        api_response = self.api.by_ids(
+        api_response = self._api.by_ids(
             ByIdsRequest.model_validate(
                 [{"key": id_, "queryType": query_type} for id_ in ids]
             )
         )
         return [api_response.root.get(id_) for id_ in ids]
 
 
 class Watchlists:
     """For finding, iterating and doing operations with watchlist objects"""
 
     def __init__(self, api_connection: BigdataConnectionProtocol):
-        self.api = api_connection
+        self._api = api_connection
 
     def get(self, id_: str, /) -> Watchlist:
         """Retrieve a watchlist by its id."""
-        api_response = self.api.get_single_watchlist(id_)
+        api_response = self._api.get_single_watchlist(id_)
         watchlist = Watchlist(
             id=api_response.id,
             name=api_response.name,
             date_created=api_response.date_created,
             last_updated=api_response.last_updated,
             items=api_response.items,
             # Keep track of the api_connection within the Watchlist instance
-            _api=self.api,
+            _api=self._api,
         )
 
         return watchlist
 
     def list(self) -> list[Watchlist]:
         """Retrieve all watchlist objects for the current user."""
-        api_response = self.api.get_all_watchlists()
+        api_response = self._api.get_all_watchlists()
         all_watchlist = [
             Watchlist(
                 id=base_watchlist.id,
                 name=base_watchlist.name,
                 date_created=base_watchlist.date_created,
                 last_updated=base_watchlist.last_updated,
                 items=None,
                 # Keep track of the api_connection within the Watchlist instance
-                _api=self.api,
+                _api=self._api,
             )
             for base_watchlist in api_response.root
         ]
 
         return all_watchlist
 
     def create(self, name: str, items: List[str]) -> Watchlist:
         """Creates a new watchlist in the system."""
-        api_response = self.api.create_watchlist(
+        api_response = self._api.create_watchlist(
             CreateWatchlistRequest(name=name, items=items)
         )
         return Watchlist(
             id=api_response.id,
             name=api_response.name,
             date_created=api_response.date_created,
             last_updated=api_response.last_updated,
             items=api_response.items,
             # Keep track of the api_connection within the Watchlist instance
-            _api=self.api,
+            _api=self._api,
         )
 
     def delete(self, id_: str, /) -> str:
         """Delete a watchlist by its id."""
-        api_response = self.api.delete_watchlist(id_)
+        api_response = self._api.delete_watchlist(id_)
         return api_response.id
 
     def update(self, id_: str, /, name=None, items=None) -> Watchlist:
         """Update a watchlist by its id."""
-        api_response = self.api.patch_watchlist(
+        api_response = self._api.patch_watchlist(
             id_, UpdateWatchlistRequest(name=name, items=items)
         )
         return Watchlist(
             id=api_response.id,
             name=api_response.name,
             date_created=api_response.date_created,
             last_updated=api_response.last_updated,
             items=api_response.items,
             # Keep track of the api_connection within the Watchlist instance
-            _api=self.api,
+            _api=self._api,
         )
 
 
 class ContentSearch:
     def __init__(self, api_connection: BigdataConnection):
-        self.api = api_connection
+        self._api = api_connection
 
-    # Search content
-
-    def new_search(
+    def new_from_query(
         self,
-        /,
+        query: QueryComponent,
         date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None,
-        keywords: Optional[list[str]] = None,
-        entities: Optional[list[str]] = None,
-        sources: Optional[list[str]] = None,
-        topics: Optional[list[str]] = None,
-        languages: Optional[list[str]] = None,
-        watchlists: Optional[list[str]] = None,
-        sortby: Optional[SortBy] = SortBy.RELEVANCE,
+        sortby: SortBy = SortBy.RELEVANCE,
         scope: FileType = FileType.ALL,
     ) -> Search:
         """
         Creates a new search object that allows you to perform a search on
-        keywords and entity_ids.
+        keywords, entities, etc.
 
         Example usage:
 
-        >>> search = bigdata.content_search.new_search(
-        ...    keywords=["tesla"],
-        ...    entities=["228D42"]
+        >>> query = Entity("228D42") & Keyword("tesla")  # doctest: +SKIP
+        >>> search = bigdata.content_search.new_from_query(
+        ...    query,
+        ...    date_range=RrollingDateRange.LAST_WEEK,
+        ...    sortby=SortBy.RELEVANCE,
+        ...    scope=FileType.ALL
         ... )                               # doctest: +SKIP
         >>> search.save()                   # doctest: +SKIP
         >>> for story in search.limit(100): # doctest: +SKIP
         >>>     print(story)                # doctest: +SKIP
         >>> print(search.get_summary())     # doctest: +SKIP
         >>> search.delete()                 # doctest: +SKIP
         """
-        return Search.from_filters(
-            api=self.api,
-            date_range=date_range,
-            keywords=keywords,
-            entities=entities,
-            sources=sources,
-            topics=topics,
-            languages=languages,
-            watchlists=watchlists,
-            sortby=sortby,
-            scope=scope,
-        )
-
-    def new_from_query(
-        self,
-        query: QueryComponent,
-        date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None,
-        sortby: SortBy = SortBy.RELEVANCE,
-        scope: FileType = FileType.ALL,
-    ) -> Search:
         return Search.from_query(
-            self.api, query, date_range=date_range, sortby=sortby, scope=scope
+            self._api, query, date_range=date_range, sortby=sortby, scope=scope
         )
 
     def get(self, id_, /) -> Search:
         """Retrieve a saved search by its id."""
-        response = self.api.get_search(id_)
-        return Search.from_saved_search_response(self.api, response)
+        response = self._api.get_search(id_)
+        return Search.from_saved_search_response(self._api, response)
 
     def list(self) -> list[Search]:
         """Retrieve all saved searches for the current user."""
-        list_response = self.api.list_searches()
+        list_response = self._api.list_searches()
         searches = []
         for search in list_response.results:
             try:
-                response = self.api.get_search(search.id)
+                response = self._api.get_search(search.id)
             except NotImplementedError as e:
                 print(
                     f"Skipping search {search.id} because it has an unsupported expression type"
                 )
                 continue
-            searches.append(Search.from_saved_search_response(self.api, response))
+            searches.append(Search.from_saved_search_response(self._api, response))
         return searches
 
     def delete(self, id_, /):
         """Delete a saved search by its id."""
-        self.api.delete_search(id_)
+        self._api.delete_search(id_)
 
 
 class Uploads:
     """For managing internal uploads. Searching will be done through content"""
 
     def __init__(self, api_connection: UploadsConnection):
-        self.api = api_connection
+        self._api = api_connection
 
     def get(self, id_, /) -> File:
         """Retrieve a file by its id."""
         response = None
         while response is None:
             try:
-                response = self.api.get_file(id_)
+                response = self._api.get_file(id_)
             except requests.exceptions.HTTPError as e:
                 # While unavailable, keep trying
                 if e.response.status_code == 425:
                     time.sleep(1)
                     continue
                 raise e
         return File(
-            _api=self.api,
+            _api=self._api,
             id=response.id,
             name=response.name,
             status=response.status,
             uploaded_at=response.uploaded_at,
             raw_size=response.raw_size,
             folder_id=response.folder_id,
             trashed=response.trashed,
@@ -353,26 +328,26 @@
         folder_id: Optional[str] = None,
         page_size: Optional[int] = None,
     ) -> list[File]:
         """Retrieve all documents for the current user."""
         date_range = (
             AbsoluteDateRange(start_date, end_date) if start_date or end_date else None
         )
-        response = self.api.list_files(
+        response = self._api.list_files(
             date_range=date_range,
             tags=tags,
             status=status,
             file_name=file_name,
             folder_id=folder_id,
             page_size=page_size,
         )
         docs = []
         for upload in response.results:
             doc = File(
-                _api=self.api,
+                _api=self._api,
                 id=upload.id,
                 name=upload.name,
                 status=upload.status,
                 uploaded_at=upload.uploaded_at,
                 raw_size=upload.raw_size,
                 folder_id=upload.folder_id,
                 trashed=upload.trashed,
@@ -408,18 +383,16 @@
         post_file_request = PostFileRequest(
             filename=filename,
             folder_id=None,
             source_url=None,
             upload_mode=None,
             properties=properties,
         )
-        post_file_request = self.api.post_file(post_file_request)
+        post_file_request = self._api.post_file(post_file_request)
 
         with open(path, "rb") as file:
             upload_file(post_file_request.location, file)
         return self.get(post_file_request.file_id)
 
     def delete(self, id_, /):
         """Delete a file by its id."""
-        self.api.delete_file(id_)
-
-    # TODO: add methods to manage folders etc
+        self._api.delete_file(id_)
```

### Comparing `bigdata_client-0.1.0/bigdata/settings.py` & `bigdata_client-0.2.0/bigdata/settings.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.1.0/pyproject.toml` & `bigdata_client-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "bigdata-client"
 packages = [
     { include = "bigdata" },
 ]
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = [
     "Bigdata Team <support@bigdata.com>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `bigdata_client-0.1.0/PKG-INFO` & `bigdata_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdata-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Bigdata Team
 Author-email: support@bigdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

