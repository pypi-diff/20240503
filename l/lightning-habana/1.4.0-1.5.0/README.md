# Comparing `tmp/lightning-habana-1.4.0.tar.gz` & `tmp/lightning_habana-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-habana-1.4.0.tar", last modified: Fri Feb 16 06:10:02 2024, max compression
+gzip compressed data, was "lightning_habana-1.5.0.tar", last modified: Fri May  3 08:20:18 2024, max compression
```

## Comparing `lightning-habana-1.4.0.tar` & `lightning_habana-1.5.0.tar`

### file list

```diff
@@ -1,66 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.083048 lightning-habana-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-02-16 06:10:02.083048 lightning-habana-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.075048 lightning-habana-1.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/requirements/_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/requirements/_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/requirements/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/requirements/lightning.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/requirements/pytorch-lightning.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 06:10:02.083048 lightning-habana-1.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4100 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.071048 lightning-habana-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.075048 lightning-habana-1.4.0/src/lightning_habana/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.075048 lightning-habana-1.4.0/src/lightning_habana/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/fabric/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9945 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/deepspeed_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/pytorch/profiler/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/profiler/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.079048 lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44378 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.083048 lightning-habana-1.4.0/src/lightning_habana/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/utils/hpu_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-02-16 06:09:53.000000 lightning-habana-1.4.0/src/lightning_habana/utils/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:10:02.083048 lightning-habana-1.4.0/src/lightning_habana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-02-16 06:10:02.000000 lightning-habana-1.4.0/src/lightning_habana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-16 06:10:02.000000 lightning-habana-1.4.0/src/lightning_habana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 06:10:02.000000 lightning-habana-1.4.0/src/lightning_habana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 06:10:02.000000 lightning-habana-1.4.0/src/lightning_habana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-16 06:10:02.000000 lightning-habana-1.4.0/src/lightning_habana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-16 06:10:02.000000 lightning-habana-1.4.0/src/lightning_habana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.319787 lightning_habana-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-03 08:20:18.319787 lightning_habana-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.311787 lightning_habana-1.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/requirements/_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/requirements/_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/requirements/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/requirements/lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/requirements/pytorch-lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 08:20:18.319787 lightning_habana-1.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4445 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.307787 lightning_habana-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.311787 lightning_habana-1.5.0/src/lightning_habana/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.311787 lightning_habana-1.5.0/src/lightning_habana/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.311787 lightning_habana-1.5.0/src/lightning_habana/fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.315787 lightning_habana-1.5.0/src/lightning_habana/fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/fabric/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.315787 lightning_habana-1.5.0/src/lightning_habana/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.315787 lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.315787 lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9945 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.315787 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/deepspeed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/fsdp_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.307787 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/quant_config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.315787 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/quant_config/fp8/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/quant_config/fp8/maxabs_measure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/quant_config/fp8/maxabs_quant.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.315787 lightning_habana-1.5.0/src/lightning_habana/pytorch/profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/profiler/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.319787 lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45029 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.319787 lightning_habana-1.5.0/src/lightning_habana/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/utils/hpu_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-05-03 08:20:13.000000 lightning_habana-1.5.0/src/lightning_habana/utils/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:20:18.319787 lightning_habana-1.5.0/src/lightning_habana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-03 08:20:18.000000 lightning_habana-1.5.0/src/lightning_habana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-03 08:20:18.000000 lightning_habana-1.5.0/src/lightning_habana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:20:18.000000 lightning_habana-1.5.0/src/lightning_habana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:20:18.000000 lightning_habana-1.5.0/src/lightning_habana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 08:20:18.000000 lightning_habana-1.5.0/src/lightning_habana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 08:20:18.000000 lightning_habana-1.5.0/src/lightning_habana.egg-info/top_level.txt
```

### Comparing `lightning-habana-1.4.0/CHANGELOG.md` & `lightning_habana-1.5.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,45 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.5.0] - 2024-05-03
+
+### Added
+
+- Added support for Intel Gaudi Profiler. Deprecate `HABANA_PROFILE` environment variable from HPUProfiler. ([#158](https://github.com/Lightning-AI/lightning-Habana/pull/158))
+- Added support for FP8 inference. ([#162](https://github.com/Lightning-AI/lightning-Habana/pull/162))
+- Added support for LightningCLI. ([#173](https://github.com/Lightning-AI/lightning-Habana/pull/173))
+- Added experimental support for FSDP on HPU. ([#174](https://github.com/Lightning-AI/lightning-Habana/pull/174))
+- Added support for FP8 inference with DeepSpeed. ([#176](https://github.com/Lightning-AI/lightning-Habana/pull/176))
+- Updated the lightning version check for using FSDP. ([#182](https://github.com/Lightning-AI/lightning-Habana/pull/182))
+
+
+### Changed
+
+- Changed HPUParallelStrategy to HPUDDPStrategy ([#160](https://github.com/Lightning-AI/lightning-Habana/pull/160))
+- Changed HPU docker image based on Synapse AI release 1.15.0 ([#166](https://github.com/Lightning-AI/lightning-Habana/pull/166))
+- Updated to Intel Gaudi software Release 1.15.1 ([#171](https://github.com/Lightning-AI/lightning-Habana/pull/171))
+
+### Fixed
+
+- Fixed "No profiler activity found" error with HPUProfiler. ([#172](https://github.com/Lightning-AI/lightning-Habana/pull/172))
+
+### Removed
+
+-
+
+### Deprecated
+
+-
+
+
 ## [1.4.0] - 2024-02-16
 
 ### Added
 
 - Added DeepSpeed precision plugin for HPU ([#147](https://github.com/Lightning-AI/lightning-Habana/pull/147))
 - Added support for fp8 training. ([#149](https://github.com/Lightning-AI/lightning-Habana/pull/149))
```

### Comparing `lightning-habana-1.4.0/LICENSE` & `lightning_habana-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/MANIFEST.in` & `lightning_habana-1.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/PKG-INFO` & `lightning_habana-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: lightning-habana
-Version: 1.4.0
+Version: 1.5.0
 Summary: Lightning support for Intel Habana accelerators
 Home-page: https://github.com/Lightning-AI/lightning-habana
 Download-URL: https://github.com/Lightning-AI/lightning-habana
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-habana/issues
 Project-URL: Documentation, https://lightning-habana.rtfd.io/en/latest/
 Project-URL: Source Code, https://github.com/Lightning-AI/lightning-habana
 Keywords: deep learning,pytorch,AI
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lightning-utilities>=0.7.0
-Provides-Extra: lightning
-Requires-Dist: lightning>=2.1.0; extra == "lightning"
 Provides-Extra: typing
-Requires-Dist: mypy==1.8.0; extra == "typing"
-Requires-Dist: pytorch-lightning==2.1.3; extra == "typing"
-Provides-Extra: pytorch-lightning
-Requires-Dist: pytorch-lightning>=2.1.0; extra == "pytorch-lightning"
+Requires-Dist: mypy==1.10.0; extra == "typing"
+Requires-Dist: pytorch-lightning==2.2.3; extra == "typing"
 Provides-Extra: base
 Requires-Dist: lightning-utilities>=0.7.0; extra == "base"
+Provides-Extra: lightning
+Requires-Dist: lightning>=2.1.0; extra == "lightning"
 Provides-Extra: examples
 Requires-Dist: jsonargparse[signatures]; extra == "examples"
+Provides-Extra: pytorch-lightning
+Requires-Dist: pytorch-lightning>=2.1.0; extra == "pytorch-lightning"
 
 # Lightning ⚡ Intel Habana
 
 [![lightning](https://img.shields.io/badge/-Lightning_2.0+-792ee5?logo=pytorchlightning&logoColor=white)](https://lightning.ai/)
 [![PyPI Status](https://badge.fury.io/py/lightning-habana.svg)](https://badge.fury.io/py/lightning-habana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-habana)](https://pypi.org/project/lightning-habana/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/lightning-Habana)](https://pepy.tech/project/lightning-habana)
@@ -97,21 +97,21 @@
 trainer = Trainer(accelerator=HPUAccelerator(), devices=8)
 # Choose the number of devices automatically.
 trainer = Trainer(accelerator=HPUAccelerator(), devices="auto")
 ```
 
 The `devices=1` parameter with HPUs enables the Habana accelerator for single card training using `SingleHPUStrategy`.
 
-The `devices>1` parameter with HPUs enables the Habana accelerator for distributed training. It uses `HPUParallelStrategy` which is based on DDP strategy with the integration of Habana’s collective communication library (HCCL) to support scale-up within a node and scale-out across multiple nodes.
+The `devices>1` parameter with HPUs enables the Habana accelerator for distributed training. It uses `HPUDDPStrategy` which is based on DDP strategy with the integration of Habana’s collective communication library (HCCL) to support scale-up within a node and scale-out across multiple nodes.
 
 # Support Matrix
 
-| **SynapseAI**         | **1.14.0**                                          |
+| **SynapseAI**         | **1.15.1**                                          |
 | --------------------- | --------------------------------------------------- |
-| PyTorch               | 2.1.1                                               |
-| (PyTorch) Lightning\* | 2.1.x                                               |
-| **Lightning Habana**  | **1.4.0**                                           |
+| PyTorch               | 2.2.0                                               |
+| (PyTorch) Lightning\* | 2.2.x                                               |
+| **Lightning Habana**  | **1.5.0**                                           |
 | DeepSpeed\*\*         | Forked from v0.12.4 of the official DeepSpeed repo. |
 
 \* covers both packages [`lightning`](https://pypi.org/project/lightning/) and [`pytorch-lightning`](https://pypi.org/project/pytorch-lightning/)
 
 For more information, check out [HPU Support Matrix](https://docs.habana.ai/en/latest/Support_Matrix/Support_Matrix.html)
```

### Comparing `lightning-habana-1.4.0/README.md` & `lightning_habana-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,21 @@
 trainer = Trainer(accelerator=HPUAccelerator(), devices=8)
 # Choose the number of devices automatically.
 trainer = Trainer(accelerator=HPUAccelerator(), devices="auto")
 ```
 
 The `devices=1` parameter with HPUs enables the Habana accelerator for single card training using `SingleHPUStrategy`.
 
-The `devices>1` parameter with HPUs enables the Habana accelerator for distributed training. It uses `HPUParallelStrategy` which is based on DDP strategy with the integration of Habana’s collective communication library (HCCL) to support scale-up within a node and scale-out across multiple nodes.
+The `devices>1` parameter with HPUs enables the Habana accelerator for distributed training. It uses `HPUDDPStrategy` which is based on DDP strategy with the integration of Habana’s collective communication library (HCCL) to support scale-up within a node and scale-out across multiple nodes.
 
 # Support Matrix
 
-| **SynapseAI**         | **1.14.0**                                          |
+| **SynapseAI**         | **1.15.1**                                          |
 | --------------------- | --------------------------------------------------- |
-| PyTorch               | 2.1.1                                               |
-| (PyTorch) Lightning\* | 2.1.x                                               |
-| **Lightning Habana**  | **1.4.0**                                           |
+| PyTorch               | 2.2.0                                               |
+| (PyTorch) Lightning\* | 2.2.x                                               |
+| **Lightning Habana**  | **1.5.0**                                           |
 | DeepSpeed\*\*         | Forked from v0.12.4 of the official DeepSpeed repo. |
 
 \* covers both packages [`lightning`](https://pypi.org/project/lightning/) and [`pytorch-lightning`](https://pypi.org/project/pytorch-lightning/)
 
 For more information, check out [HPU Support Matrix](https://docs.habana.ai/en/latest/Support_Matrix/Support_Matrix.html)
```

### Comparing `lightning-habana-1.4.0/setup.py` & `lightning_habana-1.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 import glob
 import os
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 
 from pkg_resources import parse_requirements
-from setuptools import find_packages, setup
+from setuptools import find_namespace_packages, setup
 
 _PATH_ROOT = os.path.dirname(__file__)
 _PATH_SOURCE = os.path.join(_PATH_ROOT, "src")
 _PATH_REQUIRES = os.path.join(_PATH_ROOT, "requirements")
+_PATH_QUANT_CONFIG = "src/lightning_habana/pytorch/plugins/quant_config/"
 
 
 def _load_py_module(fname, pkg="lightning_habana"):
     spec = spec_from_file_location(os.path.join(pkg, fname), os.path.join(_PATH_SOURCE, pkg, fname))
     py = module_from_spec(spec)
     spec.loader.exec_module(py)
     return py
@@ -56,19 +57,28 @@
     version=about.__version__,
     description=about.__docs__,
     author=about.__author__,
     author_email=about.__author_email__,
     url=about.__homepage__,
     download_url="https://github.com/Lightning-AI/lightning-habana",
     license=about.__license__,
-    packages=find_packages(where="src"),
+    packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
+    data_files=[
+        (
+            "jsons",
+            [
+                os.path.join(_PATH_QUANT_CONFIG, "fp8", "maxabs_measure.json"),
+                os.path.join(_PATH_QUANT_CONFIG, "fp8", "maxabs_quant.json"),
+            ],
+        )
+    ],
     zip_safe=False,
     keywords=["deep learning", "pytorch", "AI"],
     python_requires=">=3.8",
     setup_requires=["wheel"],
     install_requires=_load_requirements(),
     extras_require=_prepare_extras(),
     project_urls={
@@ -77,15 +87,15 @@
         "Source Code": "https://github.com/Lightning-AI/lightning-habana",
     },
     classifiers=[
         "Environment :: Console",
         "Natural Language :: English",
         # How mature is this project? Common values are
         #   3 - Alpha, 4 - Beta, 5 - Production/Stable
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Information Analysis",
         # Pick your license as you wish
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 
 from lightning_utilities import compare_version
 
 from lightning_habana.__about__ import *  # noqa: F401, F403
 from lightning_habana.pytorch.accelerator import HPUAccelerator
 from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
 from lightning_habana.pytorch.plugins.deepspeed_precision import HPUDeepSpeedPrecisionPlugin
+from lightning_habana.pytorch.plugins.fsdp_precision import HPUFSDPPrecision
 from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 from lightning_habana.pytorch.profiler.profiler import HPUProfiler
+from lightning_habana.pytorch.strategies.ddp import HPUDDPStrategy
 from lightning_habana.pytorch.strategies.deepspeed import HPUDeepSpeedStrategy
+from lightning_habana.pytorch.strategies.fsdp import HPUFSDPStrategy
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
 from lightning_habana.pytorch.strategies.single import SingleHPUStrategy
 from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
 if compare_version("lightning", operator.lt, "2.0.0") and compare_version("pytorch_lightning", operator.lt, "2.0.0"):
     raise ImportError(
         "You are missing `lightning` or `pytorch-lightning` package or neither of them is in version 2.0+"
@@ -42,17 +45,20 @@
 
 _PACKAGE_ROOT = os.path.dirname(__file__)
 _PROJECT_ROOT = os.path.dirname(_PACKAGE_ROOT)
 
 
 __all__ = [
     "HPUAccelerator",
+    "HPUDDPStrategy",
     "HPUDeepSpeedStrategy",
     "HPUParallelStrategy",
+    "HPUFSDPStrategy",
     "SingleHPUStrategy",
     "HPUPrecisionPlugin",
     "HPUCheckpointIO",
     "HPUDataModule",
     "HPUProfiler",
     "HPU_AVAILABLE",
     "HPUDeepSpeedPrecisionPlugin",
+    "HPUFSDPPrecision",
 ]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/fabric/plugins/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,21 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-from lightning_habana.fabric.accelerator import HPUAccelerator
-from lightning_habana.fabric.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.fabric.plugins.precision import HPUPrecision
-from lightning_habana.fabric.strategies.parallel import HPUParallelStrategy
-from lightning_habana.fabric.strategies.single import SingleHPUStrategy
 
-__all__ = [
-    "HPUAccelerator",
-    "HPUParallelStrategy",
-    "SingleHPUStrategy",
-    "HPUPrecision",
-    "HPUCheckpointIO",
-]
+__all__ = ["HPUPrecision", "HPUCheckpointIO"]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/accelerator.py` & `lightning_habana-1.5.0/src/lightning_habana/fabric/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/plugins/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/profiler/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from lightning_habana.fabric.plugins.precision import HPUPrecision
+from lightning_habana.pytorch.profiler.profiler import HPUProfiler
 
-__all__ = ["HPUPrecision", "HPUCheckpointIO"]
+__all__ = ["HPUProfiler"]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/plugins/io_plugin.py` & `lightning_habana-1.5.0/src/lightning_habana/fabric/plugins/io_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/plugins/precision.py` & `lightning_habana-1.5.0/src/lightning_habana/fabric/plugins/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/strategies/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from lightning_habana.fabric.strategies.parallel import HPUParallelStrategy
-from lightning_habana.fabric.strategies.single import SingleHPUStrategy
+from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
 
-__all__ = ["HPUParallelStrategy", "SingleHPUStrategy"]
+__all__ = ["HPUDataModule"]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/strategies/parallel.py` & `lightning_habana-1.5.0/src/lightning_habana/fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/fabric/strategies/single.py` & `lightning_habana-1.5.0/src/lightning_habana/fabric/strategies/single.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,25 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from lightning_habana.pytorch.accelerator import HPUAccelerator
 from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
 from lightning_habana.pytorch.plugins.deepspeed_precision import HPUDeepSpeedPrecisionPlugin
+from lightning_habana.pytorch.plugins.fsdp_precision import HPUFSDPPrecision
 from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 from lightning_habana.pytorch.profiler.profiler import HPUProfiler
+from lightning_habana.pytorch.strategies.ddp import HPUDDPStrategy
 from lightning_habana.pytorch.strategies.deepspeed import HPUDeepSpeedStrategy
+from lightning_habana.pytorch.strategies.fsdp import HPUFSDPStrategy
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
 from lightning_habana.pytorch.strategies.single import SingleHPUStrategy
 
 __all__ = [
     "HPUAccelerator",
+    "HPUDDPStrategy",
     "HPUDeepSpeedStrategy",
     "HPUParallelStrategy",
     "SingleHPUStrategy",
+    "HPUFSDPStrategy",
     "HPUPrecisionPlugin",
     "HPUCheckpointIO",
     "HPUProfiler",
     "HPUDataModule",
     "HPUDeepSpeedPrecisionPlugin",
+    "HPUFSDPPrecision",
 ]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/accelerator.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,11 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
-
-__all__ = ["HPUDataModule"]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/datamodule.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/datamodule/utils.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/datamodule/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from lightning_habana.pytorch.plugins.deepspeed_precision import HPUDeepSpeedPrecisionPlugin
+from lightning_habana.pytorch.plugins.fsdp_precision import HPUFSDPPrecision
 from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 
-__all__ = ["HPUPrecisionPlugin", "HPUCheckpointIO", "HPUDeepSpeedPrecisionPlugin"]
+__all__ = ["HPUPrecisionPlugin", "HPUCheckpointIO", "HPUDeepSpeedPrecisionPlugin", "HPUFSDPPrecision"]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/io_plugin.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/io_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/plugins/precision.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/plugins/precision.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,41 +7,59 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from contextlib import _GeneratorContextManager, contextmanager
-from typing import Any, Generator, Literal, Mapping, Optional, Union
+import importlib.resources
+import os
+from contextlib import contextmanager
+from typing import Any, ContextManager, Generator, Literal, Mapping, Optional, Union
 
 import torch
 from lightning_utilities import module_available
 from typing_extensions import get_args
 
+from lightning_habana.utils.imports import _HPU_SYNAPSE_GREATER_EQUAL_1_11_0, _HPU_SYNAPSE_GREATER_EQUAL_1_14_0
+from lightning_habana.utils.resources import (
+    _HABANA_FRAMEWORK_AVAILABLE,
+    _HABANA_QUANTIZATION_TOOLKIT_AVAILABLE,
+    is_fp8_available,
+    modify_fp8_json,
+)
+
 if module_available("lightning"):
     from lightning.fabric.utilities.rank_zero import rank_zero_info, rank_zero_warn
     from lightning.pytorch.plugins.precision import Precision
 elif module_available("pytorch_lightning"):
     from pytorch_lightning.plugins.precision import Precision
     from pytorch_lightning.utilities.rank_zero import rank_zero_info, rank_zero_warn
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
-from lightning_habana.utils.imports import _HPU_SYNAPSE_GREATER_EQUAL_1_11_0, _HPU_SYNAPSE_GREATER_EQUAL_1_14_0
-from lightning_habana.utils.resources import _HABANA_FRAMEWORK_AVAILABLE, is_fp8_available
-
 _PRECISION_INPUT = Literal["32", "32-true", "bf16", "bf16-mixed", "fp8"]
 
 if _HPU_SYNAPSE_GREATER_EQUAL_1_14_0 and _HABANA_FRAMEWORK_AVAILABLE:
     # Required for training in fp8 using habana transformer engine
     import habana_frameworks.torch.hpex.experimental.transformer_engine as tengine
     from habana_frameworks.torch.hpex.experimental.transformer_engine.recipe import DelayedScaling
 
+    if _HABANA_QUANTIZATION_TOOLKIT_AVAILABLE:
+        # Required for inference in fp8 using habana quantization toolkit
+        import habana_frameworks.torch.core as htcore
+
+        # Default quantization jsons
+        MAXABS_MEASURE = str(
+            importlib.resources.path("lightning_habana.pytorch.plugins.quant_config.fp8", "maxabs_measure.json")
+        )
+        MAXABS_QUANT = str(
+            importlib.resources.path("lightning_habana.pytorch.plugins.quant_config.fp8", "maxabs_quant.json")
+        )
+
 
 class HPUPrecisionPlugin(Precision):
     """Plugin that enables mixed precision support on HPUs.
 
     Args:
         precision: to enable ``torch.bfloat16`` (``'bf16-mixed'``).
         device: The device for ``torch.autocast``.
@@ -68,40 +86,109 @@
         self.device = device
 
         if any([recipe, replace_layers]) and precision != "fp8":
             rank_zero_warn(f"Precision is not 'fp8'. Params {recipe=} and {replace_layers=} will not be set.")
 
         self.recipe = None
         self.fp8_train_available = False
+        self.fp8_inference_available = False
 
         if self.precision == "fp8":
             fp8_available, reason_no_fp8 = is_fp8_available()
             if not fp8_available:
                 raise NotImplementedError(f"fp8 not supported: {reason_no_fp8}.")
             self.recipe = recipe
             self.fp8_train_available = fp8_available
+            self.fp8_inference_available = fp8_available and _HABANA_QUANTIZATION_TOOLKIT_AVAILABLE
             self.replace_layers = replace_layers
-            rank_zero_info(f"fp8 training available: {self.fp8_train_available}.")
 
-    def convert_modules(self, module: torch.nn.Module) -> torch.nn.Module:
-        """Replace layers of a module with Transformer engine equivalent layers."""
-        if self.replace_layers is True and self.fp8_train_available:
-            # In case model already contains a transformer engine modules,
-            # assume user responsibility for conversion of required layers.
-            if any(
-                "habana_frameworks.torch.hpex.experimental.transformer_engine" in m.__module__ for m in module.modules()
-            ):
-                rank_zero_info(
-                    f"Module {module} already contains transformer engine equivalent modules. Skipping conversion"
+            rank_zero_info(
+                f"fp8 training available: {self.fp8_train_available}. "
+                f"fp8 inference available: {self.fp8_inference_available}."
+            )
+
+    def _setup_fp8_quant_config(self, quant: bool = True, fp8_data_path: Optional[str] = None) -> None:
+        """Setup QUANT_CONFIG for before importing HQT."""
+        if os.environ.get("QUANT_CONFIG", None) is None:
+            # Use default jsons in case one is not provided via env variable
+            fp8_data_path = fp8_data_path if fp8_data_path is not None else os.environ.get("HABANA_LOGS")
+            assert fp8_data_path is not None
+            # Create a copy in fp8_dump_path to avoid modifying package jsons.
+            fp8_json = MAXABS_QUANT if quant else MAXABS_MEASURE
+            if fp8_data_path is not None:
+                modify_fp8_json(
+                    file_path=fp8_json,
+                    patch={
+                        "dump_stats_path": os.path.join(fp8_data_path, "hqt"),
+                        "dump_stats_xlsx_path": os.path.join(fp8_data_path, "hqt", "fp8stats.xlsx"),
+                    },
                 )
-            else:
-                _replace_layers(module)
+            os.environ["QUANT_CONFIG"] = fp8_json
+
+    def _enable_fp8_inference(
+        self, module: torch.nn.Module, quant: bool = True, fp8_data_path: Optional[str] = None
+    ) -> None:
+        """Convert module for fp8 inference.
+
+        This module cannot be used to run trainer.fit.
+
+        """
+        htcore.hpu_set_env()
+        module = module.to("hpu")
+        self._setup_fp8_inference_modules(module, quant, fp8_data_path)
+
+    def _setup_fp8_inference_modules(
+        self, module: torch.nn.Module, quant: bool = True, fp8_data_path: Optional[str] = None
+    ) -> None:
+        """Convert module for fp8 inference."""
+        try:
+            self._setup_fp8_quant_config(quant, fp8_data_path)
+            from quantization_toolkit import habana_quantization_toolkit
+
+            habana_quantization_toolkit.prep_model(module)
+            htcore.hpu_initialize(module)
+        except FileNotFoundError as e:
+            print(
+                "Please run the fp8 measurement using a portion of data and try again. "
+                "Use HPUPrecisionPlugin.convert_modules(module, inference=True, quant=False) "
+                "and run trainer.fit() to dump measurement data."
+            )
+            raise e
+        except ModuleNotFoundError as e:
+            print("quantization_toolkit not found. Please install it using `pip install habana_quantization_toolkit`.")
+            raise e
+
+    def _enable_fp8_training(self, module: torch.nn.Module) -> None:
+        """Convert module for fp8 training."""
+        # In case model already contains a transformer engine modules,
+        # assume user responsibility for conversion of required layers.
+        if any(
+            "habana_frameworks.torch.hpex.experimental.transformer_engine" in m.__module__ for m in module.modules()
+        ):
+            rank_zero_info(
+                f"Module {module} already contains transformer engine equivalent modules. Skipping conversion"
+            )
+        else:
+            _replace_layers(module)
+
+    def convert_modules(
+        self,
+        module: torch.nn.Module,
+        inference: bool = False,
+        quant: bool = True,
+        fp8_data_path: Optional[str] = None,
+    ) -> torch.nn.Module:
+        """Enable support for fp8."""
+        if inference is True and self.fp8_inference_available:
+            self._enable_fp8_inference(module, quant, fp8_data_path)
+        if self.fp8_train_available is True and self.replace_layers is True and inference is False:
+            self._enable_fp8_training(module)
         return module
 
-    def autocast_context_manager(self) -> Union[_GeneratorContextManager[Any], torch.autocast]:
+    def autocast_context_manager(self) -> Union[ContextManager[Any], torch.autocast]:
         """Return Autocast context manager."""
         if self.fp8_train_available:
             return _nested_precision_cm(fp8_enabled=(self.precision == "fp8"), recipe=self.recipe)
         return torch.autocast(device_type="hpu", dtype=torch.bfloat16, enabled=True)
 
     @contextmanager
     def forward_context(self) -> Generator[None, None, None]:
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/profiler/profiler.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/profiler/profiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,28 +85,37 @@
         group_by_input_shapes: bool = False,
         export_to_chrome: bool = True,
         row_limit: int = 20,
         sort_by_key: Optional[str] = None,
         record_module_names: bool = True,
         **profiler_kwargs: Any,
     ) -> None:
-        os.environ["HABANA_PROFILE"] = "1"
+        assert os.environ.get("HABANA_PROFILE", None) in (
+            None,
+            "profile_api_light",
+        ), "`HABANA_PROFILE` should not be set when using `HPUProfiler`"
         super().__init__(
             dirpath=dirpath,
             filename=filename,
             group_by_input_shapes=group_by_input_shapes,
             export_to_chrome=export_to_chrome,
             row_limit=row_limit,
             sort_by_key=sort_by_key or f"{'hpu' if profiler_kwargs.get('use_hpu', False) else 'cpu'}_time_total",
             record_module_names=record_module_names,
             **profiler_kwargs,
         )
-
         self.profiler: Optional[_PROFILER] = None
         self._profiler_kwargs["activities"] = self.profile_hpu_activities(self._profiler_kwargs.get("activities", None))
+        assert self._activities_patched(
+            self._profiler_kwargs["activities"]
+        ), "lightning_habana should be imported before lightning to use HPUProfiler."
+
+    def _activities_patched(self, activities: List["ProfilerActivity"]) -> bool:
+        """Checks ProfilerActivity is patched by habana_frameworks."""
+        return all(not isinstance(activity, torch._C._profiler.ProfilerActivity) for activity in activities)
 
     def profile_hpu_activities(self, activities) -> List["ProfilerActivity"]:  # type: ignore
         if not _KINETO_AVAILABLE:
             return activities
         activities.append(ProfilerActivity.HPU)
         return activities
 
@@ -155,11 +164,7 @@
             if self._schedule is not None:
                 self.profiler.step_num = self._schedule.num_step
             self.profiler.step()
             self.profiler.add_metadata("Framework", "pytorch-lightning")
 
     def summary(self) -> str:
         return "Summary not supported for HPU Profiler"
-
-    def teardown(self, stage: Optional[str]) -> None:
-        super().teardown(stage=stage)
-        os.environ.pop("HABANA_PROFILE", None)
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/__init__.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from lightning_habana.pytorch.strategies.ddp import HPUDDPStrategy
 from lightning_habana.pytorch.strategies.deepspeed import HPUDeepSpeedStrategy
+from lightning_habana.pytorch.strategies.fsdp import HPUFSDPStrategy
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
 from lightning_habana.pytorch.strategies.single import SingleHPUStrategy
 
-__all__ = ["HPUDeepSpeedStrategy", "HPUParallelStrategy", "SingleHPUStrategy"]
+__all__ = ["HPUFSDPStrategy", "HPUDDPStrategy", "HPUDeepSpeedStrategy", "HPUParallelStrategy", "SingleHPUStrategy"]
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/deepspeed.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/deepspeed.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,27 +67,27 @@
     from pytorch_lightning.utilities.types import LRSchedulerConfig
 
 import torch
 from torch.nn import Module
 from torch.optim import Optimizer
 
 from lightning_habana.pytorch.accelerator import HPUAccelerator
-from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
+from lightning_habana.pytorch.strategies.ddp import HPUDDPStrategy
 from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
 if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.core as htcore  # noqa: F401
     import habana_frameworks.torch.distributed.hccl  # noqa: F401
 
 log = logging.getLogger(__name__)
 warning_cache = WarningCache()
 
 _HPU_DEEPSPEED_AVAILABLE = (
-    # HPU deep speed is supported only through this pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.14.0
-    RequirementCache("deepspeed==0.12.4+hpu.synapse.v1.14.0")
+    # HPU deep speed is supported only through this pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.15.1
+    RequirementCache("deepspeed==0.12.4+hpu.synapse.v1.15.1")
 )
 if TYPE_CHECKING and _HPU_DEEPSPEED_AVAILABLE:
     import deepspeed
 
 
 def remove_module_hooks(model: torch.nn.Module) -> None:
     """Helper to remove all module hooks."""
@@ -97,15 +97,15 @@
         module._is_full_backward_hook = None
         module._forward_hooks = OrderedDict()
         module._forward_pre_hooks = OrderedDict()
         module._state_dict_hooks = OrderedDict()
         module._load_state_dict_pre_hooks = OrderedDict()
 
 
-class HPUDeepSpeedStrategy(HPUParallelStrategy):
+class HPUDeepSpeedStrategy(HPUDDPStrategy):
     """Strategy to support deepspeed with HPU devices."""
 
     strategy_name = "hpu_deepspeed"
     DEEPSPEED_ENV_VAR = "PL_DEEPSPEED_CONFIG_PATH"
 
     def __init__(
         self,
@@ -294,15 +294,15 @@
         # TBD - remove these work arounds
         os.environ["PT_HPU_LAZY_ACC_PAR_MODE"] = "0"
         os.environ["PT_HPU_ENABLE_REFINE_DYNAMIC_SHAPES"] = "0"
 
         if not _HPU_DEEPSPEED_AVAILABLE:
             raise MisconfigurationException(
                 "To use the `HPUDeepSpeedStrategy`, you must have hpu DeepSpeed installed."
-                " Install it by running `pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.14.0`."
+                " Install it by running `pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.15.1`."
             )
 
         super().__init__(
             accelerator=accelerator,
             parallel_devices=parallel_devices,
             cluster_environment=cluster_environment,
             precision_plugin=precision_plugin,
@@ -927,14 +927,28 @@
 
         load(self.lightning_module, prefix="")
 
     def load_optimizer_state_dict(self, checkpoint: Mapping[str, Any]) -> None:
         # Override to do nothing, the deepspeed engine already loaded the states in `load_checkpoint()`
         pass
 
+    def on_test_end(self) -> None:
+        if self.precision_plugin.precision == "fp8" and self.precision_plugin.fp8_inference_available:
+            from quantization_toolkit import habana_quantization_toolkit  # noqa
+
+            habana_quantization_toolkit.finish_measurements(self.model)
+        return super().on_test_end()
+
+    def on_predict_end(self) -> None:
+        if self.precision_plugin.precision == "fp8" and self.precision_plugin.fp8_inference_available:
+            from quantization_toolkit import habana_quantization_toolkit  # noqa
+
+            habana_quantization_toolkit.finish_measurements(self.model)
+        return super().on_predict_end()
+
     @classmethod
     def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         strategy_registry.register("hpu_deepspeed", cls, description="Default DeepSpeed Strategy")
         strategy_registry.register(
             "hpu_deepspeed_stage_1", cls, description="DeepSpeed with ZeRO Stage 1 enabled", stage=1
         )
         strategy_registry.register(
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/parallel.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,26 @@
     from lightning.fabric.utilities.distributed import group as _group
     from lightning.fabric.utilities.types import ReduceOp
     from lightning.pytorch import LightningModule
     from lightning.pytorch.accelerators import Accelerator
     from lightning.pytorch.plugins.io.wrapper import _WrappingCheckpointIO
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.ddp import DDPStrategy
+    from lightning.pytorch.utilities.rank_zero import rank_zero_warn
     from lightning.pytorch.utilities.types import STEP_OUTPUT
 elif module_available("pytorch_lightning"):
     from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning_fabric.utilities.distributed import group as _group
     from lightning_fabric.utilities.types import ReduceOp
     from pytorch_lightning import LightningModule
     from pytorch_lightning.accelerators import Accelerator
     from pytorch_lightning.plugins.io.wrapper import _WrappingCheckpointIO
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.ddp import DDPStrategy
+    from pytorch_lightning.utilities.rank_zero import rank_zero_warn
     from pytorch_lightning.utilities.types import STEP_OUTPUT
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 from torch import Tensor
 from torch.nn import Module
 from torch.optim.optimizer import Optimizer
 
@@ -70,14 +72,18 @@
         ddp_comm_state: Optional[object] = None,
         ddp_comm_hook: Optional[Callable] = None,
         ddp_comm_wrapper: Optional[Callable] = None,
         model_averaging_period: Optional[int] = None,
         process_group_backend: Optional[str] = "hccl",
         **kwargs: Any,
     ) -> None:
+        rank_zero_warn(
+            "HPUParallelStrategy will be deprecated from lightning-habana >=1.6.0, please"
+            " make use of HPUDDPStrategy."
+        )
         super().__init__(
             accelerator=accelerator,
             parallel_devices=parallel_devices,
             cluster_environment=cluster_environment,
             checkpoint_io=checkpoint_io,
             precision_plugin=precision_plugin,
             ddp_comm_state=ddp_comm_state,
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/pytorch/strategies/single.py` & `lightning_habana-1.5.0/src/lightning_habana/pytorch/strategies/single.py`

 * *Files 17% similar despite different names*

```diff
@@ -120,14 +120,28 @@
         return super().test_step(*args, **kwargs)
 
     def predict_step(self, *args: Any, **kwargs: Any) -> Any:
         # Break lazy accumulation of graph after every step
         htcore.mark_step()
         return super().predict_step(*args, **kwargs)
 
+    def on_test_end(self) -> None:
+        if self.precision_plugin.precision == "fp8" and self.precision_plugin.fp8_inference_available:
+            from quantization_toolkit import habana_quantization_toolkit  # noqa
+
+            habana_quantization_toolkit.finish_measurements(self.model)
+        return super().on_test_end()
+
+    def on_predict_end(self) -> None:
+        if self.precision_plugin.precision == "fp8" and self.precision_plugin.fp8_inference_available:
+            from quantization_toolkit import habana_quantization_toolkit  # noqa
+
+            habana_quantization_toolkit.finish_measurements(self.model)
+        return super().on_predict_end()
+
     @classmethod
     def register_strategies(cls, strategy_registry: Dict) -> None:
         strategy_registry.register(
             cls.strategy_name,
             cls,
             description=f"{cls.__class__.__name__}",
         )
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/utils/hpu_distributed.py` & `lightning_habana-1.5.0/src/lightning_habana/utils/hpu_distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.4.0/src/lightning_habana/utils/imports.py` & `lightning_habana-1.5.0/src/lightning_habana/utils/imports.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,9 +23,12 @@
 _HPU_SYNAPSE_GREATER_EQUAL_1_11_0 = Version(get_hpu_synapse_version()) >= Version("1.11.0")
 _HPU_SYNAPSE_GREATER_EQUAL_1_14_0 = Version(get_hpu_synapse_version()) >= Version("1.14.0")
 _TORCH_LESSER_EQUAL_1_13_1 = compare_version("torch", operator.le, "1.13.1")
 _TORCH_GREATER_EQUAL_2_0_0 = compare_version("torch", operator.ge, "2.0.0")
 _LIGHTNING_GREATER_EQUAL_2_0_0 = compare_version("lightning", operator.ge, "2.0.0") or compare_version(
     "pytorch_lightning", operator.ge, "2.0.0"
 )
+_LIGHTNING_GREATER_EQUAL_2_3_0 = compare_version("lightning", operator.ge, "2.3.0", True) or compare_version(
+    "pytorch_lightning", operator.ge, "2.3.0", True
+)
 _TORCHVISION_AVAILABLE = RequirementCache("torchvision")
 _KINETO_AVAILABLE = torch.profiler.kineto_available()
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana/utils/resources.py` & `lightning_habana-1.5.0/src/lightning_habana/utils/resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import json
 import re
 import subprocess
 from functools import lru_cache
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from lightning_utilities import module_available
 from lightning_utilities.core.imports import package_available
 from lightning_utilities.core.rank_zero import rank_zero_debug, rank_zero_warn
 
 _HABANA_FRAMEWORK_AVAILABLE = package_available("habana_frameworks")
+_HABANA_QUANTIZATION_TOOLKIT_AVAILABLE = package_available("quantization_toolkit")
 
 if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.hpu as torch_hpu
 
 if module_available("lightning"):
     from lightning.fabric.utilities.exceptions import MisconfigurationException
     from lightning.fabric.utilities.types import _DEVICE
@@ -134,7 +136,31 @@
     if not _HPU_SYNAPSE_GREATER_EQUAL_1_14_0:
         raise OSError("fp8 training requires `Synapse AI release >= 1.14.0`.")
     if not _HABANA_FRAMEWORK_AVAILABLE:
         raise OSError("Habana Frameworks required for training on Habana devices.")
     import habana_frameworks.torch.hpex.experimental.transformer_engine as tengine
 
     return tengine.fp8.is_fp8_available()
+
+
+def modify_fp8_json(file_path: str, patch: dict) -> None:
+    """Edit a specific entry in a JSON file.
+
+    Parameters:
+        file_path (str): The path to the JSON file.
+        patch (dict): Entries to patch in json
+
+    Returns:
+        None
+
+    """
+    # Load the JSON file
+    with open(file_path, encoding="utf-8") as file:
+        data = json.load(file)
+
+    # Edit the specified entries
+    for key, value in patch.items():
+        data[key] = value
+
+    # Update json
+    with open(file_path, "w", encoding="utf-8") as file:
+        json.dump(data, file)
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana.egg-info/PKG-INFO` & `lightning_habana-1.5.0/src/lightning_habana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: lightning-habana
-Version: 1.4.0
+Version: 1.5.0
 Summary: Lightning support for Intel Habana accelerators
 Home-page: https://github.com/Lightning-AI/lightning-habana
 Download-URL: https://github.com/Lightning-AI/lightning-habana
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-habana/issues
 Project-URL: Documentation, https://lightning-habana.rtfd.io/en/latest/
 Project-URL: Source Code, https://github.com/Lightning-AI/lightning-habana
 Keywords: deep learning,pytorch,AI
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lightning-utilities>=0.7.0
-Provides-Extra: lightning
-Requires-Dist: lightning>=2.1.0; extra == "lightning"
 Provides-Extra: typing
-Requires-Dist: mypy==1.8.0; extra == "typing"
-Requires-Dist: pytorch-lightning==2.1.3; extra == "typing"
-Provides-Extra: pytorch-lightning
-Requires-Dist: pytorch-lightning>=2.1.0; extra == "pytorch-lightning"
+Requires-Dist: mypy==1.10.0; extra == "typing"
+Requires-Dist: pytorch-lightning==2.2.3; extra == "typing"
 Provides-Extra: base
 Requires-Dist: lightning-utilities>=0.7.0; extra == "base"
+Provides-Extra: lightning
+Requires-Dist: lightning>=2.1.0; extra == "lightning"
 Provides-Extra: examples
 Requires-Dist: jsonargparse[signatures]; extra == "examples"
+Provides-Extra: pytorch-lightning
+Requires-Dist: pytorch-lightning>=2.1.0; extra == "pytorch-lightning"
 
 # Lightning ⚡ Intel Habana
 
 [![lightning](https://img.shields.io/badge/-Lightning_2.0+-792ee5?logo=pytorchlightning&logoColor=white)](https://lightning.ai/)
 [![PyPI Status](https://badge.fury.io/py/lightning-habana.svg)](https://badge.fury.io/py/lightning-habana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-habana)](https://pypi.org/project/lightning-habana/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/lightning-Habana)](https://pepy.tech/project/lightning-habana)
@@ -97,21 +97,21 @@
 trainer = Trainer(accelerator=HPUAccelerator(), devices=8)
 # Choose the number of devices automatically.
 trainer = Trainer(accelerator=HPUAccelerator(), devices="auto")
 ```
 
 The `devices=1` parameter with HPUs enables the Habana accelerator for single card training using `SingleHPUStrategy`.
 
-The `devices>1` parameter with HPUs enables the Habana accelerator for distributed training. It uses `HPUParallelStrategy` which is based on DDP strategy with the integration of Habana’s collective communication library (HCCL) to support scale-up within a node and scale-out across multiple nodes.
+The `devices>1` parameter with HPUs enables the Habana accelerator for distributed training. It uses `HPUDDPStrategy` which is based on DDP strategy with the integration of Habana’s collective communication library (HCCL) to support scale-up within a node and scale-out across multiple nodes.
 
 # Support Matrix
 
-| **SynapseAI**         | **1.14.0**                                          |
+| **SynapseAI**         | **1.15.1**                                          |
 | --------------------- | --------------------------------------------------- |
-| PyTorch               | 2.1.1                                               |
-| (PyTorch) Lightning\* | 2.1.x                                               |
-| **Lightning Habana**  | **1.4.0**                                           |
+| PyTorch               | 2.2.0                                               |
+| (PyTorch) Lightning\* | 2.2.x                                               |
+| **Lightning Habana**  | **1.5.0**                                           |
 | DeepSpeed\*\*         | Forked from v0.12.4 of the official DeepSpeed repo. |
 
 \* covers both packages [`lightning`](https://pypi.org/project/lightning/) and [`pytorch-lightning`](https://pypi.org/project/pytorch-lightning/)
 
 For more information, check out [HPU Support Matrix](https://docs.habana.ai/en/latest/Support_Matrix/Support_Matrix.html)
```

### Comparing `lightning-habana-1.4.0/src/lightning_habana.egg-info/SOURCES.txt` & `lightning_habana-1.5.0/src/lightning_habana.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,36 @@
 src/lightning_habana.egg-info/top_level.txt
 src/lightning_habana/fabric/__init__.py
 src/lightning_habana/fabric/accelerator.py
 src/lightning_habana/fabric/plugins/__init__.py
 src/lightning_habana/fabric/plugins/io_plugin.py
 src/lightning_habana/fabric/plugins/precision.py
 src/lightning_habana/fabric/strategies/__init__.py
+src/lightning_habana/fabric/strategies/ddp.py
 src/lightning_habana/fabric/strategies/parallel.py
 src/lightning_habana/fabric/strategies/single.py
 src/lightning_habana/pytorch/__init__.py
 src/lightning_habana/pytorch/accelerator.py
 src/lightning_habana/pytorch/datamodule/__init__.py
 src/lightning_habana/pytorch/datamodule/datamodule.py
 src/lightning_habana/pytorch/datamodule/utils.py
 src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py
 src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py
 src/lightning_habana/pytorch/plugins/__init__.py
 src/lightning_habana/pytorch/plugins/deepspeed_precision.py
+src/lightning_habana/pytorch/plugins/fsdp_precision.py
 src/lightning_habana/pytorch/plugins/io_plugin.py
 src/lightning_habana/pytorch/plugins/precision.py
+src/lightning_habana/pytorch/plugins/quant_config/fp8/maxabs_measure.json
+src/lightning_habana/pytorch/plugins/quant_config/fp8/maxabs_quant.json
 src/lightning_habana/pytorch/profiler/__init__.py
 src/lightning_habana/pytorch/profiler/profiler.py
 src/lightning_habana/pytorch/strategies/__init__.py
+src/lightning_habana/pytorch/strategies/ddp.py
 src/lightning_habana/pytorch/strategies/deepspeed.py
+src/lightning_habana/pytorch/strategies/fsdp.py
 src/lightning_habana/pytorch/strategies/parallel.py
 src/lightning_habana/pytorch/strategies/single.py
 src/lightning_habana/utils/__init__.py
 src/lightning_habana/utils/hpu_distributed.py
 src/lightning_habana/utils/imports.py
 src/lightning_habana/utils/resources.py
```

