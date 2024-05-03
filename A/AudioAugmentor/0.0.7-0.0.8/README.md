# Comparing `tmp/audioaugmentor-0.0.7.tar.gz` & `tmp/audioaugmentor-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioaugmentor-0.0.7.tar", last modified: Fri May  3 15:08:47 2024, max compression
+gzip compressed data, was "audioaugmentor-0.0.8.tar", last modified: Fri May  3 16:36:48 2024, max compression
```

## Comparing `audioaugmentor-0.0.7.tar` & `audioaugmentor-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 15:08:47.297405 audioaugmentor-0.0.7/
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 15:08:47.296405 audioaugmentor-0.0.7/AudioAugmentor/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.7/AudioAugmentor/__init__.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    33793 2024-05-03 15:08:20.000000 audioaugmentor-0.0.7/AudioAugmentor/core.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.7/AudioAugmentor/rir_setup.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4928 2024-05-03 15:08:37.000000 audioaugmentor-0.0.7/AudioAugmentor/sox_parser.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.7/AudioAugmentor/torchaudio_transf_wrapper.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 15:08:30.000000 audioaugmentor-0.0.7/AudioAugmentor/transf_gen.py
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 15:08:47.296405 audioaugmentor-0.0.7/AudioAugmentor.egg-info/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/SOURCES.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/dependency_links.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/requires.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/top_level.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.7/LICENSE
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 15:08:47.297405 audioaugmentor-0.0.7/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    32597 2024-05-03 14:34:45.000000 audioaugmentor-0.0.7/README.md
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 15:03:20.000000 audioaugmentor-0.0.7/pyproject.toml
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 15:08:47.297405 audioaugmentor-0.0.7/setup.cfg
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 16:36:48.350752 audioaugmentor-0.0.8/AudioAugmentor/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.8/AudioAugmentor/__init__.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34021 2024-05-03 16:35:00.000000 audioaugmentor-0.0.8/AudioAugmentor/core.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.8/AudioAugmentor/rir_setup.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4846 2024-05-03 16:35:24.000000 audioaugmentor-0.0.8/AudioAugmentor/sox_parser.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.8/AudioAugmentor/torchaudio_transf_wrapper.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 16:35:07.000000 audioaugmentor-0.0.8/AudioAugmentor/transf_gen.py
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/AudioAugmentor.egg-info/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/SOURCES.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/dependency_links.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/requires.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 16:36:48.000000 audioaugmentor-0.0.8/AudioAugmentor.egg-info/top_level.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.8/LICENSE
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    32597 2024-05-03 14:34:45.000000 audioaugmentor-0.0.8/README.md
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 16:36:43.000000 audioaugmentor-0.0.8/pyproject.toml
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 16:36:48.351752 audioaugmentor-0.0.8/setup.cfg
```

### Comparing `audioaugmentor-0.0.7/AudioAugmentor/core.py` & `audioaugmentor-0.0.8/AudioAugmentor/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,26 +361,30 @@
                         tmp = next(iter(transform))
                         p = transform['p']
                         currently_used_trasnf = get_transf(tmp, TTW_TRANSF)
                         transform = torch_randomizer(
                             getattr(TTW, currently_used_trasnf)(**transform[tmp]), p=p)
                         if transform is None:
                             continue
-                    waveform = torch.from_numpy(waveform).float()
+
+                    transform = transform.to(self.device)
+                    waveform = torch.from_numpy(waveform).float().to(self.device)
+                    print(waveform.device, self.device, transform)
                     waveform = waveform.unsqueeze(0)
                     waveform = transform(waveform)
                     if isinstance(waveform, tuple):
                         waveform = waveform[0]
-                    waveform = waveform.detach().numpy()
+                    waveform = waveform.detach().cpu().numpy()
                     waveform = waveform.squeeze(0)
 
                 elif transform.__class__.__module__.split('.')[0] == 'torch_audiomentations':
-                    waveform = torch.from_numpy(waveform).float()
+                    transform = transform.to(self.device)
+                    waveform = torch.from_numpy(waveform).float().to(self.device)
                     waveform = waveform.unsqueeze(0).unsqueeze(0)
-                    waveform = transform(waveform).detach().numpy()
+                    waveform = transform(waveform).detach().cpu().numpy()
                     waveform = waveform.squeeze(0).squeeze(0)
 
         # @@@@@@@@@@@@@@@@@@@@@@@@ SOX EFFECTS PART OF THE CODE @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
         if self.sox_effects is not None:
             if self.device == 'cuda':
                 print('WARNING: sox_effects are not supported on cuda!\n\t Using cpu.')
             # check if waveform is torch.tensor, if not convert it to torch.tensor
```

### Comparing `audioaugmentor-0.0.7/AudioAugmentor/rir_setup.py` & `audioaugmentor-0.0.8/AudioAugmentor/rir_setup.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.7/AudioAugmentor/sox_parser.py` & `audioaugmentor-0.0.8/AudioAugmentor/sox_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # Build pip package with this uncommented
 from .transf_gen import CODECS
 
 # Test sources with this uncommented
 # from transf_gen import CODECS
 
 EFFECTS_NAMES = torchaudio.sox_effects.effect_names()
-# example_sox = '--sox="norm gain 0 highpass 1000 phaser 0.5 0.6 1 0.45 0.6 -s"'
-
 
 def load_sox_file(file_path):
     """
     This function reads file containing pseudo-sox commands
     on each line and returns a list of lines from the file.
     This function also ignores lines starting with #
```

### Comparing `audioaugmentor-0.0.7/AudioAugmentor/torchaudio_transf_wrapper.py` & `audioaugmentor-0.0.8/AudioAugmentor/torchaudio_transf_wrapper.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.7/AudioAugmentor/transf_gen.py` & `audioaugmentor-0.0.8/AudioAugmentor/transf_gen.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.7/AudioAugmentor.egg-info/PKG-INFO` & `audioaugmentor-0.0.8/AudioAugmentor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioaugmentor-0.0.7/LICENSE` & `audioaugmentor-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.7/PKG-INFO` & `audioaugmentor-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioaugmentor-0.0.7/README.md` & `audioaugmentor-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.7/pyproject.toml` & `audioaugmentor-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["AudioAugmentor"]
 
 [project]
 name = "AudioAugmentor"
-version = "0.0.7"
+version = "0.0.8"
 description = "Python package for simple application of wide range of audio augmentations."
 readme = "README.md"
 authors = [{ name = "Ladislav Vašina", email = "ladislavvasina@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

