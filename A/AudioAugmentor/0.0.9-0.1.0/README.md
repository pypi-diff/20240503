# Comparing `tmp/audioaugmentor-0.0.9.tar.gz` & `tmp/audioaugmentor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioaugmentor-0.0.9.tar", last modified: Fri May  3 17:38:30 2024, max compression
+gzip compressed data, was "audioaugmentor-0.1.0.tar", last modified: Fri May  3 18:05:01 2024, max compression
```

## Comparing `audioaugmentor-0.0.9.tar` & `audioaugmentor-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/AudioAugmentor/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.9/AudioAugmentor/__init__.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34021 2024-05-03 16:35:00.000000 audioaugmentor-0.0.9/AudioAugmentor/core.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.9/AudioAugmentor/rir_setup.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4846 2024-05-03 16:35:24.000000 audioaugmentor-0.0.9/AudioAugmentor/sox_parser.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.9/AudioAugmentor/torchaudio_transf_wrapper.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 16:35:07.000000 audioaugmentor-0.0.9/AudioAugmentor/transf_gen.py
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/AudioAugmentor.egg-info/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/SOURCES.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/dependency_links.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/requires.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 17:38:30.000000 audioaugmentor-0.0.9/AudioAugmentor.egg-info/top_level.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.9/LICENSE
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    32597 2024-05-03 14:34:45.000000 audioaugmentor-0.0.9/README.md
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 17:32:11.000000 audioaugmentor-0.0.9/pyproject.toml
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 17:38:30.202767 audioaugmentor-0.0.9/setup.cfg
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 18:05:01.623200 audioaugmentor-0.1.0/
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 18:05:01.622200 audioaugmentor-0.1.0/AudioAugmentor/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.1.0/AudioAugmentor/__init__.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    33762 2024-05-03 17:47:13.000000 audioaugmentor-0.1.0/AudioAugmentor/core.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.1.0/AudioAugmentor/rir_setup.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4846 2024-05-03 16:35:24.000000 audioaugmentor-0.1.0/AudioAugmentor/sox_parser.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3741 2024-05-03 17:48:32.000000 audioaugmentor-0.1.0/AudioAugmentor/torchaudio_transf_wrapper.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 16:35:07.000000 audioaugmentor-0.1.0/AudioAugmentor/transf_gen.py
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 18:05:01.622200 audioaugmentor-0.1.0/AudioAugmentor.egg-info/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 18:05:01.000000 audioaugmentor-0.1.0/AudioAugmentor.egg-info/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 18:05:01.000000 audioaugmentor-0.1.0/AudioAugmentor.egg-info/SOURCES.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 18:05:01.000000 audioaugmentor-0.1.0/AudioAugmentor.egg-info/dependency_links.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 18:05:01.000000 audioaugmentor-0.1.0/AudioAugmentor.egg-info/requires.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 18:05:01.000000 audioaugmentor-0.1.0/AudioAugmentor.egg-info/top_level.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.1.0/LICENSE
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    35848 2024-05-03 18:05:01.623200 audioaugmentor-0.1.0/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    32597 2024-05-03 14:34:45.000000 audioaugmentor-0.1.0/README.md
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 18:04:28.000000 audioaugmentor-0.1.0/pyproject.toml
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 18:05:01.623200 audioaugmentor-0.1.0/setup.cfg
```

### Comparing `audioaugmentor-0.0.9/AudioAugmentor/core.py` & `audioaugmentor-0.1.0/AudioAugmentor/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,14 @@
                         transform = torch_randomizer(
                             getattr(TTW, currently_used_trasnf)(**transform[tmp]), p=p)
                         if transform is None:
                             continue
 
                     transform = transform.to(self.device)
                     waveform = torch.from_numpy(waveform).float().to(self.device)
-                    print(waveform.device, self.device, transform)
                     waveform = waveform.unsqueeze(0)
                     waveform = transform(waveform)
                     if isinstance(waveform, tuple):
                         waveform = waveform[0]
                     waveform = waveform.detach().cpu().numpy()
                     waveform = waveform.squeeze(0)
 
@@ -591,15 +590,14 @@
                                         orig_freq=fs, new_freq=self.sample_rate)(loaded_tensor_with_codec)
                         finally:
                             # Delete the temporary output file
                             os.remove(tmp_output_path)
 
                         data = loaded_tensor_with_codec.unsqueeze(
                             0).to(self.device)
-                        # print(f'POST:{data}, {data.shape}, {data.dtype}')
 
                     elif transform.__class__.__name__ == 'ApplyRIR':
                         x = transform.audio_sample_rate
                         if isinstance(x, dict):
                             transform = rir_setup.ApplyRIR(**x)
                         else:
                             transform = rir_setup.ApplyRIR(**x())
@@ -687,22 +685,20 @@
 
         # Pad all samples to new max_length
         if SPECTR_USED:
             for i, (data, *rest) in enumerate(transformed_batch):
                 if data.size(2) < spectr_max_length:
                     data = torch.nn.functional.pad(
                         data, (0, spectr_max_length - data.size(2)))
-                    # print(f'POST-PADDING:{data.shape}')
                     transformed_batch[i] = (data, *rest)
         else:
             for i, (data, *rest) in enumerate(transformed_batch):
                 if data.size(2) < max_length:
                     data = torch.nn.functional.pad(
                         data, (0, max_length - data.size(2)))
-                    # print(f'POST-PADDING:{data.shape}')
                     transformed_batch[i] = (data, *rest)
 
         return torch.utils.data.dataloader.default_collate(transformed_batch)
 
 
 class AugmentLocalAudioDataset:
     def __init__(
```

### Comparing `audioaugmentor-0.0.9/AudioAugmentor/rir_setup.py` & `audioaugmentor-0.1.0/AudioAugmentor/rir_setup.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.9/AudioAugmentor/sox_parser.py` & `audioaugmentor-0.1.0/AudioAugmentor/sox_parser.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.9/AudioAugmentor/torchaudio_transf_wrapper.py` & `audioaugmentor-0.1.0/AudioAugmentor/torchaudio_transf_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 def randomize_parameters(**kwargs):
     '''
     Get parameters in form [min, max, steps] and return randomized values
     Args: 
         **kwargs: Arguments of the augmentations with paramaters in form [min, max, steps]
     Returns: 
         randomized_values (dict): Dictionary of randomized parameters.
-
     '''
 
     randomized_values = {}
     for param, values in kwargs.items():
         if isinstance(values, list):
             param_values = np.arange(values[0], values[1], values[2])
             randomized_value = choice(param_values)
@@ -35,15 +34,15 @@
 def vol(
         gain,
         gain_type='amplitude'
 ):
     '''
     Wrapper for torchaudio.transforms.Vol
     https://pytorch.org/audio/main/generated/torchaudio.transforms.Vol.html
-    
+
     Args:
         gain (list): Gain in form [min, max, steps] - RANDOMIZABLE
         gain_type (str): Type of gain - One of: amplitude, power, db (Default: amplitude)
 
     Returns:
         torchaudio.transforms.Vol - Volume transfomation from the torchaudio library with randomized parameters.
     '''
```

### Comparing `audioaugmentor-0.0.9/AudioAugmentor/transf_gen.py` & `audioaugmentor-0.1.0/AudioAugmentor/transf_gen.py`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.9/AudioAugmentor.egg-info/PKG-INFO` & `audioaugmentor-0.1.0/AudioAugmentor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioaugmentor-0.0.9/LICENSE` & `audioaugmentor-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.9/PKG-INFO` & `audioaugmentor-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioaugmentor-0.0.9/README.md` & `audioaugmentor-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `audioaugmentor-0.0.9/pyproject.toml` & `audioaugmentor-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["AudioAugmentor"]
 
 [project]
 name = "AudioAugmentor"
-version = "0.0.9"
+version = "0.1.0"
 description = "Python package for simple application of wide range of audio augmentations."
 readme = "README.md"
 authors = [{ name = "Ladislav Vašina", email = "ladislavvasina@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

