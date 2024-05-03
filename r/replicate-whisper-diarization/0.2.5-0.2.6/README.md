# Comparing `tmp/replicate_whisper_diarization-0.2.5.tar.gz` & `tmp/replicate_whisper_diarization-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate_whisper_diarization-0.2.5.tar", last modified: Fri May  3 06:00:43 2024, max compression
+gzip compressed data, was "replicate_whisper_diarization-0.2.6.tar", last modified: Fri May  3 06:15:47 2024, max compression
```

## Comparing `replicate_whisper_diarization-0.2.5.tar` & `replicate_whisper_diarization-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.655955 replicate_whisper_diarization-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.651955 replicate_whisper_diarization-0.2.5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.651955 replicate_whisper_diarization-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.651955 replicate_whisper_diarization-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/.github/workflows/pypi-publish.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-03 06:00:43.655955 replicate_whisper_diarization-0.2.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.651955 replicate_whisper_diarization-0.2.5/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/notebooks/01-transcript-with-diarization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.655955 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/diarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.655955 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-03 06:00:43.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-03 06:00:43.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:00:43.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 06:00:43.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 06:00:43.000000 replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:43.655955 replicate_whisper_diarization-0.2.5/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:00:38.000000 replicate_whisper_diarization-0.2.5/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:00:43.655955 replicate_whisper_diarization-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.450462 replicate_whisper_diarization-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.446462 replicate_whisper_diarization-0.2.6/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.442462 replicate_whisper_diarization-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.446462 replicate_whisper_diarization-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/.github/workflows/pypi-publish.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-03 06:15:47.450462 replicate_whisper_diarization-0.2.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.446462 replicate_whisper_diarization-0.2.6/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/notebooks/01-transcript-with-diarization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.450462 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.450462 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-03 06:15:47.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-03 06:15:47.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:15:47.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 06:15:47.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 06:15:47.000000 replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:47.450462 replicate_whisper_diarization-0.2.6/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:15:40.000000 replicate_whisper_diarization-0.2.6/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:15:47.450462 replicate_whisper_diarization-0.2.6/setup.cfg
```

### Comparing `replicate_whisper_diarization-0.2.5/.devcontainer/Dockerfile` & `replicate_whisper_diarization-0.2.6/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/.devcontainer/devcontainer.json` & `replicate_whisper_diarization-0.2.6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/.devcontainer/docker-compose.yml` & `replicate_whisper_diarization-0.2.6/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/.github/workflows/pypi-publish.yaml` & `replicate_whisper_diarization-0.2.6/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/.gitignore` & `replicate_whisper_diarization-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/.pre-commit-config.yaml` & `replicate_whisper_diarization-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/LICENSE` & `replicate_whisper_diarization-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/PKG-INFO` & `replicate_whisper_diarization-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.5
+Version: 0.2.6
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.5/README.md` & `replicate_whisper_diarization-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/notebooks/01-transcript-with-diarization.ipynb` & `replicate_whisper_diarization-0.2.6/notebooks/01-transcript-with-diarization.ipynb`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/pyproject.toml` & `replicate_whisper_diarization-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/diarization.py` & `replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/diarization.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/language.py` & `replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/language.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/main.py` & `replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/main.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/segmentation.py` & `replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/segmentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,22 +38,22 @@
 
     if webhook_url:
         # prediction = replicate.predictions.create(
         #     version=version,
         #     input=replicate_input,
         #     webhook=webhook_url,
         # )
-        prediction = deployment.create(
+        prediction = deployment.predictions.create(
             input=replicate_input,
             webhook=webhook_url,
         )
 
         return prediction.output
 
     # prediction = replicate.predictions.create(version=version, input=replicate_input)
-    prediction = deployment.create(input=replicate_input)
+    prediction = deployment.predictions.create(input=replicate_input)
     prediction.wait()
 
     if prediction.status == "failed":
         logger.error("Diarization failed")
 
     return prediction.output
```

### Comparing `replicate_whisper_diarization-0.2.5/replicate_whisper_diarization/whisper.py` & `replicate_whisper_diarization-0.2.6/replicate_whisper_diarization/whisper.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/PKG-INFO` & `replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.5
+Version: 0.2.6
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.5/replicate_whisper_diarization.egg-info/SOURCES.txt` & `replicate_whisper_diarization-0.2.6/replicate_whisper_diarization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

