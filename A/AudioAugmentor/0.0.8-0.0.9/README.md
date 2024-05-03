# Comparing `tmp/audioaugmentor-0.0.8.tar.gz` & `tmp/audioaugmentor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioaugmentor-0.0.8.tar", last modified: Fri May  3 16:36:48 2024, max compression
+gzip compressed data, was "audioaugmentor-0.0.9.tar", last modified: Fri May  3 17:38:30 2024, max compression
```

## Comparing `audioaugmentor-0.0.8.tar` & `audioaugmentor-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 16:36:48.350752 audioaugmentor-0.0.8/AudioAugmentor/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.8/AudioAugmentor/__init__.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34021 2024-05-03 16:35:00.000000 audioaugmentor-0.0.8/AudioAugmentor/core.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.8/AudioAugmentor/rir_setup.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4846 2024-05-03 16:35:24.000000 audioaugmentor-0.0.8/AudioAugmentor/sox_parser.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.8/AudioAugmentor/torchaudio_transf_wrapper.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 16:35:07.000000 audioaugmentor-0.0.8/AudioAugmentor/transf_gen.py
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/AudioAugmentor.egg-info/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/SOURCES.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/dependency_links.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/requires.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/top_level.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.8/LICENSE
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    32597 2024-05-03 14:34:45.000000 audioaugmentor-0.0.8/README.md
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 16:36:43.000000 audioaugmentor-0.0.8/pyproject.toml
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/setup.cfg
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/AudioAugmentor/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.9/AudioAugmentor/__init__.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34021 2024-05-03 16:35:00.000000 audioaugmentor-0.0.9/AudioAugmentor/core.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.9/AudioAugmentor/rir_setup.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4846 2024-05-03 16:35:24.000000 audioaugmentor-0.0.9/AudioAugmentor/sox_parser.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.9/AudioAugmentor/torchaudio_transf_wrapper.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 16:35:07.000000 audioaugmentor-0.0.9/AudioAugmentor/transf_gen.py
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/AudioAugmentor.egg-info/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/SOURCES.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/dependency_links.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/requires.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/top_level.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.9/LICENSE
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    32597 2024-05-03 14:34:45.000000 audioaugmentor-0.0.9/README.md
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 17:32:11.000000 audioaugmentor-0.0.9/pyproject.toml
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/setup.cfg
```

### Comparing `audioaugmentor-0.0.8/AudioAugmentor/core.py` & `audioaugmentor-0.0.9/AudioAugmentor/core.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.8/AudioAugmentor/rir_setup.py` & `audioaugmentor-0.0.9/AudioAugmentor/rir_setup.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.8/AudioAugmentor/sox_parser.py` & `audioaugmentor-0.0.9/AudioAugmentor/sox_parser.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.8/AudioAugmentor/torchaudio_transf_wrapper.py` & `audioaugmentor-0.0.9/AudioAugmentor/torchaudio_transf_wrapper.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.8/AudioAugmentor/transf_gen.py` & `audioaugmentor-0.0.9/AudioAugmentor/transf_gen.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.8/AudioAugmentor.egg-info/PKG-INFO` & `audioaugmentor-0.0.9/AudioAugmentor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioaugmentor-0.0.8/LICENSE` & `audioaugmentor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.8/PKG-INFO` & `audioaugmentor-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioaugmentor-0.0.8/README.md` & `audioaugmentor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.8/pyproject.toml` & `audioaugmentor-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["AudioAugmentor"]
 
 [project]
 name = "AudioAugmentor"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python package for simple application of wide range of audio augmentations."
 readme = "README.md"
 authors = [{ name = "Ladislav Vašina", email = "ladislavvasina@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

