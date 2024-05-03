# Comparing `tmp/replicate_whisper_diarization-0.2.2.tar.gz` & `tmp/replicate_whisper_diarization-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate_whisper_diarization-0.2.2.tar", last modified: Thu May  2 21:22:31 2024, max compression
+gzip compressed data, was "replicate_whisper_diarization-0.2.3.tar", last modified: Thu May  2 21:57:39 2024, max compression
```

## Comparing `replicate_whisper_diarization-0.2.2.tar` & `replicate_whisper_diarization-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.843383 replicate_whisper_diarization-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.835384 replicate_whisper_diarization-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.github/workflows/pypi-publish.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:22:31.843383 replicate_whisper_diarization-0.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/notebooks/01-transcript-with-diarization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/diarization.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:22:31.843383 replicate_whisper_diarization-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.github/workflows/pypi-publish.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.566871 replicate_whisper_diarization-0.2.3/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/notebooks/01-transcript-with-diarization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 21:57:39.000000 replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:32.000000 replicate_whisper_diarization-0.2.3/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:57:39.570871 replicate_whisper_diarization-0.2.3/setup.cfg
```

### Comparing `replicate_whisper_diarization-0.2.2/.devcontainer/Dockerfile` & `replicate_whisper_diarization-0.2.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/.devcontainer/devcontainer.json` & `replicate_whisper_diarization-0.2.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/.devcontainer/docker-compose.yml` & `replicate_whisper_diarization-0.2.3/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/.github/workflows/pypi-publish.yaml` & `replicate_whisper_diarization-0.2.3/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/.gitignore` & `replicate_whisper_diarization-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/.pre-commit-config.yaml` & `replicate_whisper_diarization-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/LICENSE` & `replicate_whisper_diarization-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/PKG-INFO` & `replicate_whisper_diarization-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.2
+Version: 0.2.3
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.2/README.md` & `replicate_whisper_diarization-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/notebooks/01-transcript-with-diarization.ipynb` & `replicate_whisper_diarization-0.2.3/notebooks/01-transcript-with-diarization.ipynb`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/pyproject.toml` & `replicate_whisper_diarization-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/diarization.py` & `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/diarization.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/language.py` & `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/language.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import os
-from functools import lru_cache
+# import os
+# from functools import lru_cache
 
-import requests
-from mediapipe.tasks import python
-from mediapipe.tasks.python import text
+# import requests
+# from mediapipe.tasks import python
+# from mediapipe.tasks.python import text
 
 
-@lru_cache
-def download_model():
-    url = "https://storage.googleapis.com/mediapipe-models/language_detector/language_detector/float32/latest/language_detector.tflite"
+# @lru_cache
+# def download_model():
+#     url = "https://storage.googleapis.com/mediapipe-models/language_detector/language_detector/float32/latest/language_detector.tflite"
 
-    response = requests.get(url)
+#     response = requests.get(url)
 
-    os.makedirs("/tmp/cache", exist_ok=True)
-    with open("/tmp/cache/language_detector.tflite", "wb") as f:
-        f.write(response.content)
+#     os.makedirs("/tmp/cache", exist_ok=True)
+#     with open("/tmp/cache/language_detector.tflite", "wb") as f:
+#         f.write(response.content)
 
 
-@lru_cache
-def load_model():
-    download_model()
-    base_options = python.BaseOptions(
-        model_asset_path="/tmp/cache/language_detector.tflite"
-    )
-    options = text.LanguageDetectorOptions(base_options=base_options)
-    return text.LanguageDetector.create_from_options(options)
+# @lru_cache
+# def load_model():
+#     download_model()
+#     base_options = python.BaseOptions(
+#         model_asset_path="/tmp/cache/language_detector.tflite"
+#     )
+#     options = text.LanguageDetectorOptions(base_options=base_options)
+#     return text.LanguageDetector.create_from_options(options)
 
 
-def detect_language(text: str):
-    model = load_model()
+# def detect_language(text: str):
+#     model = load_model()
 
-    preds = model.detect(text)
+#     preds = model.detect(text)
 
-    return {pred.language_code: f"{pred.probability:.2f}" for pred in preds.detections}
+#     return {pred.language_code: f"{pred.probability:.2f}" for pred in preds.detections}
```

### Comparing `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/main.py` & `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from replicate_whisper_diarization.whisper import transcribe
 from replicate_whisper_diarization.segmentation import segmentate
 from replicate_whisper_diarization.diarization import align_word_and_speaker_segments
-from replicate_whisper_diarization.language import detect_language
+
+# from replicate_whisper_diarization.language import detect_language
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def run_transcript_with_diarization(
     audio_url: str,
@@ -26,13 +27,13 @@
         transcription and speaker information.
     """
     transcription = transcribe(audio_url=audio_url, language=language)
     speaker_segments = segmentate(audio_url, num_speakers, min_speakers, max_speakers)
 
     if not language:
         logger.error("Language not provided. using auto")
-        language = detect_language(transcription["transcript"])
+        # language = detect_language(transcription["transcript"])
 
     # language = transcript["detected_language"]
     word_timestamps = transcription["chunks"]
     segments = speaker_segments["segments"]
     return align_word_and_speaker_segments(segments, word_timestamps)
```

### Comparing `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/segmentation.py` & `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/segmentation.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/whisper.py` & `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization/whisper.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/PKG-INFO` & `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.2
+Version: 0.2.3
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/SOURCES.txt` & `replicate_whisper_diarization-0.2.3/replicate_whisper_diarization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

