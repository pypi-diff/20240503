# Comparing `tmp/coqui-tts-trainer-0.1.0.tar.gz` & `tmp/coqui_tts_trainer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coqui-tts-trainer-0.1.0.tar", last modified: Thu Apr  4 14:53:39 2024, max compression
+gzip compressed data, was "coqui_tts_trainer-0.1.1.tar", last modified: Fri May  3 10:32:53 2024, max compression
```

## Comparing `coqui-tts-trainer-0.1.0.tar` & `coqui_tts_trainer-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:53:39.617112 coqui-tts-trainer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-04 14:53:39.617112 coqui-tts-trainer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:53:39.617112 coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-04 14:53:39.000000 coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-04 14:53:39.000000 coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:53:39.000000 coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:53:39.000000 coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 14:53:39.000000 coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 14:53:39.000000 coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 14:53:39.617112 coqui-tts-trainer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:53:39.609112 coqui-tts-trainer-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/tests/test_continue_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/tests/test_lr_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/tests/test_num_gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/tests/test_train_batch_size_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22755 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/tests/test_train_gan.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/tests/test_train_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:53:39.613113 coqui-tts-trainer-0.1.0/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/distribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:53:39.613113 coqui-tts-trainer-0.1.0/trainer/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/aim_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/base_dash_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/dummy_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/logging/wandb_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    89781 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/trainer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:53:39.617112 coqui-tts-trainer-0.1.0/trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/utils/cpu_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/utils/cuda_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-04 14:53:33.000000 coqui-tts-trainer-0.1.0/trainer/utils/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:32:53.076634 coqui_tts_trainer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-03 10:32:53.076634 coqui_tts_trainer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:32:53.072634 coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-03 10:32:53.000000 coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-03 10:32:53.000000 coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:32:53.000000 coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:32:52.000000 coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-03 10:32:53.000000 coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 10:32:53.000000 coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 10:32:53.076634 coqui_tts_trainer-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:32:53.068634 coqui_tts_trainer-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/tests/test_continue_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/tests/test_lr_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/tests/test_num_gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/tests/test_train_batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22683 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/tests/test_train_gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/tests/test_train_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:32:53.072634 coqui_tts_trainer-0.1.1/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:32:53.072634 coqui_tts_trainer-0.1.1/trainer/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/aim_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/base_dash_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/dummy_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/logging/wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89373 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/trainer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:32:53.072634 coqui_tts_trainer-0.1.1/trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/utils/cpu_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/utils/cuda_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-03 10:32:46.000000 coqui_tts_trainer-0.1.1/trainer/utils/distributed.py
```

### Comparing `coqui-tts-trainer-0.1.0/PKG-INFO` & `coqui_tts_trainer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coqui-tts-trainer
-Version: 0.1.0
+Version: 0.1.1
 Summary: General purpose model trainer for PyTorch that is more flexible than it should be, by 🐸Coqui.
 Home-page: https://github.com/idiap/coqui-ai-Trainer
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 Maintainer: Enno Hermann
 Maintainer-email: enno.hermann@gmail.com
 License: Apache2
@@ -27,30 +27,30 @@
 Requires-Dist: torch>=1.7
 Requires-Dist: coqpit
 Requires-Dist: psutil
 Requires-Dist: fsspec
 Requires-Dist: tensorboard
 Requires-Dist: soundfile
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: accelerate; extra == "dev"
 Provides-Extra: test
 Requires-Dist: torchvision; extra == "test"
 Provides-Extra: all
 Requires-Dist: torch>=1.7; extra == "all"
 Requires-Dist: coqpit; extra == "all"
 Requires-Dist: psutil; extra == "all"
 Requires-Dist: fsspec; extra == "all"
 Requires-Dist: tensorboard; extra == "all"
 Requires-Dist: soundfile; extra == "all"
-Requires-Dist: black; extra == "all"
+Requires-Dist: black==24.2.0; extra == "all"
 Requires-Dist: coverage; extra == "all"
 Requires-Dist: isort; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pylint; extra == "all"
 Requires-Dist: accelerate; extra == "all"
 Requires-Dist: torchvision; extra == "all"
```

### Comparing `coqui-tts-trainer-0.1.0/README.md` & `coqui_tts_trainer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/PKG-INFO` & `coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coqui-tts-trainer
-Version: 0.1.0
+Version: 0.1.1
 Summary: General purpose model trainer for PyTorch that is more flexible than it should be, by 🐸Coqui.
 Home-page: https://github.com/idiap/coqui-ai-Trainer
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 Maintainer: Enno Hermann
 Maintainer-email: enno.hermann@gmail.com
 License: Apache2
@@ -27,30 +27,30 @@
 Requires-Dist: torch>=1.7
 Requires-Dist: coqpit
 Requires-Dist: psutil
 Requires-Dist: fsspec
 Requires-Dist: tensorboard
 Requires-Dist: soundfile
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: accelerate; extra == "dev"
 Provides-Extra: test
 Requires-Dist: torchvision; extra == "test"
 Provides-Extra: all
 Requires-Dist: torch>=1.7; extra == "all"
 Requires-Dist: coqpit; extra == "all"
 Requires-Dist: psutil; extra == "all"
 Requires-Dist: fsspec; extra == "all"
 Requires-Dist: tensorboard; extra == "all"
 Requires-Dist: soundfile; extra == "all"
-Requires-Dist: black; extra == "all"
+Requires-Dist: black==24.2.0; extra == "all"
 Requires-Dist: coverage; extra == "all"
 Requires-Dist: isort; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pylint; extra == "all"
 Requires-Dist: accelerate; extra == "all"
 Requires-Dist: torchvision; extra == "all"
```

### Comparing `coqui-tts-trainer-0.1.0/coqui_tts_trainer.egg-info/SOURCES.txt` & `coqui_tts_trainer-0.1.1/coqui_tts_trainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/pyproject.toml` & `coqui_tts_trainer-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/setup.py` & `coqui_tts_trainer-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/tests/test_continue_train.py` & `coqui_tts_trainer-0.1.1/tests/test_continue_train.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/tests/test_lr_schedulers.py` & `coqui_tts_trainer-0.1.1/tests/test_lr_schedulers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/tests/test_num_gpus.py` & `coqui_tts_trainer-0.1.1/tests/test_num_gpus.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/tests/test_train_batch_size_finder.py` & `coqui_tts_trainer-0.1.1/tests/test_train_batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/tests/test_train_gan.py` & `coqui_tts_trainer-0.1.1/tests/test_train_gan.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,15 @@
     class GANModel(TrainerModel):
         def __init__(self):
             super().__init__()
             data_shape = (1, 28, 28)
             self.generator = Generator(latent_dim=100, img_shape=data_shape)
             self.discriminator = Discriminator(img_shape=data_shape)
 
-        def forward(self, x):
-            ...
+        def forward(self, x): ...
 
         def train_step(self, batch, criterion, optimizer_idx):
             imgs, _ = batch
 
             # sample noise
             z = torch.randn(imgs.shape[0], 100)
             z = z.type_as(imgs)
@@ -170,16 +169,15 @@
     class GANModel(TrainerModel):
         def __init__(self):
             super().__init__()
             data_shape = (1, 28, 28)
             self.generator = Generator(latent_dim=100, img_shape=data_shape)
             self.discriminator = Discriminator(img_shape=data_shape)
 
-        def forward(self, x):
-            ...
+        def forward(self, x): ...
 
         def train_step(self, batch, criterion, optimizer_idx):
             imgs, _ = batch
 
             # sample noise
             z = torch.randn(imgs.shape[0], 100)
             z = z.type_as(imgs)
@@ -267,16 +265,15 @@
     class GANModel(TrainerModel):
         def __init__(self):
             super().__init__()
             data_shape = (1, 28, 28)
             self.generator = Generator(latent_dim=100, img_shape=data_shape)
             self.discriminator = Discriminator(img_shape=data_shape)
 
-        def forward(self, x):
-            ...
+        def forward(self, x): ...
 
         def optimize(self, batch, trainer):
             imgs, _ = batch
 
             # sample noise
             z = torch.randn(imgs.shape[0], 100)
             z = z.type_as(imgs)
@@ -381,16 +378,15 @@
     class GANModel(TrainerModel):
         def __init__(self):
             super().__init__()
             data_shape = (1, 28, 28)
             self.generator = Generator(latent_dim=100, img_shape=data_shape)
             self.discriminator = Discriminator(img_shape=data_shape)
 
-        def forward(self, x):
-            ...
+        def forward(self, x): ...
 
         def optimize(self, batch, trainer):
             imgs, _ = batch
 
             # sample noise
             z = torch.randn(imgs.shape[0], 100)
             z = z.type_as(imgs)
@@ -498,19 +494,17 @@
     class GANModel(TrainerModel):
         def __init__(self):
             super().__init__()
             data_shape = (1, 28, 28)
             self.generator = Generator(latent_dim=100, img_shape=data_shape)
             self.discriminator = Discriminator(img_shape=data_shape)
 
-        def train_step():
-            ...
+        def train_step(): ...
 
-        def forward(self, x):
-            ...
+        def forward(self, x): ...
 
         def optimize(self, batch, trainer):
             imgs, _ = batch
 
             # sample noise
             z = torch.randn(imgs.shape[0], 100)
             z = z.type_as(imgs)
```

### Comparing `coqui-tts-trainer-0.1.0/trainer/callbacks.py` & `coqui_tts_trainer-0.1.1/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/distribute.py` & `coqui_tts_trainer-0.1.1/trainer/distribute.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/generic_utils.py` & `coqui_tts_trainer-0.1.1/trainer/generic_utils.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/io.py` & `coqui_tts_trainer-0.1.1/trainer/io.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/__init__.py` & `coqui_tts_trainer-0.1.1/trainer/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/aim_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/aim_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/base_dash_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/base_dash_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/clearml_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/console_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/console_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/dummy_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/dummy_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/mlflow_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/tensorboard_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/logging/wandb_logger.py` & `coqui_tts_trainer-0.1.1/trainer/logging/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/model.py` & `coqui_tts_trainer-0.1.1/trainer/model.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/torch.py` & `coqui_tts_trainer-0.1.1/trainer/torch.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/trainer.py` & `coqui_tts_trainer-0.1.1/trainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: utf-8 -*-
 import gc
 import importlib
 import logging
 import os
 import platform
 import shutil
 import sys
 import time
 import traceback
 from contextlib import nullcontext
 from dataclasses import dataclass, field
 from inspect import signature
-from typing import Callable, Dict, List, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 import torch.distributed as dist
 from coqpit import Coqpit
 from torch import nn
 from torch.nn.parallel import DistributedDataParallel as DDP_th
 from torch.utils.data import DataLoader
@@ -59,14 +58,15 @@
 if is_apex_available():
     from apex import amp  # pylint: disable=import-error
 
 
 @dataclass
 class TrainerConfig(Coqpit):
     """Config fields tweaking the Trainer for a model.
+
     A ````ModelConfig```, by inheriting ```TrainerConfig``` must be defined for using 👟.
     Inherit this by a new model config and override the fields as needed.
     All the fields can be overridden from comman-line as ```--coqpit.arg_name=value```.
 
     Example::
 
         Run the training code by overriding the ```lr``` and ```plot_step``` fields.
@@ -130,17 +130,15 @@
         default=10000, metadata={"help": "Save local checkpoint every save_step steps. Defaults to 10000"}
     )
     save_n_checkpoints: int = field(default=5, metadata={"help": "Keep n local checkpoints. Defaults to 5"})
     save_checkpoints: bool = field(default=True, metadata={"help": "Save checkpoints locally. Defaults to True"})
     save_all_best: bool = field(
         default=False, metadata={"help": "Save all best checkpoints and keep the older ones. Defaults to False"}
     )
-    save_best_after: int = field(
-        default=0, metadata={"help": "Wait N steps to save best checkpoints. Defaults to 0"}
-    )
+    save_best_after: int = field(default=0, metadata={"help": "Wait N steps to save best checkpoints. Defaults to 0"})
     target_loss: str = field(
         default=None, metadata={"help": "Target loss name to select the best model. Defaults to None"}
     )
     # Fields for eval and test run
     print_eval: bool = field(default=False, metadata={"help": "Print eval steps on the terminal. Defaults to False"})
     test_delay_epochs: int = field(default=0, metadata={"help": "Wait N epochs before running the test. Defaults to 0"})
     run_eval: bool = field(
@@ -302,16 +300,17 @@
         train_loader: DataLoader = None,
         eval_loader: DataLoader = None,
         training_assets: Dict = {},
         parse_command_line_args: bool = True,
         callbacks: Dict[str, Callable] = {},
         gpu: int = None,
     ) -> None:
-        """Simple yet powerful 🐸💬 TTS trainer for PyTorch. It can train all the available `tts` and `vocoder` models
-        or easily be customized.
+        """Simple yet powerful 🐸💬 TTS trainer for PyTorch.
+
+        It can train all the available `tts` and `vocoder` models or easily be customized.
 
         Notes:
 
             Supports Automatic Mixed Precision training. If `Apex` is availabe, it automatically picks that, else
             it uses PyTorch's native `amp` module. `Apex` may provide more stable training in some cases.
 
         Args:
@@ -517,17 +516,16 @@
 
         if self.use_cuda:
             self.model.cuda()
             if isinstance(self.criterion, list):
                 for criterion in self.criterion:
                     if isinstance(criterion, torch.nn.Module):
                         criterion.cuda()
-            else:
-                if isinstance(self.criterion, torch.nn.Module):
-                    self.criterion.cuda()
+            elif isinstance(self.criterion, torch.nn.Module):
+                self.criterion.cuda()
 
         # setup optimizer
         self.optimizer = self.get_optimizer(self.model, self.config)
 
         # If multiple-optimizer setup with grad accumulation and without custom optimize method raise an error
         if (
             self.grad_accum_steps != 1
@@ -577,29 +575,29 @@
         rank_zero_logger_info(f"\n > Model has {num_params} parameters", logger)
 
         self.callbacks.on_init_end(self)
         self.dashboard_logger.add_config(config)
         self.save_training_script()
 
     @property
-    def use_apex(self):
+    def use_apex(self) -> bool:
         """Return True if using APEX."""
         return not self.args.use_accelerate and self._is_apex_available()
 
     @property
-    def use_pt_ddp(self):
+    def use_pt_ddp(self) -> bool:
         """Return True if using PyTorch DDP."""
         return self.num_gpus > 1 and not self.use_accelerate
 
     @property
-    def use_accelerate(self):
+    def use_accelerate(self) -> bool:
         """Return True if using HF Accelerate."""
         return self.args.use_accelerate
 
-    def setup_accelerate(self):
+    def setup_accelerate(self) -> None:
         if self.use_accelerate:
             self.model, self.optimizer, self.train_loader, self.scheduler, self.accelerator = self.init_accelerate(
                 model=self.model,
                 optimizer=self.optimizer,
                 training_dataloader=self.train_loader,
                 scheduler=self.scheduler,
                 grad_accum_steps=self.grad_accum_steps,
@@ -653,15 +651,15 @@
             for i, sched in enumerate(scheduler):
                 scheduler[i] = accelerator.prepare_scheduler(sched)
         elif scheduler is not None:
             scheduler = accelerator.prepare_scheduler(scheduler)
 
         return model, optimizer, training_dataloader, scheduler, accelerator
 
-    def save_training_script(self):
+    def save_training_script(self) -> None:
         """Save the training script to tracking dashboard and output path."""
         file_path = sys.argv[0]
         if os.path.isfile(file_path):
             file_name = os.path.basename(file_path)
             self.dashboard_logger.add_artifact(file_or_dir=file_path, name=file_name, artifact_type="file")
             with open(file_path, "r", encoding="utf8") as f:
                 self.dashboard_logger.add_text("training-script", f"{f.read()}", 0)
@@ -678,14 +676,15 @@
         training_args, coqpit_overrides = parser.parse_known_args()
         args.parse_args(training_args)
         return args, coqpit_overrides
 
     @staticmethod
     def init_loggers(config: "Coqpit", output_path: str, dashboard_logger=None, c_logger=None):
         """Init console and dashboard loggers.
+
         Use the given logger if passed externally else use config values to pick the right logger.
         Return a dashboard logger only for the rank 0 process in DDP
         Define a console logger for each process in DDP
 
         Args:
             config (Coqpit): Model config.
             output_path (str): Output path to save the training artifacts.
@@ -700,24 +699,26 @@
         # only allow dashboard logging for the main process in DDP mode
         if get_rank() > 0:
             return DummyLogger(), c_logger
         if dashboard_logger is None:
             dashboard_logger = logger_factory(config, output_path)
         return dashboard_logger, c_logger
 
-    def setup_small_run(self, small_run: int = None):
+    def setup_small_run(self, small_run: Optional[int] = None) -> None:
         """Use a subset of samples for training, evaluation and testing."""
         if small_run is not None:
             logger.info("[!] Small Run, only using %i samples.", small_run)
             self.train_samples = None if self.train_samples is None else self.train_samples[:small_run]
             self.eval_samples = None if self.eval_samples is None else self.eval_samples[:small_run]
             self.test_samples = None if self.test_samples is None else self.test_samples[:small_run]
 
     @staticmethod
-    def init_training(args: TrainerArgs, coqpit_overrides: Dict, config: Coqpit = None):
+    def init_training(
+        args: TrainerArgs, coqpit_overrides: Dict, config: Coqpit = None
+    ) -> Tuple[Coqpit, Dict[str, str]]:
         """Initialize training and update model configs from command line arguments.
 
         Args:
             args (argparse.Namespace or dict like): Parsed trainer arguments.
             config_overrides (argparse.Namespace or dict like): Parsed config overriding arguments.
             config (Coqpit): Model config. If none, it is generated from `args`. Defaults to None.
 
@@ -747,15 +748,15 @@
         if args.rank == 0:
             if args.restore_path:
                 new_fields["restore_path"] = args.restore_path
             new_fields["github_branch"] = get_git_branch()
         return config, new_fields
 
     @staticmethod
-    def setup_training_environment(args, config, gpu):
+    def setup_training_environment(args, config, gpu) -> Tuple[bool, int]:
         if platform.system() != "Windows":
             # https://github.com/pytorch/pytorch/issues/973
             import resource  # pylint: disable=import-outside-toplevel
 
             rlimit = resource.getrlimit(resource.RLIMIT_NOFILE)
             resource.setrlimit(resource.RLIMIT_NOFILE, (4096, rlimit[1]))
 
@@ -882,15 +883,15 @@
     #########################
 
     def _get_loader(
         self,
         model: nn.Module,
         config: Coqpit,
         assets: Dict,
-        is_eval: str,
+        is_eval: bool,
         samples: List,
         verbose: bool,
         num_gpus: int,
     ) -> DataLoader:
         if num_gpus > 1:
             if isimplemented(model.module, "get_data_loader"):
                 loader = model.module.get_data_loader(
@@ -898,137 +899,124 @@
                     assets,
                     is_eval,
                     samples,
                     verbose,
                     num_gpus,
                     self.args.rank,
                 )
-        else:
-            if isimplemented(model, "get_data_loader"):
-                loader = model.get_data_loader(
-                    config=config, assets=assets, is_eval=is_eval, samples=samples, verbose=verbose, num_gpus=num_gpus
-                )
+        elif isimplemented(model, "get_data_loader"):
+            loader = model.get_data_loader(
+                config=config, assets=assets, is_eval=is_eval, samples=samples, verbose=verbose, num_gpus=num_gpus
+            )
 
         assert (
             len(loader) > 0
         ), " ❗ len(DataLoader) returns 0. Make sure your dataset is not empty or len(dataset) > 0. "
         return loader
 
     def get_train_dataloader(self, training_assets: Dict, samples: List, verbose: bool) -> DataLoader:
         """Initialize and return a training data loader.
+
         Call ```model.get_train_data_loader``` if it is implemented, else call ```model.get_data_loader```
         and set ```is_eval=False```.
 
         Args:
             ap (AudioProcessor): Audio processor.
             samples (List): Data samples used for training.
             verbose (bool): enable/disable printing loader stats at initialization.
 
         Returns:
             DataLoader: Initialized training data loader.
         """
         if self.num_gpus > 1:
             if isimplemented(self.model.module, "get_train_data_loader"):
-                loader = self.model.module.get_train_data_loader(
+                return self.model.module.get_train_data_loader(
                     self.config,
                     self.training_assets,
                     samples,
                     verbose,
                     self.num_gpus,
                     self.args.rank,
                 )
-                return loader
-        else:
-            if isimplemented(self.model, "get_train_data_loader"):
-                loader = self.model.get_train_data_loader(
-                    self.config, self.training_assets, samples, verbose, self.num_gpus
-                )
-                return loader
+        elif isimplemented(self.model, "get_train_data_loader"):
+            return self.model.get_train_data_loader(self.config, self.training_assets, samples, verbose, self.num_gpus)
 
         return self._get_loader(
             self.model,
             self.config,
             training_assets,
             False,
             samples,
             verbose,
             self.num_gpus,
         )
 
     def get_eval_dataloader(self, training_assets: Dict, samples: List, verbose: bool) -> DataLoader:
         """Initialize and return a evaluation data loader.
+
         Call ```model.get_eval_data_loader``` if it is implemented, else call ```model.get_data_loader```
         and set ```is_eval=True```.
 
         Args:
             ap (AudioProcessor): Audio processor.
             samples (List): Data samples used for training.
             verbose (bool): enable/disable printing loader stats at initialization.
 
         Returns:
             DataLoader: Initialized training data loader.
         """
         if self.num_gpus > 1:
             if isimplemented(self.model.module, "get_eval_data_loader"):
-                loader = self.model.module.get_eval_data_loader(
+                return self.model.module.get_eval_data_loader(
                     self.config,
                     self.training_assets,
                     samples,
                     verbose,
                     self.num_gpus,
                     self.args.rank,
                 )
-                return loader
-        else:
-            if isimplemented(self.model, "get_eval_data_loader"):
-                loader = self.model.get_eval_data_loader(
-                    self.config, self.training_assets, samples, verbose, self.num_gpus
-                )
-                return loader
+        elif isimplemented(self.model, "get_eval_data_loader"):
+            return self.model.get_eval_data_loader(self.config, self.training_assets, samples, verbose, self.num_gpus)
 
         return self._get_loader(
             self.model,
             self.config,
             training_assets,
             True,
             samples,
             verbose,
             self.num_gpus,
         )
 
     def get_test_dataloader(self, training_assets: Dict, samples: List, verbose: bool) -> DataLoader:
         """Initialize and return a evaluation data loader.
+
         Call ```model.get_test_data_loader``` if it is implemented, else call ```model.get_data_loader```
         and set ```is_eval=True```.
 
         Args:
             ap (AudioProcessor): Audio processor.
             samples (List): Data samples used for training.
             verbose (bool): enable/disable printing loader stats at initialization.
 
         Returns:
             DataLoader: Initialized training data loader.
         """
         if self.num_gpus > 1:
             if isimplemented(self.model.module, "get_test_data_loader"):
-                loader = self.model.module.get_test_data_loader(
+                return self.model.module.get_test_data_loader(
                     self.config,
                     self.training_assets,
                     samples,
                     verbose,
                     self.num_gpus,
                     self.args.rank,
                 )
-                return loader
-        else:
-            if isimplemented(self.model, "get_test_data_loader"):
-                loader = self.model.get_test_data_loader(
-                    self.config, self.training_assets, samples, verbose, self.num_gpus
-                )
-                return loader
+        elif isimplemented(self.model, "get_test_data_loader"):
+            return self.model.get_test_data_loader(self.config, self.training_assets, samples, verbose, self.num_gpus)
 
         return self._get_loader(
             self.model,
             self.config,
             training_assets,
             True,
             samples,
@@ -1086,18 +1074,17 @@
             optimizer: Target optimizer.
         """
         for group in optimizer.param_groups:
             yield from group["params"]
 
     @staticmethod
     def _model_train_step(
-        batch: Dict, model: nn.Module, criterion: nn.Module, optimizer_idx: int = None
+        batch: Dict, model: nn.Module, criterion: nn.Module, optimizer_idx: Optional[int] = None
     ) -> Tuple[Dict, Dict]:
-        """
-        Perform a trainig forward step. Compute model outputs and losses.
+        """Perform a trainig forward step. Compute model outputs and losses.
 
         Args:
             batch (Dict): [description]
             model (nn.Module): [description]
             criterion (nn.Module): [description]
             optimizer_idx (int, optional): [description]. Defaults to None.
 
@@ -1126,15 +1113,19 @@
                 else:
                     raise ValueError(f" ❗ Unknown precision {precision}")
         elif mixed_precision:
             dtype = torch.bfloat16
         return device, dtype
 
     def detach_loss_dict(
-        self, loss_dict: Dict, step_optimizer: bool, optimizer_idx: int = None, grad_norm: float = None
+        self,
+        loss_dict: Dict,
+        step_optimizer: bool,
+        optimizer_idx: Optional[int] = None,
+        grad_norm: Optional[float] = None,
     ):
         # detach losses for logging
         loss_dict_detached = self._detach_loss_dict(loss_dict)
         # loss_dict_detached["loss"] = loss_di`ct_detached["loss"] * float(self.grad_accum_steps)
 
         if optimizer_idx is not None:
             loss_dict_detached[f"loss_{optimizer_idx}"] = loss_dict_detached.pop("loss")
@@ -1187,15 +1178,15 @@
         batch: Dict,
         model: nn.Module,
         optimizer: torch.optim.Optimizer,
         scaler: "AMPScaler",
         criterion: nn.Module,
         scheduler: Union[torch.optim.lr_scheduler._LRScheduler, List, Dict],  # pylint: disable=protected-access
         config: Coqpit,
-        optimizer_idx: int = None,
+        optimizer_idx: Optional[int] = None,
         step_optimizer: bool = True,
         num_optimizers: int = 1,
     ) -> Tuple[Dict, Dict, int]:
         """Perform a forward - backward pass and run the optimizer.
 
         Args:
             batch (Dict): Input batch. If
@@ -1212,15 +1203,14 @@
 
         Raises:
             RuntimeError: When the loss is NaN.
 
         Returns:
             Tuple[Dict, Dict, int, torch.Tensor]: model outputs, losses, step time and gradient norm.
         """
-
         step_start_time = time.time()
 
         # forward pass and loss computation
         outputs, loss_dict = self._compute_loss(
             batch=batch, model=model, criterion=criterion, config=config, optimizer_idx=optimizer_idx
         )
 
@@ -1539,18 +1529,17 @@
         torch.cuda.empty_cache()
 
     #######################
     # EVAL FUNCTIONS
     #######################
 
     def _model_eval_step(
-        self, batch: Dict, model: nn.Module, criterion: nn.Module, optimizer_idx: int = None
+        self, batch: Dict, model: nn.Module, criterion: nn.Module, optimizer_idx: Optional[int] = None
     ) -> Tuple[Dict, Dict]:
-        """
-        Perform a evaluation forward pass. Compute model outputs and losses with no gradients.
+        """Perform a evaluation forward pass. Compute model outputs and losses with no gradients.
 
         Args:
             batch (Dict): IBatch of inputs.
             model (nn.Module): Model to call evaluation.
             criterion (nn.Module): Model criterion.
             optimizer_idx (int, optional): Optimizer ID to define the closure in multi-optimizer training. Defaults to None.
 
@@ -1710,17 +1699,20 @@
             if self.num_gpus > 1:
                 self.model.module.test_log(
                     test_outputs, self.dashboard_logger, self.training_assets, self.total_steps_done
                 )
             else:
                 self.model.test_log(test_outputs, self.dashboard_logger, self.training_assets, self.total_steps_done)
 
-    def _restore_best_loss(self):
-        """Restore the best loss from the args.best_path if provided else
-        from the model (`args.continue_path`) used for resuming the training"""
+    def _restore_best_loss(self) -> None:
+        """Restore the best loss.
+
+        Restore from the args.best_path if provided else from the model
+        (`args.continue_path`) used for resuming the training.
+        """
         if self.args.continue_path and (self.restore_step != 0 or self.args.best_path):
             logger.info(" > Restoring best loss from %s ...", os.path.basename(self.args.best_path))
             ch = load_fsspec(self.args.restore_path, map_location="cpu")
             if "model_loss" in ch:
                 if isinstance(ch["model_loss"], dict):
                     self.best_loss = ch["model_loss"]
                 # For backwards-compatibility:
@@ -1728,25 +1720,26 @@
                     if self.config.run_eval:
                         self.best_loss = {"train_loss": None, "eval_loss": ch["model_loss"]}
                     else:
                         self.best_loss = {"train_loss": ch["model_loss"], "eval_loss": None}
             logger.info(" > Starting with loaded last best loss %s", self.best_loss)
 
     def test(self, model=None, test_samples=None) -> None:
-        """Run evaluation steps on the test data split. You can either provide the model and the test samples
-        explicitly or the trainer use values from the initialization.
+        """Run evaluation steps on the test data split.
+
+        You can either provide the model and the test samples
+        explicitly or the trainer uses values from the initialization.
 
         Args:
             model (nn.Module, optional): Model to use for testing. If None, use the model given in the initialization.
                 Defaults to None.
 
             test_samples (List[str], optional): List of test samples to use for testing. If None, use the test samples
                 given in the initialization. Defaults to None.
         """
-
         logger.info(" > USING TEST SET...")
         self.keep_avg_eval = KeepAverage()
 
         if model is not None:
             self.model = model
 
         eval_samples_cache = self.eval_samples
@@ -1790,15 +1783,15 @@
                 self.keep_avg_eval.avg_values if self.config.run_eval else self.keep_avg_train.avg_values,
             )
             if self.args.rank in [None, 0]:
                 self.save_best_model()
             self.callbacks.on_epoch_end(self)
             self.start_with_eval = False
 
-    def fit_with_largest_batch_size(self, starting_batch_size=2048) -> None:
+    def fit_with_largest_batch_size(self, starting_batch_size: int = 2048) -> None:
         cuda_meminfo()
         bs = starting_batch_size
         while True:
             gc.collect()
             torch.cuda.empty_cache()
             try:
                 gc.collect()
@@ -1846,23 +1839,23 @@
             if self.num_gpus > 1:
                 dist.destroy_process_group()
             # finish the wandb run and sync data
             if self.args.rank == 0:
                 self.dashboard_logger.finish()
             # stop without error signal
             try:
-                sys.exit(1)
+                sys.exit(130)
             except SystemExit:
-                os._exit(1)  # pylint: disable=protected-access
+                os._exit(130)  # pylint: disable=protected-access
         except BaseException:  # pylint: disable=broad-except
             remove_experiment_folder(self.output_path)
             traceback.print_exc()
             sys.exit(1)
 
-    def profile_fit(self, torch_profiler, epochs=None, small_run=None):
+    def profile_fit(self, torch_profiler, epochs: Optional[int] = None, small_run: Optional[int] = None):
         """Run training under the torch profiler.
 
         Example::
             Run torch profiler to profile CPU, GPU and memory usage with Tensorboard logging.
 
             >>> import torch
             >>> profiler = torch.profiler.profile(
@@ -1877,22 +1870,21 @@
             >>>     with_stack=True,
             >>> )
             >>> prof = trainer.profile_fit(profiler, epochs=1, small_run=64)
         """
         self.dashboard_logger = DummyLogger()
         # train the model for a custom number of epochs
         if epochs:
-            self.config.epocshs = epochs
+            self.config.epochs = epochs
         # use a smaller set of training samples for profiling
         if small_run:
             self.setup_small_run(small_run)
         # run profiler
         self.config.run_eval = False
         self.config.test_delay_epochs = 9999999
-        self.config.epochs = epochs
         # set a callback to progress the profiler
         self.callbacks_on_train_step_end = [  # pylint: disable=attribute-defined-outside-init
             lambda trainer: trainer.torch_profiler.step()
         ]
         # set the profiler to access in the Trainer
         self.torch_profiler = torch_profiler  # pylint: disable=attribute-defined-outside-init
         # set logger output for Tensorboard
@@ -1901,15 +1893,14 @@
         self.fit()
         self.torch_profiler.stop()
         return self.torch_profiler
 
     @rank_zero_only
     def save_best_model(self) -> None:
         """Save the best model. It only saves if the current target loss is smaller then the previous."""
-
         eval_loss = self._pick_target_avg_loss(self.keep_avg_eval)
         train_loss = self._pick_target_avg_loss(self.keep_avg_train)
 
         # save the model and update the best_loss
         self.best_loss = save_best_model(
             {"train_loss": train_loss, "eval_loss": eval_loss},
             self.best_loss,
@@ -1941,15 +1932,15 @@
             self.output_path,
             model_loss={"train_loss": train_loss, "eval_loss": eval_loss},
             save_n_checkpoints=self.config.save_n_checkpoints,
             save_func=self.dashboard_logger.save_model,
         )
 
     @rank_zero_only
-    def update_training_dashboard_logger(self, batch=None, outputs=None):
+    def update_training_dashboard_logger(self, batch=None, outputs=None) -> None:
         aliases = [
             f"epoch-{self.epochs_done}",
             f"step-{self.total_steps_done}",
         ]
         self.dashboard_logger.add_artifact(
             file_or_dir=self.output_path, name="checkpoint", artifact_type="model", aliases=aliases
         )
@@ -2054,50 +2045,46 @@
         return scheduler
 
     @staticmethod
     def restore_scheduler(
         scheduler: Union["Scheduler", List, Dict], args: Coqpit, config: Coqpit, restore_epoch: int, restore_step: int
     ) -> Union["Scheduler", List]:
         """Restore scheduler wrt restored model."""
-        if scheduler is not None:  # pylint: disable=too-many-nested-blocks
-            if args.continue_path:
-                if isinstance(scheduler, list):
-                    for s in scheduler:
-                        if s is not None:
-                            if config.scheduler_after_epoch:
-                                s.last_epoch = restore_epoch
-                            else:
-                                s.last_epoch = restore_step
-                elif isinstance(scheduler, dict):
-                    for s in scheduler.values():
-                        if s is not None:
-                            if config.scheduler_after_epoch:
-                                s.last_epoch = restore_epoch
-                            else:
-                                s.last_epoch = restore_step
-                else:
-                    if config.scheduler_after_epoch:
-                        scheduler.last_epoch = restore_epoch
-                    else:
-                        scheduler.last_epoch = restore_step
+        if scheduler is not None and args.continue_path:
+            if isinstance(scheduler, list):
+                for s in scheduler:
+                    if s is not None:
+                        if config.scheduler_after_epoch:
+                            s.last_epoch = restore_epoch
+                        else:
+                            s.last_epoch = restore_step
+            elif isinstance(scheduler, dict):
+                for s in scheduler.values():
+                    if s is not None:
+                        if config.scheduler_after_epoch:
+                            s.last_epoch = restore_epoch
+                        else:
+                            s.last_epoch = restore_step
+            elif config.scheduler_after_epoch:
+                scheduler.last_epoch = restore_epoch
+            else:
+                scheduler.last_epoch = restore_step
         return scheduler
 
     @staticmethod
     def get_criterion(model: nn.Module) -> nn.Module:
         """Receive the criterion from the model. Model must implement `get_criterion()`.
 
         Args:
             model (nn.Module): Training model.
 
         Returns:
             nn.Module: Criterion layer.
         """
-        criterion = None
-        criterion = model.get_criterion()
-        return criterion
+        return model.get_criterion()
 
     ####################
     # HELPER FUNCTIONS
     ####################
 
     @staticmethod
     def _detach_loss_dict(loss_dict: Dict) -> Dict:
@@ -2144,15 +2131,14 @@
             target_avg_loss /= len(self.optimizer)
         else:
             target_avg_loss = keep_avg_target.avg_values.get("avg_loss", 0)
         return target_avg_loss
 
     def _setup_logger_config(self, log_file: str) -> None:
         """Set up the logger based on the process rank in DDP."""
-
         logger_new = logging.getLogger("trainer")
         handler = logging.FileHandler(log_file, mode="a")
         fmt = logging.Formatter("")
         handler.setFormatter(fmt)
         logger_new.addHandler(handler)
 
         # only log to a file if rank > 0 in DDP
```

### Comparing `coqui-tts-trainer-0.1.0/trainer/trainer_utils.py` & `coqui_tts_trainer-0.1.1/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/utils/cpu_memory.py` & `coqui_tts_trainer-0.1.1/trainer/utils/cpu_memory.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-trainer-0.1.0/trainer/utils/cuda_memory.py` & `coqui_tts_trainer-0.1.1/trainer/utils/cuda_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 credit: https://github.com/BlackHC/toma/blob/master/toma/torch_cuda_memory.py
 
 Helper to free Torch cuda memory and determine when a Torch exception might be
 because of OOM conditions.
 """
+
 from __future__ import print_function
 
 import gc
 
 import torch
 
 from trainer.utils.cpu_memory import is_out_of_cpu_memory
@@ -78,17 +79,15 @@
     )
 
 
 def cuda_meminfo():
     if not torch.cuda.is_available():
         return
 
-    print(
-        "Total:", torch.cuda.memory_allocated() / 2**30, " GB Cached: ", torch.cuda.memory_reserved() / 2**30, "GB"
-    )
+    print("Total:", torch.cuda.memory_allocated() / 2**30, " GB Cached: ", torch.cuda.memory_reserved() / 2**30, "GB")
     print(
         "Max Total:",
         torch.cuda.max_memory_allocated() / 2**30,
         " GB Max Cached: ",
         torch.cuda.max_memory_reserved() / 2**30,
         "GB",
     )
```

### Comparing `coqui-tts-trainer-0.1.0/trainer/utils/distributed.py` & `coqui_tts_trainer-0.1.1/trainer/utils/distributed.py`

 * *Files identical despite different names*

