# Comparing `tmp/accmt-1.0.1.tar.gz` & `tmp/accmt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accmt-1.0.1.tar", last modified: Sun Apr 28 20:23:18 2024, max compression
+gzip compressed data, was "accmt-1.0.2.tar", last modified: Thu May  2 22:07:14 2024, max compression
```

## Comparing `accmt-1.0.1.tar` & `accmt-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:23:18.255486 accmt-1.0.1/
--rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    13885 2024-04-28 20:23:18.251953 accmt-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    13146 2024-04-21 20:01:57.000000 accmt-1.0.1/README.md
--rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      841 2024-04-28 20:23:18.259494 accmt-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 20:23:18.136928 accmt-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-28 20:23:18.196157 accmt-1.0.1/src/accmt/
--rw-rw-rw-   0        0        0      552 2024-04-28 20:04:39.000000 accmt-1.0.1/src/accmt/__init__.py
--rw-rw-rw-   0        0        0    26896 2024-04-28 20:16:30.000000 accmt-1.0.1/src/accmt/accmt.py
--rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-1.0.1/src/accmt/collate_fns.py
--rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-1.0.1/src/accmt/config.py
--rw-rw-rw-   0        0        0      161 2024-04-28 04:10:32.000000 accmt-1.0.1/src/accmt/events.py
--rw-rw-rw-   0        0        0      345 2024-04-28 20:04:47.000000 accmt-1.0.1/src/accmt/loggers.py
--rw-rw-rw-   0        0        0     4524 2024-04-28 20:14:52.000000 accmt-1.0.1/src/accmt/optimizations.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:23:18.248947 accmt-1.0.1/src/accmt.egg-info/
--rw-rw-rw-   0        0        0    13885 2024-04-28 20:23:18.000000 accmt-1.0.1/src/accmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-28 20:23:18.000000 accmt-1.0.1/src/accmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:23:18.000000 accmt-1.0.1/src/accmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-28 20:23:18.000000 accmt-1.0.1/src/accmt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-28 20:23:18.000000 accmt-1.0.1/src/accmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.768036 accmt-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    14020 2024-05-02 22:07:14.766034 accmt-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13283 2024-05-02 22:06:41.000000 accmt-1.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      841 2024-05-02 22:07:14.770037 accmt-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.683153 accmt-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.729784 accmt-1.0.2/src/accmt/
+-rw-rw-rw-   0        0        0      552 2024-04-28 20:04:39.000000 accmt-1.0.2/src/accmt/__init__.py
+-rw-rw-rw-   0        0        0    26995 2024-05-02 22:06:16.000000 accmt-1.0.2/src/accmt/accmt.py
+-rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-1.0.2/src/accmt/collate_fns.py
+-rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-1.0.2/src/accmt/config.py
+-rw-rw-rw-   0        0        0      161 2024-04-28 04:10:32.000000 accmt-1.0.2/src/accmt/events.py
+-rw-rw-rw-   0        0        0      345 2024-04-28 20:04:47.000000 accmt-1.0.2/src/accmt/loggers.py
+-rw-rw-rw-   0        0        0     4524 2024-04-29 15:38:32.000000 accmt-1.0.2/src/accmt/optimizations.py
+drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.764014 accmt-1.0.2/src/accmt.egg-info/
+-rw-rw-rw-   0        0        0    14020 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/top_level.txt
```

### Comparing `accmt-1.0.1/LICENSE` & `accmt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `accmt-1.0.1/PKG-INFO` & `accmt-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,14 +16,16 @@
 Requires-Dist: numpy
 Requires-Dist: PyYAML
 Requires-Dist: accmt-cli
 
 # AcceleratorModule
 Module similar to Lightning Module for distributed training, but with Accelerator 🤗
 
+NOTE: Some features might not be tested and could cause problems. Feel free to open an issue or send a PR to fix any problem found.
+
 AcceleratorModule will take care of the heavy lifting of distributed training on many GPUs. Accelerate is quite simple, and it has many adventages over PyTorch Lightning, mainly because it doesn't abstract the low level part of the training loop, so you can customize it however you want. The main idea of this little project is to have a standard way to make distributed training. This module let's you:
 - Define the logic involved for training.
 - Define the logic involved for evaluation.
 - Save checkpoints to recover training progress.
 - Save best model by evaluating best average validation loss at the end of every epoch.
 - Define the hyperparameters in a simple YAML file.
 - Visualize training progress using TensorBoard (train and validation losses in one graph).
```

### Comparing `accmt-1.0.1/README.md` & `accmt-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # AcceleratorModule
 Module similar to Lightning Module for distributed training, but with Accelerator 🤗
 
+NOTE: Some features might not be tested and could cause problems. Feel free to open an issue or send a PR to fix any problem found.
+
 AcceleratorModule will take care of the heavy lifting of distributed training on many GPUs. Accelerate is quite simple, and it has many adventages over PyTorch Lightning, mainly because it doesn't abstract the low level part of the training loop, so you can customize it however you want. The main idea of this little project is to have a standard way to make distributed training. This module let's you:
 - Define the logic involved for training.
 - Define the logic involved for evaluation.
 - Save checkpoints to recover training progress.
 - Save best model by evaluating best average validation loss at the end of every epoch.
 - Define the hyperparameters in a simple YAML file.
 - Visualize training progress using TensorBoard (train and validation losses in one graph).
@@ -265,8 +267,8 @@
     loss = self.alpha * student_output.loss + (1. - self.alpha) * kd_loss
 
     return loss
 ```
 
 
 ## Notes
-I will continue to update this repository to add more features overtime. If you want to contribute to this little project, feel free to make a PR 🤗.
+I will continue to update this repository to add more features overtime. If you want to contribute to this little project, feel free to make a PR 🤗.
```

### Comparing `accmt-1.0.1/setup.cfg` & `accmt-1.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6363 6d74 0d0a 7665 7273 696f   = accmt..versio
-00000020: 6e20 3d20 312e 302e 310d 0a61 7574 686f  n = 1.0.1..autho
+00000020: 6e20 3d20 312e 302e 320d 0a61 7574 686f  n = 1.0.2..autho
 00000030: 7220 3d20 6768 616e 7665 7274 0d0a 6175  r = ghanvert..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6172  thor_email = mar
 00000050: 7469 6e2e 7069 7a61 7272 6f40 6365 6e69  tin.pizarro@ceni
 00000060: 612e 636c 0d0a 6465 7363 7269 7074 696f  a.cl..descriptio
 00000070: 6e20 3d20 4163 6365 6c65 7261 746f 7220  n = Accelerator 
 00000080: 4d6f 6475 6c65 2061 6e64 2054 7261 696e  Module and Train
 00000090: 6572 2062 6173 6564 206f 6e20 4163 6365  er based on Acce
```

### Comparing `accmt-1.0.1/src/accmt/__init__.py` & `accmt-1.0.2/src/accmt/__init__.py`

 * *Files identical despite different names*

### Comparing `accmt-1.0.1/src/accmt/accmt.py` & `accmt-1.0.2/src/accmt/accmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import torch
 
 from abc import ABC
 from accelerate import Accelerator
 from accelerate.utils import LoggerType, ProjectConfiguration, tqdm
+from .loggers import TensorBoard, MLFlow
 from .events import *
 from .config import read, save_status, read_status
 import torch.optim
 import torch.optim.lr_scheduler as lr_scheduler
 from torch.utils.data import Dataset
 from typing import Any
 from typing_extensions import override
@@ -166,15 +167,15 @@
                 checkpoint = "checkpoint1",
                 resume = False,
                 model_path: str = None,
                 model_saving = "best_valid_loss",
                 enable_checkpointing = True,
                 checkpoint_every = 1,
                 logging_dir = "logs",
-                log_with = LoggerType.TENSORBOARD,
+                log_with = TensorBoard,
                 log_every = 1,
                 grad_accumulation_steps=None,
                 set_to_none=True,
                 shuffle_train=True,
                 shuffle_validation=False,
                 model_saving_below_loss=float("inf"),
                 collate_fn=None,
@@ -204,16 +205,16 @@
             
             enable_checkpointing (`bool`, *optional*, defaults to `True`):
                 Whether to save checkpoint or not.
             checkpoint_every (`int`, *optional*, defaults to `1`):
                 Checkpoint every N steps. Only works if `enable_checkpointing` is set to `True`.
             logging_dir (`str`, *optional*, defaults to `logs`):
                 Path where to save logs to show progress.
-            log_with (`str`, *optional*, defaults to `LoggerType.TENSORBOARD`):
-                `LoggerType` to log progress.
+            log_with (`str`, *optional*, defaults to `accmt.TensorBoard`):
+                Logger to log metrics.
             log_every (`int`, *optional*, defaults to `1`):
                 Log every N steps.
             grad_accumulation_steps (`int`, *optional*, defaults to `None`):
                 Accumulate gradients for N steps. Useful for training large models and simulate
                 large batches when memory is not enough. If set to `None` or `1`, no accumulation will be perfomed.
             set_to_none (`bool`, *optional*, defaults to `True`):
                 From PyTorch documentation: "instead of setting to zero, set the grads to None. This will
@@ -244,28 +245,28 @@
         self.resume = resume
         self.model_path = model_path
         self.model_saving = model_saving.lower()
         self.enable_checkpointing = enable_checkpointing
         self.checkpoint_every = checkpoint_every
         self.logging_dir = logging_dir
         self.log_every = log_every
-        self.grad_accumulation_steps = grad_accumulation_steps if grad_accumulation_steps else 1
+        self.grad_accumulation_steps = grad_accumulation_steps if grad_accumulation_steps is not None else 1
         self.set_to_none = set_to_none
         self.shuffle_train = shuffle_train
         self.shuffle_validation = shuffle_validation
         self.model_saving_below_loss = model_saving_below_loss
         self.collate_fn = collate_fn
         self.max_shard_size = max_shard_size
         self.safe_serialization = safe_serialization
         self.optimizations = optimizations if optimizations is not None else []
 
         self.accelerator = accelerator
-        self.accelerator.gradient_accumulation_steps = grad_accumulation_steps
         self.accelerator.project_configuration = ProjectConfiguration(project_dir=".", logging_dir=logging_dir, total_limit=1)
-        self.accelerator.log_with = [log_with]
+        if not isinstance(log_with, list): log_with = [log_with]
+        self.accelerator.log_with = [logger.logger for logger in log_with]
 
     def fit(self,
             module: AcceleratorModule,
             train_dataset: Dataset,
             val_dataset: Dataset = None
     ):
         """
@@ -435,21 +436,22 @@
         if loss is None:
             loss = module.step(batch)
         self._apply_on_loss_optimizations(loss)
 
         if self.grad_accumulation_steps > 1:
             loss /= self.grad_accumulation_steps
 
-        train_losses.append(loss.item())
+        loss_item = loss.item()
+        train_losses.append(loss_item)
         if step % self.log_every == 0 and self.accelerator.is_main_process:
-            self.accelerator.log({"loss": {"train": loss}}, step=global_step)
+            self.accelerator.log({"train_loss": loss_item}, step=global_step)
         
         self._apply_before_backward_optimizations(self.model.parameters())
         self.accelerator.backward(loss)
-        self._apply_after_backward_optimizations(self.model.parameters())
+        #self._apply_after_backward_optimizations(self.model.parameters())
 
         if (step % self.grad_accumulation_steps == 0) or (step == len(dataloader)):
             optimizer.step()
             if scheduler is not None:
                 scheduler.step()
             optimizer.zero_grad(set_to_none=self.set_to_none)
 
@@ -459,17 +461,18 @@
         return global_step, current_epoch_step
     
     def _validation_logic(self, module, batch, eval_losses, step, eval_step, eval_global_step):
         loss = module.validation_step(batch)
         if loss is None:
             loss = module.step(batch)
 
-        eval_losses.append(loss.item())
+        loss_item = loss.item()
+        eval_losses.append(loss_item)
         if step % self.log_every == 0:
-            self.accelerator.log({"loss": {"valid": loss.item()}}, step=eval_global_step)
+            self.accelerator.log({"val_loss": loss_item}, step=eval_global_step)
 
         eval_global_step += eval_step
 
         return eval_global_step
 
     def _save_model(self, model, best_valid_loss, best_train_loss):
         state_dict = self.accelerator.get_state_dict(model)
```

### Comparing `accmt-1.0.1/src/accmt/collate_fns.py` & `accmt-1.0.2/src/accmt/collate_fns.py`

 * *Files identical despite different names*

### Comparing `accmt-1.0.1/src/accmt/optimizations.py` & `accmt-1.0.2/src/accmt/optimizations.py`

 * *Files identical despite different names*

### Comparing `accmt-1.0.1/src/accmt.egg-info/PKG-INFO` & `accmt-1.0.2/src/accmt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,14 +16,16 @@
 Requires-Dist: numpy
 Requires-Dist: PyYAML
 Requires-Dist: accmt-cli
 
 # AcceleratorModule
 Module similar to Lightning Module for distributed training, but with Accelerator 🤗
 
+NOTE: Some features might not be tested and could cause problems. Feel free to open an issue or send a PR to fix any problem found.
+
 AcceleratorModule will take care of the heavy lifting of distributed training on many GPUs. Accelerate is quite simple, and it has many adventages over PyTorch Lightning, mainly because it doesn't abstract the low level part of the training loop, so you can customize it however you want. The main idea of this little project is to have a standard way to make distributed training. This module let's you:
 - Define the logic involved for training.
 - Define the logic involved for evaluation.
 - Save checkpoints to recover training progress.
 - Save best model by evaluating best average validation loss at the end of every epoch.
 - Define the hyperparameters in a simple YAML file.
 - Visualize training progress using TensorBoard (train and validation losses in one graph).
```

