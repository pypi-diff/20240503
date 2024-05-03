# Comparing `tmp/AudioAugmentor-0.0.5.tar.gz` & `tmp/audioaugmentor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AudioAugmentor-0.0.5.tar", last modified: Mon Mar 11 17:25:44 2024, max compression
+gzip compressed data, was "audioaugmentor-0.0.6.tar", last modified: Fri May  3 12:48:59 2024, max compression
```

## Comparing `AudioAugmentor-0.0.5.tar` & `audioaugmentor-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-03-11 17:25:44.754950 AudioAugmentor-0.0.5/
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-03-11 17:25:44.751950 AudioAugmentor-0.0.5/AudioAugmentor/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 AudioAugmentor-0.0.5/AudioAugmentor/__init__.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    33130 2024-03-11 17:25:20.000000 AudioAugmentor-0.0.5/AudioAugmentor/core.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    16203 2024-03-11 09:23:54.000000 AudioAugmentor-0.0.5/AudioAugmentor/rir_setup.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4792 2024-03-11 17:25:30.000000 AudioAugmentor-0.0.5/AudioAugmentor/sox_parser.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3587 2024-03-04 13:38:05.000000 AudioAugmentor-0.0.5/AudioAugmentor/torchaudio_transf_wrapper.py
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    14978 2024-03-11 17:25:27.000000 AudioAugmentor-0.0.5/AudioAugmentor/transf_gen.py
-drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-03-11 17:25:44.752950 AudioAugmentor-0.0.5/AudioAugmentor.egg-info/
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34538 2024-03-11 17:25:44.000000 AudioAugmentor-0.0.5/AudioAugmentor.egg-info/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-03-11 17:25:44.000000 AudioAugmentor-0.0.5/AudioAugmentor.egg-info/SOURCES.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-03-11 17:25:44.000000 AudioAugmentor-0.0.5/AudioAugmentor.egg-info/dependency_links.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-03-11 17:25:44.000000 AudioAugmentor-0.0.5/AudioAugmentor.egg-info/requires.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-03-11 17:25:44.000000 AudioAugmentor-0.0.5/AudioAugmentor.egg-info/top_level.txt
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 AudioAugmentor-0.0.5/LICENSE
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34538 2024-03-11 17:25:44.753950 AudioAugmentor-0.0.5/PKG-INFO
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)    31308 2024-03-11 17:24:36.000000 AudioAugmentor-0.0.5/README.md
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2076 2024-03-11 17:25:10.000000 AudioAugmentor-0.0.5/pyproject.toml
--rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-03-11 17:25:44.754950 AudioAugmentor-0.0.5/setup.cfg
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 12:48:59.690087 audioaugmentor-0.0.6/AudioAugmentor/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        0 2024-03-03 18:59:40.000000 audioaugmentor-0.0.6/AudioAugmentor/__init__.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    33659 2024-05-03 12:48:31.000000 audioaugmentor-0.0.6/AudioAugmentor/core.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    15834 2024-05-03 07:14:40.000000 audioaugmentor-0.0.6/AudioAugmentor/rir_setup.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     4928 2024-05-03 12:48:51.000000 audioaugmentor-0.0.6/AudioAugmentor/sox_parser.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     3746 2024-05-03 07:03:31.000000 audioaugmentor-0.0.6/AudioAugmentor/torchaudio_transf_wrapper.py
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    12953 2024-05-03 12:48:42.000000 audioaugmentor-0.0.6/AudioAugmentor/transf_gen.py
+drwxr-xr-x   0 lvasina   (1000) lvasina   (1000)        0 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/AudioAugmentor.egg-info/
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34542 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      401 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/SOURCES.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)        1 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/dependency_links.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)      436 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/requires.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       15 2024-05-03 12:48:59.000000 audioaugmentor-0.0.6/AudioAugmentor.egg-info/top_level.txt
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     1076 2024-03-03 15:53:56.000000 audioaugmentor-0.0.6/LICENSE
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    34542 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/PKG-INFO
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)    31291 2024-05-03 08:00:35.000000 audioaugmentor-0.0.6/README.md
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)     2097 2024-05-03 12:44:38.000000 audioaugmentor-0.0.6/pyproject.toml
+-rw-r--r--   0 lvasina   (1000) lvasina   (1000)       38 2024-05-03 12:48:59.691087 audioaugmentor-0.0.6/setup.cfg
```

### Comparing `AudioAugmentor-0.0.5/AudioAugmentor/core.py` & `audioaugmentor-0.0.6/AudioAugmentor/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 import numpy as np
 import torch
 import torchaudio
 import torchaudio.io as TIO
 import audiomentations as AA
 import torch_audiomentations as TA
 import torchaudio.transforms as T
+import shutil
+from pathlib import Path
+from glob import glob
+from scipy.io.wavfile import read, write
 from datasets.formatting.formatting import LazyRow
-from random import random
+import random
 
 # Build pip package with this uncommented
 from . import torchaudio_transf_wrapper as TTW
 from .transf_gen import T_TRANSF, TTW_TRANSF, get_transf
 from .sox_parser import select_random_sox, parse
 from . import rir_setup
 
@@ -48,15 +52,15 @@
     """
 
     if transformation is None:
         raise ValueError('Transformation must be specified!')
     if (p < 0) or (p > 1):
         raise ValueError('Probability p must be in range [0, 1]!')
 
-    if random() < p:
+    if random.random() < p:
         return transformation
     else:
         return None
 
 
 def apply_g726(tmp_input_path, tmp_output_path, audio_bitrate):
     """
@@ -65,14 +69,15 @@
         tmp_input_path (str): Path to the input file.
         tmp_output_path (str): Path to the output file.
         audio_bitrate (int): Audio bitrate of the output file.
 
     Returns:
         None
     """
+
     (
         ffmpeg
         .input(tmp_input_path)
         .output(
             tmp_output_path,
             acodec='g726',
             audio_bitrate=audio_bitrate,
@@ -163,15 +168,14 @@
             fd, tmp_output_path = tempfile.mkstemp(
                 suffix=suffix)
             loaded_tensor_with_codec = None
             tmp_input_path = None
             try:
                 # Create temporary file for the input
                 with tempfile.NamedTemporaryFile(delete=False, suffix='.wav') as tmp_input:
-                    # print('saving',data.to('cpu').shape, tmp_input.name)
                     torchaudio.save(
                         tmp_input.name, data.to(
                             'cpu'), sample_rate
                     )
                     tmp_input_path = tmp_input.name
                     with os.fdopen(fd, 'w') as tmp:
                         if sox_effects_to_apply[1][0] == 'g726':
@@ -202,21 +206,18 @@
                             tmp_output_path)
                         loaded_tensor_with_codec = T.Resample(
                             orig_freq=fs, new_freq=sample_rate)(loaded_tensor_with_codec)
             finally:
                 # Delete the temporary output file
                 os.remove(tmp_output_path)
             data = loaded_tensor_with_codec
-            # print(data.shape)
 
         else:
-            # print('APPLYING CODEC', sox_effects_to_apply[1][0])
             data = TIO.AudioEffector(format="wav", encoder=sox_effects_to_apply[1][0]).apply(
                 data.cpu().transpose(0, 1), sample_rate).transpose(0, 1).cpu()
-            # print(data.shape)
 
     return data
 
 
 class AugmentWaveform:
     def __init__(
         self,
@@ -298,15 +299,14 @@
                         np.expand_dims(waveform, axis=1).transpose(0, 1)
                     )
                     waveform = transform.apply(
                         transposed_waveform_tensor, self.sample_rate
                     ).transpose(0, 1).squeeze(0).numpy()
 
                 elif isinstance(transform, tuple):
-                    # print(f'PRE:{waveform}, {waveform.shape}, {waveform.dtype}')
                     data = torch.from_numpy(waveform).float()
                     suffix = None
                     if transform[0] == 'g726':
                         suffix = '.wav'
                     elif transform[0] == 'gsm':
                         suffix = '.gsm'
                     elif transform[0] == 'amr':
@@ -349,15 +349,14 @@
                                     orig_freq=fs, new_freq=self.sample_rate)(loaded_tensor_with_codec)
                     finally:
                         # Delete the temporary output file
                         os.remove(tmp_output_path)
 
                     waveform = loaded_tensor_with_codec.unsqueeze(
                         0).cpu().numpy().squeeze(0).squeeze(0)
-                    # print(f'POST:{waveform}, {waveform.shape}, {waveform.dtype}')
                 elif transform.__class__.__module__.split('.')[0] == 'torchaudio' or isinstance(transform, dict):
                     if isinstance(transform, dict):
                         tmp = next(iter(transform))
                         p = transform['p']
                         currently_used_trasnf = get_transf(tmp, TTW_TRANSF)
                         transform = torch_randomizer(
                             getattr(TTW, currently_used_trasnf)(**transform[tmp]), p=p)
@@ -375,17 +374,16 @@
                     waveform = torch.from_numpy(waveform).float()
                     waveform = waveform.unsqueeze(0).unsqueeze(0)
                     waveform = transform(waveform).detach().numpy()
                     waveform = waveform.squeeze(0).squeeze(0)
 
         # @@@@@@@@@@@@@@@@@@@@@@@@ SOX EFFECTS PART OF THE CODE @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
         if self.sox_effects is not None:
-            if self.device == 'cuda' and data.is_cuda:
-                print('WARNING: sox_effects are not supported on cuda!')
-                data = data.cpu()
+            if self.device == 'cuda':
+                print('WARNING: sox_effects are not supported on cuda!\n\t Using cpu.')
             # check if waveform is torch.tensor, if not convert it to torch.tensor
             if not isinstance(waveform, torch.Tensor):
                 waveform = torch.from_numpy(waveform).float().unsqueeze(0)
 
             if isinstance(self.sox_effects, str):
                 sox_effects_to_apply = parse(self.sox_effects)
                 # Check if sox_effects is a list of lists --> single effect, input already parsed by sox_parer
@@ -418,15 +416,15 @@
 
             # Convert waveform back from tensor
             waveform = waveform.squeeze(0).detach().numpy()
 
         return waveform
 
 
-class CollateFunction:
+class Collator:
     def __init__(
         self,
         transformations=None,
         device=None,
         sox_effects=None,
         sample_rate=None,
         verbose=False,
@@ -452,15 +450,15 @@
             device ('cpu' or 'cuda'): The device to which the data should be moved.
             sox_effects (list): List of lists, where inner lists contain sox effects with their parameters.
                                 Use sox_parser component to generate this list.
             sample_rate (int): Sampling rate on which the input data are sampled.
             verbose (bool): If True, print the current transformation being applied.
 
         Returns:
-            CollateFunction: Collate function which can be used within PyTorch's DataLoader.
+            Collator: Collate function which can be used within PyTorch's DataLoader.
         '''
 
         if transformations is None and sox_effects is None:
             raise ValueError(
                 'At least one of transformations or sox_effects must be specified!')
         if transformations is not None and sox_effects is not None:
             raise ValueError(
@@ -488,15 +486,14 @@
         transformed_batch = []
         max_length = max(x[0].size(0) if x[0].dim() ==
                          1 else x[0].size(1) for x in batch)
 
         SPECTR_USED = False
         spectr_max_length = 0
         for item in batch:
-            # print(f'ITEM: {item}')
             data, *rest = item
             # Add dimension
             data = data.unsqueeze(0)
             # Shape of the data at this point is [1, 1, 1605] (1605 is randomly chosen)
             # Apply all transformations from the transfomations chain
             if self.transformations is not None:
                 # Move the data to the selected device
@@ -536,17 +533,14 @@
                         # Effect on data is [1, 1, 1605] -> [1, 1605] -> [1605, 1] -> [1, 1605] -> [1, 1, 1605]
                         data = transform.apply(
                             data.cpu().squeeze(0).transpose(0, 1), self.sample_rate
                         ).transpose(0, 1).unsqueeze(0).to(self.device)
 
                     # This branch handles applying codecs using ffmpeg
                     elif isinstance(transform, tuple):
-                        # print('APPLYING CODEC')
-                        # print(transform, transform[0], transform[1])
-                        # print(f'PRE:{data}, {data.shape}, {data.dtype}')
                         suffix = None
                         if transform[0] == 'g726':
                             suffix = '.wav'
                         elif transform[0] == 'gsm':
                             suffix = '.gsm'
                         elif transform[0] == 'amr':
                             suffix = '.amr'
@@ -594,63 +588,59 @@
 
                         data = loaded_tensor_with_codec.unsqueeze(
                             0).to(self.device)
                         # print(f'POST:{data}, {data.shape}, {data.dtype}')
 
                     elif transform.__class__.__name__ == 'ApplyRIR':
                         x = transform.audio_sample_rate
-                        transform = rir_setup.ApplyRIR(**x())
+                        if isinstance(x, dict):
+                            transform = rir_setup.ApplyRIR(**x)
+                        else:
+                            transform = rir_setup.ApplyRIR(**x())
+
                         data = torch.from_numpy(
                             transform(data)).unsqueeze(0).unsqueeze(0).to(self.device)
-                        # print(f'POST:{data}, {data.shape}, {data.dtype}')
                     else:
-                        # print(f'PRE:{data}, {data.shape}, {data.dtype}')
                         # Check if transform is Speed from torchaudio - needs specific handling,
                         # for some reason it returns tuple, we want to get only augmented data
                         if transform.__class__.__name__ == 'Speed':
                             data = transform(data)[0]
                         elif (
                             transform.__class__.__name__ == 'Spectrogram' or
                             transform.__class__.__name__ == 'MelSpectrogram' or
                             transform.__class__.__name__ == 'TimeMasking' or
                             transform.__class__.__name__ == 'FrequencyMasking'
                         ):
-                            # print(f'PRE:{data}, {data.shape}, {data.dtype}')
                             data = transform(data[0])
-                            # print(f'POST:{data}, {data.shape}, {data.dtype}')
                             if (
                                 transform.__class__.__name__ == 'TimeMasking' or
                                 transform.__class__.__name__ == 'FrequencyMasking'
                             ):
                                 data = data.unsqueeze(0)
                             SPECTR_USED = True
 
                             # Check if spectr_max_length should be changed
                             if data.size(2) > spectr_max_length:
                                 spectr_max_length = data.size(2)
 
                         else:
-                            # print(f'PRE:{data}, {data.shape}, {data.dtype}')
                             data = transform(data)
-                            # print(f'POST:{data}, {data.shape}, {data.dtype}')
-                        # print(f'POST:{data}, {data.shape}, {data.dtype}')
                     # Check that only tensor was returned, if not make it a tensor
                     # This is done because some transforms return a tuple of (tensor, something)
                     if not isinstance(data, torch.Tensor):
                         data = data[0]
                     # Check if max_length has been changed
                     if data.size(2) > max_length:
                         max_length = data.size(2)
 
             # @@@@@@@@@@@@@@@@@@@@@@@@ SOX EFFECTS PART OF THE CODE @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
             if self.sox_effects is not None:
                 if self.device == 'cuda' and data.is_cuda:
-                    print('WARNING: sox_effects are not supported on cuda!')
+                    print('WARNING: sox_effects are not supported on cuda!\n\t Using cpu.')
                     data = data.cpu()
-                # print(f'DATA BEFORE SOX EFFECTS:{data}')
 
                 if isinstance(self.sox_effects, str):
                     sox_effects_to_apply = parse(self.sox_effects)
                     # Check if sox_effects is a list of lists --> single effect, input already parsed by sox_parer
                     if (isinstance(sox_effects_to_apply[0], list) and
                             all(isinstance(sublist, list)
                                 for sublist in sox_effects_to_apply[0])
@@ -668,30 +658,30 @@
                 # Check if sox_effects is a list of strings --> multiple effects -->
                 # --> needs to be parsed by sox_parser and some effect needs to be randomly chosen and applied
                 elif (isinstance(self.sox_effects, list) and
                       all(isinstance(sublist, str)
                           for sublist in self.sox_effects)
                       ):
                     random_sox = select_random_sox(self.sox_effects)
-
+                    print(
+                        f'CURRENT SOX THE IS BEIGN APPLIED: {random_sox}') if self.verbose else None
                     data, _ = torchaudio.sox_effects.apply_effects_tensor(
                         data.squeeze(0),
                         self.sample_rate,
                         random_sox[0]
                     )
                     if random_sox[1]:
                         data = sox_codec_handler(
                             random_sox, data, self.sample_rate)
                     data = data.unsqueeze(0)
 
             # DATA AFTER SOX EFFECTS: torch.Size([1, 1, 225600])
             data = data.detach()
             transformed_batch.append((data, *rest))
 
-        # print(f'PRE-PADDING:{data.shape}')
         # Pad all samples to new max_length
         if SPECTR_USED:
             for i, (data, *rest) in enumerate(transformed_batch):
                 if data.size(2) < spectr_max_length:
                     data = torch.nn.functional.pad(
                         data, (0, spectr_max_length - data.size(2)))
                     # print(f'POST-PADDING:{data.shape}')
@@ -700,16 +690,61 @@
             for i, (data, *rest) in enumerate(transformed_batch):
                 if data.size(2) < max_length:
                     data = torch.nn.functional.pad(
                         data, (0, max_length - data.size(2)))
                     # print(f'POST-PADDING:{data.shape}')
                     transformed_batch[i] = (data, *rest)
 
-        # print(f'TRANSFORMED BATCH: \n{transformed_batch}')
-        # print(f'lenght: {len(transformed_batch)}')
-        # print(f'type: {type(transformed_batch)}')
-        # print(f'\nDEFAULT_COLLATE: \n{torch.utils.data.dataloader.default_collate(transformed_batch)}\n')
-        # print(f'lenght: {len(torch.utils.data.dataloader.default_collate(transformed_batch))}')
-        # print(f'shape: {torch.utils.data.dataloader.default_collate(transformed_batch)}')
-        # print(f'type: {type(torch.utils.data.dataloader.default_collate(transformed_batch))}')
-        # print('#'*50)
         return torch.utils.data.dataloader.default_collate(transformed_batch)
+
+
+class AugmentLocalAudioDataset:
+    def __init__(
+        self,
+        transformations=None,
+        device=None,
+        sox_effects=None,
+        sample_rate=None,
+        verbose=False,
+    ):
+        self.transformations = transformations
+        self.device = device
+        self.sox_effects = sox_effects
+        self.sample_rate = sample_rate
+        self.verbose = verbose
+        
+        self.augment_waveform = AugmentWaveform(
+            transformations=self.transformations,
+            device=self.device,
+            sox_effects=self.sox_effects,
+            sample_rate=self.sample_rate,
+            verbose=self.verbose,
+        )
+    """
+    This is a wrapper class for AugmentWaveform class and it enables to augment local audio datasets.
+    """
+
+    def __call__(self, input_dir: str, output_dir: str):
+        # Ensure output directory exists
+        output_dir_path = Path(output_dir)
+        output_dir_path.mkdir(parents=True, exist_ok=True)
+
+        # Iterate over all files in the input directory
+        for file in Path(input_dir).glob('*'):
+            if file.is_file():
+                # Load the audio file
+                loaded_file_extension = str(file).split(".")[-1]
+                if loaded_file_extension not in ('wav', 'flac', 'ogg', 'mp3', 'aac', 'opus', 'm4a', 'wma', 'ac3'):
+                    raise ValueError(
+                        f'File {file} has unsupported extension {loaded_file_extension}. Only .wav and .flac files are supported.'
+                    )
+                tensor, sample_rate = torchaudio.load(str(file))
+                waveform = tensor[0].numpy()
+
+                # Apply transformations
+                transformed_waveform = self.augment_waveform(waveform)
+                # Save the transformed audio to the output directory
+                output_file = output_dir_path / file.name
+                write(str(output_file), sample_rate, transformed_waveform)
+
+                if self.verbose:
+                    print(f"Processed file: {file.name}")
```

### Comparing `AudioAugmentor-0.0.5/AudioAugmentor/rir_setup.py` & `audioaugmentor-0.0.6/AudioAugmentor/rir_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 File containg class that handles generating room impulse responses (RIRs) and applying them to the data.
 
 @author: Ladislav Vašina, github: LadislavVasina1
 """
 
-
 import pyroomacoustics as pra
 import torch
 import audiomentations as AA
 import torchaudio.transforms as T
 import numpy as np
 import matplotlib.pyplot as plt
 import itertools
@@ -67,34 +66,36 @@
         p1: List, containing the coordinates of the first point.
         p2: List, containing the coordinates of the second point.
         p3: List, containing the coordinates of the third point.
     
     Returns:
         area == 0: Boolean, True if the points are collinear, False otherwise.
     '''
+
     area = (
         p1[0]*(p2[1] - p3[1]) + 
         p2[0]*(p3[1] - p1[1]) + 
         p3[0]*(p1[1] - p2[1])
     )
     return area == 0
 
 
-def generate_random_convex_polygon(num_vertices, x_range=(0, 10), y_range=(0, 10)):
+def generate_random_polygon(num_vertices, x_range=(0, 10), y_range=(0, 10)):
     '''
-    This function generates a random convex polygon with a given number of vertices.
+    This function generates a random polygon with a given number of vertices.
 
     Args:
         num_vertices: Integer, number of vertices of the polygon.
         x_range: Tuple of two integers, range of x coordinates for the polygon.
         y_range: Tuple of two integers, range of y coordinates for the polygon.
     
     Returns:
         points: List of lists, containing the coordinates of the polygon vertices.
     '''
+
     # Initialize the set of points
     points_set = set()
 
     # Generate unique points
     while len(points_set) < num_vertices:
         # Generate a random angle
         angle = np.random.rand() * 2 * pi
@@ -181,14 +182,15 @@
     microphone_coordinates = generate_random_point_in_polygon(polygon)
     
     while speaker_coordinates == microphone_coordinates:
         microphone_coordinates = generate_random_point_in_polygon(polygon)
         
     return speaker_coordinates, microphone_coordinates
 
+
 def generate_number_of_rooms_with_speaker_and_microphone_coordinates(num_rooms, x_range, y_range, num_vertices_range):
     '''
     This function generates a given number of rooms with random speaker and microphone coordinates.
 
     Args:
         num_rooms: Integer, number of rooms to generate.
         x_range: Tuple of two integers, range of x coordinates for the rooms.
@@ -198,15 +200,15 @@
     Returns:
         rooms: List of tuples, containing the coordinates of the room vertices, speaker coordinates and microphone coordinates.
     '''
     
     rooms = []
     for _ in range(num_rooms):
         num_vertices = random.randint(*num_vertices_range)
-        polygon = generate_random_convex_polygon(num_vertices, x_range, y_range)
+        polygon = generate_random_polygon(num_vertices, x_range, y_range)
         speaker_coordinates, microphone_coordinates = generate_speaker_and_microphone_coordinates(polygon)
         rooms.append((polygon, speaker_coordinates, microphone_coordinates))
     return rooms
 
 
 def create_random_rir_kwargs(
         x_range,
@@ -264,18 +266,20 @@
             'source_coord': selected_source,
             'microphones_coord': selected_mics,
         }
         rir_kwargs_list.append(rir_kwargs)
 
     return rir_kwargs_list[0]
 
+
 class RandomRIRKwargs:
     '''
     Wrapper class around create_random_rir_kwargs function.
     '''
+
     def __init__(
         self,
         x_range,
         y_range,
         num_vertices_range,
         mic_height,
         source_height,
@@ -352,15 +356,18 @@
         key, value = item
         print(f'\t{key}:')
 
         for key, value in value.items():
             print(f'\t\t{key}: {value}')
     print('@'*79)
 
+
 class ApplyRIR:
+    """This class applies room impulse response (RIR) to the input audio signal."""
+
     def __init__(
         self,
         audio_sample_rate=None,
         corners_coord=None,
         walls_mat=None,
         room_height=None,
         floor_mat=None,
@@ -385,47 +392,35 @@
         self.ray_tracing = ray_tracing
         self.air_absorption = air_absorption
         # All coordintes must be in form [[x], [y], [z]] or [[x1, x2, ...], [y1, y2, ...], [z1, z2, ...]]
         self.source_coord = source_coord
         self.microphones_coord = microphones_coord
 
     def __call__(self, waveform):
-        #print all initial variables of the ApplyRIR class
-        # print(f'AUDIO SAMPLE RATE: {self.audio_sample_rate}')
-        # print(f'CORNERS COORD: {self.corners_coord}')
-        # print(f'WALLS MAT: {self.walls_mat}')
-        # print(f'ROOM HEIGHT: {self.room_height}')
-        # print(f'FLOOR MAT: {self.floor_mat}')
-        # print(f'CEILING MAT: {self.ceiling_mat}')
-        # print(f'MAX ORDER: {self.max_order}')
-        # print(f'RAY TRACING: {self.ray_tracing}')
-        # print(f'AIR ABSORPTION: {self.air_absorption}')
-        # print(f'SOURCE COORD: {self.source_coord}')
-        # print(f'MICROPHONES COORD: {self.microphones_coord}')
-    
-
-        # print(f'INITIAL DEVICE: {waveform.device}')
         # Handle device and if waveform is in the form of torch.Tensor convert it to NumPy format
+        SAMPLE_RATE_HAS_CHANGED = False
+
         if isinstance(waveform, torch.Tensor):
             initial_wav_type = waveform.dtype
             initial_device = waveform.device
             if waveform.is_cuda:
                 waveform = waveform.squeeze(0).squeeze(0).cpu()
             elif waveform.is_cpu:
                 waveform = waveform.squeeze(0).squeeze(0)
 
         elif isinstance(waveform, np.ndarray):
             initial_wav_type = waveform.dtype
 
         if not (self.audio_sample_rate == self.core_sample_rate):
+            SAMPLE_RATE_HAS_CHANGED = True
             if isinstance(waveform, torch.Tensor):
                 waveform = T.Resample(self.audio_sample_rate,
                                     self.core_sample_rate)(waveform)
             else:
-                waveform = AA.Resample(min_sample_rate=self.core_sample_rate, max_sample_rate=self.core_sample_rate, p=1.0)(waveform)
+                waveform = AA.Resample(min_sample_rate=self.core_sample_rate, max_sample_rate=self.core_sample_rate, p=1.0)(waveform, self.audio_sample_rate)
 
         room = pra.Room.from_corners(
             self.corners_coord,
             fs=self.core_sample_rate,
             max_order=self.max_order,
             materials=pra.Material(self.walls_mat),
             ray_tracing=self.ray_tracing,
@@ -467,17 +462,19 @@
         # fig.set_size_inches(5, 3)
 
         room.simulate()
         waveform = room.mic_array.signals[0, :]
         del(room)
         waveform = waveform.astype(np.float32)
 
-
         if initial_wav_type == torch.Tensor:
             waveform = torch.from_numpy(waveform)
-            # waveform = T.Resample(self.core_sample_rate,
-            #                       self.audio_sample_rate)(waveform)
             waveform = waveform.unsqueeze(0).unsqueeze(0).to(initial_device)
 
-        # print(f'FINAL SHAPE: {waveform.shape}')
-        # print(f'FINAL TYPE: {type(waveform)}')
+        if SAMPLE_RATE_HAS_CHANGED:
+            if isinstance(waveform, torch.Tensor):
+                waveform = T.Resample(self.core_sample_rate,
+                                      self.audio_sample_rate)(waveform)
+            else:
+                waveform = AA.Resample(min_sample_rate=self.audio_sample_rate, max_sample_rate=self.audio_sample_rate, p=1.0)(waveform, self.core_sample_rate)
+
         return waveform
```

### Comparing `AudioAugmentor-0.0.5/AudioAugmentor/sox_parser.py` & `audioaugmentor-0.0.6/AudioAugmentor/sox_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-File containing functions that parse pseudo-sox commands into lists of arguments
+File containing functions that parse pseudo-sox commands into lists of arguments.
 
 @author: Ladislav Vašina, github: LadislavVasina1
 """
 
 import torch
 import torchaudio
 import torchaudio.transforms as T
@@ -12,15 +12,15 @@
 # Build pip package with this uncommented
 from .transf_gen import CODECS
 
 # Test sources with this uncommented
 # from transf_gen import CODECS
 
 EFFECTS_NAMES = torchaudio.sox_effects.effect_names()
-example_sox = '--sox="norm gain 0 highpass 1000 phaser 0.5 0.6 1 0.45 0.6 -s"'
+# example_sox = '--sox="norm gain 0 highpass 1000 phaser 0.5 0.6 1 0.45 0.6 -s"'
 
 
 def load_sox_file(file_path):
     """
     This function reads file containing pseudo-sox commands
     on each line and returns a list of lines from the file.
     This function also ignores lines starting with #
@@ -138,18 +138,20 @@
         file_path: path to the file containing pseudo-sox commands
         verbose: if True, prints the loaded lines and the chosen sox command
     Returns:
         chosen_sox_cmd: a list of arguments for the chosen sox command
     """
 
     with open(file_path, 'r') as file:
-        lines = file.readlines()
+        sox_file_content = file.readlines()
+        sox_file_content = [line for line in sox_file_content if not line.strip().startswith('#')]
+
 
-    chosen_sox_cmd = choice(lines)
+    chosen_sox_cmd = choice(sox_file_content)
 
     if verbose:
         print('Loaded lines:')
-        for line in lines:
+        for line in sox_file_content:
             print(line.replace('\n', ''))
         print(f'\nChosen sox command: \n{chosen_sox_cmd}')
     
     return chosen_sox_cmd
```

### Comparing `AudioAugmentor-0.0.5/AudioAugmentor/torchaudio_transf_wrapper.py` & `audioaugmentor-0.0.6/AudioAugmentor/torchaudio_transf_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Get parameters in form [min, max, steps] and return randomized values
     Args: 
         **kwargs: Arguments of the augmentations with paramaters in form [min, max, steps]
     Returns: 
         randomized_values (dict): Dictionary of randomized parameters.
 
     '''
+
     randomized_values = {}
     for param, values in kwargs.items():
         if isinstance(values, list):
             param_values = np.arange(values[0], values[1], values[2])
             randomized_value = choice(param_values)
             randomized_values[param] = randomized_value
         else:
@@ -33,15 +34,16 @@
 
 def vol(
         gain,
         gain_type='amplitude'
 ):
     '''
     Wrapper for torchaudio.transforms.Vol
-
+    https://pytorch.org/audio/main/generated/torchaudio.transforms.Vol.html
+    
     Args:
         gain (list): Gain in form [min, max, steps] - RANDOMIZABLE
         gain_type (str): Type of gain - One of: amplitude, power, db (Default: amplitude)
 
     Returns:
         torchaudio.transforms.Vol - Volume transfomation from the torchaudio library with randomized parameters.
     '''
@@ -52,14 +54,15 @@
 
 def speed(
         orig_freq,
         factor
 ):
     '''
     Wrapper for torchaudio.transforms.Speed
+    https://pytorch.org/audio/main/generated/torchaudio.transforms.Speed.html
 
     Args:
         orig_freq (int): Original frequency of the audio
         factor (list): Factor of the speed change in form [min, max, steps] - RANDOMIZABLE
 
     Returns:
         torchaudio.transforms.Speed - Speed transfomation from the torchaudio library with randomized parameters.
```

### Comparing `AudioAugmentor-0.0.5/AudioAugmentor/transf_gen.py` & `audioaugmentor-0.0.6/AudioAugmentor/transf_gen.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-File containing functions that generate transformations from the user input
+File containing functions that generate transformations from the user input.
 
 @author: Ladislav Vašina, github: LadislavVasina1
 """
 
 import torch
 import torchaudio
 import torchaudio.transforms as T
@@ -87,15 +87,15 @@
     'PeakingFilter',            # https://iver56.github.io/audiomentations/waveform_transforms/peaking_filter/
     'SevenBandParametricEQ',    # https://iver56.github.io/audiomentations/waveform_transforms/seven_band_parametric_eq/
     'TanhDistortion',           # https://iver56.github.io/audiomentations/waveform_transforms/tanh_distortion/
     'TimeStretch',              # https://iver56.github.io/audiomentations/waveform_transforms/time_stretch/
 ]
 
 # Codecs should be used as last augmentation method.
-# Only exception is using SpecAugment, in that cas SpecAugment should be used as last method.
+# Only exception is using SpecAugment, in that case SpecAugment should be used as last method.
 CODECS = [
     "ac3",              # torchaudio
     "adpcm_ima_wav",    # ---| |----
     "adpcm_ms",         # ---| |----
     "adpcm_yamaha",     # ---| |----
     "eac3",             # ---| |----
     "flac",             # ---| |----
@@ -136,14 +136,15 @@
     Returns:
         specific transformation from the list of available transformations listed above
         or None if the transformation is not in the list
 
     This function takes user input and returns the name of the transformation.
     It can handle user input in any case (for better UX) and returns the name of the transformation.
     '''
+
     user_input_lower = user_input.lower()
     for item in list_of_transformations:
         if item.lower() == user_input_lower:
             return item
     return None
 
 
@@ -169,15 +170,19 @@
         aa_flag = get_transf(key, AA_TRANSF) in AA_TRANSF
         codec_flag = get_transf(key, CODECS) in CODECS
 
         # Handle list input of the transformation parameters
         match key:
             # Handle transformations from PYROOMACOUSTICS
             case key if pra_flag:
-                rir_kwargs = RandomRIRKwargs(**value)
+                random_rir_kwargs_unique_keys = ['x_range', 'y_range', 'num_vertices_range', 'mic_height']
+                if any(key in value for key in random_rir_kwargs_unique_keys):
+                    rir_kwargs = RandomRIRKwargs(**value)
+                else:
+                    rir_kwargs = value
                 transformations.append(
                     eval(get_transf(key, PRA_TRANSF))(rir_kwargs)
                 )
                 verbose_out(key, value, PRA_TRANSF) if verbose else None
 
             # Handle transformations from TORCH_AUDIOMENTATIONS
             case key if ta_flag:
@@ -191,25 +196,20 @@
                 transformations.append(
                     getattr(AA, get_transf(key, AA_TRANSF))(**value)
                 )
                 verbose_out(key, value, AA_TRANSF) if verbose else None
 
             # Handle transformations from TORCHAUDIO
             case key if t_flag:
-                # print(get_transf(key, TTW_TRANSF))
                 # check if values contain "p" key
                 if 'p' in value.keys():
                     # save the p value and delete it from value dictionary
                     p = value['p']
                     del value['p']
                     transformations.append(
-                        # core.torch_randomizer(
-                        #     getattr(TTW, get_transf(key, TTW_TRANSF))(**value),
-                        #     p=p
-                        # )
                         {get_transf(key, TTW_TRANSF): {**value}, 'p': p}
                     )
 
                 elif 'p' not in value.keys():
                     transformations.append(
                         getattr(T, get_transf(key, T_TRANSF))(**value)
                     )
@@ -251,50 +251,7 @@
     # Verbose out
     print(
         f'\n\nFINAL TRANSFORMATIONS LIST:\n' +
         '\n'.join(str(transformation) for transformation in transformations)
     ) if verbose else None
 
     return transformations
-
-
-# rir_kwargs = {
-#     'audio_sample_rate': 16000,
-#     'x_range': (0, 100),
-#     'y_range': (0, 100),
-#     'num_vertices_range': (3, 6),
-#     'mic_height': 1.5,
-#     'source_height': 1.5,
-#     'walls_mat': 'curtains_cotton_0.5',
-#     'room_height': 2.0,
-#     'max_order': 3,
-#     'floor_mat': 'carpet_cotton',
-#     'ceiling_mat': 'hard_surface',
-#     'ray_tracing': True,
-#     'air_absorption': True,
-# }
-# transformations = transf_gen(verbose=True,
-#                              ApplyRIR=rir_kwargs,
-#                              Vol={'gain': [0.9, 1.5, 0.1],
-#                                   'p': 0.9},
-#                             #  PitchShift={'sample_rate': 16000,
-#                             #              'n_steps': [-1, 1, 0.1],
-#                             #              'p': 0.9},
-#                             #  Speed={'orig_freq': 16000,
-#                             #         'factor': [0.9, 1.1, 0.1],
-#                             #         'p': 0.9},
-#                             #  speed='orig_freq=16000, factor=0.9',
-#                             #  Mp3Compression={'min_bitrate': 8,
-#                             #                  'max_bitrate': 64,
-#                             #                  'backend': 'pydub',
-#                             #                  'p': 1},
-#                              #    TimeInversion='p=1, sample_rate=16000',
-#                              #    TimeMasking='time_mask_param=80',
-#                              #    FrequencyMasking='freq_mask_param=80',
-#                             #  TimeInversion={'p': 1, 'sample_rate': 16000},
-#                             #  pcm_alaw=True,
-#                             #  MelSpectrogram={'sample_rate': 16000},
-#                             #  TimeMasking={'time_mask_param': 80},
-#                             #  FrequencyMasking={'freq_mask_param': 80},
-#                             #  g726={'audio_bitrate': '40k'},
-#                             #  gsm=True,
-#                              )
```

### Comparing `AudioAugmentor-0.0.5/AudioAugmentor.egg-info/PKG-INFO` & `audioaugmentor-0.0.6/AudioAugmentor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,17 +20,17 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/LadislavVasina1/AudioAugmentor
-Project-URL: Repository, https://github.com/LadislavVasina1/AudioAugmentor
-Project-URL: Issues, https://github.com/LadislavVasina1/AudioAugmentor/issues
+Project-URL: Homepage, https://github.com/LadislavVasina1/AudioAugmentor_public
+Project-URL: Repository, https://github.com/LadislavVasina1/AudioAugmentor_public
+Project-URL: Issues, https://github.com/LadislavVasina1/AudioAugmentor_public/issues
 Keywords: audio,augmentation,pytorch,machine learning,deep learning,data augmentation,audio processing,audio augmentation,audio data augmentation,audio data processing,torchaudio,ffmpeg,ffmpeg-python,audiomentations,torch-audiomentations,RIR,room impulse response,room simulation,pyroomacoustics
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -123,15 +123,15 @@
 | [Time inversion](#time-inversion)                                    |                 |           ✅          |            |                 |        |
 | [ApplyRIR (RoomSimulator)](#applyrir)                                |                 |                       |            |        ✅       |        |
 | [SevenBandParametricEQ](#sevenbandparametriceq)                      |       ✅        |                       |            |                 |        |
 | [Shift](#shift)                                                      |                 |           ✅          |            |                 |        |
 | [Speed](#speed)                                                      |                 |                       |     ✅     |                 |        |
 | [Spectrogram](#spectrogram)                                          |                 |                       |     ✅     |                 |        |
 | [TanhDistortion](#tanhdistortion)                                    |       ✅        |                       |            |                 |        |
-| [TimeMasking](#timemasking)                                             |                 |                       |     ✅     |                 |        |
+| [TimeMasking](#timemasking)                                          |                 |                       |     ✅     |                 |        |
 | [TimeStretch](#timestretch)                                          |       ✅        |                       |            |                 |        |
 | [ac3](#codecs-using-torchaudio)                                      |                 |                       |     ✅     |                 |        |
 | [adpcm_ima_wav](#codecs-using-torchaudio)                            |                 |                       |     ✅     |                 |        |
 | [adpcm_ms](#codecs-using-torchaudio)                                 |                 |                       |     ✅     |                 |        |
 | [adpcm_yamaha](#codecs-using-torchaudio)                             |                 |                       |     ✅     |                 |        |
 | [eac3](#codecs-using-torchaudio)                                     |                 |                       |     ✅     |                 |        |
 | [flac](#codecs-using-torchaudio)                                     |                 |                       |     ✅     |                 |        |
@@ -235,19 +235,19 @@
 print('SOX FILE LOADED:', sox_file_content, type(sox_file_content))
 ```
 
 
 
 **3. Apply augmentations**
 
-**a)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `CollateFunction` class. 
+**a)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `Collator` class. 
 
 Use this initiated class as an argument for the `collate_fn` parameter of PyTorch's dataloader.
 ```php
-collate_fn = core.CollateFunction(
+collate_fn = core.Collator(
     transformations=transformations, device='cpu', sox_effects=None, sample_rate=sampling_rate, verbose=True,
     #transformations=None, device='cpu', sox_effects='--sox="norm gain 20 highpass 300 phaser 0.5 0.6 1 0.45 0.6 -s" amr audio_bitrate 4.75k', sample_rate=sampling_rate, verbose=False,
     #transformations=None, device='cpu', sox_effects=sox_file_content, sample_rate=sampling_rate, verbose=False,
 )
 
 dataset = torchaudio.datasets.LIBRISPEECH("../data", url="train-clean-100", download=True)
 aug_dataloader = torch.utils.data.DataLoader(
```

### Comparing `AudioAugmentor-0.0.5/LICENSE` & `audioaugmentor-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AudioAugmentor-0.0.5/PKG-INFO` & `audioaugmentor-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAugmentor
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for simple application of wide range of audio augmentations.
 Author-email: Ladislav Vašina <ladislavvasina@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ladislav Vašina]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,17 +20,17 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/LadislavVasina1/AudioAugmentor
-Project-URL: Repository, https://github.com/LadislavVasina1/AudioAugmentor
-Project-URL: Issues, https://github.com/LadislavVasina1/AudioAugmentor/issues
+Project-URL: Homepage, https://github.com/LadislavVasina1/AudioAugmentor_public
+Project-URL: Repository, https://github.com/LadislavVasina1/AudioAugmentor_public
+Project-URL: Issues, https://github.com/LadislavVasina1/AudioAugmentor_public/issues
 Keywords: audio,augmentation,pytorch,machine learning,deep learning,data augmentation,audio processing,audio augmentation,audio data augmentation,audio data processing,torchaudio,ffmpeg,ffmpeg-python,audiomentations,torch-audiomentations,RIR,room impulse response,room simulation,pyroomacoustics
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -123,15 +123,15 @@
 | [Time inversion](#time-inversion)                                    |                 |           ✅          |            |                 |        |
 | [ApplyRIR (RoomSimulator)](#applyrir)                                |                 |                       |            |        ✅       |        |
 | [SevenBandParametricEQ](#sevenbandparametriceq)                      |       ✅        |                       |            |                 |        |
 | [Shift](#shift)                                                      |                 |           ✅          |            |                 |        |
 | [Speed](#speed)                                                      |                 |                       |     ✅     |                 |        |
 | [Spectrogram](#spectrogram)                                          |                 |                       |     ✅     |                 |        |
 | [TanhDistortion](#tanhdistortion)                                    |       ✅        |                       |            |                 |        |
-| [TimeMasking](#timemasking)                                             |                 |                       |     ✅     |                 |        |
+| [TimeMasking](#timemasking)                                          |                 |                       |     ✅     |                 |        |
 | [TimeStretch](#timestretch)                                          |       ✅        |                       |            |                 |        |
 | [ac3](#codecs-using-torchaudio)                                      |                 |                       |     ✅     |                 |        |
 | [adpcm_ima_wav](#codecs-using-torchaudio)                            |                 |                       |     ✅     |                 |        |
 | [adpcm_ms](#codecs-using-torchaudio)                                 |                 |                       |     ✅     |                 |        |
 | [adpcm_yamaha](#codecs-using-torchaudio)                             |                 |                       |     ✅     |                 |        |
 | [eac3](#codecs-using-torchaudio)                                     |                 |                       |     ✅     |                 |        |
 | [flac](#codecs-using-torchaudio)                                     |                 |                       |     ✅     |                 |        |
@@ -235,19 +235,19 @@
 print('SOX FILE LOADED:', sox_file_content, type(sox_file_content))
 ```
 
 
 
 **3. Apply augmentations**
 
-**a)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `CollateFunction` class. 
+**a)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `Collator` class. 
 
 Use this initiated class as an argument for the `collate_fn` parameter of PyTorch's dataloader.
 ```php
-collate_fn = core.CollateFunction(
+collate_fn = core.Collator(
     transformations=transformations, device='cpu', sox_effects=None, sample_rate=sampling_rate, verbose=True,
     #transformations=None, device='cpu', sox_effects='--sox="norm gain 20 highpass 300 phaser 0.5 0.6 1 0.45 0.6 -s" amr audio_bitrate 4.75k', sample_rate=sampling_rate, verbose=False,
     #transformations=None, device='cpu', sox_effects=sox_file_content, sample_rate=sampling_rate, verbose=False,
 )
 
 dataset = torchaudio.datasets.LIBRISPEECH("../data", url="train-clean-100", download=True)
 aug_dataloader = torch.utils.data.DataLoader(
```

### Comparing `AudioAugmentor-0.0.5/README.md` & `audioaugmentor-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 | [Time inversion](#time-inversion)                                    |                 |           ✅          |            |                 |        |
 | [ApplyRIR (RoomSimulator)](#applyrir)                                |                 |                       |            |        ✅       |        |
 | [SevenBandParametricEQ](#sevenbandparametriceq)                      |       ✅        |                       |            |                 |        |
 | [Shift](#shift)                                                      |                 |           ✅          |            |                 |        |
 | [Speed](#speed)                                                      |                 |                       |     ✅     |                 |        |
 | [Spectrogram](#spectrogram)                                          |                 |                       |     ✅     |                 |        |
 | [TanhDistortion](#tanhdistortion)                                    |       ✅        |                       |            |                 |        |
-| [TimeMasking](#timemasking)                                             |                 |                       |     ✅     |                 |        |
+| [TimeMasking](#timemasking)                                          |                 |                       |     ✅     |                 |        |
 | [TimeStretch](#timestretch)                                          |       ✅        |                       |            |                 |        |
 | [ac3](#codecs-using-torchaudio)                                      |                 |                       |     ✅     |                 |        |
 | [adpcm_ima_wav](#codecs-using-torchaudio)                            |                 |                       |     ✅     |                 |        |
 | [adpcm_ms](#codecs-using-torchaudio)                                 |                 |                       |     ✅     |                 |        |
 | [adpcm_yamaha](#codecs-using-torchaudio)                             |                 |                       |     ✅     |                 |        |
 | [eac3](#codecs-using-torchaudio)                                     |                 |                       |     ✅     |                 |        |
 | [flac](#codecs-using-torchaudio)                                     |                 |                       |     ✅     |                 |        |
@@ -165,19 +165,19 @@
 print('SOX FILE LOADED:', sox_file_content, type(sox_file_content))
 ```
 
 
 
 **3. Apply augmentations**
 
-**a)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `CollateFunction` class. 
+**a)** Use generated the `transformations` list, `single SoX command` or `loaded SoX file content` while initializing `Collator` class. 
 
 Use this initiated class as an argument for the `collate_fn` parameter of PyTorch's dataloader.
 ```php
-collate_fn = core.CollateFunction(
+collate_fn = core.Collator(
     transformations=transformations, device='cpu', sox_effects=None, sample_rate=sampling_rate, verbose=True,
     #transformations=None, device='cpu', sox_effects='--sox="norm gain 20 highpass 300 phaser 0.5 0.6 1 0.45 0.6 -s" amr audio_bitrate 4.75k', sample_rate=sampling_rate, verbose=False,
     #transformations=None, device='cpu', sox_effects=sox_file_content, sample_rate=sampling_rate, verbose=False,
 )
 
 dataset = torchaudio.datasets.LIBRISPEECH("../data", url="train-clean-100", download=True)
 aug_dataloader = torch.utils.data.DataLoader(
```

### Comparing `AudioAugmentor-0.0.5/pyproject.toml` & `audioaugmentor-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["AudioAugmentor"]
 
 [project]
 name = "AudioAugmentor"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python package for simple application of wide range of audio augmentations."
 readme = "README.md"
 authors = [{ name = "Ladislav Vašina", email = "ladislavvasina@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -78,10 +78,10 @@
     'py-heat-magic'
 ]
 
 requires-python = ">=3.10"
 
 
 [project.urls]
-Homepage = "https://github.com/LadislavVasina1/AudioAugmentor"
-Repository = "https://github.com/LadislavVasina1/AudioAugmentor"
-Issues = "https://github.com/LadislavVasina1/AudioAugmentor/issues"
+Homepage = "https://github.com/LadislavVasina1/AudioAugmentor_public"
+Repository = "https://github.com/LadislavVasina1/AudioAugmentor_public"
+Issues = "https://github.com/LadislavVasina1/AudioAugmentor_public/issues"
```

