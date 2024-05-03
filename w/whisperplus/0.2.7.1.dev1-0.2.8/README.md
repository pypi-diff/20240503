# Comparing `tmp/whisperplus-0.2.7.1.dev1.tar.gz` & `tmp/whisperplus-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisperplus-0.2.7.1.dev1.tar", last modified: Fri May  3 08:30:44 2024, max compression
+gzip compressed data, was "whisperplus-0.2.8.tar", last modified: Thu May  2 22:18:32 2024, max compression
```

## Comparing `whisperplus-0.2.7.1.dev1.tar` & `whisperplus-0.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-03 08:30:44.075349 whisperplus-0.2.7.1.dev1/
--rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/LICENSE
--rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/MANIFEST.in
--rw-r--r--   0 kadirnar   (501) staff       (20)     5521 2024-05-03 08:30:44.075471 whisperplus-0.2.7.1.dev1/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)     5204 2024-05-02 22:01:09.000000 whisperplus-0.2.7.1.dev1/README.md
--rw-r--r--   0 kadirnar   (501) staff       (20)      395 2024-05-03 08:30:20.000000 whisperplus-0.2.7.1.dev1/requirements.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-03 08:30:44.075760 whisperplus-0.2.7.1.dev1/setup.cfg
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/setup.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-03 08:30:44.070771 whisperplus-0.2.7.1.dev1/whisperplus/
--rw-r--r--   0 kadirnar   (501) staff       (20)      665 2024-05-03 08:30:35.000000 whisperplus-0.2.7.1.dev1/whisperplus/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/app.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-03 08:30:44.073955 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/autollm_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/lancedb_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/long_text_summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/text2speech.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2773 2024-05-02 22:00:09.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/whisper.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/whisper_autocaption.py
--rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/pipelines/whisper_diarize.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-03 08:30:44.074609 whisperplus-0.2.7.1.dev1/whisperplus/utils/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/utils/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/utils/download_utils.py
--rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.2.7.1.dev1/whisperplus/utils/text_utils.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-03 08:30:44.071609 whisperplus-0.2.7.1.dev1/whisperplus.egg-info/
--rw-r--r--   0 kadirnar   (501) staff       (20)     5521 2024-05-03 08:30:44.000000 whisperplus-0.2.7.1.dev1/whisperplus.egg-info/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)      740 2024-05-03 08:30:44.000000 whisperplus-0.2.7.1.dev1/whisperplus.egg-info/SOURCES.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-03 08:30:44.000000 whisperplus-0.2.7.1.dev1/whisperplus.egg-info/dependency_links.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      395 2024-05-03 08:30:44.000000 whisperplus-0.2.7.1.dev1/whisperplus.egg-info/requires.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-03 08:30:44.000000 whisperplus-0.2.7.1.dev1/whisperplus.egg-info/top_level.txt
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

### Comparing `whisperplus-0.2.7.1.dev1/LICENSE` & `whisperplus-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/PKG-INFO` & `whisperplus-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.2.7.1.dev1
+Version: 0.2.8
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.2.7.1.dev1 Summary:
-WhisperPlus: A Python library for WhisperPlus API. Home-page: https://
-github.com/kadirnar/whisperplus Author: kadirnar Author-email:
-kadir.nar@hotmail.com License: Apache License 2.0 Description-Content-Type:
-text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8 Summary: WhisperPlus: A
+Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
+whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
+Apache License 2.0 Description-Content-Type: text/markdown License-File:
+LICENSE
   ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
 ## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
 --no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
 [HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
 ðï¸ Usage To use the whisperplus library, follow the steps below for
```

### Comparing `whisperplus-0.2.7.1.dev1/README.md` & `whisperplus-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/setup.cfg` & `whisperplus-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/setup.py` & `whisperplus-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/__init__.py` & `whisperplus-0.2.8/whisperplus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 from whisperplus.pipelines.summarization import TextSummarizationPipeline
 from whisperplus.pipelines.text2speech import TextToSpeechPipeline
 from whisperplus.pipelines.whisper import SpeechToTextPipeline
 from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
 from whisperplus.utils.download_utils import download_and_convert_to_mp3
 from whisperplus.utils.text_utils import format_speech_to_dialogue
 
-__version__ = '0.2.7.1.dev1'
+__version__ = '0.2.8'
 __author__ = 'kadirnar'
 __license__ = 'Apache License 2.0'
```

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/app.py` & `whisperplus-0.2.8/whisperplus/app.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/autollm_chatbot.py` & `whisperplus-0.2.8/whisperplus/pipelines/autollm_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/lancedb_chatbot.py` & `whisperplus-0.2.8/whisperplus/pipelines/lancedb_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/long_text_summarization.py` & `whisperplus-0.2.8/whisperplus/pipelines/long_text_summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/summarization.py` & `whisperplus-0.2.8/whisperplus/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/text2speech.py` & `whisperplus-0.2.8/whisperplus/pipelines/text2speech.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/whisper.py` & `whisperplus-0.2.8/whisperplus/pipelines/whisper.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/whisper_autocaption.py` & `whisperplus-0.2.8/whisperplus/pipelines/whisper_autocaption.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/pipelines/whisper_diarize.py` & `whisperplus-0.2.8/whisperplus/pipelines/whisper_diarize.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/utils/download_utils.py` & `whisperplus-0.2.8/whisperplus/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus/utils/text_utils.py` & `whisperplus-0.2.8/whisperplus/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus.egg-info/PKG-INFO` & `whisperplus-0.2.8/whisperplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.2.7.1.dev1
+Version: 0.2.8
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.2.7.1.dev1 Summary:
-WhisperPlus: A Python library for WhisperPlus API. Home-page: https://
-github.com/kadirnar/whisperplus Author: kadirnar Author-email:
-kadir.nar@hotmail.com License: Apache License 2.0 Description-Content-Type:
-text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: whisperplus Version: 0.2.8 Summary: WhisperPlus: A
+Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
+whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
+Apache License 2.0 Description-Content-Type: text/markdown License-File:
+LICENSE
   ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
 ## ð ï¸ Installation ```bash pip install whisperplus pip install flash-attn
 --no-build-isolation ``` ## ð¤ Model Hub You can find the models on the
 [HuggingFace Model Hub](https://huggingface.co/models?search=whisper) ##
 ðï¸ Usage To use the whisperplus library, follow the steps below for
```

### Comparing `whisperplus-0.2.7.1.dev1/whisperplus.egg-info/SOURCES.txt` & `whisperplus-0.2.8/whisperplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

