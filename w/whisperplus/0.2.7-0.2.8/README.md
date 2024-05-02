# Comparing `tmp/whisperplus-0.2.7.tar.gz` & `tmp/whisperplus-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisperplus-0.2.7.tar", last modified: Sun Jan 21 22:22:12 2024, max compression
+gzip compressed data, was "whisperplus-0.2.8.tar", last modified: Thu May  2 22:18:32 2024, max compression
```

## Comparing `whisperplus-0.2.7.tar` & `whisperplus-0.2.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-01-21 22:22:12.817093 whisperplus-0.2.7/
--rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2023-11-21 10:00:15.000000 whisperplus-0.2.7/LICENSE
--rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-01-17 18:03:19.000000 whisperplus-0.2.7/MANIFEST.in
--rw-r--r--   0 kadirnar   (501) staff       (20)     5240 2024-01-21 22:22:12.817181 whisperplus-0.2.7/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)     4930 2024-01-21 22:20:54.000000 whisperplus-0.2.7/README.md
--rw-r--r--   0 kadirnar   (501) staff       (20)      362 2024-01-21 17:29:33.000000 whisperplus-0.2.7/requirements.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-01-21 22:22:12.817480 whisperplus-0.2.7/setup.cfg
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-01-21 22:20:54.000000 whisperplus-0.2.7/setup.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-01-21 22:22:12.814949 whisperplus-0.2.7/whisperplus/
--rw-r--r--   0 kadirnar   (501) staff       (20)      587 2024-01-21 22:22:02.000000 whisperplus-0.2.7/whisperplus/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-01-17 18:03:19.000000 whisperplus-0.2.7/whisperplus/app.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-01-21 22:22:12.816591 whisperplus-0.2.7/whisperplus/pipelines/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-01-17 18:03:19.000000 whisperplus-0.2.7/whisperplus/pipelines/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-01-21 22:20:54.000000 whisperplus-0.2.7/whisperplus/pipelines/autollm_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-01-21 22:00:00.000000 whisperplus-0.2.7/whisperplus/pipelines/lancedb_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-01-21 14:45:32.000000 whisperplus-0.2.7/whisperplus/pipelines/long_text_summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2023-11-23 20:15:03.000000 whisperplus-0.2.7/whisperplus/pipelines/summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-01-21 15:11:30.000000 whisperplus-0.2.7/whisperplus/pipelines/text2speech.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2675 2023-11-23 20:15:03.000000 whisperplus-0.2.7/whisperplus/pipelines/whisper.py
--rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2023-11-24 14:54:02.000000 whisperplus-0.2.7/whisperplus/pipelines/whisper_diarize.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-01-21 22:22:12.816988 whisperplus-0.2.7/whisperplus/utils/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2023-11-23 15:57:34.000000 whisperplus-0.2.7/whisperplus/utils/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2023-11-23 20:15:03.000000 whisperplus-0.2.7/whisperplus/utils/download_utils.py
--rw-r--r--   0 kadirnar   (501) staff       (20)      532 2023-11-24 11:00:25.000000 whisperplus-0.2.7/whisperplus/utils/text_utils.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-01-21 22:22:12.815564 whisperplus-0.2.7/whisperplus.egg-info/
--rw-r--r--   0 kadirnar   (501) staff       (20)     5240 2024-01-21 22:22:12.000000 whisperplus-0.2.7/whisperplus.egg-info/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)      695 2024-01-21 22:22:12.000000 whisperplus-0.2.7/whisperplus.egg-info/SOURCES.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-01-21 22:22:12.000000 whisperplus-0.2.7/whisperplus.egg-info/dependency_links.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      362 2024-01-21 22:22:12.000000 whisperplus-0.2.7/whisperplus.egg-info/requires.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-01-21 22:22:12.000000 whisperplus-0.2.7/whisperplus.egg-info/top_level.txt
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.113359 whisperplus-0.2.8/
+-rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.2.8/LICENSE
+-rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.2.8/MANIFEST.in
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5514 2024-05-02 22:18:32.113509 whisperplus-0.2.8/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5204 2024-05-02 22:01:09.000000 whisperplus-0.2.8/README.md
+-rw-r--r--   0 kadirnar   (501) staff       (20)      395 2024-05-02 22:01:13.000000 whisperplus-0.2.8/requirements.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-02 22:18:32.113832 whisperplus-0.2.8/setup.cfg
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.2.8/setup.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.110502 whisperplus-0.2.8/whisperplus/
+-rw-r--r--   0 kadirnar   (501) staff       (20)      658 2024-05-02 22:18:20.000000 whisperplus-0.2.8/whisperplus/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/app.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.112878 whisperplus-0.2.8/whisperplus/pipelines/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/autollm_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/lancedb_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/long_text_summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.2.8/whisperplus/pipelines/text2speech.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2773 2024-05-02 22:00:09.000000 whisperplus-0.2.8/whisperplus/pipelines/whisper.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/whisper_autocaption.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/pipelines/whisper_diarize.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.113251 whisperplus-0.2.8/whisperplus/utils/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/utils/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/utils/download_utils.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.2.8/whisperplus/utils/text_utils.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-02 22:18:32.111207 whisperplus-0.2.8/whisperplus.egg-info/
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5514 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)      740 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/SOURCES.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/dependency_links.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      395 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/requires.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-02 22:18:32.000000 whisperplus-0.2.8/whisperplus.egg-info/top_level.txt
```

### Comparing `whisperplus-0.2.7/LICENSE` & `whisperplus-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/PKG-INFO` & `whisperplus-0.2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.2.7
+Version: 0.2.8
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h2>
-    WhisperPlus: Advancing Speech2Text and Text2Speech Processing 🚀
+    WhisperPlus: Advancing Speech2Text and Text2Speech Feature 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
 <div>
     <a href="https://pypi.org/project/whisperplus" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/whisperplus.svg?color=%2334D058" alt="Supported Python versions">
@@ -25,14 +25,15 @@
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
 pip install whisperplus
+pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
 ## 🎙️ Usage
@@ -115,15 +116,15 @@
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🌠 RAG - Chat with Video(AutoLLM)
 
 ```python
-from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
+from whisperplus import AutoLLMChatWithVideo
 
 # service_context_params
 system_prompt = """
 You are an friendly ai assistant that help users find the most relevant and accurate answers
 to their questions based on the documents you have access to.
 When answering the questions, mostly rely on the info in documents.
 """
@@ -135,15 +136,15 @@
 Using the document information and mostly relying on it,
 answer the query.
 Query: {query_str}
 Answer:
 """
 
 chat = AutoLLMChatWithVideo(
-    input_file="audio.mp3",
+    input_file="input_dir",  # path of mp3 file
     openai_key="YOUR_OPENAI_KEY",  # optional
     huggingface_key="YOUR_HUGGINGFACE_KEY",  # optional
     llm_model="gpt-3.5-turbo",
     llm_max_tokens="256",
     llm_temperature="0.1",
     system_prompt=system_prompt,
     query_wrapper_prompt=query_wrapper_prompt,
@@ -160,14 +161,23 @@
 ```python
 from whisperplus import TextToSpeechPipeline
 
 tts = TextToSpeechPipeline(model_id="suno/bark")
 audio = tts(text="Hello World", voice_preset="v2/en_speaker_6")
 ```
 
+### 🎥 AutoCaption
+
+```python
+from whisperplus import WhisperAutoCaptionPipeline
+
+caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
+caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+```
+
 ## 😍 Contributing
 
 ```bash
 pip install -r dev-requirements.txt
 pre-commit install
 pre-commit run --all-files
 ```
```

#### html2text {}

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.2.7 Summary: WhisperPlus: A
+Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8 Summary: WhisperPlus: A
 Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
 whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
 Apache License 2.0 Description-Content-Type: text/markdown License-File:
 LICENSE
-********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh PPrroocceessssiinngg ?ð??? **********
+  ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus ``` ## ð¤ Model Hub
-You can find the models on the [HuggingFace Model Hub](https://huggingface.co/
-models?search=whisper) ## ðï¸ Usage To use the whisperplus library, follow
-the steps below for different tasks: ### ðµ Youtube URL to Audio ```python
-from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3 url =
-"https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
-download_and_convert_to_mp3(url) pipeline = SpeechToTextPipeline
-(model_id="openai/whisper-large-v3") transcript = pipeline(audio_path, "openai/
-whisper-large-v3", "english") print(transcript) ``` ### ð° Summarization
-```python from whisperplus import TextSummarizationPipeline summarizer =
-TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
-summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
-Long Text Support Summarization ```python from whisperplus import
-LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
-(model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
-(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
-from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
-format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
-www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
-ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
-diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
-chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
-num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
-format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
-with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
-ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
-llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
-v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
-transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
-= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
-(AutoLLM) ```python from whisperplus.pipelines.autollm_chatbot import
+## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
+--no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
+[HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
+ðï¸ Usage To use the whisperplus library, follow the steps below for
+different tasks: ### ðµ Youtube URL to Audio ```python from whisperplus
+import SpeechToTextPipeline, download_and_convert_to_mp3 url = "https://
+www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_and_convert_to_mp3
+(url) pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
+transcript = pipeline(audio_path, "openai/whisper-large-v3", "english") print
+(transcript) ``` ### ð° Summarization ```python from whisperplus import
+TextSummarizationPipeline summarizer = TextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
+print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
+```python from whisperplus import LongTextSummarizationPipeline summarizer =
+LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary_text
+= summarizer.summarize(transcript) print(summary_text) ``` ### ð¬ Speaker
+Diarization ```python from whisperplus import ( ASRDiarizationPipeline,
+download_and_convert_to_mp3, format_speech_to_dialogue, ) audio_path =
+download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
+device = "cuda" # cpu or mps pipeline = ASRDiarizationPipeline.from_pretrained
+( asr_model="openai/whisper-large-v3", diarizer_model="pyannote/speaker-
+diarization", use_auth_token=False, chunk_length_s=30, device=device, )
+output_text = pipeline(audio_path, num_speakers=2, min_speaker=1,
+max_speaker=2) dialogue = format_speech_to_dialogue(output_text) print
+(dialogue) ``` ### â­ RAG - Chat with Video(LanceDB) ```python from
+whisperplus.pipelines.chatbot import ChatWithVideo chat = ChatWithVideo
+( input_file="trascript.txt", llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
+llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf", llm_model_type="mistral",
+embedding_model_name="sentence-transformers/all-MiniLM-L6-v2", ) query = "what
+is this video about ?" response = chat.run_query(query) print(response) ``` ###
+ð  RAG - Chat with Video(AutoLLM) ```python from whisperplus import
 AutoLLMChatWithVideo # service_context_params system_prompt = """ You are an
 friendly ai assistant that help users find the most relevant and accurate
 answers to their questions based on the documents you have access to. When
 answering the questions, mostly rely on the info in documents. """
 query_wrapper_prompt = """ The document information is below. -----------------
 ---- {context_str} --------------------- Using the document information and
 mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
-AutoLLMChatWithVideo( input_file="audio.mp3", openai_key="YOUR_OPENAI_KEY", #
-optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
-turbo", llm_max_tokens="256", llm_temperature="0.1",
-system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
-embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
-= "what is this video about ?" response = chat.run_query(query) print(response)
-``` ### ðï¸ Speech to Text ```python from whisperplus import
-TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
-tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ## ð
-Contributing ```bash pip install -r dev-requirements.txt pre-commit install
-pre-commit run --all-files ``` ## ð License This project is licensed under
-the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
+AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
+openai_key="YOUR_OPENAI_KEY", # optional
+huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
+llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
+query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
+large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
+response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
+```python from whisperplus import TextToSpeechPipeline tts =
+TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello World",
+voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```python from
+whisperplus import WhisperAutoCaptionPipeline caption =
+WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3") caption
+(video_path="test.mp4", output_path="output.mp4", language="turkish") ``` ##
+ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
+install pre-commit run --all-files ``` ## ð License This project is licensed
+under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
 license} } ```
```

### Comparing `whisperplus-0.2.7/README.md` & `whisperplus-0.2.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
 <h2>
-    WhisperPlus: Advancing Speech2Text and Text2Speech Processing 🚀
+    WhisperPlus: Advancing Speech2Text and Text2Speech Feature 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
 <div>
     <a href="https://pypi.org/project/whisperplus" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/whisperplus.svg?color=%2334D058" alt="Supported Python versions">
@@ -14,14 +14,15 @@
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
 pip install whisperplus
+pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
 ## 🎙️ Usage
@@ -104,15 +105,15 @@
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🌠 RAG - Chat with Video(AutoLLM)
 
 ```python
-from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
+from whisperplus import AutoLLMChatWithVideo
 
 # service_context_params
 system_prompt = """
 You are an friendly ai assistant that help users find the most relevant and accurate answers
 to their questions based on the documents you have access to.
 When answering the questions, mostly rely on the info in documents.
 """
@@ -124,15 +125,15 @@
 Using the document information and mostly relying on it,
 answer the query.
 Query: {query_str}
 Answer:
 """
 
 chat = AutoLLMChatWithVideo(
-    input_file="audio.mp3",
+    input_file="input_dir",  # path of mp3 file
     openai_key="YOUR_OPENAI_KEY",  # optional
     huggingface_key="YOUR_HUGGINGFACE_KEY",  # optional
     llm_model="gpt-3.5-turbo",
     llm_max_tokens="256",
     llm_temperature="0.1",
     system_prompt=system_prompt,
     query_wrapper_prompt=query_wrapper_prompt,
@@ -149,14 +150,23 @@
 ```python
 from whisperplus import TextToSpeechPipeline
 
 tts = TextToSpeechPipeline(model_id="suno/bark")
 audio = tts(text="Hello World", voice_preset="v2/en_speaker_6")
 ```
 
+### 🎥 AutoCaption
+
+```python
+from whisperplus import WhisperAutoCaptionPipeline
+
+caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
+caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+```
+
 ## 😍 Contributing
 
 ```bash
 pip install -r dev-requirements.txt
 pre-commit install
 pre-commit run --all-files
 ```
```

#### html2text {}

```diff
@@ -1,59 +1,63 @@
-********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh PPrroocceessssiinngg ?ð??? **********
+  ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus ``` ## ð¤ Model Hub
-You can find the models on the [HuggingFace Model Hub](https://huggingface.co/
-models?search=whisper) ## ðï¸ Usage To use the whisperplus library, follow
-the steps below for different tasks: ### ðµ Youtube URL to Audio ```python
-from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3 url =
-"https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
-download_and_convert_to_mp3(url) pipeline = SpeechToTextPipeline
-(model_id="openai/whisper-large-v3") transcript = pipeline(audio_path, "openai/
-whisper-large-v3", "english") print(transcript) ``` ### ð° Summarization
-```python from whisperplus import TextSummarizationPipeline summarizer =
-TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
-summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
-Long Text Support Summarization ```python from whisperplus import
-LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
-(model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
-(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
-from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
-format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
-www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
-ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
-diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
-chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
-num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
-format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
-with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
-ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
-llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
-v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
-transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
-= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
-(AutoLLM) ```python from whisperplus.pipelines.autollm_chatbot import
+## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
+--no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
+[HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
+ðï¸ Usage To use the whisperplus library, follow the steps below for
+different tasks: ### ðµ Youtube URL to Audio ```python from whisperplus
+import SpeechToTextPipeline, download_and_convert_to_mp3 url = "https://
+www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_and_convert_to_mp3
+(url) pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
+transcript = pipeline(audio_path, "openai/whisper-large-v3", "english") print
+(transcript) ``` ### ð° Summarization ```python from whisperplus import
+TextSummarizationPipeline summarizer = TextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
+print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
+```python from whisperplus import LongTextSummarizationPipeline summarizer =
+LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary_text
+= summarizer.summarize(transcript) print(summary_text) ``` ### ð¬ Speaker
+Diarization ```python from whisperplus import ( ASRDiarizationPipeline,
+download_and_convert_to_mp3, format_speech_to_dialogue, ) audio_path =
+download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
+device = "cuda" # cpu or mps pipeline = ASRDiarizationPipeline.from_pretrained
+( asr_model="openai/whisper-large-v3", diarizer_model="pyannote/speaker-
+diarization", use_auth_token=False, chunk_length_s=30, device=device, )
+output_text = pipeline(audio_path, num_speakers=2, min_speaker=1,
+max_speaker=2) dialogue = format_speech_to_dialogue(output_text) print
+(dialogue) ``` ### â­ RAG - Chat with Video(LanceDB) ```python from
+whisperplus.pipelines.chatbot import ChatWithVideo chat = ChatWithVideo
+( input_file="trascript.txt", llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
+llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf", llm_model_type="mistral",
+embedding_model_name="sentence-transformers/all-MiniLM-L6-v2", ) query = "what
+is this video about ?" response = chat.run_query(query) print(response) ``` ###
+ð  RAG - Chat with Video(AutoLLM) ```python from whisperplus import
 AutoLLMChatWithVideo # service_context_params system_prompt = """ You are an
 friendly ai assistant that help users find the most relevant and accurate
 answers to their questions based on the documents you have access to. When
 answering the questions, mostly rely on the info in documents. """
 query_wrapper_prompt = """ The document information is below. -----------------
 ---- {context_str} --------------------- Using the document information and
 mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
-AutoLLMChatWithVideo( input_file="audio.mp3", openai_key="YOUR_OPENAI_KEY", #
-optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
-turbo", llm_max_tokens="256", llm_temperature="0.1",
-system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
-embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
-= "what is this video about ?" response = chat.run_query(query) print(response)
-``` ### ðï¸ Speech to Text ```python from whisperplus import
-TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
-tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ## ð
-Contributing ```bash pip install -r dev-requirements.txt pre-commit install
-pre-commit run --all-files ``` ## ð License This project is licensed under
-the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
+AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
+openai_key="YOUR_OPENAI_KEY", # optional
+huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
+llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
+query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
+large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
+response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
+```python from whisperplus import TextToSpeechPipeline tts =
+TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello World",
+voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```python from
+whisperplus import WhisperAutoCaptionPipeline caption =
+WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3") caption
+(video_path="test.mp4", output_path="output.mp4", language="turkish") ``` ##
+ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
+install pre-commit run --all-files ``` ## ð License This project is licensed
+under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
 license} } ```
```

### Comparing `whisperplus-0.2.7/setup.cfg` & `whisperplus-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/setup.py` & `whisperplus-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/__init__.py` & `whisperplus-0.2.8/whisperplus/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
 from whisperplus.pipelines.long_text_summarization import LongTextSummarizationPipeline
 from whisperplus.pipelines.summarization import TextSummarizationPipeline
 from whisperplus.pipelines.text2speech import TextToSpeechPipeline
 from whisperplus.pipelines.whisper import SpeechToTextPipeline
 from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
 from whisperplus.utils.download_utils import download_and_convert_to_mp3
 from whisperplus.utils.text_utils import format_speech_to_dialogue
 
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 __author__ = 'kadirnar'
 __license__ = 'Apache License 2.0'
```

### Comparing `whisperplus-0.2.7/whisperplus/app.py` & `whisperplus-0.2.8/whisperplus/app.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/pipelines/autollm_chatbot.py` & `whisperplus-0.2.8/whisperplus/pipelines/autollm_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/pipelines/lancedb_chatbot.py` & `whisperplus-0.2.8/whisperplus/pipelines/lancedb_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/pipelines/long_text_summarization.py` & `whisperplus-0.2.8/whisperplus/pipelines/long_text_summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/pipelines/summarization.py` & `whisperplus-0.2.8/whisperplus/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/pipelines/text2speech.py` & `whisperplus-0.2.8/whisperplus/pipelines/text2speech.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/pipelines/whisper.py` & `whisperplus-0.2.8/whisperplus/pipelines/whisper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 import torch
-from transformers import AutoModelForSpeechSeq2Seq, AutoProcessor, pipeline
+from transformers import AutoModelForSpeechSeq2Seq, AutoProcessor, BitsAndBytesConfig, pipeline
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 class SpeechToTextPipeline:
     """Class for converting audio to text using a pre-trained speech recognition model."""
 
@@ -14,62 +14,71 @@
         self.device = None
 
         if self.model is None:
             self.load_model(model_id)
         else:
             logging.info("Model already loaded.")
 
-        self.set_device()
-
-    def set_device(self):
-        """Sets the device to be used for inference based on availability."""
-        if torch.backends.mps.is_available():
-            self.device = "mps"
-        else:
-            self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
-        logging.info(f"Using device: {self.device}")
-
     def load_model(self, model_id: str = "openai/whisper-large-v3"):
         """
         Loads the pre-trained speech recognition model and moves it to the specified device.
 
         Args:
             model_id (str): Identifier of the pre-trained model to be loaded.
         """
         logging.info("Loading model...")
+
+        bnb_config = BitsAndBytesConfig(
+            load_in_4bit=True,
+            bnb_4bit_quant_type="nf4",
+            bnb_4bit_compute_dtype=torch.bfloat16,
+            bnb_4bit_use_double_quant=True,
+        )
         model = AutoModelForSpeechSeq2Seq.from_pretrained(
-            model_id, torch_dtype=torch.float16, low_cpu_mem_usage=True, use_safetensors=True)
-        model.to(self.device)
+            model_id,
+            quantization_config=bnb_config,
+            low_cpu_mem_usage=True,
+            use_safetensors=True,
+            attn_implementation="flash_attention_2",
+            device_map="auto")
+
         logging.info("Model loaded successfully.")
 
+        processor = AutoProcessor.from_pretrained(model_id)
+
+        self.processor = processor
         self.model = model
 
-    def __call__(self, audio_path: str, model_id: str = "openai/whisper-large-v3", language: str = "turkish"):
+    def __call__(
+            self,
+            chunk_length_s: int = 30,
+            stride_length_s: int = 5,
+            audio_path: str = "test.mp3",
+            max_new_tokens: int = 128,
+            batch_size: int = 100,
+            language: str = "turkish"):
         """
         Converts audio to text using the pre-trained speech recognition model.
 
         Args:
             audio_path (str): Path to the audio file to be transcribed.
-            model_id (str): Identifier of the pre-trained model to be used for transcription.
 
         Returns:
             str: Transcribed text from the audio.
         """
-        processor = AutoProcessor.from_pretrained(model_id)
         pipe = pipeline(
             "automatic-speech-recognition",
             model=self.model,
-            torch_dtype=torch.float16,
-            chunk_length_s=30,
-            max_new_tokens=128,
-            batch_size=24,
+            chunk_length_s=chunk_length_s,
+            stride_length_s=stride_length_s,
+            max_new_tokens=max_new_tokens,
+            batch_size=100,
+            device_map="auto",
             return_timestamps=True,
-            device=self.device,
-            tokenizer=processor.tokenizer,
-            feature_extractor=processor.feature_extractor,
+            tokenizer=self.processor.tokenizer,
+            feature_extractor=self.processor.feature_extractor,
             model_kwargs={"use_flash_attention_2": True},
             generate_kwargs={"language": language},
         )
         logging.info("Transcribing audio...")
-        result = pipe(audio_path)["text"]
+        result = pipe(audio_path)
         return result
```

### Comparing `whisperplus-0.2.7/whisperplus/pipelines/whisper_diarize.py` & `whisperplus-0.2.8/whisperplus/pipelines/whisper_diarize.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/utils/download_utils.py` & `whisperplus-0.2.8/whisperplus/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus/utils/text_utils.py` & `whisperplus-0.2.8/whisperplus/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7/whisperplus.egg-info/PKG-INFO` & `whisperplus-0.2.8/whisperplus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.2.7
+Version: 0.2.8
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h2>
-    WhisperPlus: Advancing Speech2Text and Text2Speech Processing 🚀
+    WhisperPlus: Advancing Speech2Text and Text2Speech Feature 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
 <div>
     <a href="https://pypi.org/project/whisperplus" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/whisperplus.svg?color=%2334D058" alt="Supported Python versions">
@@ -25,14 +25,15 @@
 </div>
 </div>
 
 ## 🛠️ Installation
 
 ```bash
 pip install whisperplus
+pip install flash-attn --no-build-isolation
 ```
 
 ## 🤗 Model Hub
 
 You can find the models on the [HuggingFace Model Hub](https://huggingface.co/models?search=whisper)
 
 ## 🎙️ Usage
@@ -115,15 +116,15 @@
 response = chat.run_query(query)
 print(response)
 ```
 
 ### 🌠 RAG - Chat with Video(AutoLLM)
 
 ```python
-from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
+from whisperplus import AutoLLMChatWithVideo
 
 # service_context_params
 system_prompt = """
 You are an friendly ai assistant that help users find the most relevant and accurate answers
 to their questions based on the documents you have access to.
 When answering the questions, mostly rely on the info in documents.
 """
@@ -135,15 +136,15 @@
 Using the document information and mostly relying on it,
 answer the query.
 Query: {query_str}
 Answer:
 """
 
 chat = AutoLLMChatWithVideo(
-    input_file="audio.mp3",
+    input_file="input_dir",  # path of mp3 file
     openai_key="YOUR_OPENAI_KEY",  # optional
     huggingface_key="YOUR_HUGGINGFACE_KEY",  # optional
     llm_model="gpt-3.5-turbo",
     llm_max_tokens="256",
     llm_temperature="0.1",
     system_prompt=system_prompt,
     query_wrapper_prompt=query_wrapper_prompt,
@@ -160,14 +161,23 @@
 ```python
 from whisperplus import TextToSpeechPipeline
 
 tts = TextToSpeechPipeline(model_id="suno/bark")
 audio = tts(text="Hello World", voice_preset="v2/en_speaker_6")
 ```
 
+### 🎥 AutoCaption
+
+```python
+from whisperplus import WhisperAutoCaptionPipeline
+
+caption = WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3")
+caption(video_path="test.mp4", output_path="output.mp4", language="turkish")
+```
+
 ## 😍 Contributing
 
 ```bash
 pip install -r dev-requirements.txt
 pre-commit install
 pre-commit run --all-files
 ```
```

#### html2text {}

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.2.7 Summary: WhisperPlus: A
+Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8 Summary: WhisperPlus: A
 Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
 whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
 Apache License 2.0 Description-Content-Type: text/markdown License-File:
 LICENSE
-********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh PPrroocceessssiinngg ?ð??? **********
+  ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
-## ð ï¸ Installation ```bash pip install whisperplus ``` ## ð¤ Model Hub
-You can find the models on the [HuggingFace Model Hub](https://huggingface.co/
-models?search=whisper) ## ðï¸ Usage To use the whisperplus library, follow
-the steps below for different tasks: ### ðµ Youtube URL to Audio ```python
-from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3 url =
-"https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
-download_and_convert_to_mp3(url) pipeline = SpeechToTextPipeline
-(model_id="openai/whisper-large-v3") transcript = pipeline(audio_path, "openai/
-whisper-large-v3", "english") print(transcript) ``` ### ð° Summarization
-```python from whisperplus import TextSummarizationPipeline summarizer =
-TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
-summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
-Long Text Support Summarization ```python from whisperplus import
-LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
-(model_id="facebook/bart-large-cnn") summary_text = summarizer.summarize
-(transcript) print(summary_text) ``` ### ð¬ Speaker Diarization ```python
-from whisperplus import ( ASRDiarizationPipeline, download_and_convert_to_mp3,
-format_speech_to_dialogue, ) audio_path = download_and_convert_to_mp3("https://
-www.youtube.com/watch?v=mRB14sFHw2E") device = "cuda" # cpu or mps pipeline =
-ASRDiarizationPipeline.from_pretrained( asr_model="openai/whisper-large-v3",
-diarizer_model="pyannote/speaker-diarization", use_auth_token=False,
-chunk_length_s=30, device=device, ) output_text = pipeline(audio_path,
-num_speakers=2, min_speaker=1, max_speaker=2) dialogue =
-format_speech_to_dialogue(output_text) print(dialogue) ``` ### â­ RAG - Chat
-with Video(LanceDB) ```python from whisperplus.pipelines.chatbot import
-ChatWithVideo chat = ChatWithVideo( input_file="trascript.txt",
-llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF", llm_model_file="mistral-7b-
-v0.1.Q4_K_M.gguf", llm_model_type="mistral", embedding_model_name="sentence-
-transformers/all-MiniLM-L6-v2", ) query = "what is this video about ?" response
-= chat.run_query(query) print(response) ``` ### ð  RAG - Chat with Video
-(AutoLLM) ```python from whisperplus.pipelines.autollm_chatbot import
+## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
+--no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
+[HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
+ðï¸ Usage To use the whisperplus library, follow the steps below for
+different tasks: ### ðµ Youtube URL to Audio ```python from whisperplus
+import SpeechToTextPipeline, download_and_convert_to_mp3 url = "https://
+www.youtube.com/watch?v=di3rHkEZuUw" audio_path = download_and_convert_to_mp3
+(url) pipeline = SpeechToTextPipeline(model_id="openai/whisper-large-v3")
+transcript = pipeline(audio_path, "openai/whisper-large-v3", "english") print
+(transcript) ``` ### ð° Summarization ```python from whisperplus import
+TextSummarizationPipeline summarizer = TextSummarizationPipeline
+(model_id="facebook/bart-large-cnn") summary = summarizer.summarize(transcript)
+print(summary[0]["summary_text"]) ``` ### ð° Long Text Support Summarization
+```python from whisperplus import LongTextSummarizationPipeline summarizer =
+LongTextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary_text
+= summarizer.summarize(transcript) print(summary_text) ``` ### ð¬ Speaker
+Diarization ```python from whisperplus import ( ASRDiarizationPipeline,
+download_and_convert_to_mp3, format_speech_to_dialogue, ) audio_path =
+download_and_convert_to_mp3("https://www.youtube.com/watch?v=mRB14sFHw2E")
+device = "cuda" # cpu or mps pipeline = ASRDiarizationPipeline.from_pretrained
+( asr_model="openai/whisper-large-v3", diarizer_model="pyannote/speaker-
+diarization", use_auth_token=False, chunk_length_s=30, device=device, )
+output_text = pipeline(audio_path, num_speakers=2, min_speaker=1,
+max_speaker=2) dialogue = format_speech_to_dialogue(output_text) print
+(dialogue) ``` ### â­ RAG - Chat with Video(LanceDB) ```python from
+whisperplus.pipelines.chatbot import ChatWithVideo chat = ChatWithVideo
+( input_file="trascript.txt", llm_model_name="TheBloke/Mistral-7B-v0.1-GGUF",
+llm_model_file="mistral-7b-v0.1.Q4_K_M.gguf", llm_model_type="mistral",
+embedding_model_name="sentence-transformers/all-MiniLM-L6-v2", ) query = "what
+is this video about ?" response = chat.run_query(query) print(response) ``` ###
+ð  RAG - Chat with Video(AutoLLM) ```python from whisperplus import
 AutoLLMChatWithVideo # service_context_params system_prompt = """ You are an
 friendly ai assistant that help users find the most relevant and accurate
 answers to their questions based on the documents you have access to. When
 answering the questions, mostly rely on the info in documents. """
 query_wrapper_prompt = """ The document information is below. -----------------
 ---- {context_str} --------------------- Using the document information and
 mostly relying on it, answer the query. Query: {query_str} Answer: """ chat =
-AutoLLMChatWithVideo( input_file="audio.mp3", openai_key="YOUR_OPENAI_KEY", #
-optional huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-
-turbo", llm_max_tokens="256", llm_temperature="0.1",
-system_prompt=system_prompt, query_wrapper_prompt=query_wrapper_prompt,
-embed_model="huggingface/BAAI/bge-large-zh", # "text-embedding-ada-002" ) query
-= "what is this video about ?" response = chat.run_query(query) print(response)
-``` ### ðï¸ Speech to Text ```python from whisperplus import
-TextToSpeechPipeline tts = TextToSpeechPipeline(model_id="suno/bark") audio =
-tts(text="Hello World", voice_preset="v2/en_speaker_6") ``` ## ð
-Contributing ```bash pip install -r dev-requirements.txt pre-commit install
-pre-commit run --all-files ``` ## ð License This project is licensed under
-the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
+AutoLLMChatWithVideo( input_file="input_dir", # path of mp3 file
+openai_key="YOUR_OPENAI_KEY", # optional
+huggingface_key="YOUR_HUGGINGFACE_KEY", # optional llm_model="gpt-3.5-turbo",
+llm_max_tokens="256", llm_temperature="0.1", system_prompt=system_prompt,
+query_wrapper_prompt=query_wrapper_prompt, embed_model="huggingface/BAAI/bge-
+large-zh", # "text-embedding-ada-002" ) query = "what is this video about ?"
+response = chat.run_query(query) print(response) ``` ### ðï¸ Speech to Text
+```python from whisperplus import TextToSpeechPipeline tts =
+TextToSpeechPipeline(model_id="suno/bark") audio = tts(text="Hello World",
+voice_preset="v2/en_speaker_6") ``` ### ð¥ AutoCaption ```python from
+whisperplus import WhisperAutoCaptionPipeline caption =
+WhisperAutoCaptionPipeline(model_id="openai/whisper-large-v3") caption
+(video_path="test.mp4", output_path="output.mp4", language="turkish") ``` ##
+ð Contributing ```bash pip install -r dev-requirements.txt pre-commit
+install pre-commit run --all-files ``` ## ð License This project is licensed
+under the terms of the Apache License 2.0. ## ð¤ Citation ```bibtex @misc
 {radford2022whisper, doi = {10.48550/ARXIV.2212.04356}, url = {https://
 arxiv.org/abs/2212.04356}, author = {Radford, Alec and Kim, Jong Wook and Xu,
 Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya}, title =
 {Robust Speech Recognition via Large-Scale Weak Supervision}, publisher =
 {arXiv}, year = {2022}, copyright = {arXiv.org perpetual, non-exclusive
 license} } ```
```

### Comparing `whisperplus-0.2.7/whisperplus.egg-info/SOURCES.txt` & `whisperplus-0.2.8/whisperplus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 whisperplus/pipelines/__init__.py
 whisperplus/pipelines/autollm_chatbot.py
 whisperplus/pipelines/lancedb_chatbot.py
 whisperplus/pipelines/long_text_summarization.py
 whisperplus/pipelines/summarization.py
 whisperplus/pipelines/text2speech.py
 whisperplus/pipelines/whisper.py
+whisperplus/pipelines/whisper_autocaption.py
 whisperplus/pipelines/whisper_diarize.py
 whisperplus/utils/__init__.py
 whisperplus/utils/download_utils.py
 whisperplus/utils/text_utils.py
```

