# Comparing `tmp/scrapegraphai-0.7.0b1.tar.gz` & `tmp/scrapegraphai-0.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.7.0b1.tar", max compression
+gzip compressed data, was "scrapegraphai-0.7.0b2.tar", max compression
```

## Comparing `scrapegraphai-0.7.0b1.tar` & `scrapegraphai-0.7.0b2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1065 2024-05-03 12:19:31.047283 scrapegraphai-0.7.0b1/LICENSE
--rw-r--r--   0        0        0    10242 2024-05-03 12:19:31.047283 scrapegraphai-0.7.0b1/README.md
--rw-r--r--   0        0        0     1738 2024-05-03 12:19:49.671407 scrapegraphai-0.7.0b1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      402 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     7126 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2672 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3594 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3880 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3650 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3749 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4575 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3738 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1959 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      342 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      463 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      676 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7932 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3716 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6987 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6431 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6987 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     6639 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5835 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5605 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3707 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6261 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1605 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-03 12:19:31.079283 scrapegraphai-0.7.0b1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    12086 1970-01-01 00:00:00.000000 scrapegraphai-0.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-03 19:41:08.123685 scrapegraphai-0.7.0b2/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-03 19:41:08.123685 scrapegraphai-0.7.0b2/README.md
+-rw-r--r--   0        0        0     1738 2024-05-03 19:41:27.831693 scrapegraphai-0.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-03 19:41:08.151686 scrapegraphai-0.7.0b2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      402 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    10586 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3594 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3880 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3650 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3749 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4575 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1959 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      342 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      463 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      676 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7932 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3716 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6987 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6431 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6987 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     6639 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3527 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1955 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     2684 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4303 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5605 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3707 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6261 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2317 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1605 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-03 19:41:08.155686 scrapegraphai-0.7.0b2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12086 1970-01-01 00:00:00.000000 scrapegraphai-0.7.0b2/PKG-INFO
```

### Comparing `scrapegraphai-0.7.0b1/LICENSE` & `scrapegraphai-0.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/README.md` & `scrapegraphai-0.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/pyproject.toml` & `scrapegraphai-0.7.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.7.0b1"
+version = "0.7.0b2"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.7.0b2/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/abstract_graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 AbstractGraph Module
 """
 
 from abc import ABC, abstractmethod
 from typing import Optional
 
-from ..models import OpenAI, Gemini, Ollama, AzureOpenAI, HuggingFace, Groq, Bedrock
+from langchain_aws.embeddings.bedrock import BedrockEmbeddings
+from langchain_community.embeddings import HuggingFaceHubEmbeddings, OllamaEmbeddings
+from langchain_openai import AzureOpenAIEmbeddings, OpenAIEmbeddings
+
 from ..helpers import models_tokens
+from ..models import AzureOpenAI, Bedrock, Gemini, Groq, HuggingFace, Ollama, OpenAI
 
 
 class AbstractGraph(ABC):
     """
     Scaffolding class for creating a graph representation and executing it.
 
     Attributes:
@@ -39,15 +43,16 @@
 
     def __init__(self, prompt: str, config: dict, source: Optional[str] = None):
 
         self.prompt = prompt
         self.source = source
         self.config = config
         self.llm_model = self._create_llm(config["llm"], chat=True)
-        self.embedder_model = self.llm_model if "embeddings" not in config else self._create_llm(
+        self.embedder_model = self._create_default_embedder(    
+            ) if "embeddings" not in config else self._create_embedder(
             config["embeddings"])
 
         # Set common configuration parameters
         self.verbose = True if config is None else config.get("verbose", False)
         self.headless = True if config is None else config.get(
             "headless", True)
 
@@ -161,14 +166,93 @@
                 "model_kwargs": {
                     "temperature": llm_params["temperature"],
                 }
             })
         else:
             raise ValueError(
                 "Model provided by the configuration not supported")
+    
+    def _create_default_embedder(self) -> object:
+        """
+        Create an embedding model instance based on the chosen llm model.
+
+        Returns:
+            object: An instance of the embedding model client.
+
+        Raises:
+            ValueError: If the model is not supported.
+        """
+
+        if isinstance(self.llm_model, OpenAI):
+            return OpenAIEmbeddings(api_key=self.llm_model.openai_api_key)
+        elif isinstance(self.llm_model, AzureOpenAIEmbeddings):
+            return self.llm_model
+        elif isinstance(self.llm_model, AzureOpenAI):
+            return AzureOpenAIEmbeddings()
+        elif isinstance(self.llm_model, Ollama):
+            # unwrap the kwargs from the model whihc is a dict
+            params = self.llm_model._lc_kwargs
+            # remove streaming and temperature
+            params.pop("streaming", None)
+            params.pop("temperature", None)
+
+            return OllamaEmbeddings(**params)
+        elif isinstance(self.llm_model, HuggingFace):
+            return HuggingFaceHubEmbeddings(model=self.llm_model.model)
+        elif isinstance(self.llm_model, Bedrock):
+            return BedrockEmbeddings(client=None, model_id=self.llm_model.model_id)
+        else:
+            raise ValueError("Embedding Model missing or not supported")
+        
+    def _create_embedder(self, embedder_config: dict) -> object:
+        """
+        Create an embedding model instance based on the configuration provided.
+
+        Args:
+            embedder_config (dict): Configuration parameters for the embedding model.
+
+        Returns:
+            object: An instance of the embedding model client.
+
+        Raises:
+            KeyError: If the model is not supported.
+        """
+        
+        # Instantiate the embedding model based on the model name
+        if "openai" in embedder_config["model"]:
+            return OpenAIEmbeddings(api_key=embedder_config["api_key"])
+
+        elif "azure" in embedder_config["model"]:
+            return AzureOpenAIEmbeddings()
+
+        elif "ollama" in embedder_config["model"]:
+            embedder_config["model"] = embedder_config["model"].split("/")[-1]
+            try:
+                models_tokens["ollama"][embedder_config["model"]]
+            except KeyError:
+                raise KeyError("Model not supported")
+            return OllamaEmbeddings(**embedder_config)
+        
+        elif "hugging_face" in embedder_config["model"]:
+            try:
+                models_tokens["hugging_face"][embedder_config["model"]]
+            except KeyError:
+                raise KeyError("Model not supported")
+            return HuggingFaceHubEmbeddings(model=embedder_config["model"])
+        
+        elif "bedrock" in embedder_config["model"]:
+            embedder_config["model"] = embedder_config["model"].split("/")[-1]
+            try:
+                models_tokens["bedrock"][embedder_config["model"]]
+            except KeyError:
+                raise KeyError("Model not supported")
+            return BedrockEmbeddings(client=None, model_id=embedder_config["model"])
+        else:
+            raise ValueError(
+                "Model provided by the configuration not supported") 
 
     def get_state(self, key=None) -> dict:
         """""
         Get the final state of the graph.
 
         Args:
             key (str, optional): The key of the final state to retrieve.
```

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.7.0b2/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.7.0b2/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.7.0b2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.7.0b2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.7.0b2/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.7.0b2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.7.0b2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/rag_node.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,22 +2,17 @@
 RAGNode Module
 """
 
 from typing import List
 from langchain.docstore.document import Document
 from langchain.retrievers import ContextualCompressionRetriever
 from langchain.retrievers.document_compressors import EmbeddingsFilter, DocumentCompressorPipeline
-from langchain_aws.embeddings.bedrock import BedrockEmbeddings
 from langchain_community.document_transformers import EmbeddingsRedundantFilter
-from langchain_community.embeddings import HuggingFaceHubEmbeddings
 from langchain_community.vectorstores import FAISS
-from langchain_community.embeddings import OllamaEmbeddings
-from langchain_openai import OpenAIEmbeddings, AzureOpenAIEmbeddings
 
-from ..models import OpenAI, Ollama, AzureOpenAI, HuggingFace, Bedrock
 from .base_node import BaseNode
 
 
 class RAGNode(BaseNode):
     """
     A node responsible for compressing the input tokens and storing the document
     in a vector database for retrieval. Relevant chunks are stored in the state.
@@ -83,39 +78,15 @@
                 },
             )
             chunked_docs.append(doc)
 
         if self.verbose:
             print("--- (updated chunks metadata) ---")
 
-        # check if embedder_model is provided, if not use llm_model
-        embedding_model = self.embedder_model if self.embedder_model else self.llm_model
-
-        if isinstance(embedding_model, OpenAI):
-            embeddings = OpenAIEmbeddings(
-                api_key=embedding_model.openai_api_key)
-        elif isinstance(embedding_model, AzureOpenAIEmbeddings):
-            embeddings = embedding_model
-        elif isinstance(embedding_model, AzureOpenAI):
-            embeddings = AzureOpenAIEmbeddings()
-        elif isinstance(embedding_model, Ollama):
-            # unwrap the kwargs from the model whihc is a dict
-            params = embedding_model._lc_kwargs
-            # remove streaming and temperature
-            params.pop("streaming", None)
-            params.pop("temperature", None)
-
-            embeddings = OllamaEmbeddings(**params)
-        elif isinstance(embedding_model, HuggingFace):
-            embeddings = HuggingFaceHubEmbeddings(model=embedding_model.model)
-        elif isinstance(embedding_model, Bedrock):
-            embeddings = BedrockEmbeddings(
-                client=None, model_id=embedding_model.model_id)
-        else:
-            raise ValueError("Embedding Model missing or not supported")
+        embeddings = self.embedder_model
 
         retriever = FAISS.from_documents(
             chunked_docs, embeddings).as_retriever()
 
         redundant_filter = EmbeddingsRedundantFilter(embeddings=embeddings)
         # similarity_threshold could be set, now k=20
         relevant_filter = EmbeddingsFilter(embeddings=embeddings)
```

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.7.0b2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/remover.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.7.0b2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.7.0b1/PKG-INFO` & `scrapegraphai-0.7.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.7.0b1
+Version: 0.7.0b2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

