# Comparing `tmp/torchaug-0.4.2.tar.gz` & `tmp/torchaug-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchaug-0.4.2.tar", last modified: Wed Mar 20 23:36:35 2024, max compression
+gzip compressed data, was "torchaug-0.5.0.tar", last modified: Fri May  3 15:08:44 2024, max compression
```

## Comparing `torchaug-0.4.2.tar` & `torchaug-0.5.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.173955 torchaug-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    21760 2024-03-20 23:36:25.000000 torchaug-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-20 23:36:35.173955 torchaug-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-20 23:36:25.000000 torchaug-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-20 23:36:25.000000 torchaug-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-20 23:36:25.000000 torchaug-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 23:36:35.173955 torchaug-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.161955 torchaug-0.4.2/torchaug/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.165955 torchaug-0.4.2/torchaug/data/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.165955 torchaug-0.4.2/torchaug/data/dataloader/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/data/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/data/dataloader/_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.165955 torchaug-0.4.2/torchaug/data/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/data/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24651 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/data/dataset/_dataset_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.169955 torchaug-0.4.2/torchaug/ta_tensors/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_batch_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_batch_concatenated_ta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_batch_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_batch_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_batch_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_batch_videos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_ta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_torch_function_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/ta_tensors/_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.169955 torchaug-0.4.2/torchaug/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    33048 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    29002 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    67947 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    20560 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19790 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.169955 torchaug-0.4.2/torchaug/transforms/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21567 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    50391 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.173955 torchaug-0.4.2/torchaug/transforms/functional/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_utils/_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-03-20 23:36:25.000000 torchaug-0.4.2/torchaug/transforms/functional/_utils/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:36:35.173955 torchaug-0.4.2/torchaug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-20 23:36:35.000000 torchaug-0.4.2/torchaug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-20 23:36:35.000000 torchaug-0.4.2/torchaug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 23:36:35.000000 torchaug-0.4.2/torchaug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-20 23:36:35.000000 torchaug-0.4.2/torchaug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 23:36:35.000000 torchaug-0.4.2/torchaug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 23:36:34.000000 torchaug-0.4.2/torchaug.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.145990 torchaug-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    21760 2024-05-03 15:08:39.000000 torchaug-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-03 15:08:44.145990 torchaug-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-03 15:08:39.000000 torchaug-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-03 15:08:39.000000 torchaug-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 15:08:39.000000 torchaug-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:08:44.145990 torchaug-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.137990 torchaug-0.5.0/torchaug/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.137990 torchaug-0.5.0/torchaug/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.137990 torchaug-0.5.0/torchaug/data/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/data/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/data/dataloader/_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.137990 torchaug-0.5.0/torchaug/data/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/data/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24651 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/data/dataset/_dataset_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.141990 torchaug-0.5.0/torchaug/ta_tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_batch_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_batch_concatenated_ta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_batch_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_batch_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_batch_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_batch_videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_ta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_torch_function_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/ta_tensors/_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.145990 torchaug-0.5.0/torchaug/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33048 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29442 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67947 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20555 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19790 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.145990 torchaug-0.5.0/torchaug/transforms/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22689 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50373 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.145990 torchaug-0.5.0/torchaug/transforms/functional/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_utils/_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-03 15:08:39.000000 torchaug-0.5.0/torchaug/transforms/functional/_utils/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:08:44.145990 torchaug-0.5.0/torchaug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-03 15:08:44.000000 torchaug-0.5.0/torchaug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-03 15:08:44.000000 torchaug-0.5.0/torchaug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:08:44.000000 torchaug-0.5.0/torchaug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 15:08:44.000000 torchaug-0.5.0/torchaug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 15:08:44.000000 torchaug-0.5.0/torchaug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:08:43.000000 torchaug-0.5.0/torchaug.egg-info/zip-safe
```

### Comparing `torchaug-0.4.2/LICENSE` & `torchaug-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/PKG-INFO` & `torchaug-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchaug
-Version: 0.4.2
+Version: 0.5.0
 Summary: Torchvision Complementary tool to perform batch and GPU data augmentations.
 Author-email: Julien Denize <julien.denize@cea.fr>
 Project-URL: Bug Tracker, https://github.com/juliendenize/torchaug/issues
 Project-URL: Download, https://github.com/juliendenize/torchaug
 Project-URL: Homepage, https://github.com/juliendenize/torchaug
 Project-URL: Source Code, https://github.com/juliendenize/torchaug
 Keywords: computer vision,deep learning,pytorch
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torchvision==0.17.1
+Requires-Dist: torchvision==0.18.0
 
 **Efficient vision data augmentations for CPU/GPU per-sample/batched data.**
 
 ***Under active development, subject to API change***
 
 [![PyPI python](https://img.shields.io/pypi/pyversions/torchaug)](https://pypi.org/project/torchaug)
 [![PyPI version](https://badge.fury.io/py/torchaug.svg)](https://pypi.org/project/torchaug)
@@ -54,15 +54,15 @@
 - For data augmentations applied on batch, the *randomness is sampled for the whole batch* and not each sample.
 
 Torchaug removes these issues and its transforms are meant to be used in place of Torchvision. It is based on the code base of Torchvision and therefore follows the same nomenclature as Torchvision with *functional* augmentations and *transforms* class wrappers. However, **Torchaug does not support transforms on Pillow images**.
 
 More details can be found in the [documentation](https://torchaug.readthedocs.io/en/).
 
 
-To be sure to retrieve the same data augmentations as Torchvision, **the components are tested to match Torchvision outputs**. We made a speed comparison [here](./docs/source/include/comparison.md).
+To be sure to retrieve the same data augmentations as Torchvision, **the components are tested to match Torchvision outputs**. We made a speed comparison [here](./docs/source/include/speed_comparison.md).
 
 
 If you find any unexpected behavior or want to suggest a change please open an issue.
 
 ## How to use
 
 1. Install Torchaug.
```

### Comparing `torchaug-0.4.2/README.md` & `torchaug-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 - For data augmentations applied on batch, the *randomness is sampled for the whole batch* and not each sample.
 
 Torchaug removes these issues and its transforms are meant to be used in place of Torchvision. It is based on the code base of Torchvision and therefore follows the same nomenclature as Torchvision with *functional* augmentations and *transforms* class wrappers. However, **Torchaug does not support transforms on Pillow images**.
 
 More details can be found in the [documentation](https://torchaug.readthedocs.io/en/).
 
 
-To be sure to retrieve the same data augmentations as Torchvision, **the components are tested to match Torchvision outputs**. We made a speed comparison [here](./docs/source/include/comparison.md).
+To be sure to retrieve the same data augmentations as Torchvision, **the components are tested to match Torchvision outputs**. We made a speed comparison [here](./docs/source/include/speed_comparison.md).
 
 
 If you find any unexpected behavior or want to suggest a change please open an issue.
 
 ## How to use
 
 1. Install Torchaug.
```

### Comparing `torchaug-0.4.2/pyproject.toml` & `torchaug-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/_utils.py` & `torchaug-0.5.0/torchaug/_utils.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/data/dataloader/_collate.py` & `torchaug-0.5.0/torchaug/data/dataloader/_collate.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/data/dataset/_dataset_wrapper.py` & `torchaug-0.5.0/torchaug/data/dataset/_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/__init__.py` & `torchaug-0.5.0/torchaug/ta_tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_batch_bounding_boxes.py` & `torchaug-0.5.0/torchaug/ta_tensors/_batch_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_batch_concatenated_ta_tensor.py` & `torchaug-0.5.0/torchaug/ta_tensors/_batch_concatenated_ta_tensor.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_batch_images.py` & `torchaug-0.5.0/torchaug/ta_tensors/_batch_images.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_batch_labels.py` & `torchaug-0.5.0/torchaug/ta_tensors/_batch_labels.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_batch_masks.py` & `torchaug-0.5.0/torchaug/ta_tensors/_batch_masks.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_batch_videos.py` & `torchaug-0.5.0/torchaug/ta_tensors/_batch_videos.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_bounding_boxes.py` & `torchaug-0.5.0/torchaug/ta_tensors/_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_image.py` & `torchaug-0.5.0/torchaug/ta_tensors/_image.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_labels.py` & `torchaug-0.5.0/torchaug/ta_tensors/_labels.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_mask.py` & `torchaug-0.5.0/torchaug/ta_tensors/_mask.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_ta_tensor.py` & `torchaug-0.5.0/torchaug/ta_tensors/_ta_tensor.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_torch_function_helpers.py` & `torchaug-0.5.0/torchaug/ta_tensors/_torch_function_helpers.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_video.py` & `torchaug-0.5.0/torchaug/ta_tensors/_video.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/ta_tensors/_wrap.py` & `torchaug-0.5.0/torchaug/ta_tensors/_wrap.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/__init__.py` & `torchaug-0.5.0/torchaug/transforms/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 # ruff: noqa: F401
 # ruff: noqa: D104
 
 from torchvision.transforms import AutoAugmentPolicy, InterpolationMode
 
 from . import functional
-from ._augment import CutMix, MixUp, RandomErasing
+from ._augment import JPEG, CutMix, MixUp, RandomErasing
 from ._auto_augment import AugMix, AutoAugment, RandAugment, TrivialAugmentWide
 from ._color import (
+    RGB,
     ColorJitter,
     Grayscale,
     RandomAdjustSharpness,
     RandomAutocontrast,
     RandomChannelPermutation,
     RandomColorJitter,
     RandomEqualize,
```

### Comparing `torchaug-0.4.2/torchaug/transforms/_augment.py` & `torchaug-0.5.0/torchaug/transforms/_augment.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #
 # Code partially based on Torchvision (BSD 3-Clause License), available at:
 #   https://github.com/pytorch/vision
 
 import math
 import numbers
 import warnings
-from typing import Any, Callable, Dict, List, Tuple
+from typing import Any, Callable, Dict, List, Sequence, Tuple, Union
 
 import torch
 from torch.nn.functional import one_hot
 from torch.utils._pytree import tree_flatten, tree_unflatten
-from torchvision.transforms.v2._utils import _parse_labels_getter, has_any, query_chw
+from torchvision.transforms.v2._utils import _check_sequence_input, _parse_labels_getter, has_any, query_chw
 
 from torchaug import ta_tensors
 
 from . import functional as F
 from ._transform import RandomApplyTransform, Transform
 from ._utils import is_pure_tensor, query_size
 
@@ -161,14 +161,56 @@
                 **params,
                 inplace=self.inplace,
             )
 
         return inpt
 
 
+class JPEG(Transform):
+    """Apply JPEG compression and decompression to the given images.
+    The input is expected to be of a tensor of dtype uint8, on CPU, and have [..., 3 or 1, H, W] shape,
+    where ... means an arbitrary number of leading dimensions.
+
+    Args:
+        quality: JPEG quality, from 1 to 100. Lower means more compression.
+            If quality is a sequence like (min, max), it specifies the range of JPEG quality to
+            randomly select from (inclusive of both ends).
+
+    Returns:
+        image with JPEG compression.
+    """
+
+    def __init__(self, quality: Union[int, Sequence[int]]):
+        super().__init__()
+        if isinstance(quality, int):
+            quality = [quality, quality]
+        else:
+            _check_sequence_input(quality, "quality", req_sizes=(2,))
+
+        if not (1 <= quality[0] <= quality[1] <= 100 and isinstance(quality[0], int) and isinstance(quality[1], int)):
+            raise ValueError(f"quality must be an integer from 1 to 100, got {quality =}")
+
+        self.quality = quality
+
+    def _get_params(
+        self,
+        flat_inputs: List[Any],
+        num_chunks: int,
+        chunks_indices: Tuple[torch.Tensor],
+    ) -> List[Dict[str, Any]]:
+        params: List[Dict[str, Any]] = []
+        for i in range(num_chunks):
+            quality = torch.randint(self.quality[0], self.quality[1] + 1, ()).item()
+            params.append({"quality": quality})
+        return params
+
+    def _transform(self, inpt: Any, params: Dict[str, Any]) -> Any:
+        return self._call_kernel(F.jpeg, inpt, quality=params["quality"])
+
+
 class _BaseMixUpCutMix(Transform):
     def __init__(self, *, alpha: float = 1.0, num_classes: int, labels_getter="default") -> None:
         super().__init__(batch_transform=True)
         self.alpha = float(alpha)
         self._dist = torch.distributions.Beta(torch.tensor([alpha]), torch.tensor([alpha]))
 
         self.num_classes = num_classes
```

### Comparing `torchaug-0.4.2/torchaug/transforms/_auto_augment.py` & `torchaug-0.5.0/torchaug/transforms/_auto_augment.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/_color.py` & `torchaug-0.5.0/torchaug/transforms/_color.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,28 @@
             num_output_channels=self.num_output_channels,
         )
 
     def extra_repr(self) -> str:  # type: ignore[override]
         return super().extra_repr(exclude_names=["num_chunks", "permute_chunks"])
 
 
+class RGB(Transform):
+    """Convert images or videos to RGB (if they are already not RGB).
+
+    If the input is a :class:`torch.Tensor`, it is expected
+    to have [..., 1 or 3, H, W] shape, where ... means an arbitrary number of leading dimensions
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def _transform(self, inpt: Any, params: Dict[str, Any]) -> Any:
+        return self._call_kernel(F.grayscale_to_rgb, inpt)
+
+
 class RandomGrayscale(RandomApplyTransform):
     """Randomly convert image or videos to grayscale with a probability of p.
 
     The input is expected to have [..., 3 or 1, H, W] shape,
     where ... means an arbitrary number of leading dimensions
 
     The output has the same number of channels as the input.
```

### Comparing `torchaug-0.4.2/torchaug/transforms/_container.py` & `torchaug-0.5.0/torchaug/transforms/_container.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/_geometry.py` & `torchaug-0.5.0/torchaug/transforms/_geometry.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/_meta.py` & `torchaug-0.5.0/torchaug/transforms/_meta.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/_misc.py` & `torchaug-0.5.0/torchaug/transforms/_misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -440,41 +440,51 @@
             It can also be a callable that takes the same input
             as the transform, and returns the labels.
     """
 
     def __init__(
         self,
         min_size: float = 1.0,
-        labels_getter: Optional[Union[Callable[[Any], Optional[torch.Tensor]], str]] = "default",
+        labels_getter: Union[Callable[[Any], Any], str, None] = "default",
     ) -> None:
         super().__init__()
 
         if min_size < 1:
             raise ValueError(f"min_size must be >= 1, got {min_size}.")
         self.min_size = min_size
 
         self.labels_getter = labels_getter
         self._labels_getter = _parse_labels_getter(labels_getter)
 
     def forward(self, *inputs: Any) -> Any:
         inputs = inputs if len(inputs) > 1 else inputs[0]
 
         labels = self._labels_getter(inputs)
-        if labels is not None and not isinstance(labels, torch.Tensor):
-            raise ValueError(
-                f"The labels in the input to forward() must be a tensor or None, got {type(labels)} instead."
-            )
+        if labels is not None:
+            msg = "The labels in the input to forward() must be a tensor or None, got {type} instead."
+            if isinstance(labels, torch.Tensor):
+                labels = (labels,)
+            elif isinstance(labels, (tuple, list)):
+                for entry in labels:
+                    if not isinstance(entry, torch.Tensor):
+                        # TODO: we don't need to enforce tensors, just that entries are indexable as t[bool_mask]
+                        raise ValueError(msg.format(type=type(entry)))
+            else:
+                raise ValueError(msg.format(type=type(labels)))
 
         flat_inputs, spec = tree_flatten(inputs)
         boxes = get_sample_or_batch_bounding_boxes(flat_inputs)
 
-        if labels is not None and boxes.shape[0] != labels.shape[0]:
-            raise ValueError(
-                f"Number of boxes (shape={boxes.shape}) and number of labels (shape={labels.shape}) do not match."
-            )
+        if labels is not None:
+            for label in labels:
+                if boxes.shape[0] != label.shape[0]:
+                    raise ValueError(
+                        f"Number of boxes (shape={boxes.shape}) and must match the number of labels."
+                        f"Found labels with shape={label.shape})."
+                    )
 
         is_batch_boxes = isinstance(boxes, ta_tensors.BatchBoundingBoxes)
 
         if not is_batch_boxes:
             boxes = cast(
                 ta_tensors.BoundingBoxes,
                 F.convert_bounding_box_format(
@@ -487,34 +497,27 @@
                 ta_tensors.BatchBoundingBoxes,
                 F.convert_bounding_box_format(
                     boxes,
                     new_format=ta_tensors.BoundingBoxFormat.XYXY,
                 ),
             )
 
-        ws, hs = boxes[:, 2] - boxes[:, 0], boxes[:, 3] - boxes[:, 1]
-        valid = (ws >= self.min_size) & (hs >= self.min_size) & (boxes >= 0).all(dim=-1)  # type: ignore[attr-defined]
-        # TODO: Do we really need to check for out of bounds here? All
-        # transforms should be clamping anyway, so this should never happen?
-        image_h, image_w = boxes.canvas_size
-        valid &= (boxes[:, 0] <= image_w) & (boxes[:, 2] <= image_w)
-        valid &= (boxes[:, 1] <= image_h) & (boxes[:, 3] <= image_h)
-
-        params = {"valid": valid.as_subclass(torch.Tensor), "labels": labels}
-        flat_outputs = [
-            # Even-though it may look like we're transforming all inputs, we don't:
-            # _transform() will only care about BoundingBoxeses and the labels
-            self._transform(inpt, params)
-            for inpt in flat_inputs
-        ]
+        valid = F._misc._get_sanitize_bounding_boxes_mask(
+            boxes,
+            format=boxes.format,
+            canvas_size=boxes.canvas_size,
+            min_size=self.min_size,
+        )
+        params = {"valid": valid, "labels": labels}
+        flat_outputs = [self._transform(inpt, params) for inpt in flat_inputs]
 
         return tree_unflatten(flat_outputs, spec)
 
     def _transform(self, inpt: Any, params: Dict[str, Any]) -> Any:
-        is_label = inpt is not None and inpt is params["labels"]
+        is_label = params["labels"] is not None and any(inpt is label for label in params["labels"])
         is_bounding_boxes = isinstance(inpt, (ta_tensors.BoundingBoxes, ta_tensors.BatchBoundingBoxes))
         is_mask = isinstance(inpt, (ta_tensors.Mask, ta_tensors.BatchMasks))
         is_bounding_boxes_or_mask = is_bounding_boxes or is_mask
 
         if not (is_label or is_bounding_boxes_or_mask):
             return inpt
```

### Comparing `torchaug-0.4.2/torchaug/transforms/_temporal.py` & `torchaug-0.5.0/torchaug/transforms/_temporal.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/_transform.py` & `torchaug-0.5.0/torchaug/transforms/_transform.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/_type_conversion.py` & `torchaug-0.5.0/torchaug/transforms/_type_conversion.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/_utils.py` & `torchaug-0.5.0/torchaug/transforms/_utils.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/__init__.py` & `torchaug-0.5.0/torchaug/transforms/functional/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @License: CECILL-C
 
 # ruff: noqa: F401
 # ruff: noqa: D104
 
 from torchvision.transforms import InterpolationMode
 
-from ._augment import erase, erase_image, erase_video
+from ._augment import erase, erase_image, erase_video, jpeg, jpeg_image, jpeg_video
 from ._color import (
     adjust_brightness,
     adjust_brightness_batch,
     adjust_brightness_batch_images,
     adjust_brightness_batch_videos,
     adjust_brightness_image,
     adjust_brightness_video,
@@ -41,14 +41,17 @@
     adjust_sharpness_video,
     autocontrast,
     autocontrast_image,
     autocontrast_video,
     equalize,
     equalize_image,
     equalize_video,
+    grayscale_to_rgb,
+    grayscale_to_rgb_image,
+    grayscale_to_rgb_video,
     invert,
     invert_image,
     invert_video,
     permute_channels,
     permute_channels_image,
     permute_channels_video,
     posterize,
@@ -152,14 +155,15 @@
     gaussian_blur_batch_images,
     gaussian_blur_batch_videos,
     gaussian_blur_image,
     gaussian_blur_video,
     normalize,
     normalize_image,
     normalize_video,
+    sanitize_bounding_boxes,
     to_dtype,
     to_dtype_image,
     to_dtype_video,
 )
 from ._temporal import uniform_temporal_subsample, uniform_temporal_subsample_video
 from ._type_conversion import to_batch_images, to_image
 from ._utils import is_pure_tensor, register_kernel
```

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_augment.py` & `torchaug-0.5.0/torchaug/transforms/functional/_augment.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Code partially based on Torchvision (BSD 3-Clause License), available at:
 #   https://github.com/pytorch/vision
 
 from __future__ import annotations
 
 import torch
 import torchvision.transforms.v2.functional as TVF
+from torchvision.io import decode_jpeg, encode_jpeg
 
 from torchaug import ta_tensors
 from torchaug._utils import _log_api_usage_once
 
 from ._utils._kernel import _get_kernel, _register_kernel_internal
 
 
@@ -58,7 +59,39 @@
     j: int,
     h: int,
     w: int,
     v: torch.Tensor,
     inplace: bool = False,
 ) -> torch.Tensor:
     return erase_image(image=video, i=i, j=j, h=h, w=w, v=v, inplace=inplace)
+
+
+def jpeg(image: torch.Tensor, quality: int) -> torch.Tensor:
+    """See :class:`~torchaug.transforms.JPEG` for details."""
+    if torch.jit.is_scripting():
+        return jpeg_image(image, quality=quality)
+
+    _log_api_usage_once(jpeg)
+
+    kernel = _get_kernel(jpeg, type(image))
+    return kernel(image, quality=quality)
+
+
+@_register_kernel_internal(jpeg, torch.Tensor)
+@_register_kernel_internal(jpeg, ta_tensors.Image)
+@_register_kernel_internal(jpeg, ta_tensors.BatchImages)
+def jpeg_image(image: torch.Tensor, quality: int) -> torch.Tensor:
+    original_shape = image.shape
+    image = image.view((-1,) + image.shape[-3:])
+
+    if image.shape[0] == 0:  # degenerate
+        return image.reshape(original_shape).clone()
+
+    image_list = [decode_jpeg(encode_jpeg(image[i], quality=quality)) for i in range(image.shape[0])]
+    image = torch.stack(image_list, dim=0).view(original_shape)
+    return image
+
+
+@_register_kernel_internal(jpeg, ta_tensors.Video)
+@_register_kernel_internal(jpeg, ta_tensors.BatchVideos)
+def jpeg_video(video: torch.Tensor, quality: int) -> torch.Tensor:
+    return jpeg_image(video, quality=quality)
```

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_color.py` & `torchaug-0.5.0/torchaug/transforms/functional/_color.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,42 @@
 
 @_register_kernel_internal(rgb_to_grayscale, ta_tensors.Video)
 @_register_kernel_internal(rgb_to_grayscale, ta_tensors.BatchVideos)
 def rgb_to_grayscale_video(video: torch.Tensor, num_output_channels: int = 1) -> torch.Tensor:
     return rgb_to_grayscale_image(image=video, num_output_channels=num_output_channels)
 
 
+def grayscale_to_rgb(inpt: torch.Tensor) -> torch.Tensor:
+    """See :class:`~torchvision.transforms.v2.GrayscaleToRgb` for details."""
+    if torch.jit.is_scripting():
+        return grayscale_to_rgb_image(inpt)
+
+    _log_api_usage_once(grayscale_to_rgb)
+
+    kernel = _get_kernel(grayscale_to_rgb, type(inpt))
+    return kernel(inpt)
+
+
+@_register_kernel_internal(grayscale_to_rgb, torch.Tensor)
+@_register_kernel_internal(grayscale_to_rgb, ta_tensors.Image)
+@_register_kernel_internal(grayscale_to_rgb, ta_tensors.BatchImages)
+def grayscale_to_rgb_image(image: torch.Tensor) -> torch.Tensor:
+    if image.shape[-3] >= 3:
+        # Image already has RGB channels. We don't need to do anything.
+        return image
+    # rgb_to_grayscale can be used to add channels so we reuse that function.
+    return _rgb_to_grayscale_image(image, num_output_channels=3, preserve_dtype=True)
+
+
+@_register_kernel_internal(grayscale_to_rgb, ta_tensors.Video)
+@_register_kernel_internal(grayscale_to_rgb, ta_tensors.BatchVideos)
+def grayscale_to_rgb_video(video: torch.Tensor) -> torch.Tensor:
+    return grayscale_to_rgb_image(video)
+
+
 def _batch_blend(images1: torch.Tensor, images2: torch.Tensor, ratio: torch.Tensor) -> torch.Tensor:
     ratio = ratio.float()
     fp = images1.is_floating_point()
     bound = _max_value(images1.dtype)
     while ratio.ndim < images1.ndim:
         ratio = ratio.unsqueeze(-1)
     output = images1.mul(ratio).add_(images2.mul(1.0 - ratio)).clamp_(0, bound)
```

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_geometry.py` & `torchaug-0.5.0/torchaug/transforms/functional/_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -964,16 +964,15 @@
     # Fill with required color
     if fill is not None:
         float_images, mask = torch.tensor_split(float_images, indices=(-1,), dim=-3)
         mask = mask.expand_as(float_images)
         fill_list = fill if isinstance(fill, (tuple, list)) else [float(fill)]  # type: ignore[arg-type]
         fill_images = torch.tensor(fill_list, dtype=float_images.dtype, device=float_images.device).view(1, -1, 1, 1)
         if mode == "nearest":
-            bool_mask = mask < 0.5
-            float_images[bool_mask] = fill_images.expand_as(float_images)[bool_mask]
+            float_images = torch.where(mask < 0.5, fill_images.expand_as(float_images), float_images)
         else:  # 'bilinear'
             # The following is mathematically equivalent to:
             # images * mask + (1.0 - mask) * fill = images * mask - fill * mask + fill = mask * (images - fill) + fill
             float_images = float_images.sub_(fill_images).mul_(mask).add_(fill_images)
 
     images = float_images.round_().to(images.dtype) if not fp else float_images
```

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_meta.py` & `torchaug-0.5.0/torchaug/transforms/functional/_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,17 +160,17 @@
     if new_format is None:
         raise TypeError("convert_bounding_box_format() missing 1 required argument: 'new_format'")
 
     if not torch.jit.is_scripting():
         _log_api_usage_once(convert_bounding_box_format)
 
     if isinstance(old_format, str):
-        old_format = ta_tensors.BoundingBoxFormat[old_format.upper()]  # type: ignore[misc]
+        old_format = ta_tensors.BoundingBoxFormat[old_format.upper()]
     if isinstance(new_format, str):
-        new_format = ta_tensors.BoundingBoxFormat[new_format.upper()]  # type: ignore[misc]
+        new_format = ta_tensors.BoundingBoxFormat[new_format.upper()]
 
     if torch.jit.is_scripting() or is_pure_tensor(inpt):
         if old_format is None:
             raise ValueError("For pure tensor inputs, `old_format` has to be passed.")
         return _convert_bounding_box_format(inpt, old_format=old_format, new_format=new_format, inplace=inplace)
     elif isinstance(inpt, (ta_tensors.BoundingBoxes, ta_tensors.BatchBoundingBoxes)):
         if old_format is not None:
```

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_temporal.py` & `torchaug-0.5.0/torchaug/transforms/functional/_temporal.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_type_conversion.py` & `torchaug-0.5.0/torchaug/transforms/functional/_type_conversion.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_utils/__init__.py` & `torchaug-0.5.0/torchaug/transforms/functional/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_utils/_kernel.py` & `torchaug-0.5.0/torchaug/transforms/functional/_utils/_kernel.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug/transforms/functional/_utils/_tensor.py` & `torchaug-0.5.0/torchaug/transforms/functional/_utils/_tensor.py`

 * *Files identical despite different names*

### Comparing `torchaug-0.4.2/torchaug.egg-info/PKG-INFO` & `torchaug-0.5.0/torchaug.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchaug
-Version: 0.4.2
+Version: 0.5.0
 Summary: Torchvision Complementary tool to perform batch and GPU data augmentations.
 Author-email: Julien Denize <julien.denize@cea.fr>
 Project-URL: Bug Tracker, https://github.com/juliendenize/torchaug/issues
 Project-URL: Download, https://github.com/juliendenize/torchaug
 Project-URL: Homepage, https://github.com/juliendenize/torchaug
 Project-URL: Source Code, https://github.com/juliendenize/torchaug
 Keywords: computer vision,deep learning,pytorch
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torchvision==0.17.1
+Requires-Dist: torchvision==0.18.0
 
 **Efficient vision data augmentations for CPU/GPU per-sample/batched data.**
 
 ***Under active development, subject to API change***
 
 [![PyPI python](https://img.shields.io/pypi/pyversions/torchaug)](https://pypi.org/project/torchaug)
 [![PyPI version](https://badge.fury.io/py/torchaug.svg)](https://pypi.org/project/torchaug)
@@ -54,15 +54,15 @@
 - For data augmentations applied on batch, the *randomness is sampled for the whole batch* and not each sample.
 
 Torchaug removes these issues and its transforms are meant to be used in place of Torchvision. It is based on the code base of Torchvision and therefore follows the same nomenclature as Torchvision with *functional* augmentations and *transforms* class wrappers. However, **Torchaug does not support transforms on Pillow images**.
 
 More details can be found in the [documentation](https://torchaug.readthedocs.io/en/).
 
 
-To be sure to retrieve the same data augmentations as Torchvision, **the components are tested to match Torchvision outputs**. We made a speed comparison [here](./docs/source/include/comparison.md).
+To be sure to retrieve the same data augmentations as Torchvision, **the components are tested to match Torchvision outputs**. We made a speed comparison [here](./docs/source/include/speed_comparison.md).
 
 
 If you find any unexpected behavior or want to suggest a change please open an issue.
 
 ## How to use
 
 1. Install Torchaug.
```

### Comparing `torchaug-0.4.2/torchaug.egg-info/SOURCES.txt` & `torchaug-0.5.0/torchaug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

