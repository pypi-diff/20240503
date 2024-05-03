# Comparing `tmp/scrapegraphai-0.6.1b1.tar.gz` & `tmp/scrapegraphai-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.6.1b1.tar", max compression
+gzip compressed data, was "scrapegraphai-0.6.2.tar", max compression
```

## Comparing `scrapegraphai-0.6.1b1.tar` & `scrapegraphai-0.6.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1065 2024-05-02 15:58:17.712082 scrapegraphai-0.6.1b1/LICENSE
--rw-r--r--   0        0        0     8876 2024-05-02 15:58:17.712082 scrapegraphai-0.6.1b1/README.md
--rw-r--r--   0        0        0     1739 2024-05-02 15:58:37.872124 scrapegraphai-0.6.1b1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      402 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     7126 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2672 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3594 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3880 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3650 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3749 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4575 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3738 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1909 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      342 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      463 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      644 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7932 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3716 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6987 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6431 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6987 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     6639 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5835 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5605 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3707 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6261 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1605 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    10720 1970-01-01 00:00:00.000000 scrapegraphai-0.6.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-02 19:06:48.483100 scrapegraphai-0.6.2/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-02 19:06:48.483100 scrapegraphai-0.6.2/README.md
+-rw-r--r--   0        0        0     1736 2024-05-02 19:07:26.195304 scrapegraphai-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      402 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     7126 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3594 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3880 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3650 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3749 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4575 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1959 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      342 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      463 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      644 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7932 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3716 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6987 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6431 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6987 2024-05-02 19:06:48.511100 scrapegraphai-0.6.2/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     6639 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3527 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1955 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     2684 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5835 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5605 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3707 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6261 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2317 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1605 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-02 19:06:48.515100 scrapegraphai-0.6.2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12084 1970-01-01 00:00:00.000000 scrapegraphai-0.6.2/PKG-INFO
```

### Comparing `scrapegraphai-0.6.1b1/LICENSE` & `scrapegraphai-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/README.md` & `scrapegraphai-0.6.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -164,15 +164,46 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-### Case 5: Extracting information using Gemini 
+
+### Case 5: Extracting information using Azure
+```python
+from langchain_openai import AzureChatOpenAI
+from langchain_openai import AzureOpenAIEmbeddings
+
+lm_model_instance = AzureChatOpenAI(
+    openai_api_version=os.environ["AZURE_OPENAI_API_VERSION"],
+    azure_deployment=os.environ["AZURE_OPENAI_CHAT_DEPLOYMENT_NAME"]
+)
+
+embedder_model_instance = AzureOpenAIEmbeddings(
+    azure_deployment=os.environ["AZURE_OPENAI_EMBEDDINGS_DEPLOYMENT_NAME"],
+    openai_api_version=os.environ["AZURE_OPENAI_API_VERSION"],
+)
+graph_config = {
+    "llm": {"model_instance": llm_model_instance},
+    "embeddings": {"model_instance": embedder_model_instance}
+}
+
+smart_scraper_graph = SmartScraperGraph(
+    prompt="""List me all the events, with the following fields: company_name, event_name, event_start_date, event_start_time, 
+    event_end_date, event_end_time, location, event_mode, event_category, 
+    third_party_redirect, no_of_days, 
+    time_in_hours, hosted_or_attending, refreshments_type, 
+    registration_available, registration_link""",
+    source="https://www.hmhco.com/event",
+    config=graph_config
+)
+```
+
+### Case 6: Extracting information using Gemini 
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 GOOGLE_APIKEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
@@ -211,14 +242,19 @@
 
 Please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
 [![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 [![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraphai)
 
+## 📈 Roadmap
+Check out the project roadmap [here](docs/README.md)! 🚀
+
+Wanna visualize the roadmap in a more interactive way? Check out the [markmap](https://markmap.js.org/repl) visualization by copy pasting the markdown content in the editor!
+
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
 
 ## 🎓 Citations
 If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
@@ -245,8 +281,8 @@
 ## 📜 License
 
 ScrapeGraphAI is licensed under the MIT License. See the [LICENSE](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE) file for more information.
 
 ## Acknowledgements
 
 - We would like to thank all the contributors to the project and the open-source community for their support.
-- ScrapeGraphAI is meant to be used for data exploration and research purposes only. We are not responsible for any misuse of the library.
+- ScrapeGraphAI is meant to be used for data exploration and research purposes only. We are not responsible for any misuse of the library.
```

### Comparing `scrapegraphai-0.6.1b1/pyproject.toml` & `scrapegraphai-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.6.1b1"
-
+version = "0.6.2"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.6.2/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.6.2/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.6.2/scrapegraphai/helpers/models_tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,17 @@
         "gpt-4-vision-preview": 128000,
         "gpt-4": 8192,
         "gpt-4-0613": 8192,
         "gpt-4-32k": 32768,
         "gpt-4-32k-0613": 32768,
     },
     "azure": {
-        "gpt-3.5-turbo": 4096
+        "gpt-3.5-turbo": 4096,
+        "gpt-4": 8192,
+        "gpt-4-32k": 32768
     },
     "gemini": {
         "gemini-pro": 128000,
     },
 
     "ollama": {
         "llama2": 4096,
@@ -61,8 +63,7 @@
         "mistral.mistral-7b-instruct-v0:2": 32768,
         "mistral.mixtral-8x7b-instruct-v0:1": 32768,
         "mistral.mistral-large-2402-v1:0": 32768,
         "cohere.embed-english-v3": 512,
         "cohere.embed-multilingual-v3": 512
     }
 }
-
```

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.6.2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.6.2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.6.2/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.6.2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.6.2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.6.2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/remover.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.6.2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.1b1/PKG-INFO` & `scrapegraphai-0.6.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.6.1b1
+Version: 0.6.2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -204,15 +204,46 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-### Case 5: Extracting information using Gemini 
+
+### Case 5: Extracting information using Azure
+```python
+from langchain_openai import AzureChatOpenAI
+from langchain_openai import AzureOpenAIEmbeddings
+
+lm_model_instance = AzureChatOpenAI(
+    openai_api_version=os.environ["AZURE_OPENAI_API_VERSION"],
+    azure_deployment=os.environ["AZURE_OPENAI_CHAT_DEPLOYMENT_NAME"]
+)
+
+embedder_model_instance = AzureOpenAIEmbeddings(
+    azure_deployment=os.environ["AZURE_OPENAI_EMBEDDINGS_DEPLOYMENT_NAME"],
+    openai_api_version=os.environ["AZURE_OPENAI_API_VERSION"],
+)
+graph_config = {
+    "llm": {"model_instance": llm_model_instance},
+    "embeddings": {"model_instance": embedder_model_instance}
+}
+
+smart_scraper_graph = SmartScraperGraph(
+    prompt="""List me all the events, with the following fields: company_name, event_name, event_start_date, event_start_time, 
+    event_end_date, event_end_time, location, event_mode, event_category, 
+    third_party_redirect, no_of_days, 
+    time_in_hours, hosted_or_attending, refreshments_type, 
+    registration_available, registration_link""",
+    source="https://www.hmhco.com/event",
+    config=graph_config
+)
+```
+
+### Case 6: Extracting information using Gemini 
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 GOOGLE_APIKEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
@@ -251,14 +282,19 @@
 
 Please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
 [![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 [![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraphai)
 
+## 📈 Roadmap
+Check out the project roadmap [here](docs/README.md)! 🚀
+
+Wanna visualize the roadmap in a more interactive way? Check out the [markmap](https://markmap.js.org/repl) visualization by copy pasting the markdown content in the editor!
+
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
 
 ## 🎓 Citations
 If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
@@ -286,8 +322,7 @@
 
 ScrapeGraphAI is licensed under the MIT License. See the [LICENSE](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/LICENSE) file for more information.
 
 ## Acknowledgements
 
 - We would like to thank all the contributors to the project and the open-source community for their support.
 - ScrapeGraphAI is meant to be used for data exploration and research purposes only. We are not responsible for any misuse of the library.
-
```

