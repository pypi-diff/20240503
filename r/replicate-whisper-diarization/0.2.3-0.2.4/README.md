# Comparing `tmp/replicate_whisper_diarization-0.2.3.tar.gz` & `tmp/replicate_whisper_diarization-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate_whisper_diarization-0.2.3.tar", last modified: Thu May  2 21:57:39 2024, max compression
+gzip compressed data, was "replicate_whisper_diarization-0.2.4.tar", last modified: Fri May  3 05:18:32 2024, max compression
```

## Comparing `replicate_whisper_diarization-0.2.3.tar` & `replicate_whisper_diarization-0.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.github/workflows/pypi-publish.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/notebooks/01-transcript-with-diarization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/diarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.082988 replicate_whisper_diarization-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.074988 replicate_whisper_diarization-0.2.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.074988 replicate_whisper_diarization-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.078988 replicate_whisper_diarization-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/.github/workflows/pypi-publish.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-03 05:18:32.082988 replicate_whisper_diarization-0.2.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.078988 replicate_whisper_diarization-0.2.4/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/notebooks/01-transcript-with-diarization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.078988 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.082988 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-03 05:18:32.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-03 05:18:32.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:18:32.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 05:18:32.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 05:18:32.000000 replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:32.078988 replicate_whisper_diarization-0.2.4/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:18:22.000000 replicate_whisper_diarization-0.2.4/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:18:32.082988 replicate_whisper_diarization-0.2.4/setup.cfg
```

### Comparing `replicate_whisper_diarization-0.2.3/.devcontainer/Dockerfile` & `replicate_whisper_diarization-0.2.4/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/.devcontainer/devcontainer.json` & `replicate_whisper_diarization-0.2.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/.devcontainer/docker-compose.yml` & `replicate_whisper_diarization-0.2.4/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/.github/workflows/pypi-publish.yaml` & `replicate_whisper_diarization-0.2.4/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/.gitignore` & `replicate_whisper_diarization-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/.pre-commit-config.yaml` & `replicate_whisper_diarization-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/LICENSE` & `replicate_whisper_diarization-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/PKG-INFO` & `replicate_whisper_diarization-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.3
+Version: 0.2.4
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.3/README.md` & `replicate_whisper_diarization-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/notebooks/01-transcript-with-diarization.ipynb` & `replicate_whisper_diarization-0.2.4/notebooks/01-transcript-with-diarization.ipynb`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/pyproject.toml` & `replicate_whisper_diarization-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/diarization.py` & `replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/diarization.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/language.py` & `replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/language.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/main.py` & `replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 # from replicate_whisper_diarization.language import detect_language
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def run_transcript_with_diarization(
-    audio_url: str,
+    audio: str,
     language: str | None = None,
     num_speakers: int | None = None,
     min_speakers: int | None = None,
     max_speakers: int | None = None,
 ) -> list[dict]:
     """
     Runs diarization on the given audio and returns a list of dictionaries containing word-level transcriptions
     along with speaker information.
 
     Args:
-        audio_url (str): The URL of the audio file to be transcribed.
+        audio (str): The URL of the audio file to be transcribed.
 
     Returns:
         list[dict]: A list of dictionaries, where each dictionary represents a word segment with its corresponding
         transcription and speaker information.
     """
-    transcription = transcribe(audio_url=audio_url, language=language)
-    speaker_segments = segmentate(audio_url, num_speakers, min_speakers, max_speakers)
+    transcription = transcribe(audio=audio, language=language)
+    speaker_segments = segmentate(audio, num_speakers, min_speakers, max_speakers)
 
     if not language:
         logger.error("Language not provided. using auto")
         # language = detect_language(transcription["transcript"])
 
     # language = transcript["detected_language"]
     word_timestamps = transcription["chunks"]
```

### Comparing `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/segmentation.py` & `replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/segmentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 MODEL_VERSION = os.getenv(
     "DIARIZATION_MODEL_VERSION",
     "f7425066750cd06fdf95b831c08bba1530f222a2eb4145f40493f431b7483b95",
 )
 
 
 def segmentate(
-    audio_url: str,
+    audio: str,
     num_speakers: int | None = None,
     min_speakers: int | None = None,
     max_speakers: int | None = None,
     webhook_url: str | None = None,
 ) -> dict:
     model = replicate.models.get(MODEL_NAME)
     version = model.versions.get(MODEL_VERSION)
     replicate_input = {
-        "audio_url": audio_url,
+        "audio": audio,
         "num_speakers": num_speakers,
         "min_speakers": min_speakers,
         "max_speakers": max_speakers,
     }
     replicate_input = {k: v for k, v in replicate_input.items() if v is not None}
 
     if webhook_url:
```

### Comparing `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/whisper.py` & `replicate_whisper_diarization-0.2.4/replicate_whisper_diarization/whisper.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 )
 
 model = replicate.models.get(MODEL_NAME)
 version = model.versions.get(MODEL_VERSION)
 
 
 def transcribe(
-    audio_url: str,
+    audio: str,
     batch_size: int = 16,
     language: str | None = None,
     webhook_url: str | None = None,
 ) -> dict:
     """
     Transcribes the audio from the given URL using the Whisper diarization model.
 
     Args:
-        audio_url (str): The URL of the audio file to transcribe.
+        audio (str): The URL of the audio file to transcribe.
         batch_size (int, optional): The batch size for processing the audio. Defaults to 16.
         language (str | None, optional): The language of the audio. Defaults to None.
         webhook_url (str | None, optional): The URL to send the transcription results to via webhook. Defaults to None.
 
     Returns:
         dict: The transcription output as a dictionary.
 
     Raises:
         Exception: If the transcription fails.
     """
     replicate_input = {
-        "audio": audio_url,
+        "audio": audio,
         "batch_size": batch_size,
         "language": language,
         "timestamp": "word",
         "task": "transcribe",
     }
     replicate_input = {k: v for k, v in replicate_input.items() if v is not None}
```

### Comparing `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/PKG-INFO` & `replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.3
+Version: 0.2.4
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/SOURCES.txt` & `replicate_whisper_diarization-0.2.4/replicate_whisper_diarization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

