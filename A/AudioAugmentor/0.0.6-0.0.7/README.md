# Comparing `tmp/audioaugmentor-0.0.6.tar.gz` & `tmp/audioaugmentor-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioaugmentor-0.0.6.tar", last modified: Fri May  3 12:48:59 2024, max compression
+gzip compressed data, was "audioaugmentor-0.0.7.tar", last modified: Fri May  3 15:08:47 2024, max compression
```

## Comparing `audioaugmentor-0.0.6.tar` & `audioaugmentor-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 12:48:59.690087 audioaugmentor-0.0.6/AudioAugmentor/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.6/AudioAugmentor/__init__.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    33659 2024-05-03 12:48:31.000000 audioaugmentor-0.0.6/AudioAugmentor/core.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.6/AudioAugmentor/rir_setup.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4928 2024-05-03 12:48:51.000000 audioaugmentor-0.0.6/AudioAugmentor/sox_parser.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.6/AudioAugmentor/torchaudio_transf_wrapper.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 12:48:42.000000 audioaugmentor-0.0.6/AudioAugmentor/transf_gen.py
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/AudioAugmentor.egg-info/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34542 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/SOURCES.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/dependency_links.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/requires.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/top_level.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.6/LICENSE
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34542 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    31291 2024-05-03 08:00:35.000000 audioaugmentor-0.0.6/README.md
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 12:44:38.000000 audioaugmentor-0.0.6/pyproject.toml
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/setup.cfg
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 15:08:47.297405 audioaugmentor-0.0.7/
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 15:08:47.296405 audioaugmentor-0.0.7/AudioAugmentor/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.7/AudioAugmentor/__init__.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    33793 2024-05-03 15:08:20.000000 audioaugmentor-0.0.7/AudioAugmentor/core.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.7/AudioAugmentor/rir_setup.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4928 2024-05-03 15:08:37.000000 audioaugmentor-0.0.7/AudioAugmentor/sox_parser.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.7/AudioAugmentor/torchaudio_transf_wrapper.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 15:08:30.000000 audioaugmentor-0.0.7/AudioAugmentor/transf_gen.py
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 15:08:47.296405 audioaugmentor-0.0.7/AudioAugmentor.egg-info/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/SOURCES.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/dependency_links.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/requires.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 15:08:47.000000 audioaugmentor-0.0.7/AudioAugmentor.egg-info/top_level.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.7/LICENSE
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 15:08:47.297405 audioaugmentor-0.0.7/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    32597 2024-05-03 14:34:45.000000 audioaugmentor-0.0.7/README.md
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 15:03:20.000000 audioaugmentor-0.0.7/pyproject.toml
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 15:08:47.297405 audioaugmentor-0.0.7/setup.cfg
```

### Comparing `audioaugmentor-0.0.6/AudioAugmentor/core.py` & `audioaugmentor-0.0.7/AudioAugmentor/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,18 @@
                     f'CURRENT TRANSFORM: {transform}') if self.verbose else None
                 if transform.__class__.__module__.split('.')[0] == AA.__name__:
                     waveform = transform(
                         waveform, sample_rate=self.sample_rate)
 
                 elif transform.__class__.__name__ == 'ApplyRIR':
                     x = transform.audio_sample_rate
-                    transform = rir_setup.ApplyRIR(**x())
+                    if isinstance(x, dict):
+                        transform = rir_setup.ApplyRIR(**x)
+                    else:
+                        transform = rir_setup.ApplyRIR(**x())
                     waveform = transform(waveform)
 
                 elif transform.__class__.__module__.split('.')[-1] == '_effector':
                     transposed_waveform_tensor = torch.from_numpy(
                         np.expand_dims(waveform, axis=1).transpose(0, 1)
                     )
                     waveform = transform.apply(
```

### Comparing `audioaugmentor-0.0.6/AudioAugmentor/rir_setup.py` & `audioaugmentor-0.0.7/AudioAugmentor/rir_setup.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.6/AudioAugmentor/sox_parser.py` & `audioaugmentor-0.0.7/AudioAugmentor/sox_parser.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.6/AudioAugmentor/torchaudio_transf_wrapper.py` & `audioaugmentor-0.0.7/AudioAugmentor/torchaudio_transf_wrapper.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.6/AudioAugmentor/transf_gen.py` & `audioaugmentor-0.0.7/AudioAugmentor/transf_gen.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.6/AudioAugmentor.egg-info/PKG-INFO` & `audioaugmentor-0.0.7/AudioAugmentor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -271,14 +271,24 @@
 # Load test wav file
 signal, fs = torchaudio.load('../data/test.wav')
 # Apply transformations
 waveform = augment(signal.numpy()[0])
 display(Audio(waveform, rate=fs))
 ```
 
+**c)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `AugmentLocalAudioDataset` class and apply the augmentations to the local audio dataset.
+```php
+augment = core.AugmentLocalAudioDataset(
+    transformations=transformations, device='cpu', sox_effects=None, sample_rate=16000, verbose=False,
+    #transformations=None, device='cpu', sox_effects='--sox="norm gain 20 highpass 300 phaser 0.5 0.6 1 0.45 0.6 -s" amr audio_bitrate 4.75k', sample_rate=16000, verbose=False,
+    #transformations=None, device='cpu', sox_effects=sox_file_content, sample_rate=16000, verbose=False,
+)
+augment(input_dir='../data/test-input-folder', output_dir='../data/test-output-folder')
+```
+
 
 # EXAMPLES OF AVAILABLE AUGMENTATIONS
 ## !!!Put following examples as an argument for `transf_gen.transf_gen` function to generate a list of transformations!!!
 
 Like this:
 ```php
 transformations = transf_gen.transf_gen(verbose=True,
@@ -528,14 +538,15 @@
 <a id="applyrir"></a>
 ### [⬆️](#available-augmentations) ApplyRIR
 ```php
 # Use this to see available materials you can use as walls_mat, floor_mat and ceiling_mat argument
 # from AudioAugmentor import rir_setup
 # rir_setup.get_all_materials_info()
 
+# This way you set up parameters when you want to generate random room parameter
 rir_kwargs = {
     'audio_sample_rate': 16000,
     'x_range': (0, 100), 
     'y_range': (0, 100), 
     'num_vertices_range': (3, 6),
     'mic_height': 1.5,
     'source_height': 1.5,
@@ -543,14 +554,28 @@
     'room_height': 2.0,
     'max_order': 3,
     'floor_mat': 'carpet_cotton',
     'ceiling_mat': 'hard_surface',
     'ray_tracing': True,
     'air_absorption': True,
 }
+# This way you set up parameters when you want to generate specific room
+rir_kwargs = {
+    'audio_sample_rate': 16000,
+    'corners_coord': [[0, 0], [0, 3], [5, 3], [5, 1], [3, 1], [3, 0]],
+    'walls_mat': 'curtains_cotton_0.5',
+    'room_height': 2.0,
+    'max_order': 3,
+    'floor_mat': 'carpet_cotton',
+    'ceiling_mat': 'hard_surface',
+    'ray_tracing': True,
+    'air_absorption': True,
+    'source_coord': [[1.0], [1.0], [0.5]],
+    'microphones_coord': [[3.5], [2.0], [0.5]],
+}
 transformations = transf_gen.transf_gen(verbose=True,
                                         ApplyRIR=rir_kwargs,
                                         )
 ```
 <a id="sevenbandparametriceq"></a>
 ### [⬆️](#available-augmentations) SevenBandParametricEQ [docs](https://iver56.github.io/audiomentations/waveform_transforms/seven_band_parametric_eq/)
 ```python
```

### Comparing `audioaugmentor-0.0.6/LICENSE` & `audioaugmentor-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.6/PKG-INFO` & `audioaugmentor-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -271,14 +271,24 @@
 # Load test wav file
 signal, fs = torchaudio.load('../data/test.wav')
 # Apply transformations
 waveform = augment(signal.numpy()[0])
 display(Audio(waveform, rate=fs))
 ```
 
+**c)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `AugmentLocalAudioDataset` class and apply the augmentations to the local audio dataset.
+```php
+augment = core.AugmentLocalAudioDataset(
+    transformations=transformations, device='cpu', sox_effects=None, sample_rate=16000, verbose=False,
+    #transformations=None, device='cpu', sox_effects='--sox="norm gain 20 highpass 300 phaser 0.5 0.6 1 0.45 0.6 -s" amr audio_bitrate 4.75k', sample_rate=16000, verbose=False,
+    #transformations=None, device='cpu', sox_effects=sox_file_content, sample_rate=16000, verbose=False,
+)
+augment(input_dir='../data/test-input-folder', output_dir='../data/test-output-folder')
+```
+
 
 # EXAMPLES OF AVAILABLE AUGMENTATIONS
 ## !!!Put following examples as an argument for `transf_gen.transf_gen` function to generate a list of transformations!!!
 
 Like this:
 ```php
 transformations = transf_gen.transf_gen(verbose=True,
@@ -528,14 +538,15 @@
 <a id="applyrir"></a>
 ### [⬆️](#available-augmentations) ApplyRIR
 ```php
 # Use this to see available materials you can use as walls_mat, floor_mat and ceiling_mat argument
 # from AudioAugmentor import rir_setup
 # rir_setup.get_all_materials_info()
 
+# This way you set up parameters when you want to generate random room parameter
 rir_kwargs = {
     'audio_sample_rate': 16000,
     'x_range': (0, 100), 
     'y_range': (0, 100), 
     'num_vertices_range': (3, 6),
     'mic_height': 1.5,
     'source_height': 1.5,
@@ -543,14 +554,28 @@
     'room_height': 2.0,
     'max_order': 3,
     'floor_mat': 'carpet_cotton',
     'ceiling_mat': 'hard_surface',
     'ray_tracing': True,
     'air_absorption': True,
 }
+# This way you set up parameters when you want to generate specific room
+rir_kwargs = {
+    'audio_sample_rate': 16000,
+    'corners_coord': [[0, 0], [0, 3], [5, 3], [5, 1], [3, 1], [3, 0]],
+    'walls_mat': 'curtains_cotton_0.5',
+    'room_height': 2.0,
+    'max_order': 3,
+    'floor_mat': 'carpet_cotton',
+    'ceiling_mat': 'hard_surface',
+    'ray_tracing': True,
+    'air_absorption': True,
+    'source_coord': [[1.0], [1.0], [0.5]],
+    'microphones_coord': [[3.5], [2.0], [0.5]],
+}
 transformations = transf_gen.transf_gen(verbose=True,
                                         ApplyRIR=rir_kwargs,
                                         )
 ```
 <a id="sevenbandparametriceq"></a>
 ### [⬆️](#available-augmentations) SevenBandParametricEQ [docs](https://iver56.github.io/audiomentations/waveform_transforms/seven_band_parametric_eq/)
 ```python
```

### Comparing `audioaugmentor-0.0.6/README.md` & `audioaugmentor-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,24 @@
 # Load test wav file
 signal, fs = torchaudio.load('../data/test.wav')
 # Apply transformations
 waveform = augment(signal.numpy()[0])
 display(Audio(waveform, rate=fs))
 ```
 
+**c)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `AugmentLocalAudioDataset` class and apply the augmentations to the local audio dataset.
+```php
+augment = core.AugmentLocalAudioDataset(
+    transformations=transformations, device='cpu', sox_effects=None, sample_rate=16000, verbose=False,
+    #transformations=None, device='cpu', sox_effects='--sox="norm gain 20 highpass 300 phaser 0.5 0.6 1 0.45 0.6 -s" amr audio_bitrate 4.75k', sample_rate=16000, verbose=False,
+    #transformations=None, device='cpu', sox_effects=sox_file_content, sample_rate=16000, verbose=False,
+)
+augment(input_dir='../data/test-input-folder', output_dir='../data/test-output-folder')
+```
+
 
 # EXAMPLES OF AVAILABLE AUGMENTATIONS
 ## !!!Put following examples as an argument for `transf_gen.transf_gen` function to generate a list of transformations!!!
 
 Like this:
 ```php
 transformations = transf_gen.transf_gen(verbose=True,
@@ -458,14 +468,15 @@
 <a id="applyrir"></a>
 ### [⬆️](#available-augmentations) ApplyRIR
 ```php
 # Use this to see available materials you can use as walls_mat, floor_mat and ceiling_mat argument
 # from AudioAugmentor import rir_setup
 # rir_setup.get_all_materials_info()
 
+# This way you set up parameters when you want to generate random room parameter
 rir_kwargs = {
     'audio_sample_rate': 16000,
     'x_range': (0, 100), 
     'y_range': (0, 100), 
     'num_vertices_range': (3, 6),
     'mic_height': 1.5,
     'source_height': 1.5,
@@ -473,14 +484,28 @@
     'room_height': 2.0,
     'max_order': 3,
     'floor_mat': 'carpet_cotton',
     'ceiling_mat': 'hard_surface',
     'ray_tracing': True,
     'air_absorption': True,
 }
+# This way you set up parameters when you want to generate specific room
+rir_kwargs = {
+    'audio_sample_rate': 16000,
+    'corners_coord': [[0, 0], [0, 3], [5, 3], [5, 1], [3, 1], [3, 0]],
+    'walls_mat': 'curtains_cotton_0.5',
+    'room_height': 2.0,
+    'max_order': 3,
+    'floor_mat': 'carpet_cotton',
+    'ceiling_mat': 'hard_surface',
+    'ray_tracing': True,
+    'air_absorption': True,
+    'source_coord': [[1.0], [1.0], [0.5]],
+    'microphones_coord': [[3.5], [2.0], [0.5]],
+}
 transformations = transf_gen.transf_gen(verbose=True,
                                         ApplyRIR=rir_kwargs,
                                         )
 ```
 <a id="sevenbandparametriceq"></a>
 ### [⬆️](#available-augmentations) SevenBandParametricEQ [docs](https://iver56.github.io/audiomentations/waveform_transforms/seven_band_parametric_eq/)
 ```python
```

### Comparing `audioaugmentor-0.0.6/pyproject.toml` & `audioaugmentor-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["AudioAugmentor"]
 
 [project]
 name = "AudioAugmentor"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python package for simple application of wide range of audio augmentations."
 readme = "README.md"
 authors = [{ name = "Ladislav Vašina", email = "ladislavvasina@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

