# Comparing `tmp/cognee-0.1.6.tar.gz` & `tmp/cognee-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognee-0.1.6.tar", max compression
+gzip compressed data, was "cognee-0.1.7.tar", max compression
```

## Comparing `cognee-0.1.6.tar` & `cognee-0.1.7.tar`

### file list

```diff
@@ -1,170 +1,168 @@
--rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.6/LICENSE
--rw-r--r--   0        0        0     3668 2024-04-24 17:34:59.318133 cognee-0.1.6/README.md
--rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.6/cognee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.6/cognee/api/__init__.py
--rw-r--r--   0        0        0     4370 2024-04-25 22:16:19.632624 cognee-0.1.6/cognee/api/client.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.6/cognee/api/v1/__init__.py
--rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.6/cognee/api/v1/add/__init__.py
--rw-r--r--   0        0        0     4716 2024-04-25 22:16:19.633201 cognee-0.1.6/cognee/api/v1/add/add.py
--rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.6/cognee/api/v1/add/add_standalone.py
--rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.6/cognee/api/v1/add/remember.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633260 cognee-0.1.6/cognee/api/v1/cognify/__init__.py
--rw-r--r--   0        0        0     7522 2024-04-26 16:35:59.726003 cognee-0.1.6/cognee/api/v1/cognify/cognify.py
--rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.6/cognee/api/v1/config/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-24 17:34:59.319404 cognee-0.1.6/cognee/api/v1/config/config.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633793 cognee-0.1.6/cognee/api/v1/datasets/__init__.py
--rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.6/cognee/api/v1/datasets/datasets.py
--rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.6/cognee/api/v1/prune/__init__.py
--rw-r--r--   0        0        0      965 2024-04-20 17:06:04.933673 cognee-0.1.6/cognee/api/v1/prune/prune.py
--rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.6/cognee/api/v1/search/__init__.py
--rw-r--r--   0        0        0     3611 2024-04-25 22:16:19.634363 cognee-0.1.6/cognee/api/v1/search/search.py
--rw-r--r--   0        0        0     6489 2024-04-25 22:16:19.634966 cognee-0.1.6/cognee/config.py
--rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.6/cognee/fetch_secret.py
--rw-r--r--   0        0        0     7705 2024-04-26 16:35:54.784457 cognee-0.1.6/cognee/infrastructure/InfrastructureConfig.py
--rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.6/cognee/infrastructure/__init__.py
--rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.6/cognee/infrastructure/data/__init__.py
--rw-r--r--   0        0        0     4456 2024-04-24 17:34:59.321526 cognee-0.1.6/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635699 cognee-0.1.6/cognee/infrastructure/data/chunking/__init__.py
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.6/cognee/infrastructure/data/models/Data.py
--rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.6/cognee/infrastructure/data/models/Dataset.py
--rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.6/cognee/infrastructure/data/models/DatasetData.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.6/cognee/infrastructure/data/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635851 cognee-0.1.6/cognee/infrastructure/data/utils/__init__.py
--rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.6/cognee/infrastructure/data/utils/extract_keywords.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.6/cognee/infrastructure/databases/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.6/cognee/infrastructure/databases/graph/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-26 16:35:59.726347 cognee-0.1.6/cognee/infrastructure/databases/graph/get_graph_client.py
--rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.6/cognee/infrastructure/databases/graph/graph_db_interface.py
--rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.6/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
--rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.6/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.6/cognee/infrastructure/databases/graph/networkx/__init__.py
--rw-r--r--   0        0        0     5302 2024-04-26 16:35:59.726597 cognee-0.1.6/cognee/infrastructure/databases/graph/networkx/adapter.py
--rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.6/cognee/infrastructure/databases/relational/DatabaseEngine.py
--rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.6/cognee/infrastructure/databases/relational/ModelBase.py
--rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.6/cognee/infrastructure/databases/relational/__init__.py
--rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.6/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637021 cognee-0.1.6/cognee/infrastructure/databases/relational/duckdb/__init__.py
--rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.6/cognee/infrastructure/databases/relational/relational_db_interface.py
--rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.6/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.6/cognee/infrastructure/databases/relational/sqlite/__init__.py
--rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.6/cognee/infrastructure/databases/relational/utils/__init__.py
--rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.6/cognee/infrastructure/databases/relational/utils/with_rollback.py
--rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.6/cognee/infrastructure/databases/vector/__init__.py
--rw-r--r--   0        0        0     1410 2024-04-20 17:06:04.937392 cognee-0.1.6/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
--rw-r--r--   0        0        0      237 2024-03-29 12:58:54.564681 cognee-0.1.6/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637164 cognee-0.1.6/cognee/infrastructure/databases/vector/embeddings/__init__.py
--rw-r--r--   0        0        0     2791 2024-04-26 16:35:54.784817 cognee-0.1.6/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py
--rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.6/cognee/infrastructure/databases/vector/models/CollectionConfig.py
--rw-r--r--   0        0        0      261 2024-04-26 13:17:36.397644 cognee-0.1.6/cognee/infrastructure/databases/vector/models/DataPoint.py
--rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.6/cognee/infrastructure/databases/vector/models/ScoredResult.py
--rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.6/cognee/infrastructure/databases/vector/models/VectorConfig.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637726 cognee-0.1.6/cognee/infrastructure/databases/vector/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637873 cognee-0.1.6/cognee/infrastructure/databases/vector/pinecone/__init__.py
--rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.6/cognee/infrastructure/databases/vector/pinecone/adapter.py
--rw-r--r--   0        0        0     6658 2024-04-26 16:44:50.179240 cognee-0.1.6/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
--rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.6/cognee/infrastructure/databases/vector/qdrant/__init__.py
--rw-r--r--   0        0        0     2195 2024-04-26 16:35:54.785670 cognee-0.1.6/cognee/infrastructure/databases/vector/vector_db_interface.py
--rw-r--r--   0        0        0     4965 2024-04-26 16:35:54.786038 cognee-0.1.6/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
--rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.6/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
--rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.6/cognee/infrastructure/files/__init__.py
--rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.6/cognee/infrastructure/files/add_file_to_storage.py
--rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.6/cognee/infrastructure/files/remove_file_from_storage.py
--rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.6/cognee/infrastructure/files/storage/LocalStorage.py
--rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.6/cognee/infrastructure/files/storage/StorageManager.py
--rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.6/cognee/infrastructure/files/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.6/cognee/infrastructure/files/utils/__init__.py
--rw-r--r--   0        0        0      392 2024-04-23 10:42:22.654946 cognee-0.1.6/cognee/infrastructure/files/utils/extract_text_from_file.py
--rw-r--r--   0        0        0      835 2024-04-23 10:42:22.655413 cognee-0.1.6/cognee/infrastructure/files/utils/get_file_metadata.py
--rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.6/cognee/infrastructure/files/utils/get_file_size.py
--rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.6/cognee/infrastructure/files/utils/guess_file_type.py
--rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.6/cognee/infrastructure/files/utils/is_text_content.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.6/cognee/infrastructure/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.6/cognee/infrastructure/llm/anthropic/__init__.py
--rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.6/cognee/infrastructure/llm/anthropic/adapter.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639301 cognee-0.1.6/cognee/infrastructure/llm/generic_llm_api/__init__.py
--rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.6/cognee/infrastructure/llm/generic_llm_api/adapter.py
--rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.6/cognee/infrastructure/llm/get_llm_client.py
--rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.6/cognee/infrastructure/llm/llm_interface.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.6/cognee/infrastructure/llm/openai/__init__.py
--rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.6/cognee/infrastructure/llm/openai/adapter.py
--rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.6/cognee/infrastructure/llm/prompts/__init__.py
--rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.6/cognee/infrastructure/llm/prompts/classify_content.txt
--rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.6/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
--rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.6/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
--rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.6/cognee/infrastructure/llm/prompts/read_query_prompt.py
--rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.6/cognee/infrastructure/llm/prompts/render_prompt.py
--rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.6/cognee/infrastructure/llm/prompts/summarize_content.txt
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.6/cognee/infrastructure/pipeline/models/Operation.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639465 cognee-0.1.6/cognee/infrastructure/pipeline/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.6/cognee/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.6/cognee/modules/cognify/__init__.py
--rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.6/cognee/modules/cognify/dataset.py
--rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.6/cognee/modules/cognify/evaluate.py
--rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.6/cognee/modules/cognify/graph/__init__.py
--rw-r--r--   0        0        0     1186 2024-04-25 22:16:19.640140 cognee-0.1.6/cognee/modules/cognify/graph/add_classification_nodes.py
--rw-r--r--   0        0        0     4928 2024-04-26 16:35:54.786327 cognee-0.1.6/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
--rw-r--r--   0        0        0     1138 2024-04-25 22:16:19.640702 cognee-0.1.6/cognee/modules/cognify/graph/add_cognitive_layers.py
--rw-r--r--   0        0        0     2065 2024-04-26 16:35:54.786614 cognee-0.1.6/cognee/modules/cognify/graph/add_data_chunks.py
--rw-r--r--   0        0        0      801 2024-04-26 16:35:59.727655 cognee-0.1.6/cognee/modules/cognify/graph/add_document_node.py
--rw-r--r--   0        0        0     1948 2024-04-26 16:35:54.786821 cognee-0.1.6/cognee/modules/cognify/graph/add_label_nodes.py
--rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.6/cognee/modules/cognify/graph/add_node_connections.py
--rw-r--r--   0        0        0      798 2024-04-25 09:42:30.766937 cognee-0.1.6/cognee/modules/cognify/graph/add_summary_nodes.py
--rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.6/cognee/modules/cognify/graph/create.py
--rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.6/cognee/modules/cognify/graph/initialize_graph.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.6/cognee/modules/cognify/llm/__init__.py
--rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.6/cognee/modules/cognify/llm/resolve_cross_graph_references.py
--rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.6/cognee/modules/cognify/test.py
--rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.6/cognee/modules/cognify/train.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641213 cognee-0.1.6/cognee/modules/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641372 cognee-0.1.6/cognee/modules/data/extraction/__init__.py
--rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.6/cognee/modules/data/extraction/extract_categories.py
--rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.6/cognee/modules/data/extraction/extract_cognitive_layers.py
--rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.6/cognee/modules/data/extraction/extract_summary.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641459 cognee-0.1.6/cognee/modules/data/extraction/knowledge_graph/__init__.py
--rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.6/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
--rw-r--r--   0        0        0     1102 2024-04-25 09:42:30.767456 cognee-0.1.6/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
--rw-r--r--   0        0        0     4740 2024-04-25 22:16:19.641944 cognee-0.1.6/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
--rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.6/cognee/modules/data/get_cognitive_layers.py
--rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.6/cognee/modules/data/get_content_categories.py
--rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.6/cognee/modules/data/get_content_summary.py
--rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.6/cognee/modules/data/get_layer_graphs.py
--rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.6/cognee/modules/discovery/__init__.py
--rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.6/cognee/modules/discovery/discover_directory_datasets.py
--rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.6/cognee/modules/ingestion/__init__.py
--rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.6/cognee/modules/ingestion/add_data_to_dataset.py
--rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.6/cognee/modules/ingestion/classify.py
--rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.6/cognee/modules/ingestion/data_types/BinaryData.py
--rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.6/cognee/modules/ingestion/data_types/IngestionData.py
--rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.6/cognee/modules/ingestion/data_types/TextData.py
--rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.6/cognee/modules/ingestion/data_types/__init__.py
--rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.6/cognee/modules/ingestion/exceptions.py
--rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.6/cognee/modules/ingestion/identify.py
--rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.6/cognee/modules/ingestion/save.py
--rw-r--r--   0        0        0        0 2024-04-26 16:35:54.786961 cognee-0.1.6/cognee/modules/memory/__init__.py
--rw-r--r--   0        0        0       55 2024-04-26 16:35:54.787188 cognee-0.1.6/cognee/modules/memory/vector/__init__.py
--rw-r--r--   0        0        0      378 2024-04-26 16:35:54.787346 cognee-0.1.6/cognee/modules/memory/vector/create_vector_memory.py
--rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.6/cognee/modules/search/CogneeSearch.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.6/cognee/modules/search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.6/cognee/modules/search/graph/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.6/cognee/modules/search/graph/search_adjacent.py
--rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.6/cognee/modules/search/graph/search_categories.py
--rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.6/cognee/modules/search/graph/search_neighbour.py
--rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.6/cognee/modules/search/graph/search_summary.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.6/cognee/modules/search/vector/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-20 17:45:36.721313 cognee-0.1.6/cognee/modules/search/vector/search_similarity.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.6/cognee/modules/users/__init__.py
--rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.6/cognee/modules/users/memory/__init__.py
--rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.6/cognee/modules/users/memory/create_information_points.py
--rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.6/cognee/modules/users/memory/is_existing_memory.py
--rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.6/cognee/modules/users/memory/register_memory_for_user.py
--rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.6/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
--rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.6/cognee/root_dir.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.6/cognee/shared/__init__.py
--rw-r--r--   0        0        0     8633 2024-04-25 09:42:30.768854 cognee-0.1.6/cognee/shared/data_models.py
--rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.6/cognee/shared/encode_uuid.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.642031 cognee-0.1.6/cognee/tests/__init__.py
--rw-r--r--   0        0        0      985 2024-04-25 22:16:19.642354 cognee-0.1.6/cognee/tests/test_data/Natural_language_processing.txt
--rwxr-xr-x   0        0        0     5982 2024-04-25 22:16:19.642833 cognee-0.1.6/cognee/tests/test_library.py
--rw-r--r--   0        0        0     9487 2024-04-25 22:16:19.643423 cognee-0.1.6/cognee/utils.py
--rw-r--r--   0        0        0     3511 2024-04-26 16:36:14.100526 cognee-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7203 1970-01-01 00:00:00.000000 cognee-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3795 2024-05-03 08:46:46.343235 cognee-0.1.7/README.md
+-rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.7/cognee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.7/cognee/api/__init__.py
+-rw-r--r--   0        0        0     4370 2024-04-25 22:16:19.632624 cognee-0.1.7/cognee/api/client.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.7/cognee/api/v1/__init__.py
+-rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.7/cognee/api/v1/add/__init__.py
+-rw-r--r--   0        0        0     4716 2024-04-25 22:16:19.633201 cognee-0.1.7/cognee/api/v1/add/add.py
+-rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.7/cognee/api/v1/add/add_standalone.py
+-rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.7/cognee/api/v1/add/remember.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633260 cognee-0.1.7/cognee/api/v1/cognify/__init__.py
+-rw-r--r--   0        0        0     7358 2024-05-03 08:36:42.745390 cognee-0.1.7/cognee/api/v1/cognify/cognify.py
+-rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.7/cognee/api/v1/config/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-24 17:34:59.319404 cognee-0.1.7/cognee/api/v1/config/config.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633793 cognee-0.1.7/cognee/api/v1/datasets/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.7/cognee/api/v1/datasets/datasets.py
+-rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.7/cognee/api/v1/prune/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-30 16:56:32.066819 cognee-0.1.7/cognee/api/v1/prune/prune.py
+-rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.7/cognee/api/v1/search/__init__.py
+-rw-r--r--   0        0        0     3611 2024-04-25 22:16:19.634363 cognee-0.1.7/cognee/api/v1/search/search.py
+-rw-r--r--   0        0        0     6489 2024-04-25 22:16:19.634966 cognee-0.1.7/cognee/config.py
+-rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.7/cognee/fetch_secret.py
+-rw-r--r--   0        0        0     8308 2024-05-03 08:36:42.745874 cognee-0.1.7/cognee/infrastructure/InfrastructureConfig.py
+-rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.7/cognee/infrastructure/__init__.py
+-rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.7/cognee/infrastructure/data/__init__.py
+-rw-r--r--   0        0        0     4456 2024-04-24 17:34:59.321526 cognee-0.1.7/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635699 cognee-0.1.7/cognee/infrastructure/data/chunking/__init__.py
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.7/cognee/infrastructure/data/models/Data.py
+-rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.7/cognee/infrastructure/data/models/Dataset.py
+-rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.7/cognee/infrastructure/data/models/DatasetData.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.7/cognee/infrastructure/data/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635851 cognee-0.1.7/cognee/infrastructure/data/utils/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.7/cognee/infrastructure/data/utils/extract_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.7/cognee/infrastructure/databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.7/cognee/infrastructure/databases/graph/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-29 10:09:13.468512 cognee-0.1.7/cognee/infrastructure/databases/graph/get_graph_client.py
+-rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.7/cognee/infrastructure/databases/graph/graph_db_interface.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.7/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
+-rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.7/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.7/cognee/infrastructure/databases/graph/networkx/__init__.py
+-rw-r--r--   0        0        0     5302 2024-04-29 10:11:05.964933 cognee-0.1.7/cognee/infrastructure/databases/graph/networkx/adapter.py
+-rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.7/cognee/infrastructure/databases/relational/DatabaseEngine.py
+-rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.7/cognee/infrastructure/databases/relational/ModelBase.py
+-rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.7/cognee/infrastructure/databases/relational/__init__.py
+-rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.7/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637021 cognee-0.1.7/cognee/infrastructure/databases/relational/duckdb/__init__.py
+-rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.7/cognee/infrastructure/databases/relational/relational_db_interface.py
+-rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.7/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.7/cognee/infrastructure/databases/relational/sqlite/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.7/cognee/infrastructure/databases/relational/utils/__init__.py
+-rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.7/cognee/infrastructure/databases/relational/utils/with_rollback.py
+-rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.7/cognee/infrastructure/databases/vector/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-03 08:36:42.746430 cognee-0.1.7/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
+-rw-r--r--   0        0        0      243 2024-05-03 08:36:42.746729 cognee-0.1.7/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637164 cognee-0.1.7/cognee/infrastructure/databases/vector/embeddings/__init__.py
+-rw-r--r--   0        0        0     5264 2024-05-03 08:36:42.747158 cognee-0.1.7/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py
+-rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.7/cognee/infrastructure/databases/vector/models/CollectionConfig.py
+-rw-r--r--   0        0        0      398 2024-05-03 08:36:42.747541 cognee-0.1.7/cognee/infrastructure/databases/vector/models/DataPoint.py
+-rw-r--r--   0        0        0       69 2024-05-03 08:36:42.747946 cognee-0.1.7/cognee/infrastructure/databases/vector/models/PayloadSchema.py
+-rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.7/cognee/infrastructure/databases/vector/models/ScoredResult.py
+-rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.7/cognee/infrastructure/databases/vector/models/VectorConfig.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637726 cognee-0.1.7/cognee/infrastructure/databases/vector/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637873 cognee-0.1.7/cognee/infrastructure/databases/vector/pinecone/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.7/cognee/infrastructure/databases/vector/pinecone/adapter.py
+-rw-r--r--   0        0        0     6706 2024-05-03 08:36:42.748385 cognee-0.1.7/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
+-rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.7/cognee/infrastructure/databases/vector/qdrant/__init__.py
+-rw-r--r--   0        0        0     1362 2024-05-03 08:36:42.748791 cognee-0.1.7/cognee/infrastructure/databases/vector/vector_db_interface.py
+-rw-r--r--   0        0        0     4500 2024-05-03 08:36:42.749289 cognee-0.1.7/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
+-rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.7/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.7/cognee/infrastructure/files/__init__.py
+-rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.7/cognee/infrastructure/files/add_file_to_storage.py
+-rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.7/cognee/infrastructure/files/remove_file_from_storage.py
+-rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.7/cognee/infrastructure/files/storage/LocalStorage.py
+-rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.7/cognee/infrastructure/files/storage/StorageManager.py
+-rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.7/cognee/infrastructure/files/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.7/cognee/infrastructure/files/utils/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-23 10:42:22.654946 cognee-0.1.7/cognee/infrastructure/files/utils/extract_text_from_file.py
+-rw-r--r--   0        0        0      835 2024-04-23 10:42:22.655413 cognee-0.1.7/cognee/infrastructure/files/utils/get_file_metadata.py
+-rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.7/cognee/infrastructure/files/utils/get_file_size.py
+-rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.7/cognee/infrastructure/files/utils/guess_file_type.py
+-rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.7/cognee/infrastructure/files/utils/is_text_content.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.7/cognee/infrastructure/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.7/cognee/infrastructure/llm/anthropic/__init__.py
+-rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.7/cognee/infrastructure/llm/anthropic/adapter.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639301 cognee-0.1.7/cognee/infrastructure/llm/generic_llm_api/__init__.py
+-rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.7/cognee/infrastructure/llm/generic_llm_api/adapter.py
+-rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.7/cognee/infrastructure/llm/get_llm_client.py
+-rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.7/cognee/infrastructure/llm/llm_interface.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.7/cognee/infrastructure/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.7/cognee/infrastructure/llm/openai/adapter.py
+-rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.7/cognee/infrastructure/llm/prompts/__init__.py
+-rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.7/cognee/infrastructure/llm/prompts/classify_content.txt
+-rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
+-rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
+-rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.7/cognee/infrastructure/llm/prompts/read_query_prompt.py
+-rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.7/cognee/infrastructure/llm/prompts/render_prompt.py
+-rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.7/cognee/infrastructure/llm/prompts/summarize_content.txt
+-rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.7/cognee/infrastructure/pipeline/models/Operation.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639465 cognee-0.1.7/cognee/infrastructure/pipeline/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.7/cognee/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.7/cognee/modules/cognify/__init__.py
+-rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.7/cognee/modules/cognify/dataset.py
+-rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.7/cognee/modules/cognify/evaluate.py
+-rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.7/cognee/modules/cognify/graph/__init__.py
+-rw-r--r--   0        0        0     1186 2024-04-25 22:16:19.640140 cognee-0.1.7/cognee/modules/cognify/graph/add_classification_nodes.py
+-rw-r--r--   0        0        0     5201 2024-05-03 08:36:42.749768 cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
+-rw-r--r--   0        0        0     1138 2024-04-25 22:16:19.640702 cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layers.py
+-rw-r--r--   0        0        0     1483 2024-05-03 08:36:42.750160 cognee-0.1.7/cognee/modules/cognify/graph/add_data_chunks.py
+-rw-r--r--   0        0        0     1005 2024-05-03 08:36:42.750569 cognee-0.1.7/cognee/modules/cognify/graph/add_document_node.py
+-rw-r--r--   0        0        0     2145 2024-05-03 08:36:42.750991 cognee-0.1.7/cognee/modules/cognify/graph/add_label_nodes.py
+-rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.7/cognee/modules/cognify/graph/add_node_connections.py
+-rw-r--r--   0        0        0      798 2024-04-25 09:42:30.766937 cognee-0.1.7/cognee/modules/cognify/graph/add_summary_nodes.py
+-rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.7/cognee/modules/cognify/graph/create.py
+-rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.7/cognee/modules/cognify/graph/initialize_graph.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.7/cognee/modules/cognify/llm/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.7/cognee/modules/cognify/llm/resolve_cross_graph_references.py
+-rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.7/cognee/modules/cognify/test.py
+-rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.7/cognee/modules/cognify/train.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641213 cognee-0.1.7/cognee/modules/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641372 cognee-0.1.7/cognee/modules/data/extraction/__init__.py
+-rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.7/cognee/modules/data/extraction/extract_categories.py
+-rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.7/cognee/modules/data/extraction/extract_cognitive_layers.py
+-rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.7/cognee/modules/data/extraction/extract_summary.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641459 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
+-rw-r--r--   0        0        0     1042 2024-05-03 08:36:42.751386 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
+-rw-r--r--   0        0        0     4740 2024-04-25 22:16:19.641944 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
+-rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.7/cognee/modules/data/get_cognitive_layers.py
+-rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.7/cognee/modules/data/get_content_categories.py
+-rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.7/cognee/modules/data/get_content_summary.py
+-rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.7/cognee/modules/data/get_layer_graphs.py
+-rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.7/cognee/modules/discovery/__init__.py
+-rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.7/cognee/modules/discovery/discover_directory_datasets.py
+-rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.7/cognee/modules/ingestion/__init__.py
+-rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.7/cognee/modules/ingestion/add_data_to_dataset.py
+-rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.7/cognee/modules/ingestion/classify.py
+-rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.7/cognee/modules/ingestion/data_types/BinaryData.py
+-rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.7/cognee/modules/ingestion/data_types/IngestionData.py
+-rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.7/cognee/modules/ingestion/data_types/TextData.py
+-rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.7/cognee/modules/ingestion/data_types/__init__.py
+-rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.7/cognee/modules/ingestion/exceptions.py
+-rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.7/cognee/modules/ingestion/identify.py
+-rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.7/cognee/modules/ingestion/save.py
+-rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.7/cognee/modules/search/CogneeSearch.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.7/cognee/modules/search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.7/cognee/modules/search/graph/__init__.py
+-rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.7/cognee/modules/search/graph/search_adjacent.py
+-rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.7/cognee/modules/search/graph/search_categories.py
+-rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.7/cognee/modules/search/graph/search_neighbour.py
+-rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.7/cognee/modules/search/graph/search_summary.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.7/cognee/modules/search/vector/__init__.py
+-rw-r--r--   0        0        0     1614 2024-05-03 08:36:42.751852 cognee-0.1.7/cognee/modules/search/vector/search_similarity.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.7/cognee/modules/users/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.7/cognee/modules/users/memory/__init__.py
+-rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.7/cognee/modules/users/memory/create_information_points.py
+-rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.7/cognee/modules/users/memory/is_existing_memory.py
+-rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.7/cognee/modules/users/memory/register_memory_for_user.py
+-rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.7/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
+-rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.7/cognee/root_dir.py
+-rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.7/cognee/shared/__init__.py
+-rw-r--r--   0        0        0     8633 2024-04-25 09:42:30.768854 cognee-0.1.7/cognee/shared/data_models.py
+-rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.7/cognee/shared/encode_uuid.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:16:19.642031 cognee-0.1.7/cognee/tests/__init__.py
+-rw-r--r--   0        0        0      985 2024-04-25 22:16:19.642354 cognee-0.1.7/cognee/tests/test_data/Natural_language_processing.txt
+-rwxr-xr-x   0        0        0     5982 2024-04-25 22:16:19.642833 cognee-0.1.7/cognee/tests/test_library.py
+-rw-r--r--   0        0        0     9487 2024-04-25 22:16:19.643423 cognee-0.1.7/cognee/utils.py
+-rw-r--r--   0        0        0     2775 2024-05-03 08:43:06.425402 cognee-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6856 1970-01-01 00:00:00.000000 cognee-0.1.7/PKG-INFO
```

### Comparing `cognee-0.1.6/LICENSE` & `cognee-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/README.md` & `cognee-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,22 +37,32 @@
 
 
 
 
 
 ## 📦 Installation
 
-With pip:
+### With pip
 
 ```bash
+pip install cognee
+```
+
+Use Weaviate vector storage:
+```bash
 pip install "cognee[weaviate]"
 ```
 
-With poetry:
+### With poetry
+
+```bash
+poetry add cognee
+```
 
+Use Weaviate vector storage:
 ```bash
 poetry add "cognee[weaviate]"
 ```
 
 ## 💻 Usage
 
 ### Setup
```

#### html2text {}

```diff
@@ -2,18 +2,20 @@
 vector retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
 Open-source framework for creating self-improving deterministic outputs for
 LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
 ![Cognee Demo](assets/cognee_demo.gif) Try it in a Google collab _n_o_t_e_b_o_o_k or
 have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n Join our _D_i_s_c_o_r_d community ## ð¦
-Installation With pip: ```bash pip install "cognee[weaviate]" ``` With poetry:
-```bash poetry add "cognee[weaviate]" ``` ## ð» Usage ### Setup ``` import os
-os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"]
-= "YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+Installation ### With pip ```bash pip install cognee ``` Use Weaviate vector
+storage: ```bash pip install "cognee[weaviate]" ``` ### With poetry ```bash
+poetry add cognee ``` Use Weaviate vector storage: ```bash poetry add "cognee
+[weaviate]" ``` ## ð» Usage ### Setup ``` import os os.environ
+["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"] =
+"YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
 ``` You can also use Ollama or Anyscale as your LLM provider. For more info on
 local models check our [docs](https://topoteretes.github.io/cognee) ### Run ```
 import cognee text = """Natural language processing (NLP) is an
 interdisciplinary subfield of computer science and information retrieval"""
 cognee.add([text], "example_dataset") # Add a new piece of information
 cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
 cognee.search("SIMILARITY", "computer science") # Query cognee for the
```

### Comparing `cognee-0.1.6/cognee/api/client.py` & `cognee-0.1.7/cognee/api/client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/api/v1/add/add.py` & `cognee-0.1.7/cognee/api/v1/add/add.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/api/v1/add/add_standalone.py` & `cognee-0.1.7/cognee/api/v1/add/add_standalone.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/api/v1/add/remember.py` & `cognee-0.1.7/cognee/api/v1/add/remember.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/api/v1/cognify/cognify.py` & `cognee-0.1.7/cognee/api/v1/cognify/cognify.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from cognee.modules.cognify.graph.add_classification_nodes import add_classification_nodes
 from cognee.modules.cognify.graph.add_cognitive_layer_graphs import add_cognitive_layer_graphs
 from cognee.modules.cognify.graph.add_summary_nodes import add_summary_nodes
 from cognee.modules.cognify.graph.add_node_connections import group_nodes_by_layer, \
     graph_ready_output, connect_nodes_in_graph
 from cognee.modules.cognify.llm.resolve_cross_graph_references import resolve_cross_graph_references
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
-from cognee.modules.cognify.graph.add_label_nodes import add_label_nodes
 from cognee.modules.cognify.graph.add_cognitive_layers import add_cognitive_layers
 # from cognee.modules.cognify.graph.initialize_graph import initialize_graph
 from cognee.infrastructure.files.utils.guess_file_type import guess_file_type, FileTypeException
 from cognee.infrastructure.files.utils.extract_text_from_file import extract_text_from_file
 from cognee.infrastructure import infrastructure_config
 from cognee.modules.data.get_content_categories import get_content_categories
 from cognee.modules.data.get_content_summary import get_content_summary
@@ -37,15 +36,15 @@
 USER_ID = "default_user"
 
 logger = logging.getLogger("cognify")
 
 async def cognify(datasets: Union[str, List[str]] = None):
     """This function is responsible for the cognitive processing of the content."""
     # Has to be loaded in advance, multithreading doesn't work without it.
-    nltk.download('stopwords', quiet=True)
+    nltk.download("stopwords", quiet=True)
     stopwords.ensure_loaded()
 
     graph_db_type = infrastructure_config.get_config()["graph_engine"]
 
     graph_client = await get_graph_client(graph_db_type)
 
     db_engine = infrastructure_config.get_config()["database_engine"]
@@ -80,46 +79,46 @@
     chunk_engine = infrastructure_config.get_config()["chunk_engine"]
     chunk_strategy = infrastructure_config.get_config()["chunk_strategy"]
 
     for (dataset_name, files) in dataset_files:
         for file_metadata in files:
             with open(file_metadata["file_path"], "rb") as file:
                 try:
+                    document_id = await add_document_node(
+                        graph_client,
+                        parent_node_id = f"DefaultGraphModel__{USER_ID}",
+                        document_metadata = file_metadata,
+                    )
+
                     file_type = guess_file_type(file)
                     text = extract_text_from_file(file, file_type)
                     subchunks = chunk_engine.chunk_data(chunk_strategy, text, config.chunk_size, config.chunk_overlap)
 
                     if dataset_name not in data_chunks:
                         data_chunks[dataset_name] = []
 
                     for subchunk in subchunks:
-                        data_chunks[dataset_name].append(dict(text = subchunk, chunk_id = str(uuid4()), file_metadata = file_metadata))
+                        data_chunks[dataset_name].append(dict(document_id = document_id, chunk_id = str(uuid4()), text = subchunk))
                 except FileTypeException:
                     logger.warning("File (%s) has an unknown file type. We are skipping it.", file_metadata["id"])
 
     added_chunks: list[tuple[str, str, dict]] = await add_data_chunks(data_chunks)
 
     await asyncio.gather(
-        *[process_text(chunk["collection"], chunk["chunk_id"], chunk["text"], chunk["file_metadata"]) for chunk in added_chunks]
+        *[process_text(chunk["document_id"], chunk["chunk_id"], chunk["collection"], chunk["text"]) for chunk in added_chunks]
     )
 
     return graph_client.graph
 
-async def process_text(chunk_collection: str, chunk_id: str, input_text: str, file_metadata: dict):
-    print(f"Processing chunk ({chunk_id}) from document ({file_metadata['id']}).")
-
-    graph_client = await get_graph_client(infrastructure_config.get_config()["graph_engine"])
+async def process_text(document_id: str, chunk_id: str, chunk_collection: str, input_text: str):
+    raw_document_id = document_id.split("__")[-1]
 
-    document_id = await add_document_node(
-        graph_client,
-        parent_node_id = f"DefaultGraphModel__{USER_ID}", #make a param of defaultgraph model to make sure when user passes his stuff, it doesn't break pipeline
-        document_metadata = file_metadata,
-    )
+    print(f"Processing chunk ({chunk_id}) from document ({raw_document_id}).")
 
-    await add_label_nodes(graph_client, document_id, chunk_id, file_metadata["keywords"].split("|"))
+    graph_client = await get_graph_client(infrastructure_config.get_config()["graph_engine"])
 
     classified_categories = await get_content_categories(input_text)
     await add_classification_nodes(
         graph_client,
         parent_node_id = document_id,
         categories = classified_categories,
     )
@@ -135,15 +134,15 @@
     cognitive_layers = (await add_cognitive_layers(graph_client, document_id, cognitive_layers))[:2]
 
     layer_graphs = await get_layer_graphs(input_text, cognitive_layers)
     await add_cognitive_layer_graphs(graph_client, chunk_collection, chunk_id, layer_graphs)
 
     if infrastructure_config.get_config()["connect_documents"] is True:
         db_engine = infrastructure_config.get_config()["database_engine"]
-        relevant_documents_to_connect = db_engine.fetch_cognify_data(excluded_document_id = file_metadata["id"])
+        relevant_documents_to_connect = db_engine.fetch_cognify_data(excluded_document_id = raw_document_id)
 
         list_of_nodes = []
 
         relevant_documents_to_connect.append({
             "layer_id": document_id,
         })
```

### Comparing `cognee-0.1.6/cognee/api/v1/config/config.py` & `cognee-0.1.7/cognee/api/v1/config/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/api/v1/datasets/datasets.py` & `cognee-0.1.7/cognee/api/v1/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/api/v1/prune/prune.py` & `cognee-0.1.7/cognee/api/v1/prune/prune.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/api/v1/search/search.py` & `cognee-0.1.7/cognee/api/v1/search/search.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/config.py` & `cognee-0.1.7/cognee/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/fetch_secret.py` & `cognee-0.1.7/cognee/fetch_secret.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/InfrastructureConfig.py` & `cognee-0.1.7/cognee/infrastructure/InfrastructureConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from cognee.config import Config
 from .databases.relational import DuckDBAdapter, DatabaseEngine
 from .databases.vector.vector_db_interface import VectorDBInterface
-from .databases.vector.qdrant.QDrantAdapter import QDrantAdapter
 from .databases.vector.embeddings.DefaultEmbeddingEngine import DefaultEmbeddingEngine
 from .llm.llm_interface import LLMInterface
 from .llm.openai.adapter import OpenAIAdapter
 from .files.storage import LocalStorage
 from .data.chunking.DefaultChunkEngine import DefaultChunkEngine
 from ..shared.data_models import GraphDBType, DefaultContentPrediction, KnowledgeGraph, SummarizedContent, \
     LabeledContent, DefaultCognitiveLayer
@@ -77,38 +76,51 @@
 
         if self.chunk_engine is None:
             self.chunk_engine = DefaultChunkEngine()
 
         if (config_entity is None or config_entity == "llm_engine") and self.llm_engine is None:
             self.llm_engine = OpenAIAdapter(config.openai_key, config.openai_model)
 
+        if (config_entity is None or config_entity == "database_directory_path") and self.database_directory_path is None:
+            self.database_directory_path = self.system_root_directory + "/" + config.db_path
+
+        if (config_entity is None or config_entity == "database_file_path") and self.database_file_path is None:
+            self.database_file_path = self.system_root_directory + "/" + config.db_path + "/" + config.db_name
+
         if (config_entity is None or config_entity == "vector_engine") and self.vector_engine is None:
             try:
                 from .databases.vector.weaviate_db import WeaviateAdapter
 
                 if config.weaviate_url is None and config.weaviate_api_key is None:
                     raise EnvironmentError("Weaviate is not configured!")
 
                 self.vector_engine = WeaviateAdapter(
                     config.weaviate_url,
                     config.weaviate_api_key,
                     embedding_engine = self.embedding_engine
                 )
             except (EnvironmentError, ModuleNotFoundError):
-                self.vector_engine = QDrantAdapter(
-                    qdrant_url = config.qdrant_url,
-                    qdrant_api_key = config.qdrant_api_key,
-                    embedding_engine = self.embedding_engine
-                )
-
-        if (config_entity is None or config_entity == "database_directory_path") and self.database_directory_path is None:
-            self.database_directory_path = self.system_root_directory + "/" + config.db_path
+                if config.qdrant_url and config.qdrant_api_key:
+                    from .databases.vector.qdrant.QDrantAdapter import QDrantAdapter
 
-        if (config_entity is None or config_entity == "database_file_path") and self.database_file_path is None:
-            self.database_file_path = self.system_root_directory + "/" + config.db_path + "/" + config.db_name
+                    self.vector_engine = QDrantAdapter(
+                        qdrant_url = config.qdrant_url,
+                        qdrant_api_key = config.qdrant_api_key,
+                        embedding_engine = self.embedding_engine
+                    )
+                else:
+                    from .databases.vector.lancedb.LanceDBAdapter import LanceDBAdapter
+                    lance_db_path = self.database_directory_path + "/cognee.lancedb"
+                    LocalStorage.ensure_directory_exists(lance_db_path)
+
+                    self.vector_engine = LanceDBAdapter(
+                        uri = lance_db_path,
+                        api_key = None,
+                        embedding_engine = self.embedding_engine,
+                    )
 
         if config_entity is not None:
             return getattr(self, config_entity)
 
         return {
             "llm_engine": self.llm_engine,
             "vector_engine": self.vector_engine,
```

### Comparing `cognee-0.1.6/cognee/infrastructure/data/chunking/DefaultChunkEngine.py` & `cognee-0.1.7/cognee/infrastructure/data/chunking/DefaultChunkEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/data/models/Data.py` & `cognee-0.1.7/cognee/infrastructure/data/models/Data.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/data/models/Dataset.py` & `cognee-0.1.7/cognee/infrastructure/data/models/Dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/data/models/DatasetData.py` & `cognee-0.1.7/cognee/infrastructure/data/models/DatasetData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/data/utils/extract_keywords.py` & `cognee-0.1.7/cognee/infrastructure/data/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/graph/get_graph_client.py` & `cognee-0.1.7/cognee/infrastructure/databases/graph/get_graph_client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/graph/graph_db_interface.py` & `cognee-0.1.7/cognee/infrastructure/databases/graph/graph_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py` & `cognee-0.1.7/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/graph/networkx/adapter.py` & `cognee-0.1.7/cognee/infrastructure/databases/graph/networkx/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py` & `cognee-0.1.7/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/relational/relational_db_interface.py` & `cognee-0.1.7/cognee/infrastructure/databases/relational/relational_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py` & `cognee-0.1.7/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/relational/utils/with_rollback.py` & `cognee-0.1.7/cognee/infrastructure/databases/relational/utils/with_rollback.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py` & `cognee-0.1.7/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import List
 
 import instructor
 from openai import AsyncOpenAI
 from fastembed import TextEmbedding
-from fastembed import TextEmbedding
-from openai import AsyncOpenAI
 
 from cognee.config import Config
 from cognee.root_dir import get_absolute_path
 from .EmbeddingEngine import EmbeddingEngine
 
 config = Config()
 config.load()
```

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py` & `cognee-0.1.7/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         result = await client.collection_exists(collection_name)
         await client.close()
         return result
 
     async def create_collection(
       self,
       collection_name: str,
+      payload_schema = None,
     ):
         client = self.get_qdrant_client()
 
         result = await client.create_collection(
             collection_name = collection_name,
             vectors_config = {
                 "text": models.VectorParams(
@@ -89,15 +90,15 @@
         client = self.get_qdrant_client()
 
         data_vectors = await self.embed_data([data_point.get_embeddable_data() for data_point in data_points])
 
         def convert_to_qdrant_point(data_point: DataPoint):
             return models.PointStruct(
                 id = data_point.id,
-                payload = data_point.payload,
+                payload = data_point.payload.dict(),
                 vector = {
                     "text": data_vectors[data_points.index(data_point)]
                 }
             )
 
         points = [convert_to_qdrant_point(point) for point in data_points]
 
@@ -106,17 +107,17 @@
             points = points
         )
 
         await client.close()
 
         return result
 
-    async def retrieve(self, collection_name: str, data_id: str):
+    async def retrieve(self, collection_name: str, data_point_id: str):
         client = self.get_qdrant_client()
-        results = await client.retrieve(collection_name, [data_id], with_payload = True)
+        results = await client.retrieve(collection_name, [data_point_id], with_payload = True)
         await client.close()
         return results[0] if len(results) > 0 else None
 
     async def search(
         self,
         collection_name: str,
         query_text: Optional[str] = None,
```

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/vector/vector_db_interface.py` & `cognee-0.1.7/cognee/infrastructure/llm/llm_interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,40 @@
-from typing import List, Protocol, Optional
-from abc import abstractmethod
-from .models.DataPoint import DataPoint
-
-class VectorDBInterface(Protocol):
-    """ Collections """
-    @abstractmethod
-    async def create_collection(
-        self,
-        collection_name: str
-    ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def update_collection(
-    #     self,
-    #     collection_name: str,
-    #     collection_config: object
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def delete_collection(
-    #     self,
-    #     collection_name: str
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def create_vector_index(
-    #     self,
-    #     collection_name: str,
-    #     vector_index_config: object
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def create_data_index(
-    #     self,
-    #     collection_name: str,
-    #     vector_index_config: object
-    # ): raise NotImplementedError
+""" LLM Interface """
 
-    """ Data points """
-    @abstractmethod
-    async def create_data_points(
-        self,
-        collection_name: str,
-        data_points: List[DataPoint]
-    ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def get_data_point(
-    #     self,
-    #     collection_name: str,
-    #     data_point_id: str
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def update_data_point(
-    #     self,
-    #     collection_name: str,
-    #     data_point_id: str,
-    #     payload: object
-    # ): raise NotImplementedError
-
-    # @abstractmethod
-    # async def delete_data_point(
-    #     self,
-    #     collection_name: str,
-    #     data_point_id: str
-    # ): raise NotImplementedError
-
-    """ Search """
+from typing import Type, Protocol
+from abc import abstractmethod
+from pydantic import BaseModel
+class LLMInterface(Protocol):
+    """ LLM Interface """
+
+    # @abstractmethod
+    # async def async_get_embedding_with_backoff(self, text, model="text-embedding-ada-002"):
+    #     """To get text embeddings, import/call this function"""
+    #     raise NotImplementedError
+    #
+    # @abstractmethod
+    # def get_embedding_with_backoff(self, text: str, model: str = "text-embedding-ada-002"):
+    #     """To get text embeddings, import/call this function"""
+    #     raise NotImplementedError
+    #
+    # @abstractmethod
+    # async def async_get_batch_embeddings_with_backoff(self, texts: List[str], models: List[str]):
+    #     """To get multiple text embeddings in parallel, import/call this function"""
+    #     raise NotImplementedError
+
+    # """ Get completions """
+    # async def acompletions_with_backoff(self, **kwargs):
+    #     raise NotImplementedError
+    #
+    """ Structured output """
     @abstractmethod
-    async def search(
-        self,
-        collection_name: str,
-        query_text: Optional[str],
-        query_vector: Optional[List[float]],
-        limit: int,
-        with_vector: bool = False
-
-    ): raise NotImplementedError
+    async def acreate_structured_output(self,
+                                        text_input: str,
+                                        system_prompt: str,
+                                        response_model: Type[BaseModel]) -> BaseModel:
+        """To get structured output, import/call this function"""
+        raise NotImplementedError
 
     @abstractmethod
-    async def batch_search(
-        self,
-        collection_name: str,
-        query_texts: List[str],
-        limit: int,
-        with_vectors: bool = False
-    ): raise NotImplementedError
+    def show_prompt(self, text_input: str, system_prompt: str) -> str:
+        """To get structured output, import/call this function"""
+        raise NotImplementedError
```

### Comparing `cognee-0.1.6/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py` & `cognee-0.1.7/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,90 +17,82 @@
         import weaviate.classes as wvc
       
         self.embedding_engine = embedding_engine
 
         self.client = weaviate.connect_to_wcs(
             cluster_url=url,
             auth_credentials=weaviate.auth.AuthApiKey(api_key),
-            # headers = {
-            #     "X-OpenAI-Api-Key": openai_api_key
-            # },
             additional_config=wvc.init.AdditionalConfig(timeout=wvc.init.Timeout(init=30))
         )
 
     async def embed_data(self, data: List[str]) -> List[float]:
         return await self.embedding_engine.embed_text(data)
 
     async def collection_exists(self, collection_name: str) -> bool:
-        event_loop = asyncio.get_event_loop()
+        future = asyncio.Future()
 
-        def sync_collection_exists():
-            return self.client.collections.exists(collection_name)
+        future.set_result(self.client.collections.exists(collection_name))
 
-        return await event_loop.run_in_executor(None, sync_collection_exists)
+        return await future
 
-    async def create_collection(self, collection_name: str):
+    async def create_collection(
+        self,
+        collection_name: str,
+        payload_schema = None,
+    ):
         import weaviate.classes.config as wvcc
 
-        event_loop = asyncio.get_event_loop()
+        future = asyncio.Future()
 
-        def sync_create_collection():
-            return self.client.collections.create(
+        future.set_result(
+            self.client.collections.create(
                 name=collection_name,
                 properties=[
                     wvcc.Property(
                         name="text",
                         data_type=wvcc.DataType.TEXT,
                         skip_vectorization=True
                     )
                 ]
             )
+        )
 
-        # try:
-        result = await event_loop.run_in_executor(None, sync_create_collection)
-        # finally:
-        #     event_loop.shutdown_executor()
-
-        return result
+        return await future
 
     def get_collection(self, collection_name: str):
         return self.client.collections.get(collection_name)
 
     async def create_data_points(self, collection_name: str, data_points: List[DataPoint]):
         from weaviate.classes.data import DataObject
 
         data_vectors = await self.embed_data(
             list(map(lambda data_point: data_point.get_embeddable_data(), data_points)))
 
         def convert_to_weaviate_data_points(data_point: DataPoint):
             return DataObject(
-                uuid=data_point.id,
-                properties=data_point.payload,
-                vector=data_vectors[data_points.index(data_point)]
+                uuid = data_point.id,
+                properties = data_point.payload.dict(),
+                vector = data_vectors[data_points.index(data_point)]
             )
 
         objects = list(map(convert_to_weaviate_data_points, data_points))
 
         return self.get_collection(collection_name).data.insert_many(objects)
 
-    async def retrieve(self, collection_name: str, data_id: str):
-        def sync_retrieve():
-            return self.get_collection(collection_name).query.fetch_object_by_id(UUID(data_id))
-
-        event_loop = asyncio.get_event_loop()
-
-        # try:
-        data_point = await event_loop.run_in_executor(None, sync_retrieve)
-        # finally:
-            # event_loop.shutdown_executor()
+    async def retrieve(self, collection_name: str, data_point_id: str):
+        future = asyncio.Future()
+
+        data_point = self.get_collection(collection_name).query.fetch_object_by_id(UUID(data_point_id))
 
         data_point.payload = data_point.properties
         del data_point.properties
 
-        return data_point
+        future.set_result(data_point)
+
+        return await future
 
     async def search(
             self,
             collection_name: str,
             query_text: Optional[str] = None,
             query_vector: Optional[List[float]] = None,
             limit: int = None,
@@ -110,15 +102,14 @@
 
         if query_text is None and query_vector is None:
             raise ValueError("One of query_text or query_vector must be provided!")
 
         if query_vector is None:
             query_vector = (await self.embed_data([query_text]))[0]
 
-        # def sync_search():
         search_result = self.get_collection(collection_name).query.hybrid(
             query = None,
             vector = query_vector,
             limit = limit,
             include_vector = with_vector,
             return_metadata = wvc.query.MetadataQuery(score=True),
         )
```

### Comparing `cognee-0.1.6/cognee/infrastructure/files/storage/LocalStorage.py` & `cognee-0.1.7/cognee/infrastructure/files/storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/files/storage/StorageManager.py` & `cognee-0.1.7/cognee/infrastructure/files/storage/StorageManager.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/files/utils/get_file_metadata.py` & `cognee-0.1.7/cognee/infrastructure/files/utils/get_file_metadata.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/files/utils/guess_file_type.py` & `cognee-0.1.7/cognee/infrastructure/files/utils/guess_file_type.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/files/utils/is_text_content.py` & `cognee-0.1.7/cognee/infrastructure/files/utils/is_text_content.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/anthropic/adapter.py` & `cognee-0.1.7/cognee/infrastructure/llm/anthropic/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/generic_llm_api/adapter.py` & `cognee-0.1.7/cognee/infrastructure/llm/generic_llm_api/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/get_llm_client.py` & `cognee-0.1.7/cognee/infrastructure/llm/get_llm_client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/openai/adapter.py` & `cognee-0.1.7/cognee/infrastructure/llm/openai/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/prompts/classify_content.txt` & `cognee-0.1.7/cognee/infrastructure/llm/prompts/classify_content.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/prompts/generate_cog_layers.txt` & `cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_cog_layers.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt` & `cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/prompts/read_query_prompt.py` & `cognee-0.1.7/cognee/infrastructure/llm/prompts/read_query_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/llm/prompts/render_prompt.py` & `cognee-0.1.7/cognee/infrastructure/llm/prompts/render_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/infrastructure/pipeline/models/Operation.py` & `cognee-0.1.7/cognee/infrastructure/pipeline/models/Operation.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/dataset.py` & `cognee-0.1.7/cognee/modules/cognify/dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/evaluate.py` & `cognee-0.1.7/cognee/modules/cognify/evaluate.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/add_classification_nodes.py` & `cognee-0.1.7/cognee/modules/cognify/graph/add_classification_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py` & `cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from uuid import uuid4
 from typing import List, Tuple, TypedDict
+from pydantic import BaseModel
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.vector import DataPoint
 from cognee.shared.data_models import KnowledgeGraph
 from cognee.utils import extract_pos_tags, extract_named_entities, extract_sentiment_vader
 
 class GraphLike(TypedDict):
     nodes: List
@@ -102,22 +103,30 @@
                 dict(relationship_name = edge.relationship_name),
             ))
 
         await graph_client.add_nodes(graph_nodes)
 
         await graph_client.add_edges(graph_edges)
 
+        class References(BaseModel):
+            node_id: str
+            cognitive_layer: str
+
+        class PayloadSchema(BaseModel):
+            value: str
+            references: References
+
         try:
-            await vector_client.create_collection(layer_id)
+            await vector_client.create_collection(layer_id, payload_schema = PayloadSchema)
         except Exception:
             # It's ok if the collection already exists.
             pass
 
         data_points = [
-            DataPoint(
+            DataPoint[PayloadSchema](
                 id = str(uuid4()),
                 payload = dict(
                     value = node_data["name"],
                     references = dict(
                         node_id = node_id,
                         cognitive_layer = layer_id,
                     ),
```

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/add_cognitive_layers.py` & `cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layers.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/add_document_node.py` & `cognee-0.1.7/cognee/modules/cognify/graph/add_document_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from cognee.shared.data_models import Document
+from cognee.modules.cognify.graph.add_label_nodes import add_label_nodes
 from cognee.infrastructure.databases.graph.graph_db_interface import GraphDBInterface
 
 async def add_document_node(graph_client: GraphDBInterface, parent_node_id, document_metadata):
     document_id = f"DOCUMENT__{document_metadata['id']}"
 
-
-
-
-
     document = await graph_client.extract_node(document_id)
 
     if not document:
         document = Document(
             id = document_id,
             title = document_metadata["name"],
             file_path = document_metadata["file_path"],
         ).model_dump()
 
     document["entity_type"] = "Document"
 
     await graph_client.add_node(document_id, document)
 
-    await graph_client.add_edge(parent_node_id, document_id, "has_document", dict(relationship_name = "has_document"))
+    await graph_client.add_edge(
+        parent_node_id,
+        document_id,
+        "has_document",
+        dict(relationship_name = "has_document"),
+    )
+
+    await add_label_nodes(graph_client, document_id, document_metadata["keywords"].split("|"))
 
     return document_id
```

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/add_label_nodes.py` & `cognee-0.1.7/cognee/modules/cognify/graph/add_label_nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from uuid import uuid4
 from typing import List
 from datetime import datetime
+from pydantic import BaseModel
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.vector import DataPoint
 
-async def add_label_nodes(graph_client, parent_node_id: str, chunk_id: str, keywords: List[str]) -> None:
+async def add_label_nodes(graph_client, parent_node_id: str, keywords: List[str]) -> None:
     vector_client = infrastructure_config.get_config("vector_engine")
 
     keyword_nodes = []
 
     for keyword in keywords:
         keyword_id = f"DATA_LABEL_{keyword.upper().replace(' ', '_')}"
 
         keyword_nodes.append((
             keyword_id,
             dict(
                 id = keyword_id,
-                chunk_id = chunk_id,
                 name = keyword.lower().capitalize(),
                 keyword = keyword.lower(),
                 entity_type = "Keyword",
                 created_at = datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                 updated_at = datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             ),
         ))
@@ -32,29 +32,37 @@
             parent_node_id,
             keyword_id,
             "refers_to",
             dict(relationship_name = "refers_to"),
         ) for (keyword_id, __) in keyword_nodes
     ])
 
+    class References(BaseModel):
+        node_id: str
+        cognitive_layer: str
+
+    class PayloadSchema(BaseModel):
+        value: str
+        references: References
+
     # Add data to vector
     keyword_data_points = [
-        DataPoint(
+        DataPoint[PayloadSchema](
             id = str(uuid4()),
             payload = dict(
                 value = keyword_data["keyword"],
                 references = dict(
                     node_id = keyword_node_id,
                     cognitive_layer = parent_node_id,
                 ),
             ),
             embed_field = "value"
         ) for (keyword_node_id, keyword_data) in keyword_nodes
     ]
 
     try:
-        await vector_client.create_collection(parent_node_id)
+        await vector_client.create_collection(parent_node_id, payload_schema = PayloadSchema)
     except Exception:
         # It's ok if the collection already exists.
         pass
 
     await vector_client.create_data_points(parent_node_id, keyword_data_points)
```

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/add_node_connections.py` & `cognee-0.1.7/cognee/modules/cognify/graph/add_node_connections.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/add_summary_nodes.py` & `cognee-0.1.7/cognee/modules/cognify/graph/add_summary_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/create.py` & `cognee-0.1.7/cognee/modules/cognify/graph/create.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/graph/initialize_graph.py` & `cognee-0.1.7/cognee/modules/cognify/graph/initialize_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/llm/resolve_cross_graph_references.py` & `cognee-0.1.7/cognee/modules/cognify/llm/resolve_cross_graph_references.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/test.py` & `cognee-0.1.7/cognee/modules/cognify/test.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/cognify/train.py` & `cognee-0.1.7/cognee/modules/cognify/train.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/data/extraction/extract_categories.py` & `cognee-0.1.7/cognee/modules/data/extraction/extract_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py` & `cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py` & `cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 
         def sync_extract_knowledge_graph():
             return compiled_extract_knowledge_graph(context = text, question = "")
 
         return (await event_loop.run_in_executor(None, sync_extract_knowledge_graph)).graph
         # return compiled_extract_knowledge_graph(text, question = "").graph
     except Exception as error:
-        logger.error("Error extracting graph from content: %s", error, exc_info = True)
-        
+        # TODO: Log error to Sentry
+
         return await extract_content_graph(text, cognitive_layer, graph_model)
```

### Comparing `cognee-0.1.6/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py` & `cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/data/get_cognitive_layers.py` & `cognee-0.1.7/cognee/modules/data/get_cognitive_layers.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/data/get_content_categories.py` & `cognee-0.1.7/cognee/modules/data/get_content_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/data/get_layer_graphs.py` & `cognee-0.1.7/cognee/modules/data/get_layer_graphs.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/discovery/discover_directory_datasets.py` & `cognee-0.1.7/cognee/modules/discovery/discover_directory_datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/ingestion/add_data_to_dataset.py` & `cognee-0.1.7/cognee/modules/ingestion/add_data_to_dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/ingestion/data_types/BinaryData.py` & `cognee-0.1.7/cognee/modules/ingestion/data_types/BinaryData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/ingestion/data_types/TextData.py` & `cognee-0.1.7/cognee/modules/ingestion/data_types/TextData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/ingestion/save.py` & `cognee-0.1.7/cognee/modules/ingestion/save.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/search/CogneeSearch.py` & `cognee-0.1.7/cognee/modules/search/CogneeSearch.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/search/graph/search_adjacent.py` & `cognee-0.1.7/cognee/modules/search/graph/search_adjacent.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/search/graph/search_categories.py` & `cognee-0.1.7/cognee/modules/search/graph/search_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/search/graph/search_neighbour.py` & `cognee-0.1.7/cognee/modules/search/graph/search_neighbour.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/search/graph/search_summary.py` & `cognee-0.1.7/cognee/modules/search/graph/search_summary.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/modules/search/vector/search_similarity.py` & `cognee-0.1.7/cognee/modules/search/vector/search_similarity.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,26 +21,29 @@
 
         if len(results) > 0:
             graph_nodes.extend([
                 dict(
                     layer_id = result.payload["references"]["cognitive_layer"],
                     node_id = result.payload["references"]["node_id"],
                     score = result.score,
-                ) for result in results if result.score > 0.5
+                ) for result in results if result.score > 0.8
             ])
 
     if len(graph_nodes) == 0:
         return []
 
     relevant_context = []
 
     for graph_node_data in graph_nodes:
         graph_node = await graph_client.extract_node(graph_node_data["node_id"])
 
         if "chunk_collection" not in graph_node and "chunk_id" not in graph_node:
             continue
 
-        vector_point = await vector_engine.retrieve(graph_node["chunk_collection"], graph_node["chunk_id"])
+        vector_point = await vector_engine.retrieve(
+            graph_node["chunk_collection"],
+            graph_node["chunk_id"],
+        )
 
         relevant_context.append(vector_point.payload["text"])
 
     return deduplicate(relevant_context)
```

### Comparing `cognee-0.1.6/cognee/modules/users/memory/create_information_points.py` & `cognee-0.1.7/cognee/modules/users/memory/create_information_points.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json` & `cognee-0.1.7/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/shared/data_models.py` & `cognee-0.1.7/cognee/shared/data_models.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/tests/test_data/Natural_language_processing.txt` & `cognee-0.1.7/cognee/tests/test_data/Natural_language_processing.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/tests/test_library.py` & `cognee-0.1.7/cognee/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/cognee/utils.py` & `cognee-0.1.7/cognee/utils.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.6/pyproject.toml` & `cognee-0.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognee"
-version = "0.1.6"
+version = "0.1.7"
 description = "Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning."
 authors = ["Vasilije Markovic", "Boris Arzentar"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.cognee.ai"
 repository = "https://github.com/topoteretes/cognee"
 classifiers = [
@@ -23,18 +23,16 @@
 pydantic = "^2.5.0"
 python-dotenv = "1.0.1"
 fastapi = "^0.109.2"
 uvicorn = "0.22.0"
 boto3 = "^1.26.125"
 gunicorn = "^20.1.0"
 sqlalchemy = "^2.0.21"
-asyncpg = "^0.28.0"
 instructor = "1.2.1"
 networkx = "^3.2.1"
-graphviz = "^0.20.1"
 debugpy = "^1.8.0"
 pyarrow = "^15.0.0"
 pylint = "^3.0.3"
 aiosqlite = "^0.20.0"
 pandas = "^2.2.0"
 greenlet = "^3.0.3"
 ruff = "^0.2.2"
@@ -49,51 +47,36 @@
 graphistry = "^0.33.5"
 tenacity = "^8.2.3"
 weaviate-client = "^4.5.4"
 scikit-learn = "^1.4.1.post1"
 fastembed = "^0.2.5"
 pypdf = "^4.1.0"
 anthropic = "^0.21.3"
-xmltodict = "^0.13.0"
 neo4j = "^5.18.0"
 jinja2 = "^3.1.3"
 matplotlib = "^3.8.3"
 nest-asyncio = "^1.6.0"
 structlog = "^24.1.0"
 tiktoken = "^0.6.0"
 dspy-ai = "2.4.3"
 posthog = "^3.5.0"
 lancedb = "^0.6.10"
+tantivy = "^0.21.0"
 
 
 [tool.poetry.extras]
-dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb", "dbt-snowflake", "dbt-athena-community", "dbt-databricks"]
-gcp = ["grpcio", "google-cloud-bigquery", "db-dtypes", "gcsfs"]
-# bigquery is alias on gcp extras
-bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
-postgres = ["psycopg2-binary", "psycopg2cffi"]
-redshift = ["psycopg2-binary", "psycopg2cffi"]
 parquet = ["pyarrow"]
 duckdb = ["duckdb"]
 filesystem = ["s3fs", "botocore"]
-s3 = ["s3fs", "botocore"]
-gs = ["gcsfs"]
-az = ["adlfs"]
-snowflake = ["snowflake-connector-python"]
 motherduck = ["duckdb", "pyarrow"]
 cli = ["pipdeptree", "cron-descriptor"]
-athena = ["pyathena", "pyarrow", "s3fs", "botocore"]
 weaviate = ["weaviate-client"]
-mssql = ["pyodbc"]
-synapse = ["pyodbc", "adlfs", "pyarrow"]
-databricks = ["databricks-sql-connector"]
-lancedb = ["lancedb"]
-pinecone = ["pinecone-client"]
+qdrant = ["qdrant-client"]
 neo4j = ["neo4j", "py2neo"]
-notebook =[ "ipykernel","overrides", "ipywidgets", "jupyterlab", "jupyterlab_widgets", "jupyterlab-server", "jupyterlab-git"]
+notebook = ["ipykernel","overrides", "ipywidgets", "jupyterlab", "jupyterlab_widgets", "jupyterlab-server", "jupyterlab-git"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 coverage = "^7.3.2"
 mypy = "^1.7.1"
 notebook = "^7.1.1"
@@ -106,15 +89,14 @@
 pytest-examples = "^0.0.10"
 mkdocs-jupyter = "^0.24.6"
 mkdocs-minify-plugin = "^0.8.0"
 mkdocs-redirects = "^1.2.1"
 
 [tool.poetry.group.test-docs.dependencies]
 fastapi = "^0.109.2"
-redis = "^5.0.1"
 diskcache = "^5.6.3"
 pandas = "^2.2.0"
 tabulate = "^0.9.0"
 
 
 [tool.ruff] # https://beta.ruff.rs/docs/
 line-length = 100
```

### Comparing `cognee-0.1.6/PKG-INFO` & `cognee-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognee
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning.
 Home-page: https://www.cognee.ai
 License: Apache-2.0
 Author: Vasilije Markovic
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,81 +13,65 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: athena
-Provides-Extra: az
-Provides-Extra: bigquery
 Provides-Extra: cli
-Provides-Extra: databricks
-Provides-Extra: dbt
 Provides-Extra: duckdb
 Provides-Extra: filesystem
-Provides-Extra: gcp
-Provides-Extra: gs
-Provides-Extra: lancedb
 Provides-Extra: motherduck
-Provides-Extra: mssql
 Provides-Extra: neo4j
 Provides-Extra: notebook
 Provides-Extra: parquet
-Provides-Extra: pinecone
-Provides-Extra: postgres
-Provides-Extra: redshift
-Provides-Extra: s3
-Provides-Extra: snowflake
-Provides-Extra: synapse
+Provides-Extra: qdrant
 Provides-Extra: weaviate
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
-Requires-Dist: asyncpg (>=0.28.0,<0.29.0)
 Requires-Dist: boto3 (>=1.26.125,<2.0.0)
 Requires-Dist: debugpy (>=1.8.0,<2.0.0)
 Requires-Dist: dlt (>=0.4.7,<0.5.0)
 Requires-Dist: dspy-ai (==2.4.3)
 Requires-Dist: duckdb-engine (>=0.11.2,<0.12.0)
 Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra == "duckdb" or extra == "motherduck"
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fastembed (>=0.2.5,<0.3.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: graphistry (>=0.33.5,<0.34.0)
-Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: instructor (==1.2.1)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: lancedb (>=0.6.10,<0.7.0) ; extra == "lancedb"
+Requires-Dist: lancedb (>=0.6.10,<0.7.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==1.14.3)
 Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: posthog (>=3.5.0,<4.0.0)
-Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena" or extra == "synapse"
+Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "parquet" or extra == "motherduck"
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pylint (>=3.0.3,<4.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
-Requires-Dist: qdrant-client (>=1.9.0,<2.0.0)
+Requires-Dist: qdrant-client (>=1.9.0,<2.0.0) ; extra == "qdrant"
 Requires-Dist: ruff (>=0.2.2,<0.3.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
+Requires-Dist: tantivy (>=0.21.0,<0.22.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: uvicorn (==0.22.0)
 Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate"
-Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/topoteretes/cognee
 Description-Content-Type: text/markdown
 
 # cognee
 
 Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and vector retrieval
 
@@ -126,22 +110,32 @@
 
 
 
 
 
 ## 📦 Installation
 
-With pip:
+### With pip
 
 ```bash
+pip install cognee
+```
+
+Use Weaviate vector storage:
+```bash
 pip install "cognee[weaviate]"
 ```
 
-With poetry:
+### With poetry
+
+```bash
+poetry add cognee
+```
 
+Use Weaviate vector storage:
 ```bash
 poetry add "cognee[weaviate]"
 ```
 
 ## 💻 Usage
 
 ### Setup
```

#### html2text {}

```diff
@@ -1,66 +1,62 @@
-Metadata-Version: 2.1 Name: cognee Version: 0.1.6 Summary: Cognee - is a
+Metadata-Version: 2.1 Name: cognee Version: 0.1.7 Summary: Cognee - is a
 library for enriching LLM context with a semantic layer for better
 understanding and reasoning. Home-page: https://www.cognee.ai License: Apache-
 2.0 Author: Vasilije Markovic Requires-Python: >=3.9.0,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Software
-Development :: Libraries Provides-Extra: athena Provides-Extra: az Provides-
-Extra: bigquery Provides-Extra: cli Provides-Extra: databricks Provides-Extra:
-dbt Provides-Extra: duckdb Provides-Extra: filesystem Provides-Extra: gcp
-Provides-Extra: gs Provides-Extra: lancedb Provides-Extra: motherduck Provides-
-Extra: mssql Provides-Extra: neo4j Provides-Extra: notebook Provides-Extra:
-parquet Provides-Extra: pinecone Provides-Extra: postgres Provides-Extra:
-redshift Provides-Extra: s3 Provides-Extra: snowflake Provides-Extra: synapse
-Provides-Extra: weaviate Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-
-Dist: aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: anthropic (>=0.21.3,<0.22.0)
-Requires-Dist: asyncpg (>=0.28.0,<0.29.0) Requires-Dist: boto3
-(>=1.26.125,<2.0.0) Requires-Dist: debugpy (>=1.8.0,<2.0.0) Requires-Dist: dlt
-(>=0.4.7,<0.5.0) Requires-Dist: dspy-ai (==2.4.3) Requires-Dist: duckdb-engine
-(>=0.11.2,<0.12.0) Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra ==
-"duckdb" or extra == "motherduck" Requires-Dist: fastapi (>=0.109.2,<0.110.0)
-Requires-Dist: fastembed (>=0.2.5,<0.3.0) Requires-Dist: filetype
-(>=1.2.0,<2.0.0) Requires-Dist: graphistry (>=0.33.5,<0.34.0) Requires-Dist:
-graphviz (>=0.20.1,<0.21.0) Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-
-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: instructor (==1.2.1) Requires-
-Dist: jinja2 (>=3.1.3,<4.0.0) Requires-Dist: lancedb (>=0.6.10,<0.7.0) ; extra
-== "lancedb" Requires-Dist: matplotlib (>=3.8.3,<4.0.0) Requires-Dist: neo4j
-(>=5.18.0,<6.0.0) ; extra == "neo4j" Requires-Dist: nest-asyncio
-(>=1.6.0,<2.0.0) Requires-Dist: networkx (>=3.2.1,<4.0.0) Requires-Dist: nltk
-(>=3.8.1,<4.0.0) Requires-Dist: openai (==1.14.3) Requires-Dist: overrides
-(>=7.7.0,<8.0.0) ; extra == "notebook" Requires-Dist: pandas (>=2.2.0,<3.0.0)
-Requires-Dist: posthog (>=3.5.0,<4.0.0) Requires-Dist: pyarrow
-(>=15.0.0,<16.0.0) ; extra == "bigquery" or extra == "parquet" or extra ==
-"motherduck" or extra == "athena" or extra == "synapse" Requires-Dist: pydantic
-(>=2.5.0,<3.0.0) Requires-Dist: pylint (>=3.0.3,<4.0.0) Requires-Dist: pypdf
-(>=4.1.0,<5.0.0) Requires-Dist: python-dotenv (==1.0.1) Requires-Dist: qdrant-
-client (>=1.9.0,<2.0.0) Requires-Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist:
-scikit-learn (>=1.4.1.post1,<2.0.0) Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
-Requires-Dist: structlog (>=24.1.0,<25.0.0) Requires-Dist: tenacity
-(>=8.2.3,<9.0.0) Requires-Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist:
-uvicorn (==0.22.0) Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra ==
-"weaviate" Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL: Repository,
-https://github.com/topoteretes/cognee Description-Content-Type: text/markdown #
-cognee Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and
-vector retrieval
+Development :: Libraries Provides-Extra: cli Provides-Extra: duckdb Provides-
+Extra: filesystem Provides-Extra: motherduck Provides-Extra: neo4j Provides-
+Extra: notebook Provides-Extra: parquet Provides-Extra: qdrant Provides-Extra:
+weaviate Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aiosqlite
+(>=0.20.0,<0.21.0) Requires-Dist: anthropic (>=0.21.3,<0.22.0) Requires-Dist:
+boto3 (>=1.26.125,<2.0.0) Requires-Dist: debugpy (>=1.8.0,<2.0.0) Requires-
+Dist: dlt (>=0.4.7,<0.5.0) Requires-Dist: dspy-ai (==2.4.3) Requires-Dist:
+duckdb-engine (>=0.11.2,<0.12.0) Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0)
+; extra == "duckdb" or extra == "motherduck" Requires-Dist: fastapi
+(>=0.109.2,<0.110.0) Requires-Dist: fastembed (>=0.2.5,<0.3.0) Requires-Dist:
+filetype (>=1.2.0,<2.0.0) Requires-Dist: graphistry (>=0.33.5,<0.34.0)
+Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-Dist: gunicorn
+(>=20.1.0,<21.0.0) Requires-Dist: instructor (==1.2.1) Requires-Dist: jinja2
+(>=3.1.3,<4.0.0) Requires-Dist: lancedb (>=0.6.10,<0.7.0) Requires-Dist:
+matplotlib (>=3.8.3,<4.0.0) Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra ==
+"neo4j" Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist: networkx
+(>=3.2.1,<4.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai
+(==1.14.3) Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
+Requires-Dist: pandas (>=2.2.0,<3.0.0) Requires-Dist: posthog (>=3.5.0,<4.0.0)
+Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "parquet" or extra ==
+"motherduck" Requires-Dist: pydantic (>=2.5.0,<3.0.0) Requires-Dist: pylint
+(>=3.0.3,<4.0.0) Requires-Dist: pypdf (>=4.1.0,<5.0.0) Requires-Dist: python-
+dotenv (==1.0.1) Requires-Dist: qdrant-client (>=1.9.0,<2.0.0) ; extra ==
+"qdrant" Requires-Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist: scikit-learn
+(>=1.4.1.post1,<2.0.0) Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0) Requires-
+Dist: structlog (>=24.1.0,<25.0.0) Requires-Dist: tantivy (>=0.21.0,<0.22.0)
+Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-Dist: tiktoken
+(>=0.6.0,<0.7.0) Requires-Dist: uvicorn (==0.22.0) Requires-Dist: weaviate-
+client (>=4.5.4,<5.0.0) ; extra == "weaviate" Project-URL: Repository, https://
+github.com/topoteretes/cognee Description-Content-Type: text/markdown # cognee
+Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and vector
+retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
 Open-source framework for creating self-improving deterministic outputs for
 LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
 ![Cognee Demo](assets/cognee_demo.gif) Try it in a Google collab _n_o_t_e_b_o_o_k or
 have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n Join our _D_i_s_c_o_r_d community ## ð¦
-Installation With pip: ```bash pip install "cognee[weaviate]" ``` With poetry:
-```bash poetry add "cognee[weaviate]" ``` ## ð» Usage ### Setup ``` import os
-os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"]
-= "YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+Installation ### With pip ```bash pip install cognee ``` Use Weaviate vector
+storage: ```bash pip install "cognee[weaviate]" ``` ### With poetry ```bash
+poetry add cognee ``` Use Weaviate vector storage: ```bash poetry add "cognee
+[weaviate]" ``` ## ð» Usage ### Setup ``` import os os.environ
+["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"] =
+"YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
 ``` You can also use Ollama or Anyscale as your LLM provider. For more info on
 local models check our [docs](https://topoteretes.github.io/cognee) ### Run ```
 import cognee text = """Natural language processing (NLP) is an
 interdisciplinary subfield of computer science and information retrieval"""
 cognee.add([text], "example_dataset") # Add a new piece of information
 cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
 cognee.search("SIMILARITY", "computer science") # Query cognee for the
```

