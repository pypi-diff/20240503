# Comparing `tmp/openvoicechat-0.1.tar.gz` & `tmp/openvoicechat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvoicechat-0.1.tar", last modified: Fri May  3 21:12:41 2024, max compression
+gzip compressed data, was "openvoicechat-0.1.1.tar", last modified: Fri May  3 21:17:13 2024, max compression
```

## Comparing `openvoicechat-0.1.tar` & `openvoicechat-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:12:41.907579 openvoicechat-0.1/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)    11357 2024-05-01 20:34:23.000000 openvoicechat-0.1/LICENSE
--rw-r--r--   0 fakhir    (1000) fakhir    (1000)      844 2024-05-03 21:12:41.907579 openvoicechat-0.1/PKG-INFO
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1402 2024-05-02 20:34:44.000000 openvoicechat-0.1/README.md
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:12:41.903579 openvoicechat-0.1/openvoicechat/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      147 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/__init__.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:12:41.903579 openvoicechat-0.1/openvoicechat/llm/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      188 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/llm/__init__.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1884 2024-05-03 19:45:40.000000 openvoicechat-0.1/openvoicechat/llm/base.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1403 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/llm/llm_gpt.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3104 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/llm/llm_hf.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1764 2024-05-02 20:34:54.000000 openvoicechat-0.1/openvoicechat/llm/llm_llama.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)    14665 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/prompts.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:12:41.903579 openvoicechat-0.1/openvoicechat/stt/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      171 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/stt/__init__.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3658 2024-05-03 19:45:40.000000 openvoicechat-0.1/openvoicechat/stt/base.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     2175 2024-05-03 19:53:08.000000 openvoicechat-0.1/openvoicechat/stt/stt_deepgram.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1016 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/stt/stt_hf.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1534 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/stt/stt_vosk.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:12:41.907579 openvoicechat-0.1/openvoicechat/tts/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      325 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/tts/__init__.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     5558 2024-05-03 20:01:51.000000 openvoicechat-0.1/openvoicechat/tts/base.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1827 2024-05-03 19:53:08.000000 openvoicechat-0.1/openvoicechat/tts/tts_elevenlabs.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1526 2024-05-03 19:53:08.000000 openvoicechat-0.1/openvoicechat/tts/tts_hf.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     2823 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/tts/tts_parler.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1505 2024-05-03 18:59:12.000000 openvoicechat-0.1/openvoicechat/tts/tts_piper.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3106 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/tts/tts_tortoise.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1086 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/tts/tts_xtts.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3307 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/utils.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1155 2024-05-02 20:34:44.000000 openvoicechat-0.1/openvoicechat/vad.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:12:41.907579 openvoicechat-0.1/openvoicechat.egg-info/
--rw-r--r--   0 fakhir    (1000) fakhir    (1000)      844 2024-05-03 21:12:41.000000 openvoicechat-0.1/openvoicechat.egg-info/PKG-INFO
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      844 2024-05-03 21:12:41.000000 openvoicechat-0.1/openvoicechat.egg-info/SOURCES.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)        1 2024-05-03 21:12:41.000000 openvoicechat-0.1/openvoicechat.egg-info/dependency_links.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      252 2024-05-03 21:12:41.000000 openvoicechat-0.1/openvoicechat.egg-info/requires.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)       14 2024-05-03 21:12:41.000000 openvoicechat-0.1/openvoicechat.egg-info/top_level.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)       38 2024-05-03 21:12:41.907579 openvoicechat-0.1/setup.cfg
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      666 2024-05-03 21:12:38.000000 openvoicechat-0.1/setup.py
+drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:17:13.434712 openvoicechat-0.1.1/
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)    11357 2024-05-01 20:34:23.000000 openvoicechat-0.1.1/LICENSE
+-rw-r--r--   0 fakhir    (1000) fakhir    (1000)      896 2024-05-03 21:17:13.434712 openvoicechat-0.1.1/PKG-INFO
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1389 2024-05-03 21:13:31.000000 openvoicechat-0.1.1/README.md
+drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:17:13.430712 openvoicechat-0.1.1/openvoicechat/
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      147 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/__init__.py
+drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:17:13.430712 openvoicechat-0.1.1/openvoicechat/llm/
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      188 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/llm/__init__.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1884 2024-05-03 19:45:40.000000 openvoicechat-0.1.1/openvoicechat/llm/base.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1403 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/llm/llm_gpt.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3104 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/llm/llm_hf.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1764 2024-05-02 20:34:54.000000 openvoicechat-0.1.1/openvoicechat/llm/llm_llama.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)    14665 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/prompts.py
+drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:17:13.430712 openvoicechat-0.1.1/openvoicechat/stt/
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      171 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/stt/__init__.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3658 2024-05-03 19:45:40.000000 openvoicechat-0.1.1/openvoicechat/stt/base.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     2175 2024-05-03 19:53:08.000000 openvoicechat-0.1.1/openvoicechat/stt/stt_deepgram.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1016 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/stt/stt_hf.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1534 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/stt/stt_vosk.py
+drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:17:13.430712 openvoicechat-0.1.1/openvoicechat/tts/
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      325 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/tts/__init__.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     5558 2024-05-03 20:01:51.000000 openvoicechat-0.1.1/openvoicechat/tts/base.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1827 2024-05-03 19:53:08.000000 openvoicechat-0.1.1/openvoicechat/tts/tts_elevenlabs.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1526 2024-05-03 19:53:08.000000 openvoicechat-0.1.1/openvoicechat/tts/tts_hf.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     2823 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/tts/tts_parler.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1505 2024-05-03 18:59:12.000000 openvoicechat-0.1.1/openvoicechat/tts/tts_piper.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3106 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/tts/tts_tortoise.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1086 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/tts/tts_xtts.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3307 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/utils.py
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1155 2024-05-02 20:34:44.000000 openvoicechat-0.1.1/openvoicechat/vad.py
+drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-03 21:17:13.434712 openvoicechat-0.1.1/openvoicechat.egg-info/
+-rw-r--r--   0 fakhir    (1000) fakhir    (1000)      896 2024-05-03 21:17:13.000000 openvoicechat-0.1.1/openvoicechat.egg-info/PKG-INFO
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      844 2024-05-03 21:17:13.000000 openvoicechat-0.1.1/openvoicechat.egg-info/SOURCES.txt
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)        1 2024-05-03 21:17:13.000000 openvoicechat-0.1.1/openvoicechat.egg-info/dependency_links.txt
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      252 2024-05-03 21:17:13.000000 openvoicechat-0.1.1/openvoicechat.egg-info/requires.txt
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)       14 2024-05-03 21:17:13.000000 openvoicechat-0.1.1/openvoicechat.egg-info/top_level.txt
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)       38 2024-05-03 21:17:13.434712 openvoicechat-0.1.1/setup.cfg
+-rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      718 2024-05-03 21:17:04.000000 openvoicechat-0.1.1/setup.py
```

### Comparing `openvoicechat-0.1/LICENSE` & `openvoicechat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/PKG-INFO` & `openvoicechat-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: openvoicechat
-Version: 0.1
+Version: 0.1.1
+Home-page: http://www.fakhirali.pk/OpenVoiceChat/
 License-File: LICENSE
 Requires-Dist: sounddevice
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: pygame
 Requires-Dist: pyaudio
 Requires-Dist: librosa
```

### Comparing `openvoicechat-0.1/README.md` & `openvoicechat-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,9 +55,8 @@
 Similary "piper" can be replaced by any of the following
 - piper
 - vosk
 - llama
 - open_ai
 - tortoise
 - xtts
-- parler_tts
 - transformers
```

### Comparing `openvoicechat-0.1/openvoicechat/llm/base.py` & `openvoicechat-0.1.1/openvoicechat/llm/base.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/llm/llm_gpt.py` & `openvoicechat-0.1.1/openvoicechat/llm/llm_gpt.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/llm/llm_hf.py` & `openvoicechat-0.1.1/openvoicechat/llm/llm_hf.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/llm/llm_llama.py` & `openvoicechat-0.1.1/openvoicechat/llm/llm_llama.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/prompts.py` & `openvoicechat-0.1.1/openvoicechat/prompts.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/stt/base.py` & `openvoicechat-0.1.1/openvoicechat/stt/base.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/stt/stt_deepgram.py` & `openvoicechat-0.1.1/openvoicechat/stt/stt_deepgram.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/stt/stt_hf.py` & `openvoicechat-0.1.1/openvoicechat/stt/stt_hf.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/stt/stt_vosk.py` & `openvoicechat-0.1.1/openvoicechat/stt/stt_vosk.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/tts/base.py` & `openvoicechat-0.1.1/openvoicechat/tts/base.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/tts/tts_elevenlabs.py` & `openvoicechat-0.1.1/openvoicechat/tts/tts_elevenlabs.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/tts/tts_hf.py` & `openvoicechat-0.1.1/openvoicechat/tts/tts_hf.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/tts/tts_parler.py` & `openvoicechat-0.1.1/openvoicechat/tts/tts_parler.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/tts/tts_piper.py` & `openvoicechat-0.1.1/openvoicechat/tts/tts_piper.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/tts/tts_tortoise.py` & `openvoicechat-0.1.1/openvoicechat/tts/tts_tortoise.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/tts/tts_xtts.py` & `openvoicechat-0.1.1/openvoicechat/tts/tts_xtts.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/utils.py` & `openvoicechat-0.1.1/openvoicechat/utils.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat/vad.py` & `openvoicechat-0.1.1/openvoicechat/vad.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1/openvoicechat.egg-info/PKG-INFO` & `openvoicechat-0.1.1/openvoicechat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: openvoicechat
-Version: 0.1
+Version: 0.1.1
+Home-page: http://www.fakhirali.pk/OpenVoiceChat/
 License-File: LICENSE
 Requires-Dist: sounddevice
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: pygame
 Requires-Dist: pyaudio
 Requires-Dist: librosa
```

### Comparing `openvoicechat-0.1/openvoicechat.egg-info/SOURCES.txt` & `openvoicechat-0.1.1/openvoicechat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

