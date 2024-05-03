# Comparing `tmp/netspresso_trainer-0.2.0.tar.gz` & `tmp/netspresso_trainer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netspresso_trainer-0.2.0.tar", last modified: Mon Apr 15 01:10:44 2024, max compression
+gzip compressed data, was "netspresso_trainer-0.2.1.tar", last modified: Fri May  3 09:30:37 2024, max compression
```

## Comparing `netspresso_trainer-0.2.0.tar` & `netspresso_trainer-0.2.1.tar`

### file list

```diff
@@ -1,230 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.609402 netspresso_trainer-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.617402 netspresso_trainer-0.2.0/src/netspresso_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.617402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/image_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/evaluator_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/evaluator_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/inferencer_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/inferencer_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/pose_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/pose_estimation/rtmcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/pidnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/pose_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/pose_estimation/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/darknet.py
--rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/efficientformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/pidnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/core/fc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/anchor_free_decoupled_head.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/experimental/rtmcc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/yolopafpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/base_metaformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/depth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/pidnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/pose_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/pose_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/register.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_warm_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/poly_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/step_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/trainer_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/trainer_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/engine_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/fx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/model_ema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.617402 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.921729 netspresso_trainer-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-03 09:30:37.921729 netspresso_trainer-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:30:37.921729 netspresso_trainer-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.893729 netspresso_trainer-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.901729 netspresso_trainer-0.2.1/src/netspresso_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.901729 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.901729 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/image_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/pose_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/collate_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/evaluator_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/evaluator_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/inferencer_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/inferencer_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/detection/retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/detection/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/pose_estimation/rtmcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.905729 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/losses/segmentation/pidnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/classification/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/detection/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/pose_estimation/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/segmentation/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.909729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/core/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/efficientformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mixnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/experimental/pidnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/core/fc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/anchor_free_decoupled_head.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/experimental/rtmcc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.913729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.917729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/experimental/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/experimental/yolopafpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.917729 netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/base_metaformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/pidnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.917729 netspresso_trainer-0.2.1/src/netspresso_trainer/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/optimizers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/optimizers/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/optimizers/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.917729 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.917729 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/pose_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.921729 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/pose_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.921729 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/cosine_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/cosine_warm_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/poly_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/step_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/trainer_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/trainer_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.921729 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/engine_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/fx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/model_ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-03 09:30:29.000000 netspresso_trainer-0.2.1/src/netspresso_trainer/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:30:37.901729 netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-03 09:30:37.000000 netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-05-03 09:30:37.000000 netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:30:37.000000 netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 09:30:37.000000 netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 09:30:37.000000 netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 09:30:37.000000 netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/top_level.txt
```

### Comparing `netspresso_trainer-0.2.0/LICENSE` & `netspresso_trainer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/PKG-INFO` & `netspresso_trainer-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,143 @@
-Metadata-Version: 2.1
-Name: netspresso_trainer
-Version: 0.2.0
-Summary: NetsPresso Python Package
-Home-page: https://github.com/Nota-NetsPresso/netspresso-trainer
-Author: NetsPresso
-Author-email: netspresso@nota.ai
-License: UNKNOWN
-Description: <div align="center">
-            <img src="./assets/netspresso_trainer_header_tmp.png" width="800"/>
-        </div>
-        </br>
-        
-        <center style="white-space: pre-line">
-        Start training models (including ViTs) with <b>NetsPresso Trainer</b>,
-        compress and deploy your model with <b>NetsPresso</b>!
-        </center>
-        </br>
-        
-        <div align="center">
-        <p align="center">
-          <a href="https://py.netspresso.ai/">Website</a> •
-          <a href="#getting-started">Getting Started</a> •
-          <a href="https://github.com/Nota-NetsPresso/netspresso-trainer/issues">Issues</a> •
-          <a href="https://nota-netspresso.github.io/netspresso-trainer">Docs</a>
-        </p>
-        </div>
-        
-        _____
-        
-        ## Table of contents
-        
-        <!-- toc -->
-        
-        - [Installation](#installation)
-        - [Getting started](#getting-started)
-        
-        <!-- tocstop -->
-        
-        ## Installation (Stable)
-        
-        ### Prerequisites
-        
-        - Python `3.8` | `3.9` | `3.10`
-        - PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
-        
-        ### Install with pypi
-        
-        ```bash
-        pip install netspresso_trainer
-        ```
-        
-        ### Install with GitHub
-        
-        ```bash
-        pip install git+https://github.com/Nota-NetsPresso/netspresso-trainer.git@master
-        ```
-        
-        To install with editable mode,
-        
-        ```bash
-        git clone -b master https://github.com/Nota-NetsPresso/netspresso-trainer.git
-        pip install -e netspresso-trainer
-        ```
-        
-        ### Set-up with docker
-        
-        Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
-        For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
-        
-        ## Getting started
-        
-        Write your training script in `train.py` like:
-        
-        ```python
-        from netspresso_trainer import train_cli
-        
-        if __name__ == '__main__':
-            logging_dir = train_cli()
-            print(f"Training results are saved at: {logging_dir}")
-        ```
-        
-        Then, train your model with your own configuraiton:
-        
-        ```bash
-        python train.py\
-          --data config/data/beans.yaml\
-          --augmentation config/augmentation/classification.yaml\
-          --model config/model/resnet/resnet50-classification.yaml\
-          --training config/training/classification.yaml\
-          --logging config/logging.yaml\
-          --environment config/environment.yaml
-        ```
-        
-        Or you can start NetsPresso Trainer by just executing console script which has same feature.
-        
-        ```bash
-        netspresso-train\
-          --data config/data/beans.yaml\
-          --augmentation config/augmentation/classification.yaml\
-          --model config/model/resnet/resnet50-classification.yaml\
-          --training config/training/classification.yaml\
-          --logging config/logging.yaml\
-          --environment config/environment.yaml
-        ```
-        
-        Please refer to [`scripts/example_train.sh`](./scripts/example_train.sh).
-        
-        NetsPresso Trainer is compatible with [NetsPresso](https://netspresso.ai/) service. We provide NetsPresso Trainer tutorial that contains whole procedure from model train to model compression and benchmark. Please refer to our [colab tutorial](https://colab.research.google.com/drive/1RBKMCPEa4x-4X31zqzTS8WgQI9TQt3e-?usp=sharing).
-        
-        ## Tensorboard
-        
-        We provide basic tensorboard to track your training status. Run the tensorboard with the following command: 
-        
-        ```bash
-        tensorboard --logdir ./outputs --port 50001 --bind_all
-        ```
-        
-        where `PORT` for tensorboard is 50001.  
-        Note that the default directory of saving result will be `./outputs` directory.
-        
-        
-        ## Pretrained weights
-        
-        Please refer to our [official documentation](https://nota-netspresso.github.io/netspresso-trainer/) for pretrained weights supported by NetsPresso Trainer.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+<div align="center">
+    <img src="./assets/netspresso_trainer_header_tmp.png" width="800"/>
+</div>
+</br>
+
+<center style="white-space: pre-line">
+Start training models (including ViTs) with <b>NetsPresso Trainer</b>,
+compress and deploy your model with <b>NetsPresso</b>!
+</center>
+</br>
+
+<div align="center">
+<p align="center">
+  <a href="https://py.netspresso.ai/">Website</a> •
+  <a href="#getting-started">Getting Started</a> •
+  <a href="https://github.com/Nota-NetsPresso/netspresso-trainer/issues">Issues</a> •
+  <a href="https://nota-netspresso.github.io/netspresso-trainer">Docs</a>
+</p>
+</div>
+
+_____
+
+## Table of contents
+
+<!-- toc -->
+
+- [Installation](#installation)
+- [Getting started](#getting-started)
+
+<!-- tocstop -->
+
+## Installation (Stable)
+
+### Prerequisites
+
+- Python `3.8` | `3.9` | `3.10`
+- PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
+
+### Install with pypi
+
+```bash
+pip install netspresso_trainer
+```
+
+### Install with GitHub
+
+```bash
+pip install git+https://github.com/Nota-NetsPresso/netspresso-trainer.git@master
+```
+
+To install with editable mode,
+
+```bash
+git clone -b master https://github.com/Nota-NetsPresso/netspresso-trainer.git
+pip install -e netspresso-trainer
+```
+
+### Set-up with docker
+
+Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
+For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
+
+## Getting started
+
+Write your training script in `train.py` like:
+
+```python
+from netspresso_trainer import train_cli
+
+if __name__ == '__main__':
+    logging_dir = train_cli()
+    print(f"Training results are saved at: {logging_dir}")
+```
+
+Then, train your model with your own configuraiton:
+
+```bash
+python train.py\
+  --data config/data/beans.yaml\
+  --augmentation config/augmentation/classification.yaml\
+  --model config/model/resnet/resnet50-classification.yaml\
+  --training config/training/classification.yaml\
+  --logging config/logging.yaml\
+  --environment config/environment.yaml
+```
+
+Or you can start NetsPresso Trainer by just executing console script which has same feature.
+
+```bash
+netspresso-train\
+  --data config/data/beans.yaml\
+  --augmentation config/augmentation/classification.yaml\
+  --model config/model/resnet/resnet50-classification.yaml\
+  --training config/training/classification.yaml\
+  --logging config/logging.yaml\
+  --environment config/environment.yaml
+```
+
+Please refer to [`scripts/example_train.sh`](./scripts/example_train.sh).
+
+NetsPresso Trainer is compatible with [NetsPresso](https://netspresso.ai/) service. We provide NetsPresso Trainer tutorial that contains whole procedure from model train to model compression and benchmark. Please refer to our [colab tutorial](https://colab.research.google.com/drive/1RBKMCPEa4x-4X31zqzTS8WgQI9TQt3e-?usp=sharing).
+
+## Dataset preparation (Local)
+
+NetsPresso Trainer is designed to accommodate a variety of tasks, each requiring different dataset formats. You can find the specific dataset formats for each task in our [documentation](https://nota-netspresso.github.io/netspresso-trainer/components/data/).
+
+If you are interested in utilizing open datasets, you can use them by following the [instructions](https://nota-netspresso.github.io/netspresso-trainer/getting_started/dataset_preparation/local/#open-datasets).
+
+### Image classification
+
+- [CIFAR100](https://github.com/Nota-NetsPresso/netspresso-trainer/blob/dev/tools/open_dataset_tool/cifar100.py)
+- [ImageNet1K](https://github.com/Nota-NetsPresso/netspresso-trainer/blob/dev/tools/open_dataset_tool/imagenet1k.py)
+
+### Semantic segmentation
+
+- [PascalVOC 2012](https://github.com/Nota-NetsPresso/netspresso-trainer/blob/dev/tools/open_dataset_tool/voc2012_seg.py)
+
+### Object detection
+
+- [COCO 2017](https://github.com/Nota-NetsPresso/netspresso-trainer/blob/dev/tools/open_dataset_tool/coco2017.py)
+
+### Pose estimation
+
+- [WFLW](https://github.com/Nota-NetsPresso/netspresso-trainer/blob/dev/tools/open_dataset_tool/wflw.py)
+
+## Dataset preparation (Huggingface)
+
+NetsPresso Trainer is also compatible with huggingface dataset. To use datasets of huggingface, please check [instructions in our documentations](https://nota-netspresso.github.io/netspresso-trainer/getting_started/dataset_preparation/huggingface/). This enables to utilize a wide range of pre-built datasets which are beneficial for various training scenarios.
+
+## Pretrained weights
+
+Please refer to our [official documentation](https://nota-netspresso.github.io/netspresso-trainer/) for pretrained weights supported by NetsPresso Trainer.
+
+## Tensorboard
+
+We provide basic tensorboard to track your training status. Run the tensorboard with the following command: 
+
+```bash
+tensorboard --logdir ./outputs --port 50001 --bind_all
+```
+
+where `PORT` for tensorboard is 50001.  
+Note that the default directory of saving result will be `./outputs` directory.
```

### Comparing `netspresso_trainer-0.2.0/pyproject.toml` & `netspresso_trainer-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/setup.py` & `netspresso_trainer-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/image_proc.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/image_proc.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/mixing.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/mixing.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/mosaic.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/custom/mosaic.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/registry.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/registry.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/transforms.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/augmentation/transforms.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/base.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from abc import ABC, abstractmethod, abstractproperty
 from itertools import repeat
 from pathlib import Path
 
 import numpy as np
 import torch
 import torch.utils.data as data
+from loguru import logger
 
 
 class BaseCustomDataset(data.Dataset):
 
-    def __init__(self, conf_data, conf_augmentation, model_name, idx_to_class, split, samples, transform, with_label, **kwargs):
+    def __init__(self, conf_data, conf_augmentation, model_name, idx_to_class, split, samples, transform, **kwargs):
         super(BaseCustomDataset, self).__init__()
         self.conf_data = conf_data
         self.conf_augmentation = conf_augmentation
         self.model_name = model_name
 
         self.transform = transform(conf_augmentation)
         self.samples = samples
 
         self._root = conf_data.path.root
         self._idx_to_class = idx_to_class
         self._num_classes = len(self._idx_to_class)
         self._split = split
-        self._with_label = with_label
 
         self.cache = False
 
     @abstractmethod
     def __getitem__(self, index):
         pass
 
@@ -50,29 +50,25 @@
     def root(self):
         return self._root
 
     @property
     def mode(self):
         return self._split
 
-    @property
-    def with_label(self):
-        return self._with_label
 
 class BaseHFDataset(data.Dataset):
 
-    def __init__(self, conf_data, conf_augmentation, model_name, root, split, transform, with_label):
+    def __init__(self, conf_data, conf_augmentation, model_name, root, split, transform):
         super(BaseHFDataset, self).__init__()
         self.conf_data = conf_data
         self.conf_augmentation = conf_augmentation
         self.model_name = model_name
         self.transform = transform(conf_augmentation)
         self._root = root
         self._split = split
-        self._with_label = with_label
 
     def _load_dataset(self, root, subset_name=None, cache_dir=None):
         from datasets import load_dataset
         if cache_dir is not None:
             Path(cache_dir).mkdir(exist_ok=True, parents=True)
         total_dataset = load_dataset(root, name=subset_name, cache_dir=cache_dir)
         return total_dataset
@@ -97,28 +93,61 @@
     def root(self):
         return self._name
 
     @property
     def mode(self):
         return self._split
 
-    @property
-    def with_label(self):
-        return self._with_label
-
 
-class BaseDataSampler(ABC):
+class BaseSampleLoader(ABC):
     def __init__(self, conf_data, train_valid_split_ratio):
         self.conf_data = conf_data
         self.train_valid_split_ratio = train_valid_split_ratio
 
     @abstractmethod
     def load_data(self):
         raise NotImplementedError
 
     @abstractmethod
-    def load_samples(self):
+    def load_id_mapping(self):
+        raise NotImplementedError
+
+    @abstractmethod
+    def load_class_map(self, id_mapping):
         raise NotImplementedError
 
+    def load_samples(self):
+        assert self.conf_data.id_mapping is not None
+        id_mapping = self.load_id_mapping()
+        misc = self.load_class_map(id_mapping)
+
+        train_samples, valid_samples, test_samples = self.load_split_samples()
+        return train_samples, valid_samples, test_samples, misc
+
+    def load_split_samples(self):
+        exists_train = self.conf_data.path.train.image is not None
+        exists_valid = self.conf_data.path.valid.image is not None
+        exists_test = self.conf_data.path.test.image is not None
+
+        train_samples = None
+        valid_samples = None
+        test_samples = None
+
+        if exists_train:
+            train_samples = self.load_data(split='train')
+        if exists_valid:
+            valid_samples = self.load_data(split='valid')
+        if exists_test:
+            test_samples = self.load_data(split='test')
+
+        if not exists_valid and exists_train:
+            logger.info(f"Validation set is not provided in config. Split automatically training set by {self.train_valid_split_ratio:.1f}:{1-self.train_valid_split_ratio:.1f}.")
+            num_train_splitted = int(len(train_samples) * self.train_valid_split_ratio)
+            train_samples, valid_samples = \
+                data.random_split(train_samples, [num_train_splitted, len(train_samples) - num_train_splitted],
+                                  generator=torch.Generator().manual_seed(42))
+
+        return train_samples, valid_samples, test_samples
+
     @abstractmethod
     def load_huggingface_samples(self):
         raise NotImplementedError
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/builder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,86 @@
 import os
 from functools import partial
 from pathlib import Path
-from typing import Dict, List, Optional, Type, Union
+from typing import Dict, List, Literal, Optional, Type, Union
 
 import torch.distributed as dist
+import torch.utils.data as data
 from loguru import logger
+from omegaconf import DictConfig
 
 from .augmentation.registry import TRANSFORM_DICT
-from .classification import classification_mix_collate_fn, classification_onehot_collate_fn
-from .detection import detection_collate_fn
 from .registry import CREATE_TRANSFORM, CUSTOM_DATASET, DATA_SAMPLER, HUGGINGFACE_DATASET
+from .utils.collate_fn import classification_mix_collate_fn, classification_onehot_collate_fn, detection_collate_fn
 from .utils.loader import create_loader
 
 TRAIN_VALID_SPLIT_RATIO = 0.9
 
-def build_dataset(conf_data, conf_augmentation, task: str, model_name: str, distributed: bool):
 
+def dataset_path_check(conf_data: DictConfig, mode: Literal['train', 'test']):
+    if mode == 'train':
+        train_check = (conf_data.path.train.image is not None) and (conf_data.path.train.label is not None)
+        assert train_check, "For training, train split of dataset must be provided."
+
+        if conf_data.path.test.image:
+            logger.warning('For training, test split of dataset is not needed. This field will be ignored.')
+        conf_data.path.test.image = None
+        conf_data.path.test.label = None
+
+    elif mode == 'test':
+        assert conf_data.path.test.image is not None, "For test, test split of dataset must be provided."
+
+        if conf_data.path.train.image:
+            logger.warning('For test (evaluation or inference), train split of dataset is not needed. This field will be ignored.')
+        conf_data.path.train.image = None
+        conf_data.path.train.label = None
+
+        if conf_data.path.valid.image:
+            logger.warning('For test (evaluation or inference), valid split of dataset is not needed. This field will be ignored.')
+        conf_data.path.valid.image = None
+        conf_data.path.valid.label = None
+
+    else:
+        raise ValueError(f"mode of build_dataset cannot be {mode}. Must be one of ['train', 'test'].")
+
+
+def loaded_dataset_check(
+    conf_data: DictConfig,
+    train_dataset: data.Dataset,
+    valid_dataset: data.Dataset,
+    test_dataset: data.Dataset,
+    distributed: bool,
+    mode: Literal['train', 'test']
+):
+    if mode == 'train':
+        if not distributed or dist.get_rank() == 0:
+            logger.info(f"Summary | Dataset: <{conf_data.name}> (with {conf_data.format} format)")
+            logger.info(f"Summary | Training dataset: {len(train_dataset)} sample(s)")
+            if valid_dataset is not None:
+                logger.info(f"Summary | Validation dataset: {len(valid_dataset)} sample(s)")
+        assert len(train_dataset) > 0, "Training dataset has no samples. Please check your dataset configuration."
+
+    elif mode == 'test':
+        if not distributed or dist.get_rank() == 0:
+            logger.info(f"Summary | Dataset: <{conf_data.name}> (with {conf_data.format} format)")
+            logger.info(f"Summary | Test dataset: {len(test_dataset)} sample(s)")
+        assert len(test_dataset) > 0, "Test dataset has no samples. Please check your dataset configuration."
+
+    else:
+        raise ValueError(f"mode of build_dataset cannot be {mode}. Must be one of ['train', 'test'].")
+
+
+def build_dataset(
+    conf_data: DictConfig,
+    conf_augmentation: DictConfig,
+    task: str,
+    model_name: str,
+    distributed: bool,
+    mode: Literal['train', 'test'],
+):
     if not distributed or dist.get_rank() == 0:
         logger.info('-'*40)
         logger.info("Loading data...")
 
     task = conf_data.task
 
     assert task in DATA_SAMPLER, f"Data sampler for {task} is not yet supported!"
@@ -28,21 +89,22 @@
     target_transform = CREATE_TRANSFORM(model_name, is_training=False)
 
     data_format = conf_data.format
 
     assert data_format in ['local', 'huggingface'], f"No such data format named {data_format} in {['local', 'huggingface']}!"
 
     if data_format == 'local':
+        dataset_path_check(conf_data=conf_data, mode=mode)
+
         assert task in CUSTOM_DATASET, f"Local dataset for {task} is not yet supported!"
         data_sampler = DATA_SAMPLER[task](conf_data, train_valid_split_ratio=TRAIN_VALID_SPLIT_RATIO)
 
         train_samples, valid_samples, test_samples, misc = data_sampler.load_samples()
         idx_to_class = misc['idx_to_class'] if 'idx_to_class' in misc else None
         label_value_to_idx = misc['label_value_to_idx'] if 'label_value_to_idx' in misc else None
-        test_with_label = misc['test_with_label'] if 'test_with_label' in misc else None
 
         train_dataset = None
         if train_samples is not None:
             train_dataset = CUSTOM_DATASET[task](
                 conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='train',
                 samples=train_samples, transform=train_transform, label_value_to_idx=label_value_to_idx
             )
@@ -54,28 +116,26 @@
                 samples=valid_samples, transform=target_transform, label_value_to_idx=label_value_to_idx
             )
 
         test_dataset = None
         if test_samples is not None:
             test_dataset = CUSTOM_DATASET[task](
                 conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='test',
-                samples=test_samples, transform=target_transform,
-                with_label=test_with_label, label_value_to_idx=label_value_to_idx
+                samples=test_samples, transform=target_transform, label_value_to_idx=label_value_to_idx
             )
 
     elif data_format == 'huggingface':
         assert task in CUSTOM_DATASET, f"HuggingFace dataset for {task} is not yet supported!"
         assert task in DATA_SAMPLER, f"Data sampler for {task} is not yet supported!"
 
         data_sampler = DATA_SAMPLER[task](conf_data, train_valid_split_ratio=TRAIN_VALID_SPLIT_RATIO)
 
         train_samples, valid_samples, test_samples, misc = data_sampler.load_huggingface_samples()
         idx_to_class = misc['idx_to_class'] if 'idx_to_class' in misc else None
         label_value_to_idx = misc['label_value_to_idx'] if 'label_value_to_idx' in misc else None
-        test_with_label = misc['test_with_label'] if 'test_with_label' in misc else None
 
         # Assumed hugging face dataset always has training split
         train_dataset = HUGGINGFACE_DATASET[task](
             conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='train',
             huggingface_dataset=train_samples, transform=train_transform, label_value_to_idx=label_value_to_idx
         )
 
@@ -89,14 +149,15 @@
         test_dataset = None
         if test_samples is not None:
             test_dataset = HUGGINGFACE_DATASET[task](
                 conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='test',
                 huggingface_dataset=test_samples, transform=target_transform, label_value_to_idx=label_value_to_idx
             )
 
+    loaded_dataset_check(conf_data, train_dataset, valid_dataset, test_dataset, distributed, mode)
     return train_dataset, valid_dataset, test_dataset
 
 
 def build_dataloader(conf, task: str, model_name: str, dataset, phase, profile=False):
     is_training = phase == 'train'
 
     #TODO: Temporarily set ``cache_data`` as optional since this is experimental
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/dataset.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/pose_estimation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,157 @@
-import csv
-import random
-from collections import Counter
+import json
+from functools import partial
 from itertools import chain
+from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
-import torch
+import numpy as np
+import PIL.Image as Image
+import torch.distributed as dist
 from loguru import logger
-from omegaconf import DictConfig
-from torch.nn import functional as F
-from torch.utils.data import random_split
+from omegaconf import ListConfig
 
-from ..base import BaseDataSampler
-from ..utils.constants import IMG_EXTENSIONS
-from ..utils.misc import natural_key
+from .base import BaseCustomDataset, BaseSampleLoader
+from .utils.constants import IMG_EXTENSIONS
+from .utils.misc import natural_key
 
-VALID_IMG_EXTENSIONS = IMG_EXTENSIONS + tuple((x.upper() for x in IMG_EXTENSIONS))
 
-
-def load_custom_class_map(id_mapping: List[str]):
-    idx_to_class: Dict[int, str] = dict(enumerate(id_mapping))
-    return idx_to_class
-
-
-def load_class_map_with_id_mapping(labels_path: Optional[Union[str, Path]]):
-    # Assume the `map_or_filename` is path for csv label file
-    assert labels_path.exists(), f"Cannot locate specified class map file {labels_path}!"
-    class_map_ext = labels_path.suffix.lower()
-    assert class_map_ext == '.csv', f"Unsupported class map file extension ({class_map_ext})!"
-
-    with open(labels_path, newline='') as csvfile:
-        reader = csv.DictReader(csvfile)
-        file_to_idx = {row['image_id']: int(row['class']) for row in reader}
-
-    return file_to_idx
-
-
-def is_file_dict(image_dir: Union[Path, str], file_or_dir_to_idx):
-    image_dir = Path(image_dir)
-    candidate_name = list(file_or_dir_to_idx.keys())[0]
-    file_or_dir: Path = image_dir / candidate_name
-    if file_or_dir.exists():
-        return file_or_dir.is_file()
-
-    file_candidates = list(image_dir.glob(f"{candidate_name}.*"))
-    assert len(file_candidates) != 0, f"Unknown label format! Is there any something file like {file_or_dir} ?"
-
-    return True
-
-
-def classification_mix_collate_fn(original_batch, mix_transforms):
-    indices = []
-    images = []
-    target = []
-    for data_sample in original_batch:
-        indices.append(data_sample[0])
-        images.append(data_sample[1])
-        target.append(data_sample[2])
-
-    indices = torch.tensor(indices, dtype=torch.long)
-    images = torch.stack(images, dim=0)
-    target = torch.tensor(target, dtype=torch.long)
-
-    images, target = mix_transforms(images, target)
-
-    outputs = (indices, images, target)
-    return outputs
-
-
-def classification_onehot_collate_fn(original_batch, num_classes):
-    indices = []
-    images = []
-    target = []
-    for data_sample in original_batch:
-        indices.append(data_sample[0])
-        images.append(data_sample[1])
-        target.append(data_sample[2])
-
-    indices = torch.tensor(indices, dtype=torch.long)
-    images = torch.stack(images, dim=0)
-    target = torch.tensor(target, dtype=torch.long)
-    if -1 not in target:
-        target = F.one_hot(target, num_classes=num_classes).to(dtype=images.dtype)
-
-    outputs = (indices, images, target)
-    return outputs
-
-
-class ClassficationDataSampler(BaseDataSampler):
+class PoseEstimationSampleLoader(BaseSampleLoader):
     def __init__(self, conf_data, train_valid_split_ratio):
-        super(ClassficationDataSampler, self).__init__(conf_data, train_valid_split_ratio)
+        super(PoseEstimationSampleLoader, self).__init__(conf_data, train_valid_split_ratio)
 
     def load_data(self, split='train'):
+        assert split in ['train', 'valid', 'test'], f"split should be either {['train', 'valid', 'test']}."
         data_root = Path(self.conf_data.path.root)
         split_dir = self.conf_data.path[split]
         image_dir: Path = data_root / split_dir.image
-        annotation_path: Optional[Path] = data_root / split_dir.label if split_dir.label is not None else None
-        images_and_targets: List[Dict[str, Optional[Union[str, int]]]] = []
-
-        assert split in ['train', 'valid', 'test'], f"split should be either {['train', 'valid', 'test']}"
-        if annotation_path is not None:
-            file_to_idx = load_class_map_with_id_mapping(annotation_path)
+        annotation_dir: Optional[Path] = data_root / split_dir.label if split_dir.label is not None else None
+        images: List[str] = []
+        labels: List[str] = []
+        images_and_targets: List[Dict[str, str]] = []
+        if annotation_dir is not None:
             for ext in IMG_EXTENSIONS:
                 for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}')):
-                    if file.name in file_to_idx:
-                        images_and_targets.append({'image': str(file), 'label': file_to_idx[file.name]})
+                    ann_path_maybe = annotation_dir / file.with_suffix('.txt').name
+                    if not ann_path_maybe.exists():
                         continue
-                    logger.debug(f"Found file without label: {file}")
+                    images.append(str(file))
+                    labels.append(str(ann_path_maybe))
+                # TODO: get paired data from regex pattern matching (self.conf_data.path.pattern)
+
+            images = sorted(images, key=lambda k: natural_key(k))
+            labels = sorted(labels, key=lambda k: natural_key(k))
+            images_and_targets.extend([{'image': str(image), 'label': str(label)} for image, label in zip(images, labels)])
+
         else:
-            if split in ['train', 'valid']:
-                raise ValueError("For train and valid split, label path must be provided!")
-            for ext in VALID_IMG_EXTENSIONS:
-                images_and_targets.extend([{'image': str(file), 'label': None} for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}'))])
+            for ext in IMG_EXTENSIONS:
+                images_and_targets.extend([{'image': str(file), 'label': None}
+                                        for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}'))])
+            images_and_targets = sorted(images_and_targets, key=lambda k: natural_key(k['image']))
 
-        images_and_targets = sorted(images_and_targets, key=lambda k: natural_key(k['image']))
         return images_and_targets
 
-    def load_samples(self):
-        assert self.conf_data.id_mapping is not None
-        id_mapping = list(self.conf_data.id_mapping)
-        idx_to_class = load_custom_class_map(id_mapping=id_mapping)
-
-        exists_train = self.conf_data.path.train.image is not None
-        exists_valid = self.conf_data.path.valid.image is not None
-        exists_test = self.conf_data.path.test.image is not None
-
-        train_samples = None
-        valid_samples = None
-        test_samples = None
-
-        if exists_train:
-            train_samples = self.load_data(split='train')
-        if exists_valid:
-            valid_samples = self.load_data(split='valid')
-        if exists_test:
-            test_samples = self.load_data(split='test')
-
-        if not exists_valid:
-            num_train_splitted = int(len(train_samples) * self.train_valid_split_ratio)
-            train_samples, valid_samples = \
-                random_split(train_samples, [num_train_splitted, len(train_samples) - num_train_splitted],
-                                generator=torch.Generator().manual_seed(42))
+    def load_id_mapping(self):
+        root_path = Path(self.conf_data.path.root)
+
+        if isinstance(self.conf_data.id_mapping, ListConfig):
+            return list(self.conf_data.id_mapping)
+        elif isinstance(self.conf_data.id_mapping, str):
+            id_mapping_path = root_path / self.conf_data.id_mapping
+            with open(id_mapping_path, 'r') as f:
+                id_mapping = json.load(f)
+            return id_mapping
+        else:
+            raise ValueError(f"Invalid id_mapping type: {type(self.conf_data.id_mapping)}")
 
-        return train_samples, valid_samples, test_samples, {'idx_to_class': idx_to_class}
+    def load_class_map(self, id_mapping):
+        idx_to_class: Dict[int, str] = dict(enumerate(id_mapping))
+        return {'idx_to_class': idx_to_class}
 
     def load_huggingface_samples(self):
-        from datasets import ClassLabel, load_dataset
+        raise NotImplementedError
 
-        cache_dir = self.conf_data.metadata.custom_cache_dir
-        root = self.conf_data.metadata.repo
-        subset_name = self.conf_data.metadata.subset
-        if cache_dir is not None:
-            cache_dir = Path(cache_dir)
-            Path(cache_dir).mkdir(exist_ok=True, parents=True)
-        total_dataset = load_dataset(root, name=subset_name, cache_dir=cache_dir)
-
-        label_feature_name = self.conf_data.metadata.features.label
-        # Assumed hugging face dataset always has training split
-        label_feature = total_dataset['train'].features[label_feature_name]
-        if isinstance(label_feature, ClassLabel):
-            labels: List[str] = label_feature.names
-        else:
-            labels = list({sample[label_feature_name] for sample in total_dataset['train']})
 
-        if isinstance(labels[0], int):
-            # TODO: find class_map <-> idx and apply it (ex. using id_mapping)
-            idx_to_class: Dict[int, int] = {k: k for k in labels}
-        elif isinstance(labels[0], str):
-            idx_to_class: Dict[int, str] = dict(enumerate(labels))
-
-        exists_valid = 'validation' in total_dataset
-        exists_test = 'test' in total_dataset
-
-        train_samples = total_dataset['train']
-        valid_samples = None
-        if exists_valid:
-            valid_samples = total_dataset['validation']
-        test_samples = None
-        if exists_test:
-            test_samples = total_dataset['test']
-
-        if not exists_valid:
-            splitted_datasets = train_samples.train_test_split(test_size=(1 - self.train_valid_split_ratio))
-            train_samples = splitted_datasets['train']
-            valid_samples = splitted_datasets['test']
-        return train_samples, valid_samples, test_samples, {'idx_to_class': idx_to_class}
+class PoseEstimationCustomDataset(BaseCustomDataset):
+
+    def __init__(self, conf_data, conf_augmentation, model_name, idx_to_class,
+                 split, samples, transform=None, **kwargs):
+        super(PoseEstimationCustomDataset, self).__init__(
+            conf_data, conf_augmentation, model_name, idx_to_class,
+            split, samples, transform, **kwargs
+        )
+        flattened_samples = []
+        # label field must be filled
+        for sample in self.samples:
+            flattened_sample = {}
+            with open(sample['label'], 'r') as f:
+                lines = f.readlines()
+                f.close()
+            flattened_sample = [{'image': sample['image'], 'label': line.strip()} for line in lines]
+            flattened_samples += flattened_sample
+        self.samples = flattened_samples
+
+        # Build flip map. This is needed when try randomflip augmentation.
+        if split == 'train':
+            trasnform_names = {transform_conf['name'] for transform_conf in conf_augmentation[split]}
+            flips = {'randomhorizontalflip', 'randomverticalflip'}
+            if len(trasnform_names.intersection(flips)) > 0:
+                class_to_idx = {self._idx_to_class[i]['name']: i for i in self._idx_to_class}
+                self.flip_indices = np.zeros(self._num_classes).astype('int')
+                for idx in self._idx_to_class:
+                    idx_swap = self._idx_to_class[idx]['swap']
+                    assert idx_swap is not None, "To apply flip transform, keypoint swap info must be filled."
+                    self.flip_indices[idx] = class_to_idx[idx_swap] if idx_swap else -1
+
+    def cache_dataset(self, sampler, distributed):
+        if (not distributed) or (distributed and dist.get_rank() == 0):
+            logger.info(f'Caching | Loading samples of {self.mode} to memory... This can take minutes.')
+
+        def _load(i, samples):
+            image = Image.open(Path(samples[i]['image'])).convert('RGB')
+            return i, image
+
+        num_threads = 8 # TODO: Compute appropriate num_threads
+        load_imgs = ThreadPool(num_threads).imap(
+            partial(_load, samples=self.samples),
+            sampler
+        )
+        for i, image in load_imgs:
+            self.samples[i]['image'] = image
+
+        self.cache = True
+
+    def __getitem__(self, index):
+        img = self.samples[index]['image']
+        ann = self.samples[index]['label'] # TODO: Pose estimation is not assuming that label can be None now
+
+        if not self.cache:
+            img = Image.open(Path(img)).convert('RGB')
+
+        w, h = img.size
+
+        outputs = {}
+        outputs.update({'indices': index})
+        if ann is None:
+            out = self.transform(image=img)
+            outputs.update({'pixel_values': out['image'], 'org_shape': (h, w)})
+            return outputs
+
+        ann = ann.split(' ')
+        bbox = ann[-4:]
+        keypoints = ann[:-4]
+
+        bbox = np.array(bbox).astype('float32')[np.newaxis, ...]
+        keypoints = np.array(keypoints).reshape(-1, 3).astype('float32')[np.newaxis, ...]
+
+        out = self.transform(image=img, bbox=bbox, keypoint=keypoints, dataset=self)
+
+        # Use only one instance keypoints
+        outputs.update({'pixel_values': out['image'], 'keypoints': out['keypoint'][0]})
+        if self._split in ['train', 'training']:
+            return outputs
+
+        assert self._split in ['val', 'valid', 'test']
+        # outputs.update({'org_img': org_img, 'org_shape': (h, w)})  # TODO: return org_img with batch_size > 1
+        outputs.update({'org_shape': (h, w)})
+        return outputs
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/local.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/detection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,95 @@
+import json
 import os
 from functools import partial
+from itertools import chain
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
-from typing import List
+from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import PIL.Image as Image
 import torch
 import torch.distributed as dist
 from loguru import logger
-from omegaconf import OmegaConf
+from omegaconf import ListConfig
 
-from ..base import BaseCustomDataset
-
-ID2LABEL_FILENAME = "id2label.json"
-TEMP_COCO_LABEL_FILE = "data/detection/coco.yaml"
-
-
-def exist_name(candidate, folder_iterable):
-    try:
-        return list(filter(lambda x: candidate[0] in x, folder_iterable))[0]
-    except IndexError:
-        return list(filter(lambda x: candidate[1] in x, folder_iterable))[0]
+from .base import BaseCustomDataset, BaseSampleLoader
+from .utils.constants import IMG_EXTENSIONS
+from .utils.misc import get_detection_label, natural_key
+
+
+class DetectionSampleLoader(BaseSampleLoader):
+    def __init__(self, conf_data, train_valid_split_ratio):
+        super(DetectionSampleLoader, self).__init__(conf_data, train_valid_split_ratio)
+
+    def load_data(self, split='train'):
+        assert split in ['train', 'valid', 'test'], f"split should be either {['train', 'valid', 'test']}."
+        data_root = Path(self.conf_data.path.root)
+        split_dir = self.conf_data.path[split]
+        image_dir: Path = data_root / split_dir.image
+        annotation_dir: Optional[Path] = data_root / split_dir.label if split_dir.label is not None else None
+        images: List[str] = []
+        labels: List[str] = []
+        images_and_targets: List[Dict[str, str]] = []
+        if annotation_dir is not None:
+            for ext in IMG_EXTENSIONS:
+                for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}')):
+                    ann_path_maybe = annotation_dir / file.with_suffix('.txt').name
+                    if not ann_path_maybe.exists():
+                        continue
+                    images.append(str(file))
+                    labels.append(str(ann_path_maybe))
+                # TODO: get paired data from regex pattern matching (self.conf_data.path.pattern)
+
+            images = sorted(images, key=lambda k: natural_key(k))
+            labels = sorted(labels, key=lambda k: natural_key(k))
+            images_and_targets.extend([{'image': str(image), 'label': str(label)} for image, label in zip(images, labels)])
 
+        else:
+            for ext in IMG_EXTENSIONS:
+                images_and_targets.extend([{'image': str(file), 'label': None}
+                                        for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}'))])
+            images_and_targets = sorted(images_and_targets, key=lambda k: natural_key(k['image']))
+
+        return images_and_targets
+
+    def load_id_mapping(self):
+        root_path = Path(self.conf_data.path.root)
+
+        if isinstance(self.conf_data.id_mapping, ListConfig):
+            return list(self.conf_data.id_mapping)
+
+        elif isinstance(self.conf_data.id_mapping, str):
+            id_mapping_path = root_path / self.conf_data.id_mapping
+            if not os.path.isfile(id_mapping_path):
+                raise FileNotFoundError(f"File not found: {id_mapping_path}")
+
+            with open(id_mapping_path, 'r') as f:
+                id_mapping = json.load(f)
+            return id_mapping
 
-def get_label(label_file: Path):
-    target = Path(label_file).read_text()
+        else:
+            raise ValueError(f"Unsupported id_mapping value {self.conf_data.id_mapping}")
 
-    if target == '': # target label can be empty string
-        target_array = np.zeros((0, 5))
-    else:
-        try:
-            target_array = np.array([list(map(float, box.split(' '))) for box in target.split('\n') if box.strip()])
-        except ValueError as e:
-            print(target)
-            raise e
+    def load_class_map(self, id_mapping):
+        idx_to_class: Dict[int, str] = dict(enumerate(id_mapping))
+        return {'idx_to_class': idx_to_class}
 
-    label, boxes = target_array[:, 0], target_array[:, 1:]
-    label = label[..., np.newaxis]
-    return label, boxes
+    def load_huggingface_samples(self):
+        raise NotImplementedError
 
 
 class DetectionCustomDataset(BaseCustomDataset):
 
     def __init__(self, conf_data, conf_augmentation, model_name, idx_to_class,
-                 split, samples, transform=None, with_label=True, **kwargs):
+                 split, samples, transform=None, **kwargs):
         super(DetectionCustomDataset, self).__init__(
             conf_data, conf_augmentation, model_name, idx_to_class,
-            split, samples, transform, with_label, **kwargs
+            split, samples, transform, **kwargs,
         )
 
     @staticmethod
     def xywhn2xyxy(original: np.ndarray, w: int, h: int, padw=0, padh=0):
         converted = original.copy()
         # left, top (lt)
         converted[..., 0] = w * (original[..., 0] - original[..., 2] / 2) + padw
@@ -65,15 +103,15 @@
         if (not distributed) or (distributed and dist.get_rank() == 0):
             logger.info(f'Caching | Loading samples of {self.mode} to memory... This can take minutes.')
 
         def _load(i, samples):
             image = Image.open(Path(samples[i]['image'])).convert('RGB')
             label = self.samples[i]['label']
             if label is not None:
-                label = get_label(Path(label))
+                label = get_detection_label(Path(label))
             return i, image, label
 
         num_threads = 8 # TODO: Compute appropriate num_threads
         load_imgs = ThreadPool(num_threads).imap(
             partial(_load, samples=self.samples),
             sampler
         )
@@ -86,15 +124,15 @@
     def __getitem__(self, index):
         if self.cache:
             img = self.samples[index]['image']
             ann = self.samples[index]['label']
         else:
             img = Image.open(self.samples[index]['image']).convert('RGB')
             ann_path = Path(self.samples[index]['label']) if self.samples[index]['label'] is not None else None
-            ann = get_label(Path(ann_path)) if ann_path is not None else None
+            ann = get_detection_label(Path(ann_path)) if ann_path is not None else None
 
         w, h = img.size
 
         outputs = {}
         outputs.update({'indices': index})
         if ann is None:
             out = self.transform(image=img)
@@ -126,12 +164,11 @@
         img = Image.open(str(img_path)).convert('RGB')
 
         org_img = img.copy()
         w, h = img.size
         if ann_path is None:
             return org_img, np.zeros(0, 1), np.zeros(0, 5)
 
-        label, boxes_yolo = get_label(Path(ann_path))
+        label, boxes_yolo = get_detection_label(Path(ann_path))
         boxes = self.xywhn2xyxy(boxes_yolo, w, h)
 
         return org_img, label, boxes
-
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/loader.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/loader.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/sampler.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/dataloaders/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/evaluator_common.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/evaluator_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,15 @@
     if conf.distributed and conf.rank != 0:
         torch.distributed.barrier()  # wait for rank 0 to download dataset
 
     single_task_model = is_single_task_model(conf.model)
     conf.model.single_task_model = single_task_model
 
     # Build dataloader
-    _, _, test_dataset = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed)
-    assert test_dataset is not None, "For evaluation, valid split of dataset must be provided."
-    if not distributed or dist.get_rank() == 0:
-        logger.info(f"Summary | Dataset: <{conf.data.name}> (with {conf.data.format} format)")
-        logger.info(f"Summary | Validation dataset: {len(test_dataset)} sample(s)")
+    _, _, test_dataset = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed, mode='test')
 
     if conf.distributed and conf.rank == 0:
         torch.distributed.barrier()
 
     eval_dataloader = build_dataloader(conf, task, model_name, dataset=test_dataset, phase='val')
 
     # Build model
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/evaluator_main.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/evaluator_main.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/inferencer_common.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/inferencer_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,19 +41,15 @@
     if conf.distributed and conf.rank != 0:
         torch.distributed.barrier()  # wait for rank 0 to download dataset
 
     single_task_model = is_single_task_model(conf.model)
     conf.model.single_task_model = single_task_model
 
     # Build dataloader
-    _, _, test_dataset = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed)
-    assert test_dataset is not None, "For inference, test split of dataset must be provided."
-    if not distributed or dist.get_rank() == 0:
-        logger.info(f"Summary | Dataset: <{conf.data.name}> (with {conf.data.format} format)")
-        logger.info(f"Summary | Test dataset: {len(test_dataset)} sample(s)")
+    _, _, test_dataset = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed, mode='test')
 
     if conf.distributed and conf.rank == 0:
         torch.distributed.barrier()
 
     test_dataloader = build_dataloader(conf, task, model_name, dataset=test_dataset, phase='val')
 
     # Build model
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/inferencer_main.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/inferencer_main.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/base.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/base.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/builder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/builder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/image.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/image.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/stdout.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/tensorboard.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/visualizer.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/loggers/visualizer.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/builder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/losses/builder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/common.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/losses/common.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/retinanet.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/losses/detection/retinanet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/yolox.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/losses/detection/yolox.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/pose_estimation/rtmcc.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/losses/pose_estimation/rtmcc.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/pidnet.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/losses/segmentation/pidnet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/builder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/builder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/metric.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/classification/metric.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/metric.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/detection/metric.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/pose_estimation/metric.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/pose_estimation/metric.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/registry.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/registry.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/metric.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/metrics/segmentation/metric.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/resnet.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/core/resnet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/darknet.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/darknet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/efficientformer.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/efficientformer.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixnet.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mixnet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilevit.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/mobilevit.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/vit.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/backbones/experimental/vit.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/base.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/base.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/builder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/builder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/pidnet.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/full/experimental/pidnet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/core/fc.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/classification/core/fc.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/anchor_free_decoupled_head.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/anchor_free_decoupled_head.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/experimental/rtmcc.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/pose_estimation/experimental/rtmcc.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/fpn.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/experimental/fpn.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/yolopafpn.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/necks/experimental/yolopafpn.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/base_metaformer.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/base_metaformer.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/custom.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/custom.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/depth.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/depth.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/pidnet.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/op/pidnet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/registry.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/registry.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/models/utils.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/models/utils.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/builder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/optimizers/builder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/custom.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/optimizers/custom.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/base.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/builder.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/builder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/evaluation.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/evaluation.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/inference.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/inference.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/registry.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/registry.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/base.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         #TODO: Temporarily set ``mixed_precision`` as optional since this is experimental
         if hasattr(conf, 'training'):
             self.mixed_precision = conf.training.mixed_precision if hasattr(conf.training, 'mixed_precision') else False
         else:
             self.mixed_precision = False
         if self.mixed_precision:
             if self.single_gpu_or_rank_zero:
+                logger.info("-" * 40)
                 logger.info("Mixed precision training activated.")
             self.data_type = torch.float16
         else:
             self.data_type = torch.float32
         self.grad_scaler = torch.cuda.amp.GradScaler(enabled=self.mixed_precision)
 
     @abstractmethod
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/classification.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/classification.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/detection.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/detection.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/pose_estimation.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/segmentation.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/task_processors/segmentation.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/train.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/pipelines/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,18 +133,18 @@
                 time_for_epoch = self.timer.get(name=f'train_epoch_{num_epoch}', as_pop=False)
 
                 if self.single_gpu_or_rank_zero:
                     self.log_end_epoch(epoch=num_epoch,
                                        time_for_epoch=time_for_epoch,
                                        valid_samples=valid_samples,
                                        valid_logging=with_valid_logging)
+                    self.save_summary()
                     if with_checkpoint_saving:
                         assert with_valid_logging
                         self.save_checkpoint(epoch=num_epoch)
-                        self.save_summary()
                     logger.info("-" * 40)
 
                 self.scheduler.step()  # call after reporting the current `learning_rate`
 
             self.timer.end_record(name='train_all')
             total_train_time = self.timer.get(name='train_all', as_pop=False)
             logger.info(f"Total time: {total_train_time:.2f} s")
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/detection.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/detection.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/pose_estimation.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/register.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/postprocessors/registry.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/base.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/base.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_lr.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_warm_restart.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/cosine_warm_restart.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/poly_lr.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/poly_lr.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/registry.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/step_lr.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/schedulers/step_lr.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/trainer_common.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/trainer_common.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,21 +38,15 @@
     if conf.distributed and conf.rank != 0:
         torch.distributed.barrier()  # wait for rank 0 to download dataset
 
     single_task_model = is_single_task_model(conf.model)
     conf.model.single_task_model = single_task_model
 
     # Build dataloaders
-    train_dataset, valid_dataset, _ = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed)
-    assert train_dataset is not None, "For training, train split of dataset must be provided."
-    if not distributed or dist.get_rank() == 0:
-        logger.info(f"Summary | Dataset: <{conf.data.name}> (with {conf.data.format} format)")
-        logger.info(f"Summary | Training dataset: {len(train_dataset)} sample(s)")
-        if valid_dataset is not None:
-            logger.info(f"Summary | Validation dataset: {len(valid_dataset)} sample(s)")
+    train_dataset, valid_dataset, _ = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed, mode='train')
 
     # TODO: Temporarily set batch_size in train_dataset for RandomResize. This better to be removed later.
     train_dataset.batch_size = conf.environment.batch_size
 
     if conf.distributed and conf.rank == 0:
         torch.distributed.barrier()
```

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/trainer_main.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/trainer_main.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/checkpoint.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/engine_utils.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/engine_utils.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/environment.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/environment.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/fx.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/fx.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/logger.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/logger.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/model_ema.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/model_ema.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/onnx.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/record.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/record.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/stats.py` & `netspresso_trainer-0.2.1/src/netspresso_trainer/utils/stats.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/SOURCES.txt` & `netspresso_trainer-0.2.1/src/netspresso_trainer.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,37 +15,28 @@
 src/netspresso_trainer.egg-info/dependency_links.txt
 src/netspresso_trainer.egg-info/entry_points.txt
 src/netspresso_trainer.egg-info/requires.txt
 src/netspresso_trainer.egg-info/top_level.txt
 src/netspresso_trainer/dataloaders/__init__.py
 src/netspresso_trainer/dataloaders/base.py
 src/netspresso_trainer/dataloaders/builder.py
+src/netspresso_trainer/dataloaders/classification.py
+src/netspresso_trainer/dataloaders/detection.py
+src/netspresso_trainer/dataloaders/pose_estimation.py
 src/netspresso_trainer/dataloaders/registry.py
+src/netspresso_trainer/dataloaders/segmentation.py
 src/netspresso_trainer/dataloaders/augmentation/__init__.py
 src/netspresso_trainer/dataloaders/augmentation/registry.py
 src/netspresso_trainer/dataloaders/augmentation/transforms.py
 src/netspresso_trainer/dataloaders/augmentation/custom/__init__.py
 src/netspresso_trainer/dataloaders/augmentation/custom/image_proc.py
 src/netspresso_trainer/dataloaders/augmentation/custom/mixing.py
 src/netspresso_trainer/dataloaders/augmentation/custom/mosaic.py
-src/netspresso_trainer/dataloaders/classification/__init__.py
-src/netspresso_trainer/dataloaders/classification/dataset.py
-src/netspresso_trainer/dataloaders/classification/huggingface.py
-src/netspresso_trainer/dataloaders/classification/local.py
-src/netspresso_trainer/dataloaders/detection/__init__.py
-src/netspresso_trainer/dataloaders/detection/dataset.py
-src/netspresso_trainer/dataloaders/detection/local.py
-src/netspresso_trainer/dataloaders/pose_estimation/__init__.py
-src/netspresso_trainer/dataloaders/pose_estimation/dataset.py
-src/netspresso_trainer/dataloaders/pose_estimation/local.py
-src/netspresso_trainer/dataloaders/segmentation/__init__.py
-src/netspresso_trainer/dataloaders/segmentation/dataset.py
-src/netspresso_trainer/dataloaders/segmentation/huggingface.py
-src/netspresso_trainer/dataloaders/segmentation/local.py
 src/netspresso_trainer/dataloaders/utils/__init__.py
+src/netspresso_trainer/dataloaders/utils/collate_fn.py
 src/netspresso_trainer/dataloaders/utils/constants.py
 src/netspresso_trainer/dataloaders/utils/loader.py
 src/netspresso_trainer/dataloaders/utils/misc.py
 src/netspresso_trainer/dataloaders/utils/sampler.py
 src/netspresso_trainer/loggers/__init__.py
 src/netspresso_trainer/loggers/base.py
 src/netspresso_trainer/loggers/builder.py
@@ -148,15 +139,15 @@
 src/netspresso_trainer/pipelines/task_processors/pose_estimation.py
 src/netspresso_trainer/pipelines/task_processors/segmentation.py
 src/netspresso_trainer/postprocessors/__init__.py
 src/netspresso_trainer/postprocessors/builder.py
 src/netspresso_trainer/postprocessors/classification.py
 src/netspresso_trainer/postprocessors/detection.py
 src/netspresso_trainer/postprocessors/pose_estimation.py
-src/netspresso_trainer/postprocessors/register.py
+src/netspresso_trainer/postprocessors/registry.py
 src/netspresso_trainer/postprocessors/segmentation.py
 src/netspresso_trainer/schedulers/__init__.py
 src/netspresso_trainer/schedulers/base.py
 src/netspresso_trainer/schedulers/builder.py
 src/netspresso_trainer/schedulers/cosine_lr.py
 src/netspresso_trainer/schedulers/cosine_warm_restart.py
 src/netspresso_trainer/schedulers/poly_lr.py
```

