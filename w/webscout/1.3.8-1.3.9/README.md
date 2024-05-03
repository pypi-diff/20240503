# Comparing `tmp/webscout-1.3.8.tar.gz` & `tmp/webscout-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.3.8.tar", last modified: Sat Apr 27 04:17:20 2024, max compression
+gzip compressed data, was "webscout-1.3.9.tar", last modified: Fri May  3 04:56:08 2024, max compression
```

## Comparing `webscout-1.3.8.tar` & `webscout-1.3.9.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 04:17:19.994212 webscout-1.3.8/
-drwxrwxrwx   0        0        0        0 2024-04-27 04:17:17.415532 webscout-1.3.8/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:17:17.511538 webscout-1.3.8/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:17:17.645641 webscout-1.3.8/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:17:17.731006 webscout-1.3.8/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-26 07:30:49.000000 webscout-1.3.8/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-26 07:30:49.000000 webscout-1.3.8/LICENSE.md
--rw-rw-rw-   0        0        0    32476 2024-04-27 04:17:19.937220 webscout-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    30264 2024-04-26 07:30:49.000000 webscout-1.3.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 04:17:19.995217 webscout-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2744 2024-04-27 04:03:52.000000 webscout-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:17:19.573478 webscout-1.3.8/webscout/
--rw-rw-rw-   0        0        0   110135 2024-04-27 04:03:40.000000 webscout-1.3.8/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/AIbase.py
--rw-rw-rw-   0        0        0    32585 2024-04-26 17:05:18.000000 webscout-1.3.8/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/LLM.py
--rw-rw-rw-   0        0        0     1042 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/exceptions.py
--rw-rw-rw-   0        0        0    16831 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/models.py
--rw-rw-rw-   0        0        0    20622 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-27 04:03:58.000000 webscout-1.3.8/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/voice.py
--rw-rw-rw-   0        0        0    80881 2024-04-26 16:26:03.000000 webscout-1.3.8/webscout/webai.py
--rw-rw-rw-   0        0        0     3085 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-26 07:30:49.000000 webscout-1.3.8/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:17:19.892217 webscout-1.3.8/webscout.egg-info/
--rw-rw-rw-   0        0        0    32476 2024-04-27 04:17:16.000000 webscout-1.3.8/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-04-27 04:17:16.000000 webscout-1.3.8/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:17:16.000000 webscout-1.3.8/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-27 04:17:16.000000 webscout-1.3.8/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      341 2024-04-27 04:17:16.000000 webscout-1.3.8/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-27 04:17:16.000000 webscout-1.3.8/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 04:56:07.630790 webscout-1.3.9/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:56:05.832325 webscout-1.3.9/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:56:06.107872 webscout-1.3.9/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:56:06.339994 webscout-1.3.9/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:56:06.459578 webscout-1.3.9/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-26 07:30:49.000000 webscout-1.3.9/LICENSE.md
+-rw-rw-rw-   0        0        0    31949 2024-05-03 04:56:07.354297 webscout-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    29695 2024-05-03 03:46:18.000000 webscout-1.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 04:56:07.632798 webscout-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2772 2024-05-03 03:40:51.000000 webscout-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:56:07.103063 webscout-1.3.9/webscout/
+-rw-rw-rw-   0        0        0   202197 2024-05-03 04:52:32.000000 webscout-1.3.9/webscout/AI.py
+-rw-rw-rw-   0        0        0     4710 2024-05-03 04:08:13.000000 webscout-1.3.9/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33135 2024-05-03 04:26:47.000000 webscout-1.3.9/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/LLM.py
+-rw-rw-rw-   0        0        0     1046 2024-05-03 03:49:13.000000 webscout-1.3.9/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/__main__.py
+-rw-rw-rw-   0        0        0      939 2024-05-03 03:36:32.000000 webscout-1.3.9/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/cli.py
+-rw-rw-rw-   0        0        0      378 2024-05-03 02:40:34.000000 webscout-1.3.9/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24451 2024-05-03 03:31:40.000000 webscout-1.3.9/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-05-03 03:38:17.000000 webscout-1.3.9/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/voice.py
+-rw-rw-rw-   0        0        0    81661 2024-05-03 04:48:27.000000 webscout-1.3.9/webscout/webai.py
+-rw-rw-rw-   0        0        0     3085 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:56:07.333311 webscout-1.3.9/webscout.egg-info/
+-rw-rw-rw-   0        0        0    31949 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-05-03 04:56:05.000000 webscout-1.3.9/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.3.8/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.3.9/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.3.9/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/DeepWEBS/networks/filepath_converter.py` & `webscout-1.3.9/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/DeepWEBS/networks/google_searcher.py` & `webscout-1.3.9/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/DeepWEBS/networks/network_configs.py` & `webscout-1.3.9/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.3.9/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/DeepWEBS/utilsdw/enver.py` & `webscout-1.3.9/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/DeepWEBS/utilsdw/logger.py` & `webscout-1.3.9/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/LICENSE.md` & `webscout-1.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/PKG-INFO` & `webscout-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.8
+Version: 1.3.9
 Summary: Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -43,14 +43,15 @@
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
+Requires-Dist: appdirsGoogleBard1>=2.1.4
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 #  webscout
 <p align="center">
 
@@ -93,18 +94,16 @@
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
-    - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
-    - [11. `Reka` - chat with reka](#11-reka---chat-with-reka)
-    - [12. `Cohere` - chat with cohere](#12-cohere---chat-with-cohere)
-  - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
+    - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
+    - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -685,47 +684,36 @@
 response = koboldai.ask(prompt)
 
 # Extract and print the message from the response
 message = koboldai.get_message(response)
 print(message)
 
 ```
-### 10. `Sean` - chat With Sean
-```python
-from webscout.AI import Sean
-
-a = Sean(is_conversation=True, max_tokens=8000, timeout=30)
-# This example sends a simple greeting and prints the response
-prompt = "tell me about india"
-response_str = a.chat(prompt)
-print(response_str)
-```
 
-### 11. `Reka` - chat with reka
+### 10. `Reka` - chat with reka
 ```python
 from webscout.AI import REKA
 
 a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
-### 12. `Cohere` - chat with cohere
+### 11. `Cohere` - chat with cohere
 ```python
 from webscout.AI import Cohere
 
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
-## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
@@ -840,15 +828,15 @@
         webai_bot = Main(
             max_tokens=500, 
             provider="cohere",
             temperature=0.7,  
             top_k=40,          
             top_p=0.95,        
             model="command-r-plus",  # Replace with your desired model
-            auth="0zoQbKs1AAgd8WrPBO9CTIGgVvm5ZMbDcCqJOVyl",     # Replace with your auth key/value (if needed)
+            auth=None,     # Replace with your auth key/value (if needed)
             timeout=30,
             disable_conversation=True,
             filepath=None,
             update_file=True,
             intro=None,
             rawdog=True,
             history_offset=10250,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.8 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.3.9 Summary: Search for
 anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc
 Also containes AI models, can transcribe yt videos, have TTS support and now
 has webai(terminal gpt and open interpeter) support Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -21,17 +21,17 @@
 curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
 asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Requires-Dist: PyYAML Provides-Extra: dev Requires-Dist:
-ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" #
-webscout
+Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist:
+appdirsGoogleBard1>=2.1.4 Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
+== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
        _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos, have TTS support and now has webai(terminal gpt and open
  interpeter) support ## Table of Contents - [webscout](#webscout) - [Table of
    Contents](#table-of-contents) - [Install](#install) - [CLI version](#cli-
      version) - [CLI to use LLM](#cli-to-use-llm) - [Regions](#regions) -
   [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
@@ -59,54 +59,52 @@
 `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
 - search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
 image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
 [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
   [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
 blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
  with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
-  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` - chat With Sean]
- (#10-sean---chat-with-sean) - [11. `Reka` - chat with reka](#11-reka---chat-
-with-reka) - [12. `Cohere` - chat with cohere](#12-cohere---chat-with-cohere) -
- [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-
-  llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet]
-(#llm-with-internet) - [`Webai` - terminal gpt and a open interpeter](#webai---
-    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
- ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
-  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
-Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
-for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
- Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
-cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
-fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
-for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
- for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
-lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
- my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
-    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
- Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
-for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
- ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
-for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
- for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka]
+ (#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---
+chat-with-cohere) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) -
+  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
+   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
+version ```python3 python -m webscout --help ``` | Command | Description | |---
+----------------------------------------|--------------------------------------
+ -----------------------------------------------------------------| | python -
+ m webscout answers -k Text | CLI function to perform an answers search using
+ Webscout. | | python -m webscout images -k Text | CLI function to perform an
+    images search using Webscout. | | python -m webscout maps -k Text | CLI
+function to perform a maps search using Webscout. | | python -m webscout news -
+  k Text | CLI function to perform a news search using Webscout. | | python -
+ m webscout suggestions -k Text | CLI function to perform a suggestions search
+using Webscout. | | python -m webscout text -k Text | CLI function to perform a
+  text search using Webscout. | | python -m webscout translate -k Text | CLI
+function to perform translate using Webscout. | | python -m webscout version |
+  A command-line interface command that prints and returns the version of the
+  program. | | python -m webscout videos -k Text | CLI function to perform a
+  videos search using DuckDuckGo API. | ## CLI to use LLM ```python python -
+  m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for
+Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for
+ Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg
+for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
+  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
+Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
+de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
+for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
+for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
+lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
+  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
+ Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
+  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
+ Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
+     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
+    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
+Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
+   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
      Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Transcriber The
    transcriber function in webscout is a handy tool that transcribes YouTube
  videos. Here's an example code demonstrating its usage: ```python import sys
 from webscout import transcriber def extract_transcript(video_id): """Extracts
         the transcript from a YouTube video.""" try: transcript_list =
    transcriber.list_transcripts(video_id) for transcript in transcript_list:
      transcript_data_list = transcript.fetch() lang = transcript.language
@@ -305,73 +303,68 @@
     simple greeting and prints the response prompt = "tell me about india"
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
-(message) ``` ### 10. `Sean` - chat With Sean ```python from webscout.AI import
-Sean a = Sean(is_conversation=True, max_tokens=8000, timeout=30) # This example
-sends a simple greeting and prints the response prompt = "tell me about india"
-  response_str = a.chat(prompt) print(response_str) ``` ### 11. `Reka` - chat
-with reka ```python from webscout.AI import REKA a = REKA(is_conversation=True,
-    max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
- response_str = a.chat(prompt) print(response_str) ``` ### 12. `Cohere` - chat
-        with cohere ```python from webscout.AI import Cohere a = Cohere
- (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
-me about india" response_str = a.chat(prompt) print(response_str) ``` ## usage
-  of special .LLM file from webscout (webscout.LLM) ### `LLM` ```python from
-   webscout.LLM import LLM # Read the system message from the file with open
-('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
-   class with the model name and system message llm = LLM(model="microsoft/
- WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
-input user_input = input("User: ") # Define the messages to be sent messages =
- [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
-get the response response = llm.chat(messages) # Print the response print("AI:
-   ", response) ``` ### `LLM` with internet ```python from __future__ import
-  annotations from typing import List, Optional from webscout import LLM from
-   webscout import WEBS import warnings system_message: str = ( "As AI, you
-  possess internet access and are capable of executing real-time web searches
-     based on user inputs. " "You shall utilize this capability to enrich
-conversations, offer informed insights, and augment your ability to " "respond
- accurately and thoroughly. However, refrain from stating 'You have provided a
-   list of strings,' ensuring " "seamless interactions with users. Embrace a
-    responsive demeanor, harnessing available online resources to address "
-  "queries, share pertinent content, and facilitate meaningful exchanges. By
-  doing so, you create value through " "connection and engagement, ultimately
- enhancing overall user satisfaction and experience. Additionally, " "continue
- upholding the principles of respect, impartiality, and intellectual integrity
-       throughout all interactions." ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
- Parameters ---------- user_input : str The user input to be used for the web
-  search webs : WEBS The web search instance to be used to perform the search
-max_results : int, optional The maximum number of search results to include in
-    the response, by default 10 Returns ------- Optional[str] The response
-generated by the LLM model, or None if there is no response """ # Perform a web
-    search based on the user input search_results: List[str] = [] for r in
-    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
-max_results=max_results ): search_results.append(str(r)) # Convert each result
-to a string # Define the messages to be sent, including the user input, search
-results, and system message messages = [ {"role": "user", "content": user_input
-  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
- chat method to get the response response = LLM.chat(messages) return response
-if __name__ == "__main__": while True: # Get the user input user_input = input
-("User: ") # Perform a web search based on the user input with WEBS() as webs:
-response = chat(user_input, webs) # Print the response if response: print("AI:
-  ", response) else: print("No response") ``` ## `Webai` - terminal gpt and a
-         open interpeter ```python from webscout.webai import Main def
- use_rawdog_with_webai(prompt): """ Wrap the webscout default method in a try-
-except block to catch any unhandled exceptions and print a helpful message. """
-  try: webai_bot = Main( max_tokens=500, provider="cohere", temperature=0.7,
-top_k=40, top_p=0.95, model="command-r-plus", # Replace with your desired model
-auth="0zoQbKs1AAgd8WrPBO9CTIGgVvm5ZMbDcCqJOVyl", # Replace with your auth key/
-    value (if needed) timeout=30, disable_conversation=True, filepath=None,
-       update_file=True, intro=None, rawdog=True, history_offset=10250,
+(message) ``` ### 10. `Reka` - chat with reka ```python from webscout.AI import
+  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
+      prompt = "tell me about india" response_str = a.chat(prompt) print
+     (response_str) ``` ### 11. `Cohere` - chat with cohere ```python from
+  webscout.AI import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
+  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
+ (prompt) print(response_str) ``` ### `LLM` ```python from webscout.LLM import
+  LLM # Read the system message from the file with open('system.txt', 'r') as
+ file: system_message = file.read() # Initialize the LLM class with the model
+     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
+ system_message=system_message) while True: # Get the user input user_input =
+input("User: ") # Define the messages to be sent messages = [ {"role": "user",
+  "content": user_input} ] # Use the mistral_chat method to get the response
+response = llm.chat(messages) # Print the response print("AI: ", response) ```
+   ### `LLM` with internet ```python from __future__ import annotations from
+typing import List, Optional from webscout import LLM from webscout import WEBS
+import warnings system_message: str = ( "As AI, you possess internet access and
+ are capable of executing real-time web searches based on user inputs. " "You
+shall utilize this capability to enrich conversations, offer informed insights,
+  and augment your ability to " "respond accurately and thoroughly. However,
+    refrain from stating 'You have provided a list of strings,' ensuring "
+ "seamless interactions with users. Embrace a responsive demeanor, harnessing
+available online resources to address " "queries, share pertinent content, and
+   facilitate meaningful exchanges. By doing so, you create value through "
+"connection and engagement, ultimately enhancing overall user satisfaction and
+  experience. Additionally, " "continue upholding the principles of respect,
+  impartiality, and intellectual integrity throughout all interactions." ) #
+       Ignore the specific UserWarning warnings.filterwarnings("ignore",
+      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
+ (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
+ [str]: """ Chat function to perform a web search based on the user input and
+generate a response using the LLM model. Parameters ---------- user_input : str
+    The user input to be used for the web search webs : WEBS The web search
+   instance to be used to perform the search max_results : int, optional The
+  maximum number of search results to include in the response, by default 10
+Returns ------- Optional[str] The response generated by the LLM model, or None
+  if there is no response """ # Perform a web search based on the user input
+search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
+          safesearch="off", timelimit="y", max_results=max_results ):
+ search_results.append(str(r)) # Convert each result to a string # Define the
+   messages to be sent, including the user input, search results, and system
+message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
+results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
+     response response = LLM.chat(messages) return response if __name__ ==
+  "__main__": while True: # Get the user input user_input = input("User: ") #
+ Perform a web search based on the user input with WEBS() as webs: response =
+chat(user_input, webs) # Print the response if response: print("AI:", response)
+else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
+ ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
+    """ Wrap the webscout default method in a try-except block to catch any
+  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
+  ( max_tokens=500, provider="cohere", temperature=0.7, top_k=40, top_p=0.95,
+model="command-r-plus", # Replace with your desired model auth=None, # Replace
+  with your auth key/value (if needed) timeout=30, disable_conversation=True,
+filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
       awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
 webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
      if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
 use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
                         --provider "phind" --rawdog ```
```

### Comparing `webscout-1.3.8/README.md` & `webscout-1.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,16 @@
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
-    - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
-    - [11. `Reka` - chat with reka](#11-reka---chat-with-reka)
-    - [12. `Cohere` - chat with cohere](#12-cohere---chat-with-cohere)
-  - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
+    - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
+    - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -632,47 +630,36 @@
 response = koboldai.ask(prompt)
 
 # Extract and print the message from the response
 message = koboldai.get_message(response)
 print(message)
 
 ```
-### 10. `Sean` - chat With Sean
-```python
-from webscout.AI import Sean
-
-a = Sean(is_conversation=True, max_tokens=8000, timeout=30)
-# This example sends a simple greeting and prints the response
-prompt = "tell me about india"
-response_str = a.chat(prompt)
-print(response_str)
-```
 
-### 11. `Reka` - chat with reka
+### 10. `Reka` - chat with reka
 ```python
 from webscout.AI import REKA
 
 a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
-### 12. `Cohere` - chat with cohere
+### 11. `Cohere` - chat with cohere
 ```python
 from webscout.AI import Cohere
 
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
-## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
@@ -787,15 +774,15 @@
         webai_bot = Main(
             max_tokens=500, 
             provider="cohere",
             temperature=0.7,  
             top_k=40,          
             top_p=0.95,        
             model="command-r-plus",  # Replace with your desired model
-            auth="0zoQbKs1AAgd8WrPBO9CTIGgVvm5ZMbDcCqJOVyl",     # Replace with your auth key/value (if needed)
+            auth=None,     # Replace with your auth key/value (if needed)
             timeout=30,
             disable_conversation=True,
             filepath=None,
             update_file=True,
             intro=None,
             rawdog=True,
             history_offset=10250,
```

#### html2text {}

```diff
@@ -30,54 +30,52 @@
 `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
 - search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
 image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
 [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
   [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
 blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
  with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
-  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` - chat With Sean]
- (#10-sean---chat-with-sean) - [11. `Reka` - chat with reka](#11-reka---chat-
-with-reka) - [12. `Cohere` - chat with cohere](#12-cohere---chat-with-cohere) -
- [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-
-  llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet]
-(#llm-with-internet) - [`Webai` - terminal gpt and a open interpeter](#webai---
-    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
- ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
-  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
-Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
-for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
- Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
-cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
-fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
-for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
- for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
-lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
- my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
-    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
- Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
-for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
- ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
-for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
- for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka]
+ (#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---
+chat-with-cohere) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) -
+  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
+   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
+version ```python3 python -m webscout --help ``` | Command | Description | |---
+----------------------------------------|--------------------------------------
+ -----------------------------------------------------------------| | python -
+ m webscout answers -k Text | CLI function to perform an answers search using
+ Webscout. | | python -m webscout images -k Text | CLI function to perform an
+    images search using Webscout. | | python -m webscout maps -k Text | CLI
+function to perform a maps search using Webscout. | | python -m webscout news -
+  k Text | CLI function to perform a news search using Webscout. | | python -
+ m webscout suggestions -k Text | CLI function to perform a suggestions search
+using Webscout. | | python -m webscout text -k Text | CLI function to perform a
+  text search using Webscout. | | python -m webscout translate -k Text | CLI
+function to perform translate using Webscout. | | python -m webscout version |
+  A command-line interface command that prints and returns the version of the
+  program. | | python -m webscout videos -k Text | CLI function to perform a
+  videos search using DuckDuckGo API. | ## CLI to use LLM ```python python -
+  m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for
+Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for
+ Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg
+for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
+  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
+Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
+de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
+for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
+for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
+lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
+  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
+ Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
+  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
+ Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
+     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
+    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
+Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
+   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
      Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Transcriber The
    transcriber function in webscout is a handy tool that transcribes YouTube
  videos. Here's an example code demonstrating its usage: ```python import sys
 from webscout import transcriber def extract_transcript(video_id): """Extracts
         the transcript from a YouTube video.""" try: transcript_list =
    transcriber.list_transcripts(video_id) for transcript in transcript_list:
      transcript_data_list = transcript.fetch() lang = transcript.language
@@ -276,73 +274,68 @@
     simple greeting and prints the response prompt = "tell me about india"
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
-(message) ``` ### 10. `Sean` - chat With Sean ```python from webscout.AI import
-Sean a = Sean(is_conversation=True, max_tokens=8000, timeout=30) # This example
-sends a simple greeting and prints the response prompt = "tell me about india"
-  response_str = a.chat(prompt) print(response_str) ``` ### 11. `Reka` - chat
-with reka ```python from webscout.AI import REKA a = REKA(is_conversation=True,
-    max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
- response_str = a.chat(prompt) print(response_str) ``` ### 12. `Cohere` - chat
-        with cohere ```python from webscout.AI import Cohere a = Cohere
- (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
-me about india" response_str = a.chat(prompt) print(response_str) ``` ## usage
-  of special .LLM file from webscout (webscout.LLM) ### `LLM` ```python from
-   webscout.LLM import LLM # Read the system message from the file with open
-('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
-   class with the model name and system message llm = LLM(model="microsoft/
- WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
-input user_input = input("User: ") # Define the messages to be sent messages =
- [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
-get the response response = llm.chat(messages) # Print the response print("AI:
-   ", response) ``` ### `LLM` with internet ```python from __future__ import
-  annotations from typing import List, Optional from webscout import LLM from
-   webscout import WEBS import warnings system_message: str = ( "As AI, you
-  possess internet access and are capable of executing real-time web searches
-     based on user inputs. " "You shall utilize this capability to enrich
-conversations, offer informed insights, and augment your ability to " "respond
- accurately and thoroughly. However, refrain from stating 'You have provided a
-   list of strings,' ensuring " "seamless interactions with users. Embrace a
-    responsive demeanor, harnessing available online resources to address "
-  "queries, share pertinent content, and facilitate meaningful exchanges. By
-  doing so, you create value through " "connection and engagement, ultimately
- enhancing overall user satisfaction and experience. Additionally, " "continue
- upholding the principles of respect, impartiality, and intellectual integrity
-       throughout all interactions." ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
- Parameters ---------- user_input : str The user input to be used for the web
-  search webs : WEBS The web search instance to be used to perform the search
-max_results : int, optional The maximum number of search results to include in
-    the response, by default 10 Returns ------- Optional[str] The response
-generated by the LLM model, or None if there is no response """ # Perform a web
-    search based on the user input search_results: List[str] = [] for r in
-    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
-max_results=max_results ): search_results.append(str(r)) # Convert each result
-to a string # Define the messages to be sent, including the user input, search
-results, and system message messages = [ {"role": "user", "content": user_input
-  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
- chat method to get the response response = LLM.chat(messages) return response
-if __name__ == "__main__": while True: # Get the user input user_input = input
-("User: ") # Perform a web search based on the user input with WEBS() as webs:
-response = chat(user_input, webs) # Print the response if response: print("AI:
-  ", response) else: print("No response") ``` ## `Webai` - terminal gpt and a
-         open interpeter ```python from webscout.webai import Main def
- use_rawdog_with_webai(prompt): """ Wrap the webscout default method in a try-
-except block to catch any unhandled exceptions and print a helpful message. """
-  try: webai_bot = Main( max_tokens=500, provider="cohere", temperature=0.7,
-top_k=40, top_p=0.95, model="command-r-plus", # Replace with your desired model
-auth="0zoQbKs1AAgd8WrPBO9CTIGgVvm5ZMbDcCqJOVyl", # Replace with your auth key/
-    value (if needed) timeout=30, disable_conversation=True, filepath=None,
-       update_file=True, intro=None, rawdog=True, history_offset=10250,
+(message) ``` ### 10. `Reka` - chat with reka ```python from webscout.AI import
+  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
+      prompt = "tell me about india" response_str = a.chat(prompt) print
+     (response_str) ``` ### 11. `Cohere` - chat with cohere ```python from
+  webscout.AI import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
+  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
+ (prompt) print(response_str) ``` ### `LLM` ```python from webscout.LLM import
+  LLM # Read the system message from the file with open('system.txt', 'r') as
+ file: system_message = file.read() # Initialize the LLM class with the model
+     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
+ system_message=system_message) while True: # Get the user input user_input =
+input("User: ") # Define the messages to be sent messages = [ {"role": "user",
+  "content": user_input} ] # Use the mistral_chat method to get the response
+response = llm.chat(messages) # Print the response print("AI: ", response) ```
+   ### `LLM` with internet ```python from __future__ import annotations from
+typing import List, Optional from webscout import LLM from webscout import WEBS
+import warnings system_message: str = ( "As AI, you possess internet access and
+ are capable of executing real-time web searches based on user inputs. " "You
+shall utilize this capability to enrich conversations, offer informed insights,
+  and augment your ability to " "respond accurately and thoroughly. However,
+    refrain from stating 'You have provided a list of strings,' ensuring "
+ "seamless interactions with users. Embrace a responsive demeanor, harnessing
+available online resources to address " "queries, share pertinent content, and
+   facilitate meaningful exchanges. By doing so, you create value through "
+"connection and engagement, ultimately enhancing overall user satisfaction and
+  experience. Additionally, " "continue upholding the principles of respect,
+  impartiality, and intellectual integrity throughout all interactions." ) #
+       Ignore the specific UserWarning warnings.filterwarnings("ignore",
+      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
+ (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
+ [str]: """ Chat function to perform a web search based on the user input and
+generate a response using the LLM model. Parameters ---------- user_input : str
+    The user input to be used for the web search webs : WEBS The web search
+   instance to be used to perform the search max_results : int, optional The
+  maximum number of search results to include in the response, by default 10
+Returns ------- Optional[str] The response generated by the LLM model, or None
+  if there is no response """ # Perform a web search based on the user input
+search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
+          safesearch="off", timelimit="y", max_results=max_results ):
+ search_results.append(str(r)) # Convert each result to a string # Define the
+   messages to be sent, including the user input, search results, and system
+message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
+results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
+     response response = LLM.chat(messages) return response if __name__ ==
+  "__main__": while True: # Get the user input user_input = input("User: ") #
+ Perform a web search based on the user input with WEBS() as webs: response =
+chat(user_input, webs) # Print the response if response: print("AI:", response)
+else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
+ ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
+    """ Wrap the webscout default method in a try-except block to catch any
+  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
+  ( max_tokens=500, provider="cohere", temperature=0.7, top_k=40, top_p=0.95,
+model="command-r-plus", # Replace with your desired model auth=None, # Replace
+  with your auth key/value (if needed) timeout=30, disable_conversation=True,
+filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
       awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
 webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
      if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
 use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
                         --provider "phind" --rawdog ```
```

### Comparing `webscout-1.3.8/setup.py` & `webscout-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.3.8", 
+    version="1.3.9", 
     description="Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -47,15 +47,16 @@
         "requests",
         "sse_starlette",
         "termcolor",
         "tiktoken",
         "tldextract",
         "orjson",
         "PyYAML",
-        # "appdirs"
+        "appdirs"
+        "GoogleBard1>=2.1.4"
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout-ai-phindsearch = webscout.AI:phindsearch",
             "webscout-ai-yepchat = webscout.AI:yepchat",
             "webscout-ai = webscout.AI:cli",
```

### Comparing `webscout-1.3.8/webscout/AIbase.py` & `webscout-1.3.9/webscout/AIbase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
 from abc import abstractmethod
 
 
 class Provider(ABC):
-    """Base class for models class"""
+    """Base class for providers"""
 
     @abstractmethod
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
@@ -63,8 +63,76 @@
 
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
+        raise NotImplementedError("Method needs to be implemented in subclass")
+
+
+class AsyncProvider(ABC):
+    """Asynchronous base class for providers"""
+
+    @abstractmethod
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Asynchronously chat with AI
+
+        Args:
+            prompt (str): Prompt to be sent
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "completion": "\nNext: domestic cat breeds with short hair >>",
+            "stop_reason": null,
+            "truncated": false,
+            "stop": null,
+            "model": "llama-2-13b-chat",
+            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
+            "exception": null
+        }
+        ```
+        """
+        raise NotImplementedError("Method needs to be implemented in subclass")
+
+    @abstractmethod
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Asynchronously generate response `str`
+        Args:
+            prompt (str): Prompt to be sent
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+        raise NotImplementedError("Method needs to be implemented in subclass")
+
+    @abstractmethod
+    async def get_message(self, response: dict) -> str:
+        """Asynchronously retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
         raise NotImplementedError("Method needs to be implemented in subclass")
```

### Comparing `webscout-1.3.8/webscout/AIutel.py` & `webscout-1.3.9/webscout/AIutel.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,43 @@
     "opengpt",
     "koboldai",
     "gemini",
     "phind",
     "blackboxai",
     "g4fauto",
     "perplexity",
-    "sean",
     "groq",
     "reka",
-    "cohere"
+    "cohere",
+    "yepchat",
 ]
 
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
+def sanitize_stream(
+    chunk: str, intro_value: str = "data:", to_json: bool = True
+) -> str | dict:
+    """Remove streaming flags
 
+    Args:
+        chunk (str): Streamig chunk.
+        intro_value (str, optional): streaming flag. Defaults to "data:".
+        to_json (bool, optional). Return chunk as dictionary. Defaults to True.
+
+    Returns:
+        str: Sanitized streaming value.
+    """
+
+    if chunk.startswith(intro_value):
+        chunk = chunk[len(intro_value) :]
+
+    return json.loads(chunk) if to_json else chunk
 def run_system_command(
     command: str,
     exit_on_error: bool = True,
     stdout_error: bool = True,
     help: str = None,
 ):
     """Run commands against system
```

### Comparing `webscout-1.3.8/webscout/DWEBS.py` & `webscout-1.3.9/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/LLM.py` & `webscout-1.3.9/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/__init__.py` & `webscout-1.3.9/webscout/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     "opengpt",
     "koboldai",
     "gemini",
     "phind",
     "blackboxai",
     "g4fauto",
     "perplexity",
-    "sean",
     "groq",
     "reka",
-    "cohere"
+    "cohere",
+    "yepchat",
 ]
 
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
```

### Comparing `webscout-1.3.8/webscout/cli.py` & `webscout-1.3.9/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/g4f.py` & `webscout-1.3.9/webscout/g4f.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import g4f
 from webscout.AIutel import Optimizers
 from webscout.AIutel import Conversation
 from webscout.AIutel import AwesomePrompts
-from webscout.AIbase import Provider
+from webscout.AIbase import Provider, AsyncProvider
 from webscout.AIutel import available_providers
 
 
 g4f.debug.version_check = False
 
 working_providers = available_providers
 
@@ -22,15 +22,207 @@
 default_models = {
     "completion": "text-davinci-003",
     "chat_completion": "gpt-3.5-turbo",
 }
 
 default_provider = "Koala"
 
+class AsyncGPT4FREE(AsyncProvider):
+    def __init__(
+        self,
+        provider: str = default_provider,
+        is_conversation: bool = True,
+        auth: str = None,
+        max_tokens: int = 600,
+        model: str = None,
+        ignore_working: bool = False,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Initialies GPT4FREE
+
+        Args:
+            provider (str, optional): gpt4free based provider name. Defaults to Koala.
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            auth (str, optional): Authentication value for the provider incase it needs. Defaults to None.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            model (str, optional): LLM model name. Defaults to text-davinci-003|gpt-3.5-turbo.
+            ignore_working (bool, optional): Ignore working status of the provider. Defaults to False.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        assert provider in available_providers, (
+            f"Provider '{provider}' is not yet supported. "
+            f"Try others like {', '.join(available_providers)}"
+        )
+        if model is None:
+            model = default_models["chat_completion"]
+
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation,
+            self.max_tokens_to_sample,
+            filepath,
+            update_file,
+        )
+        self.conversation.history_offset = history_offset
+        self.model = model
+        self.provider = provider
+        self.ignore_working = ignore_working
+        self.auth = auth
+        self.proxy = None if not proxies else list(proxies.values())[0]
 
+    def __str__(self):
+        return f"AsyncGPTFREE(provider={self.provider})"
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content
+        ```json
+        {
+          "text" : "How may I help you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = dict(
+            model=self.model,
+            provider=self.provider,  # g4f.Provider.Aichat,
+            messages=[{"role": "user", "content": conversation_prompt}],
+            stream=True,
+            ignore_working=self.ignore_working,
+            auth=self.auth,
+            proxy=self.proxy,
+            timeout=self.timeout,
+        )
+
+        async def format_response(response):
+            return dict(text=response)
+
+        async def for_stream():
+            previous_chunks = ""
+            response = g4f.ChatCompletion.create_async(**payload)
+
+            async for chunk in response:
+                previous_chunks += chunk
+                formatted_resp = await format_response(previous_chunks)
+                self.last_response.update(formatted_resp)
+                yield previous_chunks if raw else formatted_resp
+
+            self.conversation.update_chat_history(
+                prompt,
+                previous_chunks,
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
 class GPT4FREE(Provider):
     def __init__(
         self,
         provider: str = default_provider,
         is_conversation: bool = True,
         auth: str = None,
         max_tokens: int = 600,
```

### Comparing `webscout-1.3.8/webscout/models.py` & `webscout-1.3.9/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/transcriber.py` & `webscout-1.3.9/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/utils.py` & `webscout-1.3.9/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/voice.py` & `webscout-1.3.9/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/webai.py` & `webscout-1.3.9/webscout/webai.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from webscout.AIutel import RawDog
 from webscout.AIutel import Audio
 from webscout import available_providers
 from colorama import Fore
 from colorama import init as init_colorama
 from dotenv import load_dotenv
 import g4f
-
 import webscout.AIutel
 
 init_colorama(autoreset=True)
 
 load_dotenv()  # loads .env variables
 
 logging.basicConfig(
@@ -468,14 +467,33 @@
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
+            elif provider == "yepchat":
+                from webscout.AI import YEPCHAT
+
+                self.bot = YEPCHAT(
+                    is_conversation=disable_conversation,
+                    max_tokens=max_tokens,
+                    temperature=temperature,
+                    presence_penalty=top_p,
+                    frequency_penalty=top_k,
+                    top_p=top_p,
+                    model=getOr(model, "Mixtral-8x7B-Instruct-v0.1"),
+                    timeout=timeout,
+                    intro=intro,
+                    filepath=filepath,
+                    update_file=update_file,
+                    proxies=proxies,
+                    history_offset=history_offset,
+                    act=awesome_prompt,
+                )
             elif provider == "groq":
                 assert auth, (
                     "GROQ's API-key is required. " "Use the flag `--key` or `-k`"
                 )
                 from webscout.AI import GROQ
 
 
@@ -1131,15 +1149,15 @@
 
 class EntryGroup:
     """Entry commands"""
 
     # @staticmethod
     @click.group()
     @click.version_option(
-        webscout.__version__, "-v", "--version", package_name="Webscout"
+        webscout.__version__, "-v", "--version", package_name="webscout"
     )
     @click.help_option("-h", "--help")
     def webai_():
         pass
 
     @staticmethod
     @webai_.group()
```

### Comparing `webscout-1.3.8/webscout/webscout_search.py` & `webscout-1.3.9/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout/webscout_search_async.py` & `webscout-1.3.9/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.8/webscout.egg-info/PKG-INFO` & `webscout-1.3.9/webscout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.8
+Version: 1.3.9
 Summary: Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -43,14 +43,15 @@
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
+Requires-Dist: appdirsGoogleBard1>=2.1.4
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 #  webscout
 <p align="center">
 
@@ -93,18 +94,16 @@
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
-    - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
-    - [11. `Reka` - chat with reka](#11-reka---chat-with-reka)
-    - [12. `Cohere` - chat with cohere](#12-cohere---chat-with-cohere)
-  - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
+    - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
+    - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -685,47 +684,36 @@
 response = koboldai.ask(prompt)
 
 # Extract and print the message from the response
 message = koboldai.get_message(response)
 print(message)
 
 ```
-### 10. `Sean` - chat With Sean
-```python
-from webscout.AI import Sean
-
-a = Sean(is_conversation=True, max_tokens=8000, timeout=30)
-# This example sends a simple greeting and prints the response
-prompt = "tell me about india"
-response_str = a.chat(prompt)
-print(response_str)
-```
 
-### 11. `Reka` - chat with reka
+### 10. `Reka` - chat with reka
 ```python
 from webscout.AI import REKA
 
 a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
-### 12. `Cohere` - chat with cohere
+### 11. `Cohere` - chat with cohere
 ```python
 from webscout.AI import Cohere
 
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
-## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
@@ -840,15 +828,15 @@
         webai_bot = Main(
             max_tokens=500, 
             provider="cohere",
             temperature=0.7,  
             top_k=40,          
             top_p=0.95,        
             model="command-r-plus",  # Replace with your desired model
-            auth="0zoQbKs1AAgd8WrPBO9CTIGgVvm5ZMbDcCqJOVyl",     # Replace with your auth key/value (if needed)
+            auth=None,     # Replace with your auth key/value (if needed)
             timeout=30,
             disable_conversation=True,
             filepath=None,
             update_file=True,
             intro=None,
             rawdog=True,
             history_offset=10250,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.8 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.3.9 Summary: Search for
 anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc
 Also containes AI models, can transcribe yt videos, have TTS support and now
 has webai(terminal gpt and open interpeter) support Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -21,17 +21,17 @@
 curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
 asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Requires-Dist: PyYAML Provides-Extra: dev Requires-Dist:
-ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" #
-webscout
+Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist:
+appdirsGoogleBard1>=2.1.4 Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
+== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
        _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos, have TTS support and now has webai(terminal gpt and open
  interpeter) support ## Table of Contents - [webscout](#webscout) - [Table of
    Contents](#table-of-contents) - [Install](#install) - [CLI version](#cli-
      version) - [CLI to use LLM](#cli-to-use-llm) - [Regions](#regions) -
   [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
@@ -59,54 +59,52 @@
 `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
 - search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
 image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
 [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
   [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
 blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
  with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
-  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` - chat With Sean]
- (#10-sean---chat-with-sean) - [11. `Reka` - chat with reka](#11-reka---chat-
-with-reka) - [12. `Cohere` - chat with cohere](#12-cohere---chat-with-cohere) -
- [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-
-  llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) - [`LLM` with internet]
-(#llm-with-internet) - [`Webai` - terminal gpt and a open interpeter](#webai---
-    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
- ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
-  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
-Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
-for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
- Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
-cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
-fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
-for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
- for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
-lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
- my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
-    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
- Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
-for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
- ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
-for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
- for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka]
+ (#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---
+chat-with-cohere) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) -
+  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
+   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
+version ```python3 python -m webscout --help ``` | Command | Description | |---
+----------------------------------------|--------------------------------------
+ -----------------------------------------------------------------| | python -
+ m webscout answers -k Text | CLI function to perform an answers search using
+ Webscout. | | python -m webscout images -k Text | CLI function to perform an
+    images search using Webscout. | | python -m webscout maps -k Text | CLI
+function to perform a maps search using Webscout. | | python -m webscout news -
+  k Text | CLI function to perform a news search using Webscout. | | python -
+ m webscout suggestions -k Text | CLI function to perform a suggestions search
+using Webscout. | | python -m webscout text -k Text | CLI function to perform a
+  text search using Webscout. | | python -m webscout translate -k Text | CLI
+function to perform translate using Webscout. | | python -m webscout version |
+  A command-line interface command that prints and returns the version of the
+  program. | | python -m webscout videos -k Text | CLI function to perform a
+  videos search using DuckDuckGo API. | ## CLI to use LLM ```python python -
+  m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for
+Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for
+ Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg
+for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
+  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
+Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
+de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
+for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
+for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
+lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
+  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
+ Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
+  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
+ Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
+     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
+    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
+Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
+   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
      Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Transcriber The
    transcriber function in webscout is a handy tool that transcribes YouTube
  videos. Here's an example code demonstrating its usage: ```python import sys
 from webscout import transcriber def extract_transcript(video_id): """Extracts
         the transcript from a YouTube video.""" try: transcript_list =
    transcriber.list_transcripts(video_id) for transcript in transcript_list:
      transcript_data_list = transcript.fetch() lang = transcript.language
@@ -305,73 +303,68 @@
     simple greeting and prints the response prompt = "tell me about india"
 response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
   ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
 with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
  AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
  response from the AI response = koboldai.ask(prompt) # Extract and print the
    message from the response message = koboldai.get_message(response) print
-(message) ``` ### 10. `Sean` - chat With Sean ```python from webscout.AI import
-Sean a = Sean(is_conversation=True, max_tokens=8000, timeout=30) # This example
-sends a simple greeting and prints the response prompt = "tell me about india"
-  response_str = a.chat(prompt) print(response_str) ``` ### 11. `Reka` - chat
-with reka ```python from webscout.AI import REKA a = REKA(is_conversation=True,
-    max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
- response_str = a.chat(prompt) print(response_str) ``` ### 12. `Cohere` - chat
-        with cohere ```python from webscout.AI import Cohere a = Cohere
- (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
-me about india" response_str = a.chat(prompt) print(response_str) ``` ## usage
-  of special .LLM file from webscout (webscout.LLM) ### `LLM` ```python from
-   webscout.LLM import LLM # Read the system message from the file with open
-('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
-   class with the model name and system message llm = LLM(model="microsoft/
- WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
-input user_input = input("User: ") # Define the messages to be sent messages =
- [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
-get the response response = llm.chat(messages) # Print the response print("AI:
-   ", response) ``` ### `LLM` with internet ```python from __future__ import
-  annotations from typing import List, Optional from webscout import LLM from
-   webscout import WEBS import warnings system_message: str = ( "As AI, you
-  possess internet access and are capable of executing real-time web searches
-     based on user inputs. " "You shall utilize this capability to enrich
-conversations, offer informed insights, and augment your ability to " "respond
- accurately and thoroughly. However, refrain from stating 'You have provided a
-   list of strings,' ensuring " "seamless interactions with users. Embrace a
-    responsive demeanor, harnessing available online resources to address "
-  "queries, share pertinent content, and facilitate meaningful exchanges. By
-  doing so, you create value through " "connection and engagement, ultimately
- enhancing overall user satisfaction and experience. Additionally, " "continue
- upholding the principles of respect, impartiality, and intellectual integrity
-       throughout all interactions." ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
- Parameters ---------- user_input : str The user input to be used for the web
-  search webs : WEBS The web search instance to be used to perform the search
-max_results : int, optional The maximum number of search results to include in
-    the response, by default 10 Returns ------- Optional[str] The response
-generated by the LLM model, or None if there is no response """ # Perform a web
-    search based on the user input search_results: List[str] = [] for r in
-    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
-max_results=max_results ): search_results.append(str(r)) # Convert each result
-to a string # Define the messages to be sent, including the user input, search
-results, and system message messages = [ {"role": "user", "content": user_input
-  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
- chat method to get the response response = LLM.chat(messages) return response
-if __name__ == "__main__": while True: # Get the user input user_input = input
-("User: ") # Perform a web search based on the user input with WEBS() as webs:
-response = chat(user_input, webs) # Print the response if response: print("AI:
-  ", response) else: print("No response") ``` ## `Webai` - terminal gpt and a
-         open interpeter ```python from webscout.webai import Main def
- use_rawdog_with_webai(prompt): """ Wrap the webscout default method in a try-
-except block to catch any unhandled exceptions and print a helpful message. """
-  try: webai_bot = Main( max_tokens=500, provider="cohere", temperature=0.7,
-top_k=40, top_p=0.95, model="command-r-plus", # Replace with your desired model
-auth="0zoQbKs1AAgd8WrPBO9CTIGgVvm5ZMbDcCqJOVyl", # Replace with your auth key/
-    value (if needed) timeout=30, disable_conversation=True, filepath=None,
-       update_file=True, intro=None, rawdog=True, history_offset=10250,
+(message) ``` ### 10. `Reka` - chat with reka ```python from webscout.AI import
+  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
+      prompt = "tell me about india" response_str = a.chat(prompt) print
+     (response_str) ``` ### 11. `Cohere` - chat with cohere ```python from
+  webscout.AI import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
+  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
+ (prompt) print(response_str) ``` ### `LLM` ```python from webscout.LLM import
+  LLM # Read the system message from the file with open('system.txt', 'r') as
+ file: system_message = file.read() # Initialize the LLM class with the model
+     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
+ system_message=system_message) while True: # Get the user input user_input =
+input("User: ") # Define the messages to be sent messages = [ {"role": "user",
+  "content": user_input} ] # Use the mistral_chat method to get the response
+response = llm.chat(messages) # Print the response print("AI: ", response) ```
+   ### `LLM` with internet ```python from __future__ import annotations from
+typing import List, Optional from webscout import LLM from webscout import WEBS
+import warnings system_message: str = ( "As AI, you possess internet access and
+ are capable of executing real-time web searches based on user inputs. " "You
+shall utilize this capability to enrich conversations, offer informed insights,
+  and augment your ability to " "respond accurately and thoroughly. However,
+    refrain from stating 'You have provided a list of strings,' ensuring "
+ "seamless interactions with users. Embrace a responsive demeanor, harnessing
+available online resources to address " "queries, share pertinent content, and
+   facilitate meaningful exchanges. By doing so, you create value through "
+"connection and engagement, ultimately enhancing overall user satisfaction and
+  experience. Additionally, " "continue upholding the principles of respect,
+  impartiality, and intellectual integrity throughout all interactions." ) #
+       Ignore the specific UserWarning warnings.filterwarnings("ignore",
+      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
+ (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
+  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
+ [str]: """ Chat function to perform a web search based on the user input and
+generate a response using the LLM model. Parameters ---------- user_input : str
+    The user input to be used for the web search webs : WEBS The web search
+   instance to be used to perform the search max_results : int, optional The
+  maximum number of search results to include in the response, by default 10
+Returns ------- Optional[str] The response generated by the LLM model, or None
+  if there is no response """ # Perform a web search based on the user input
+search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
+          safesearch="off", timelimit="y", max_results=max_results ):
+ search_results.append(str(r)) # Convert each result to a string # Define the
+   messages to be sent, including the user input, search results, and system
+message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
+results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
+     response response = LLM.chat(messages) return response if __name__ ==
+  "__main__": while True: # Get the user input user_input = input("User: ") #
+ Perform a web search based on the user input with WEBS() as webs: response =
+chat(user_input, webs) # Print the response if response: print("AI:", response)
+else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
+ ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
+    """ Wrap the webscout default method in a try-except block to catch any
+  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
+  ( max_tokens=500, provider="cohere", temperature=0.7, top_k=40, top_p=0.95,
+model="command-r-plus", # Replace with your desired model auth=None, # Replace
+  with your auth key/value (if needed) timeout=30, disable_conversation=True,
+filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
       awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
 webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
      if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
 use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
                         --provider "phind" --rawdog ```
```

### Comparing `webscout-1.3.8/webscout.egg-info/SOURCES.txt` & `webscout-1.3.9/webscout.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 webscout/AI.py
 webscout/AIbase.py
 webscout/AIutel.py
 webscout/DWEBS.py
 webscout/LLM.py
 webscout/__init__.py
 webscout/__main__.py
+webscout/async_providers.py
 webscout/cli.py
 webscout/exceptions.py
 webscout/g4f.py
 webscout/models.py
 webscout/transcriber.py
 webscout/utils.py
 webscout/version.py
```

