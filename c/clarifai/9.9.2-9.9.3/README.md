# Comparing `tmp/clarifai-9.9.2.tar.gz` & `tmp/clarifai-9.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.9.2.tar", last modified: Wed Oct 11 14:34:25 2023, max compression
+gzip compressed data, was "clarifai-9.9.3.tar", last modified: Mon Oct 16 18:10:40 2023, max compression
```

## Comparing `clarifai-9.9.2.tar` & `clarifai-9.9.3.tar`

### file list

```diff
@@ -1,510 +1,510 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.292875 clarifai-9.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-10-11 14:34:12.000000 clarifai-9.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-10-11 14:34:12.000000 clarifai-9.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2023-10-11 14:34:25.292875 clarifai-9.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2023-10-11 14:34:12.000000 clarifai-9.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.236874 clarifai-9.9.2/clarifai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.236874 clarifai-9.9.2/clarifai/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13909 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/auth/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/auth/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/auth/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/client/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22809 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/client/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13909 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/auth/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/auth/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/auth/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14742 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    31391 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/lister.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/client/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/constants/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/datasets/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/export/inputs_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/datasets/upload/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/datasets/upload/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.240874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/cifar_small_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/cifar_small_train.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.244874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.244874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.224874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.244874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/
--rw-r--r--   0 runner    (1001) docker     (127)    49005 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    49264 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    43410 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    33826 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47755 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.244874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/
--rw-r--r--   0 runner    (1001) docker     (127)    43856 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47022 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    46176 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    37327 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    32557 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.248874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/
--rw-r--r--   0 runner    (1001) docker     (127)    26278 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    45386 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    40566 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47620 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    52635 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.248874 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/
--rw-r--r--   0 runner    (1001) docker     (127)    44858 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    49950 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    51306 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    34567 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    56869 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.248874 clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.248874 clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   237144 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)   270347 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/train.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.248874 clarifai-9.9.2/clarifai/datasets/upload/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/loaders/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/loaders/coco_captions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/loaders/coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/loaders/coco_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/loaders/imagenet_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/loaders/xview_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/datasets/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.248874 clarifai-9.9.2/clarifai/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/cli/model_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/cli/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/docs/custom_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/docs/dependencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/docs/model_types.md
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/docs/output.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.252874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_embedding/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.256874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.260874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.260874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.260874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.260874 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.260874 clarifai-9.9.2/clarifai/models/model_serving/model_config/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.260874 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/text-classifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/text-embedder.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/text-to-image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/text-to-text.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/visual-classifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/visual-detector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/visual-embedder.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/visual-segmenter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/model_config/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.260874 clarifai-9.9.2/clarifai/models/model_serving/models/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/models/default_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/models/model_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/models/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/models/pb_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/models/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/modules/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/modules/css.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/modules/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/modules/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/runners/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/schema/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai/urls/
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/urls/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/workflows/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/workflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai/workflows/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.236874 clarifai-9.9.2/clarifai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2023-10-11 14:34:25.000000 clarifai-9.9.2/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24579 2023-10-11 14:34:25.000000 clarifai-9.9.2/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 14:34:25.000000 clarifai-9.9.2/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-11 14:34:25.000000 clarifai-9.9.2/clarifai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-11 14:34:25.000000 clarifai-9.9.2/clarifai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-11 14:34:25.000000 clarifai-9.9.2/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.264874 clarifai-9.9.2/clarifai_utils/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13909 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/auth/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/auth/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/auth/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/client/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22809 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/client/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13909 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/auth/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/auth/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/auth/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14742 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    31391 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/lister.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/client/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/constants/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/datasets/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/export/inputs_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/datasets/upload/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.268875 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/cifar_small_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/cifar_small_train.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.272874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.272874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.232874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.272874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/
--rw-r--r--   0 runner    (1001) docker     (127)    49005 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    49264 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    43410 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    33826 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47755 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.272874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/
--rw-r--r--   0 runner    (1001) docker     (127)    43856 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47022 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    46176 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    37327 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    32557 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.272874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/
--rw-r--r--   0 runner    (1001) docker     (127)    26278 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    45386 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    40566 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47620 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    52635 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.276874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/
--rw-r--r--   0 runner    (1001) docker     (127)    44858 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    49950 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    51306 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    34567 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    56869 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.276874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.276874 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   237144 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)   270347 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/train.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.276874 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/coco_captions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/coco_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/imagenet_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/xview_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/datasets/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.276874 clarifai-9.9.2/clarifai_utils/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/cli/model_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/cli/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/docs/custom_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/docs/dependencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/docs/model_types.md
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/docs/output.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.280875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_embedding/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.284875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.288875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.288875 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/config.pbtxt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/labels.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.288875 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.288875 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/text-classifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/text-embedder.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/text-to-image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/text-to-text.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/visual-classifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/visual-detector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/visual-embedder.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/visual-segmenter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.288875 clarifai-9.9.2/clarifai_utils/models/model_serving/models/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/models/default_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/models/model_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/models/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/models/pb_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/models/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.288875 clarifai-9.9.2/clarifai_utils/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/modules/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/modules/css.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/modules/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/modules/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.292875 clarifai-9.9.2/clarifai_utils/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/runners/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.292875 clarifai-9.9.2/clarifai_utils/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/schema/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.292875 clarifai-9.9.2/clarifai_utils/urls/
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/urls/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.292875 clarifai-9.9.2/clarifai_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.292875 clarifai-9.9.2/clarifai_utils/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/workflows/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/workflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-10-11 14:34:12.000000 clarifai-9.9.2/clarifai_utils/workflows/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 14:34:25.292875 clarifai-9.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-10-11 14:34:12.000000 clarifai-9.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 14:34:25.292875 clarifai-9.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2023-10-11 14:34:12.000000 clarifai-9.9.2/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-10-11 14:34:12.000000 clarifai-9.9.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2023-10-11 14:34:12.000000 clarifai-9.9.2/tests/test_data_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-10-11 14:34:12.000000 clarifai-9.9.2/tests/test_model_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2023-10-11 14:34:12.000000 clarifai-9.9.2/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2023-10-11 14:34:12.000000 clarifai-9.9.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2023-10-11 14:34:12.000000 clarifai-9.9.2/tests/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2023-10-16 18:10:30.000000 clarifai-9.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-10-16 18:10:30.000000 clarifai-9.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2023-10-16 18:10:40.544292 clarifai-9.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2023-10-16 18:10:30.000000 clarifai-9.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.500291 clarifai-9.9.3/clarifai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.500291 clarifai-9.9.3/clarifai/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/auth/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/auth/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/auth/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25409 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/auth/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/auth/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/auth/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14953 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35851 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/client/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/constants/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/export/inputs_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/upload/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/cifar_small_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/cifar_small_train.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.504291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.492291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.508291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/
+-rw-r--r--   0 runner    (1001) docker     (127)    49005 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    49264 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    43410 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    33826 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47755 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.508291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/
+-rw-r--r--   0 runner    (1001) docker     (127)    43856 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47022 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    46176 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    37327 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    32557 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.508291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/
+-rw-r--r--   0 runner    (1001) docker     (127)    26278 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    45386 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    40566 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47620 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    52635 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.508291 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/
+-rw-r--r--   0 runner    (1001) docker     (127)    44858 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    49950 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    51306 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    34567 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    56869 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.508291 clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.508291 clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   237144 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   270347 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/train.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/datasets/upload/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/loaders/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/loaders/coco_captions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/loaders/coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/loaders/coco_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/loaders/imagenet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/loaders/xview_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/datasets/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/cli/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/docs/custom_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/docs/dependencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/docs/model_types.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/docs/output.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.512291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_embedding/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.516291 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/models/model_serving/model_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/text-classifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/text-embedder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/text-to-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/text-to-text.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/visual-classifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/visual-detector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/visual-embedder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/visual-segmenter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/model_config/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/models/model_serving/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/models/default_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/models/model_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/models/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/models/pb_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/modules/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/modules/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/modules/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/modules/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/runners/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/schema/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/urls/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.520292 clarifai-9.9.3/clarifai/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/workflows/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/workflows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai/workflows/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.500291 clarifai-9.9.3/clarifai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2023-10-16 18:10:40.000000 clarifai-9.9.3/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24579 2023-10-16 18:10:40.000000 clarifai-9.9.3/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 18:10:40.000000 clarifai-9.9.3/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-16 18:10:40.000000 clarifai-9.9.3/clarifai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-16 18:10:40.000000 clarifai-9.9.3/clarifai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-16 18:10:40.000000 clarifai-9.9.3/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/auth/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/auth/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/auth/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25409 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/auth/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/auth/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/auth/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14953 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35851 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/client/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/constants/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/datasets/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/export/inputs_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/datasets/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.524292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.528292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/cifar_small_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/cifar_small_train.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.528292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.528292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.496291 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.528292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/
+-rw-r--r--   0 runner    (1001) docker     (127)    49005 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    49264 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    43410 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    33826 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47755 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.528292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/
+-rw-r--r--   0 runner    (1001) docker     (127)    43856 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47022 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    46176 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    37327 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    32557 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.528292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/
+-rw-r--r--   0 runner    (1001) docker     (127)    26278 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    45386 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    40566 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47620 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    52635 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.532292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/
+-rw-r--r--   0 runner    (1001) docker     (127)    44858 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    49950 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    51306 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    34567 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    56869 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.532292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.532292 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   237144 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   270347 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/train.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.532292 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/coco_captions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/coco_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/imagenet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/xview_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/datasets/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.532292 clarifai-9.9.3/clarifai_utils/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.532292 clarifai-9.9.3/clarifai_utils/models/model_serving/
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.532292 clarifai-9.9.3/clarifai_utils/models/model_serving/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/cli/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/docs/custom_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/docs/dependencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/docs/model_types.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/docs/output.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_embedding/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.536292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/config.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/labels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/text-classifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/text-embedder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/text-to-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/text-to-text.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/visual-classifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/visual-detector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/visual-embedder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/visual-segmenter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.540292 clarifai-9.9.3/clarifai_utils/models/model_serving/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/models/default_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/models/model_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/models/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/models/pb_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/clarifai_utils/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/modules/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/modules/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/modules/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/modules/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/clarifai_utils/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/runners/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/clarifai_utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/schema/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/clarifai_utils/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/urls/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/clarifai_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/clarifai_utils/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/workflows/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/workflows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-10-16 18:10:30.000000 clarifai-9.9.3/clarifai_utils/workflows/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 18:10:40.544292 clarifai-9.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-10-16 18:10:30.000000 clarifai-9.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:10:40.544292 clarifai-9.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2023-10-16 18:10:30.000000 clarifai-9.9.3/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-10-16 18:10:30.000000 clarifai-9.9.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2023-10-16 18:10:30.000000 clarifai-9.9.3/tests/test_data_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-10-16 18:10:30.000000 clarifai-9.9.3/tests/test_model_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2023-10-16 18:10:30.000000 clarifai-9.9.3/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2023-10-16 18:10:30.000000 clarifai-9.9.3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2023-10-16 18:10:30.000000 clarifai-9.9.3/tests/test_stub.py
```

### Comparing `clarifai-9.9.2/LICENSE` & `clarifai-9.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/PKG-INFO` & `clarifai-9.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.9.2
+Version: 9.9.3
 Summary: Clarifai Python SDK
 Home-page: https://github.com/Clarifai/clarifai-python
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
@@ -21,36 +21,26 @@
 <h2 align="center">
 Clarifai Python SDK</a>
 </h2>
 
 
 
 <p align="center">
-  <a href="https://clarifaicommunity.slack.com/" target="_blank"> <img src="https://img.shields.io/badge/slack-chat-green.svg?logo=slack&color=4ec528" alt="Slack">
+  <a href="https://discord.gg/M32V7a7a" target="_blank"> <img src="https://img.shields.io/badge/discord-chat-green.svg?logo=discord&color=4ec528" alt="Discord">
+  </a>
+  <a href="https://pypi.org/project/clarifai" target="_blank"> <img src="https://img.shields.io/pypi/dm/clarifai" alt="PyPI - Downloads">
   </a>
-
 </p>
 
 
 
 
 This is the official Python client for interacting with our powerful [API](https://docs.clarifai.com). The Clarifai Python SDK offers a comprehensive set of tools to integrate Clarifai's AI platform to leverage computer vision capabiities like classification , detection ,segementation and natural language capabilities like classification , summarisation , generation , Q&A ,etc into your applications. With just a few lines of code, you can leverage cutting-edge artificial intelligence to unlock valuable insights from visual and textual content.
 
----
-**Website**: [https://www.clarifai.com](https://www.clarifai.com/)
-
-**Demo**: [https://clarifai.com/demo](https://clarifai.com/demo)
-
-**Sign up for a free Account**: [https://clarifai.com/signup](https://clarifai.com/signup)
-
-**Developer Guide**: [https://docs.clarifai.com](https://docs.clarifai.com/)
-
-**Clarifai Community**: [https://clarifai.com/explore](https://clarifai.com/explore)
-
-**Python SDK Docs**: [https://docs.clarifai.com/python-sdk/api-reference](https://docs.clarifai.com/python-sdk/api-reference)
+[Website](https://www.clarifai.com/) | [Demo](https://clarifai.com/demo) | [Signup for a Free Account](https://clarifai.com/signup) | [API Docs](https://docs.clarifai.com/) | [Clarifai Community](https://clarifai.com/explore) | [Python SDK Docs](https://docs.clarifai.com/python-sdk/api-reference) | [Examples](https://github.com/Clarifai/examples) | [Colab Notebooks](https://github.com/Clarifai/colab-notebooks)
 
 
 ---
 
 ## Installation
 
 
@@ -84,15 +74,16 @@
 
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.user import User
 client = User(user_id="user_id")
 
 # Get all apps
-apps = client.list_apps()
+apps_generator = client.list_apps()
+apps = list(apps_generator)
 ```
 
 ### Interacting with Datasets
 
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
@@ -114,33 +105,45 @@
 # Note: clarifai-data-protobuf.zip is acquired through exporting datasets within the Clarifai Platform.
 Dataset().export(save_path='output.zip', local_archive_path='clarifai-data-protobuf.zip')
 ```
 
 
 ### Interacting with Inputs
 
+#### Input upload
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.user import User
 app = User(user_id="user_id").app(app_id="app_id")
 input_obj = app.inputs()
 
 #input upload from url
 input_obj.upload_from_url(input_id = 'demo', image_url='https://samples.clarifai.com/metro-north.jpg')
 
 #input upload from filename
 input_obj.upload_from_file(input_id = 'demo', video_file='demo.mp4')
 
-#listing inputs
-input_obj.list_inputs()
-
 # text upload
 input_obj.upload_text(input_id = 'demo', raw_text = 'This is a test')
 ```
 
+#### Input listing
+```python
+#listing inputs
+input_generator = input_obj.list_inputs(page_no=1,per_page=10,input_type='image')
+inputs_list = list(input_generator)
+
+#listing annotations
+annotation_generator = input_obj.list_annotations(batch_input=inputs_list)
+annotations_list = list(annotation_generator)
+
+#listing concepts
+all_concepts = list(app.list_concepts())
+```
+
 
 ### Interacting with Models
 
 #### Model Predict
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.model import Model
@@ -161,25 +164,26 @@
 model_prediction = model.predict_by_url(url="VIDEO_URL", input_type="video")
 ```
 #### Models Listing
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
 # List all model versions
-all_model_versions = model.list_versions()
+all_model_versions = list(model.list_versions())
 
 # Go to specific model version
 model_v1 = client.app("app_id").model(model_id="model_id", model_version_id="model_version_id")
 
 # List all models in an app
-all_models = app.list_models()
+all_models = list(app.list_models())
 
 # List all models in community filtered by model_type, description
 all_llm_community_models = App().list_models(filter_by={"query": "LLM",
                                                         "model_type_id": "text-to-text"}, only_in_app=False)
+all_llm_community_models = list(all_llm_community_models)
 ```
 
 ### Interacting with Workflows
 
 #### Workflow Predict
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
@@ -196,24 +200,25 @@
 ```
 
 #### Workflows Listing
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
 # List all workflow versions
-all_workflow_versions = workflow.list_versions()
+all_workflow_versions = list(workflow.list_versions())
 
 # Go to specific workflow version
 workflow_v1 = Workflow(workflow_id="workflow_id", workflow_version=dict(id="workflow_version_id"), app_id="app_id", user_id="user_id")
 
 # List all workflow in an app
-all_workflow = app.list_workflow()
+all_workflow = list(app.list_workflow())
 
 # List all workflow in community filtered by description
 all_face_community_workflows = App().list_workflows(filter_by={"query": "face"}, only_in_app=False) # Get all face related workflows
+all_face_community_workflows = list(all_face_community_workflows)
 ```
 #### Workflow Create
 Create a new workflow specified by a yaml config file.
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.app import App
 app = App(app_id="app_id", user_id="user_id")
```

#### html2text {}

```diff
@@ -1,104 +1,111 @@
-Metadata-Version: 2.1 Name: clarifai Version: 9.9.2 Summary: Clarifai Python
+Metadata-Version: 2.1 Name: clarifai Version: 9.9.3 Summary: Clarifai Python
 SDK Home-page: https://github.com/Clarifai/clarifai-python Author: Clarifai
 Author-email: support@clarifai.com License: Apache 2.0 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                            ************ _[[_CC_ll_aa_rr_ii_ff_aa_ii_]] ************
                         ********** CCllaarriiffaaii PPyytthhoonn SSDDKK **********
-                                    _[_S_l_a_c_k_]
+                          _[_D_i_s_c_o_r_d_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]
 This is the official Python client for interacting with our powerful [API]
 (https://docs.clarifai.com). The Clarifai Python SDK offers a comprehensive set
 of tools to integrate Clarifai's AI platform to leverage computer vision
 capabiities like classification , detection ,segementation and natural language
 capabilities like classification , summarisation , generation , Q&A ,etc into
 your applications. With just a few lines of code, you can leverage cutting-edge
 artificial intelligence to unlock valuable insights from visual and textual
-content. --- **Website**: [https://www.clarifai.com](https://www.clarifai.com/
-) **Demo**: [https://clarifai.com/demo](https://clarifai.com/demo) **Sign up
-for a free Account**: [https://clarifai.com/signup](https://clarifai.com/
-signup) **Developer Guide**: [https://docs.clarifai.com](https://
-docs.clarifai.com/) **Clarifai Community**: [https://clarifai.com/explore]
-(https://clarifai.com/explore) **Python SDK Docs**: [https://docs.clarifai.com/
-python-sdk/api-reference](https://docs.clarifai.com/python-sdk/api-reference) -
--- ## Installation Install from PyPi: ```bash pip install -U clarifai ```
-Install from Source: ```bash git clone https://github.com/Clarifai/clarifai-
-python.git cd clarifai-python python3 -m venv env source env/bin/activate pip3
-install -r requirements.txt ``` ## Getting started Clarifai uses **Personal
-Access Tokens(PATs)** to validate requests. You can create and manage PATs
-under your Clarifai account security settings. Export your PAT as an
-environment variable. Then, import and initialize the API Client. ```cmd export
-CLARIFAI_PAT={your personal access token} ``` ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.user import User client =
-User(user_id="user_id") # Get all apps apps = client.list_apps() ``` ###
-Interacting with Datasets ```python # Note: CLARIFAI_PAT must be set as env
-variable. # Create app and dataset app = client.create_app(app_id="demo_app",
-base_workflow="Universal") dataset = app.create_dataset
-(dataset_id="demo_dataset") # execute data upload to Clarifai app dataset
-dataset.upload_dataset(task='visual_segmentation', split="train",
+content. [Website](https://www.clarifai.com/) | [Demo](https://clarifai.com/
+demo) | [Signup for a Free Account](https://clarifai.com/signup) | [API Docs]
+(https://docs.clarifai.com/) | [Clarifai Community](https://clarifai.com/
+explore) | [Python SDK Docs](https://docs.clarifai.com/python-sdk/api-
+reference) | [Examples](https://github.com/Clarifai/examples) | [Colab
+Notebooks](https://github.com/Clarifai/colab-notebooks) --- ## Installation
+Install from PyPi: ```bash pip install -U clarifai ``` Install from Source:
+```bash git clone https://github.com/Clarifai/clarifai-python.git cd clarifai-
+python python3 -m venv env source env/bin/activate pip3 install -
+r requirements.txt ``` ## Getting started Clarifai uses **Personal Access
+Tokens(PATs)** to validate requests. You can create and manage PATs under your
+Clarifai account security settings. Export your PAT as an environment variable.
+Then, import and initialize the API Client. ```cmd export CLARIFAI_PAT={your
+personal access token} ``` ```python # Note: CLARIFAI_PAT must be set as env
+variable. from clarifai.client.user import User client = User
+(user_id="user_id") # Get all apps apps_generator = client.list_apps() apps =
+list(apps_generator) ``` ### Interacting with Datasets ```python # Note:
+CLARIFAI_PAT must be set as env variable. # Create app and dataset app =
+client.create_app(app_id="demo_app", base_workflow="Universal") dataset =
+app.create_dataset(dataset_id="demo_dataset") # execute data upload to Clarifai
+app dataset dataset.upload_dataset(task='visual_segmentation', split="train",
 dataset_loader='coco_segmentation') #upload text from csv
 dataset.upload_from_csv(csv_path='csv_path', input_type='text', csv_type='raw',
 labels=True) #upload data from folder dataset.upload_from_folder
 (folder_path='folder_path', input_type='text', labels=True) # Export Dataset
 from clarifai.client.dataset import Dataset # Note: clarifai-data-protobuf.zip
 is acquired through exporting datasets within the Clarifai Platform. Dataset
 ().export(save_path='output.zip', local_archive_path='clarifai-data-
-protobuf.zip') ``` ### Interacting with Inputs ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.user import User app = User
-(user_id="user_id").app(app_id="app_id") input_obj = app.inputs() #input upload
-from url input_obj.upload_from_url(input_id = 'demo', image_url='https://
-samples.clarifai.com/metro-north.jpg') #input upload from filename
-input_obj.upload_from_file(input_id = 'demo', video_file='demo.mp4') #listing
-inputs input_obj.list_inputs() # text upload input_obj.upload_text(input_id =
-'demo', raw_text = 'This is a test') ``` ### Interacting with Models #### Model
-Predict ```python # Note: CLARIFAI_PAT must be set as env variable. from
-clarifai.client.model import Model # Model Predict model_prediction = Model
-("https://clarifai.com/anthropic/completion/models/claude-v2").predict_by_bytes
-(b"Write a tweet on future of AI", "text") model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id") model_prediction = model.predict_by_url
-(url="url", input_type="image") # Supports image, text, audio, video #
-Customizing Model Inference Output model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id", output_config={"min_value": 0.98}) #
-Return predictions having prediction confidence > 0.98 model_prediction =
-model.predict_by_filepath(filepath="local_filepath", input_type="text") #
-Supports image, text, audio, video model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id", output_config={"sample_ms": 2000}) #
-Return predictions for specified interval model_prediction =
-model.predict_by_url(url="VIDEO_URL", input_type="video") ``` #### Models
-Listing ```python # Note: CLARIFAI_PAT must be set as env variable. # List all
-model versions all_model_versions = model.list_versions() # Go to specific
-model version model_v1 = client.app("app_id").model(model_id="model_id",
-model_version_id="model_version_id") # List all models in an app all_models =
-app.list_models() # List all models in community filtered by model_type,
-description all_llm_community_models = App().list_models(filter_by={"query":
-"LLM", "model_type_id": "text-to-text"}, only_in_app=False) ``` ### Interacting
-with Workflows #### Workflow Predict ```python # Note: CLARIFAI_PAT must be set
-as env variable. from clarifai.client.workflow import Workflow # Workflow
-Predict workflow = Workflow("workflow_url") # Example: https://clarifai.com/
-clarifai/main/workflows/Face-Sentiment workflow_prediction =
-workflow.predict_by_url(url="url", input_type="image") # Supports image, text,
-audio, video # Customizing Workflow Inference Output workflow = Workflow
-(user_id="user_id", app_id="app_id", workflow_id="workflow_id", output_config=
+protobuf.zip') ``` ### Interacting with Inputs #### Input upload ```python #
+Note: CLARIFAI_PAT must be set as env variable. from clarifai.client.user
+import User app = User(user_id="user_id").app(app_id="app_id") input_obj =
+app.inputs() #input upload from url input_obj.upload_from_url(input_id =
+'demo', image_url='https://samples.clarifai.com/metro-north.jpg') #input upload
+from filename input_obj.upload_from_file(input_id = 'demo',
+video_file='demo.mp4') # text upload input_obj.upload_text(input_id = 'demo',
+raw_text = 'This is a test') ``` #### Input listing ```python #listing inputs
+input_generator = input_obj.list_inputs
+(page_no=1,per_page=10,input_type='image') inputs_list = list(input_generator)
+#listing annotations annotation_generator = input_obj.list_annotations
+(batch_input=inputs_list) annotations_list = list(annotation_generator)
+#listing concepts all_concepts = list(app.list_concepts()) ``` ### Interacting
+with Models #### Model Predict ```python # Note: CLARIFAI_PAT must be set as
+env variable. from clarifai.client.model import Model # Model Predict
+model_prediction = Model("https://clarifai.com/anthropic/completion/models/
+claude-v2").predict_by_bytes(b"Write a tweet on future of AI", "text") model =
+Model(user_id="user_id", app_id="app_id", model_id="model_id") model_prediction
+= model.predict_by_url(url="url", input_type="image") # Supports image, text,
+audio, video # Customizing Model Inference Output model = Model
+(user_id="user_id", app_id="app_id", model_id="model_id", output_config=
 {"min_value": 0.98}) # Return predictions having prediction confidence > 0.98
-workflow_prediction = workflow.predict_by_filepath(filepath="local_filepath",
-input_type="text") # Supports image, text, audio, video ``` #### Workflows
-Listing ```python # Note: CLARIFAI_PAT must be set as env variable. # List all
-workflow versions all_workflow_versions = workflow.list_versions() # Go to
-specific workflow version workflow_v1 = Workflow(workflow_id="workflow_id",
+model_prediction = model.predict_by_filepath(filepath="local_filepath",
+input_type="text") # Supports image, text, audio, video model = Model
+(user_id="user_id", app_id="app_id", model_id="model_id", output_config=
+{"sample_ms": 2000}) # Return predictions for specified interval
+model_prediction = model.predict_by_url(url="VIDEO_URL", input_type="video")
+``` #### Models Listing ```python # Note: CLARIFAI_PAT must be set as env
+variable. # List all model versions all_model_versions = list
+(model.list_versions()) # Go to specific model version model_v1 = client.app
+("app_id").model(model_id="model_id", model_version_id="model_version_id") #
+List all models in an app all_models = list(app.list_models()) # List all
+models in community filtered by model_type, description
+all_llm_community_models = App().list_models(filter_by={"query": "LLM",
+"model_type_id": "text-to-text"}, only_in_app=False) all_llm_community_models =
+list(all_llm_community_models) ``` ### Interacting with Workflows #### Workflow
+Predict ```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.workflow import Workflow # Workflow Predict workflow = Workflow
+("workflow_url") # Example: https://clarifai.com/clarifai/main/workflows/Face-
+Sentiment workflow_prediction = workflow.predict_by_url(url="url",
+input_type="image") # Supports image, text, audio, video # Customizing Workflow
+Inference Output workflow = Workflow(user_id="user_id", app_id="app_id",
+workflow_id="workflow_id", output_config={"min_value": 0.98}) # Return
+predictions having prediction confidence > 0.98 workflow_prediction =
+workflow.predict_by_filepath(filepath="local_filepath", input_type="text") #
+Supports image, text, audio, video ``` #### Workflows Listing ```python # Note:
+CLARIFAI_PAT must be set as env variable. # List all workflow versions
+all_workflow_versions = list(workflow.list_versions()) # Go to specific
+workflow version workflow_v1 = Workflow(workflow_id="workflow_id",
 workflow_version=dict(id="workflow_version_id"), app_id="app_id",
-user_id="user_id") # List all workflow in an app all_workflow =
-app.list_workflow() # List all workflow in community filtered by description
+user_id="user_id") # List all workflow in an app all_workflow = list
+(app.list_workflow()) # List all workflow in community filtered by description
 all_face_community_workflows = App().list_workflows(filter_by={"query":
-"face"}, only_in_app=False) # Get all face related workflows ``` #### Workflow
-Create Create a new workflow specified by a yaml config file. ```python # Note:
-CLARIFAI_PAT must be set as env variable. from clarifai.client.app import App
-app = App(app_id="app_id", user_id="user_id") workflow = app.create_workflow
-(config_filepath="config.yml") ``` #### Workflow Export Export an existing
-workflow from Clarifai as a local yaml file. ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.workflow import Workflow
-workflow = Workflow("https://clarifai.com/clarifai/main/workflows/
-Demographics") workflow.export('demographics_workflow.yml') ``` ## More
-Examples See many more code examples in this [repo](https://github.com/
-Clarifai/examples). Also see the official [Python SDK docs](https://clarifai-
-python.readthedocs.io/en/latest/index.html)
+"face"}, only_in_app=False) # Get all face related workflows
+all_face_community_workflows = list(all_face_community_workflows) ``` ####
+Workflow Create Create a new workflow specified by a yaml config file.
+```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.app import App app = App(app_id="app_id", user_id="user_id")
+workflow = app.create_workflow(config_filepath="config.yml") ``` #### Workflow
+Export Export an existing workflow from Clarifai as a local yaml file.
+```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.workflow import Workflow workflow = Workflow("https://
+clarifai.com/clarifai/main/workflows/Demographics") workflow.export
+('demographics_workflow.yml') ``` ## More Examples See many more code examples
+in this [repo](https://github.com/Clarifai/examples). Also see the official
+[Python SDK docs](https://clarifai-python.readthedocs.io/en/latest/index.html)
```

### Comparing `clarifai-9.9.2/README.md` & `clarifai-9.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,36 +5,26 @@
 <h2 align="center">
 Clarifai Python SDK</a>
 </h2>
 
 
 
 <p align="center">
-  <a href="https://clarifaicommunity.slack.com/" target="_blank"> <img src="https://img.shields.io/badge/slack-chat-green.svg?logo=slack&color=4ec528" alt="Slack">
+  <a href="https://discord.gg/M32V7a7a" target="_blank"> <img src="https://img.shields.io/badge/discord-chat-green.svg?logo=discord&color=4ec528" alt="Discord">
+  </a>
+  <a href="https://pypi.org/project/clarifai" target="_blank"> <img src="https://img.shields.io/pypi/dm/clarifai" alt="PyPI - Downloads">
   </a>
-
 </p>
 
 
 
 
 This is the official Python client for interacting with our powerful [API](https://docs.clarifai.com). The Clarifai Python SDK offers a comprehensive set of tools to integrate Clarifai's AI platform to leverage computer vision capabiities like classification , detection ,segementation and natural language capabilities like classification , summarisation , generation , Q&A ,etc into your applications. With just a few lines of code, you can leverage cutting-edge artificial intelligence to unlock valuable insights from visual and textual content.
 
----
-**Website**: [https://www.clarifai.com](https://www.clarifai.com/)
-
-**Demo**: [https://clarifai.com/demo](https://clarifai.com/demo)
-
-**Sign up for a free Account**: [https://clarifai.com/signup](https://clarifai.com/signup)
-
-**Developer Guide**: [https://docs.clarifai.com](https://docs.clarifai.com/)
-
-**Clarifai Community**: [https://clarifai.com/explore](https://clarifai.com/explore)
-
-**Python SDK Docs**: [https://docs.clarifai.com/python-sdk/api-reference](https://docs.clarifai.com/python-sdk/api-reference)
+[Website](https://www.clarifai.com/) | [Demo](https://clarifai.com/demo) | [Signup for a Free Account](https://clarifai.com/signup) | [API Docs](https://docs.clarifai.com/) | [Clarifai Community](https://clarifai.com/explore) | [Python SDK Docs](https://docs.clarifai.com/python-sdk/api-reference) | [Examples](https://github.com/Clarifai/examples) | [Colab Notebooks](https://github.com/Clarifai/colab-notebooks)
 
 
 ---
 
 ## Installation
 
 
@@ -68,15 +58,16 @@
 
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.user import User
 client = User(user_id="user_id")
 
 # Get all apps
-apps = client.list_apps()
+apps_generator = client.list_apps()
+apps = list(apps_generator)
 ```
 
 ### Interacting with Datasets
 
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
@@ -98,33 +89,45 @@
 # Note: clarifai-data-protobuf.zip is acquired through exporting datasets within the Clarifai Platform.
 Dataset().export(save_path='output.zip', local_archive_path='clarifai-data-protobuf.zip')
 ```
 
 
 ### Interacting with Inputs
 
+#### Input upload
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.user import User
 app = User(user_id="user_id").app(app_id="app_id")
 input_obj = app.inputs()
 
 #input upload from url
 input_obj.upload_from_url(input_id = 'demo', image_url='https://samples.clarifai.com/metro-north.jpg')
 
 #input upload from filename
 input_obj.upload_from_file(input_id = 'demo', video_file='demo.mp4')
 
-#listing inputs
-input_obj.list_inputs()
-
 # text upload
 input_obj.upload_text(input_id = 'demo', raw_text = 'This is a test')
 ```
 
+#### Input listing
+```python
+#listing inputs
+input_generator = input_obj.list_inputs(page_no=1,per_page=10,input_type='image')
+inputs_list = list(input_generator)
+
+#listing annotations
+annotation_generator = input_obj.list_annotations(batch_input=inputs_list)
+annotations_list = list(annotation_generator)
+
+#listing concepts
+all_concepts = list(app.list_concepts())
+```
+
 
 ### Interacting with Models
 
 #### Model Predict
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.model import Model
@@ -145,25 +148,26 @@
 model_prediction = model.predict_by_url(url="VIDEO_URL", input_type="video")
 ```
 #### Models Listing
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
 # List all model versions
-all_model_versions = model.list_versions()
+all_model_versions = list(model.list_versions())
 
 # Go to specific model version
 model_v1 = client.app("app_id").model(model_id="model_id", model_version_id="model_version_id")
 
 # List all models in an app
-all_models = app.list_models()
+all_models = list(app.list_models())
 
 # List all models in community filtered by model_type, description
 all_llm_community_models = App().list_models(filter_by={"query": "LLM",
                                                         "model_type_id": "text-to-text"}, only_in_app=False)
+all_llm_community_models = list(all_llm_community_models)
 ```
 
 ### Interacting with Workflows
 
 #### Workflow Predict
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
@@ -180,24 +184,25 @@
 ```
 
 #### Workflows Listing
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
 # List all workflow versions
-all_workflow_versions = workflow.list_versions()
+all_workflow_versions = list(workflow.list_versions())
 
 # Go to specific workflow version
 workflow_v1 = Workflow(workflow_id="workflow_id", workflow_version=dict(id="workflow_version_id"), app_id="app_id", user_id="user_id")
 
 # List all workflow in an app
-all_workflow = app.list_workflow()
+all_workflow = list(app.list_workflow())
 
 # List all workflow in community filtered by description
 all_face_community_workflows = App().list_workflows(filter_by={"query": "face"}, only_in_app=False) # Get all face related workflows
+all_face_community_workflows = list(all_face_community_workflows)
 ```
 #### Workflow Create
 Create a new workflow specified by a yaml config file.
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.app import App
 app = App(app_id="app_id", user_id="user_id")
```

#### html2text {}

```diff
@@ -1,97 +1,104 @@
                            ************ _[[_CC_ll_aa_rr_ii_ff_aa_ii_]] ************
                         ********** CCllaarriiffaaii PPyytthhoonn SSDDKK **********
-                                    _[_S_l_a_c_k_]
+                          _[_D_i_s_c_o_r_d_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]
 This is the official Python client for interacting with our powerful [API]
 (https://docs.clarifai.com). The Clarifai Python SDK offers a comprehensive set
 of tools to integrate Clarifai's AI platform to leverage computer vision
 capabiities like classification , detection ,segementation and natural language
 capabilities like classification , summarisation , generation , Q&A ,etc into
 your applications. With just a few lines of code, you can leverage cutting-edge
 artificial intelligence to unlock valuable insights from visual and textual
-content. --- **Website**: [https://www.clarifai.com](https://www.clarifai.com/
-) **Demo**: [https://clarifai.com/demo](https://clarifai.com/demo) **Sign up
-for a free Account**: [https://clarifai.com/signup](https://clarifai.com/
-signup) **Developer Guide**: [https://docs.clarifai.com](https://
-docs.clarifai.com/) **Clarifai Community**: [https://clarifai.com/explore]
-(https://clarifai.com/explore) **Python SDK Docs**: [https://docs.clarifai.com/
-python-sdk/api-reference](https://docs.clarifai.com/python-sdk/api-reference) -
--- ## Installation Install from PyPi: ```bash pip install -U clarifai ```
-Install from Source: ```bash git clone https://github.com/Clarifai/clarifai-
-python.git cd clarifai-python python3 -m venv env source env/bin/activate pip3
-install -r requirements.txt ``` ## Getting started Clarifai uses **Personal
-Access Tokens(PATs)** to validate requests. You can create and manage PATs
-under your Clarifai account security settings. Export your PAT as an
-environment variable. Then, import and initialize the API Client. ```cmd export
-CLARIFAI_PAT={your personal access token} ``` ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.user import User client =
-User(user_id="user_id") # Get all apps apps = client.list_apps() ``` ###
-Interacting with Datasets ```python # Note: CLARIFAI_PAT must be set as env
-variable. # Create app and dataset app = client.create_app(app_id="demo_app",
-base_workflow="Universal") dataset = app.create_dataset
-(dataset_id="demo_dataset") # execute data upload to Clarifai app dataset
-dataset.upload_dataset(task='visual_segmentation', split="train",
+content. [Website](https://www.clarifai.com/) | [Demo](https://clarifai.com/
+demo) | [Signup for a Free Account](https://clarifai.com/signup) | [API Docs]
+(https://docs.clarifai.com/) | [Clarifai Community](https://clarifai.com/
+explore) | [Python SDK Docs](https://docs.clarifai.com/python-sdk/api-
+reference) | [Examples](https://github.com/Clarifai/examples) | [Colab
+Notebooks](https://github.com/Clarifai/colab-notebooks) --- ## Installation
+Install from PyPi: ```bash pip install -U clarifai ``` Install from Source:
+```bash git clone https://github.com/Clarifai/clarifai-python.git cd clarifai-
+python python3 -m venv env source env/bin/activate pip3 install -
+r requirements.txt ``` ## Getting started Clarifai uses **Personal Access
+Tokens(PATs)** to validate requests. You can create and manage PATs under your
+Clarifai account security settings. Export your PAT as an environment variable.
+Then, import and initialize the API Client. ```cmd export CLARIFAI_PAT={your
+personal access token} ``` ```python # Note: CLARIFAI_PAT must be set as env
+variable. from clarifai.client.user import User client = User
+(user_id="user_id") # Get all apps apps_generator = client.list_apps() apps =
+list(apps_generator) ``` ### Interacting with Datasets ```python # Note:
+CLARIFAI_PAT must be set as env variable. # Create app and dataset app =
+client.create_app(app_id="demo_app", base_workflow="Universal") dataset =
+app.create_dataset(dataset_id="demo_dataset") # execute data upload to Clarifai
+app dataset dataset.upload_dataset(task='visual_segmentation', split="train",
 dataset_loader='coco_segmentation') #upload text from csv
 dataset.upload_from_csv(csv_path='csv_path', input_type='text', csv_type='raw',
 labels=True) #upload data from folder dataset.upload_from_folder
 (folder_path='folder_path', input_type='text', labels=True) # Export Dataset
 from clarifai.client.dataset import Dataset # Note: clarifai-data-protobuf.zip
 is acquired through exporting datasets within the Clarifai Platform. Dataset
 ().export(save_path='output.zip', local_archive_path='clarifai-data-
-protobuf.zip') ``` ### Interacting with Inputs ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.user import User app = User
-(user_id="user_id").app(app_id="app_id") input_obj = app.inputs() #input upload
-from url input_obj.upload_from_url(input_id = 'demo', image_url='https://
-samples.clarifai.com/metro-north.jpg') #input upload from filename
-input_obj.upload_from_file(input_id = 'demo', video_file='demo.mp4') #listing
-inputs input_obj.list_inputs() # text upload input_obj.upload_text(input_id =
-'demo', raw_text = 'This is a test') ``` ### Interacting with Models #### Model
-Predict ```python # Note: CLARIFAI_PAT must be set as env variable. from
-clarifai.client.model import Model # Model Predict model_prediction = Model
-("https://clarifai.com/anthropic/completion/models/claude-v2").predict_by_bytes
-(b"Write a tweet on future of AI", "text") model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id") model_prediction = model.predict_by_url
-(url="url", input_type="image") # Supports image, text, audio, video #
-Customizing Model Inference Output model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id", output_config={"min_value": 0.98}) #
-Return predictions having prediction confidence > 0.98 model_prediction =
-model.predict_by_filepath(filepath="local_filepath", input_type="text") #
-Supports image, text, audio, video model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id", output_config={"sample_ms": 2000}) #
-Return predictions for specified interval model_prediction =
-model.predict_by_url(url="VIDEO_URL", input_type="video") ``` #### Models
-Listing ```python # Note: CLARIFAI_PAT must be set as env variable. # List all
-model versions all_model_versions = model.list_versions() # Go to specific
-model version model_v1 = client.app("app_id").model(model_id="model_id",
-model_version_id="model_version_id") # List all models in an app all_models =
-app.list_models() # List all models in community filtered by model_type,
-description all_llm_community_models = App().list_models(filter_by={"query":
-"LLM", "model_type_id": "text-to-text"}, only_in_app=False) ``` ### Interacting
-with Workflows #### Workflow Predict ```python # Note: CLARIFAI_PAT must be set
-as env variable. from clarifai.client.workflow import Workflow # Workflow
-Predict workflow = Workflow("workflow_url") # Example: https://clarifai.com/
-clarifai/main/workflows/Face-Sentiment workflow_prediction =
-workflow.predict_by_url(url="url", input_type="image") # Supports image, text,
-audio, video # Customizing Workflow Inference Output workflow = Workflow
-(user_id="user_id", app_id="app_id", workflow_id="workflow_id", output_config=
+protobuf.zip') ``` ### Interacting with Inputs #### Input upload ```python #
+Note: CLARIFAI_PAT must be set as env variable. from clarifai.client.user
+import User app = User(user_id="user_id").app(app_id="app_id") input_obj =
+app.inputs() #input upload from url input_obj.upload_from_url(input_id =
+'demo', image_url='https://samples.clarifai.com/metro-north.jpg') #input upload
+from filename input_obj.upload_from_file(input_id = 'demo',
+video_file='demo.mp4') # text upload input_obj.upload_text(input_id = 'demo',
+raw_text = 'This is a test') ``` #### Input listing ```python #listing inputs
+input_generator = input_obj.list_inputs
+(page_no=1,per_page=10,input_type='image') inputs_list = list(input_generator)
+#listing annotations annotation_generator = input_obj.list_annotations
+(batch_input=inputs_list) annotations_list = list(annotation_generator)
+#listing concepts all_concepts = list(app.list_concepts()) ``` ### Interacting
+with Models #### Model Predict ```python # Note: CLARIFAI_PAT must be set as
+env variable. from clarifai.client.model import Model # Model Predict
+model_prediction = Model("https://clarifai.com/anthropic/completion/models/
+claude-v2").predict_by_bytes(b"Write a tweet on future of AI", "text") model =
+Model(user_id="user_id", app_id="app_id", model_id="model_id") model_prediction
+= model.predict_by_url(url="url", input_type="image") # Supports image, text,
+audio, video # Customizing Model Inference Output model = Model
+(user_id="user_id", app_id="app_id", model_id="model_id", output_config=
 {"min_value": 0.98}) # Return predictions having prediction confidence > 0.98
-workflow_prediction = workflow.predict_by_filepath(filepath="local_filepath",
-input_type="text") # Supports image, text, audio, video ``` #### Workflows
-Listing ```python # Note: CLARIFAI_PAT must be set as env variable. # List all
-workflow versions all_workflow_versions = workflow.list_versions() # Go to
-specific workflow version workflow_v1 = Workflow(workflow_id="workflow_id",
+model_prediction = model.predict_by_filepath(filepath="local_filepath",
+input_type="text") # Supports image, text, audio, video model = Model
+(user_id="user_id", app_id="app_id", model_id="model_id", output_config=
+{"sample_ms": 2000}) # Return predictions for specified interval
+model_prediction = model.predict_by_url(url="VIDEO_URL", input_type="video")
+``` #### Models Listing ```python # Note: CLARIFAI_PAT must be set as env
+variable. # List all model versions all_model_versions = list
+(model.list_versions()) # Go to specific model version model_v1 = client.app
+("app_id").model(model_id="model_id", model_version_id="model_version_id") #
+List all models in an app all_models = list(app.list_models()) # List all
+models in community filtered by model_type, description
+all_llm_community_models = App().list_models(filter_by={"query": "LLM",
+"model_type_id": "text-to-text"}, only_in_app=False) all_llm_community_models =
+list(all_llm_community_models) ``` ### Interacting with Workflows #### Workflow
+Predict ```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.workflow import Workflow # Workflow Predict workflow = Workflow
+("workflow_url") # Example: https://clarifai.com/clarifai/main/workflows/Face-
+Sentiment workflow_prediction = workflow.predict_by_url(url="url",
+input_type="image") # Supports image, text, audio, video # Customizing Workflow
+Inference Output workflow = Workflow(user_id="user_id", app_id="app_id",
+workflow_id="workflow_id", output_config={"min_value": 0.98}) # Return
+predictions having prediction confidence > 0.98 workflow_prediction =
+workflow.predict_by_filepath(filepath="local_filepath", input_type="text") #
+Supports image, text, audio, video ``` #### Workflows Listing ```python # Note:
+CLARIFAI_PAT must be set as env variable. # List all workflow versions
+all_workflow_versions = list(workflow.list_versions()) # Go to specific
+workflow version workflow_v1 = Workflow(workflow_id="workflow_id",
 workflow_version=dict(id="workflow_version_id"), app_id="app_id",
-user_id="user_id") # List all workflow in an app all_workflow =
-app.list_workflow() # List all workflow in community filtered by description
+user_id="user_id") # List all workflow in an app all_workflow = list
+(app.list_workflow()) # List all workflow in community filtered by description
 all_face_community_workflows = App().list_workflows(filter_by={"query":
-"face"}, only_in_app=False) # Get all face related workflows ``` #### Workflow
-Create Create a new workflow specified by a yaml config file. ```python # Note:
-CLARIFAI_PAT must be set as env variable. from clarifai.client.app import App
-app = App(app_id="app_id", user_id="user_id") workflow = app.create_workflow
-(config_filepath="config.yml") ``` #### Workflow Export Export an existing
-workflow from Clarifai as a local yaml file. ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.workflow import Workflow
-workflow = Workflow("https://clarifai.com/clarifai/main/workflows/
-Demographics") workflow.export('demographics_workflow.yml') ``` ## More
-Examples See many more code examples in this [repo](https://github.com/
-Clarifai/examples). Also see the official [Python SDK docs](https://clarifai-
-python.readthedocs.io/en/latest/index.html)
+"face"}, only_in_app=False) # Get all face related workflows
+all_face_community_workflows = list(all_face_community_workflows) ``` ####
+Workflow Create Create a new workflow specified by a yaml config file.
+```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.app import App app = App(app_id="app_id", user_id="user_id")
+workflow = app.create_workflow(config_filepath="config.yml") ``` #### Workflow
+Export Export an existing workflow from Clarifai as a local yaml file.
+```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.workflow import Workflow workflow = Workflow("https://
+clarifai.com/clarifai/main/workflows/Demographics") workflow.export
+('demographics_workflow.yml') ``` ## More Examples See many more code examples
+in this [repo](https://github.com/Clarifai/examples). Also see the official
+[Python SDK docs](https://clarifai-python.readthedocs.io/en/latest/index.html)
```

### Comparing `clarifai-9.9.2/clarifai/auth/helper.py` & `clarifai-9.9.3/clarifai/auth/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,24 +224,14 @@
         user_id: CLARIFAI_USER_ID env var.
         app_id: CLARIFAI_APP_ID env var.
         one of:
           token: CLARIFAI_SESSION_TOKEN env var.
           pat: CLARIFAI_PAT env var.
         base: CLARIFAI_API_BASE env var.
     """
-    error_description = """
-Please check the following required vars are in your env:
- - 'CLARIFAI_USER_ID': the user ID accessing the module.
- - 'CLARIFAI_APP_ID': the app the module is being accessed from.
- - 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT': to authenticate the calling user with a session token or personal access token.
-
-Additionally, these optional params are supported:
- - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
- - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
-"""
     user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
     token = os.environ.get("CLARIFAI_SESSION_TOKEN", "")
     pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
     return cls(user_id, app_id, pat, token, base, ui, validate)
```

### Comparing `clarifai-9.9.2/clarifai/auth/register.py` & `clarifai-9.9.3/clarifai/auth/register.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/auth/stub.py` & `clarifai-9.9.3/clarifai/auth/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/client/__init__.py` & `clarifai-9.9.3/clarifai/client/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/client/app.py` & `clarifai-9.9.3/clarifai/client/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import uuid
-from typing import Any, Dict, List
+from typing import Any, Dict, Generator
 
 import yaml
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
+from clarifai_grpc.grpc.api.resources_pb2 import Concept
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from google.protobuf.json_format import MessageToDict
 
 from clarifai.client.base import BaseClient
 from clarifai.client.dataset import Dataset
 from clarifai.client.input import Inputs
 from clarifai.client.lister import Lister
@@ -47,159 +48,229 @@
       kwargs = {'user_id': user_id}
     self.kwargs = {**kwargs, 'id': app_id}
     self.app_info = resources_pb2.App(**self.kwargs)
     self.logger = get_logger(logger_level="INFO", name=__name__)
     BaseClient.__init__(self, user_id=self.user_id, app_id=self.id, base=base_url)
     Lister.__init__(self)
 
-  def list_datasets(self) -> List[Dataset]:
+  def list_datasets(self, page_no: int = None,
+                    per_page: int = None) -> Generator[Dataset, None, None]:
     """Lists all the datasets for the app.
 
-    Returns:
-        List[Dataset]: A list of Dataset objects for the datasets in the app.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Dataset: Dataset objects for the datasets in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_datasets = app.list_datasets()
+        >>> all_datasets = list(app.list_datasets())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(
-        user_app_id=self.user_app_id,
-        per_page=self.default_page_size,
-    )
-    all_datasets_info = list(
-        self.list_all_pages_generator(self.STUB.ListDatasets, service_pb2.ListDatasetsRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id,)
+    all_datasets_info = self.list_pages_generator(
+        self.STUB.ListDatasets,
+        service_pb2.ListDatasetsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
     for dataset_info in all_datasets_info:
       if 'version' in list(dataset_info.keys()):
         del dataset_info['version']['metrics']
+      yield Dataset(**dataset_info)
 
-    return [Dataset(**dataset_info) for dataset_info in all_datasets_info]
-
-  def list_models(self, filter_by: Dict[str, Any] = {}, only_in_app: bool = True) -> List[Model]:
+  def list_models(self,
+                  filter_by: Dict[str, Any] = {},
+                  only_in_app: bool = True,
+                  page_no: int = None,
+                  per_page: int = None) -> Generator[Model, None, None]:
     """Lists all the available models for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of models.
         only_in_app (bool): If True, only return models that are in the app.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Model]: A list of Model objects for the models in the app.
+    Yields:
+        Model: Model objects for the models in the app.
 
     Example:
         >>> from clarifai.client.user import User
         >>> app = User(user_id="user_id").app(app_id="app_id")
-        >>> all_models = app.list_models()
-    """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_models_info = list(
-        self.list_all_pages_generator(self.STUB.ListModels, service_pb2.ListModelsRequest,
-                                      request_data))
+        >>> all_models = list(app.list_models())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_models_info = self.list_pages_generator(
+        self.STUB.ListModels,
+        service_pb2.ListModelsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    filtered_models_info = []
     for model_info in all_models_info:
       if 'model_version' not in list(model_info.keys()):
         continue
       if only_in_app:
         if model_info['app_id'] != self.id:
           continue
-      filtered_models_info.append(model_info)
-
-    return [Model(**model_info) for model_info in filtered_models_info]
+      yield Model(**model_info)
 
-  def list_workflows(self, filter_by: Dict[str, Any] = {},
-                     only_in_app: bool = True) -> List[Workflow]:
+  def list_workflows(self,
+                     filter_by: Dict[str, Any] = {},
+                     only_in_app: bool = True,
+                     page_no: int = None,
+                     per_page: int = None) -> Generator[Workflow, None, None]:
     """Lists all the available workflows for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of workflows.
         only_in_app (bool): If True, only return workflows that are in the app.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Workflow]: A list of Workflow objects for the workflows in the app.
+    Yields:
+        Workflow: Workflow objects for the workflows in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_workflows = app.list_workflows()
+        >>> all_workflows = list(app.list_workflows())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_workflows_info = list(
-        self.list_all_pages_generator(self.STUB.ListWorkflows, service_pb2.ListWorkflowsRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_workflows_info = self.list_pages_generator(
+        self.STUB.ListWorkflows,
+        service_pb2.ListWorkflowsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    filtered_workflows_info = []
     for workflow_info in all_workflows_info:
       if only_in_app:
         if workflow_info['app_id'] != self.id:
           continue
-      filtered_workflows_info.append(workflow_info)
-
-    return [Workflow(**workflow_info) for workflow_info in all_workflows_info]
+      yield Workflow(**workflow_info)
 
-  def list_modules(self, filter_by: Dict[str, Any] = {}, only_in_app: bool = True) -> List[Module]:
+  def list_modules(self,
+                   filter_by: Dict[str, Any] = {},
+                   only_in_app: bool = True,
+                   page_no: int = None,
+                   per_page: int = None) -> Generator[Module, None, None]:
     """Lists all the available modules for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of modules.
         only_in_app (bool): If True, only return modules that are in the app.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Module]: A list of Module objects for the modules in the app.
+    Yields:
+        Module: Module objects for the modules in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_modules = app.list_modules()
+        >>> all_modules = list(app.list_modules())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_modules_info = list(
-        self.list_all_pages_generator(self.STUB.ListModules, service_pb2.ListModulesRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_modules_info = self.list_pages_generator(
+        self.STUB.ListModules,
+        service_pb2.ListModulesRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    filtered_modules_info = []
     for module_info in all_modules_info:
       if only_in_app:
         if module_info['app_id'] != self.id:
           continue
-      filtered_modules_info.append(module_info)
+      yield Module(**module_info)
 
-    return [Module(**module_info) for module_info in filtered_modules_info]
-
-  def list_installed_module_versions(self, filter_by: Dict[str, Any] = {}) -> List[Module]:
+  def list_installed_module_versions(self,
+                                     filter_by: Dict[str, Any] = {},
+                                     page_no: int = None,
+                                     per_page: int = None) -> Generator[Module, None, None]:
     """Lists all installed module versions in the app.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of installed module versions.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Module]: A list of Module objects for the installed module versions in the app.
+    Yields:
+        Module: Module objects for the installed module versions in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_installed_module_versions = app.list_installed_module_versions()
+        >>> all_installed_module_versions = list(app.list_installed_module_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_imv_infos = list(
-        self.list_all_pages_generator(self.STUB.ListInstalledModuleVersions,
-                                      service_pb2.ListInstalledModuleVersionsRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_imv_infos = self.list_pages_generator(
+        self.STUB.ListInstalledModuleVersions,
+        service_pb2.ListInstalledModuleVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
     for imv_info in all_imv_infos:
       del imv_info['deploy_url']
       del imv_info['installed_module_version_id']  # TODO: remove this after the backend fix
+      yield Module(module_id=imv_info['module_version']['module_id'], **imv_info)
+
+  def list_concepts(self, page_no: int = None,
+                    per_page: int = None) -> Generator[Concept, None, None]:
+    """Lists all the concepts for the app.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    return [
-        Module(module_id=imv_info['module_version']['module_id'], **imv_info)
-        for imv_info in all_imv_infos
-    ]
-
-  def list_concepts(self):
-    """Lists all the concepts for the app."""
-    pass  # TODO
+    Yields:
+        Concept: Concepts in the app.
+
+    Example:
+        >>> from clarifai.client.app import App
+        >>> app = App(app_id="app_id", user_id="user_id")
+        >>> all_concepts = list(app.list_concepts())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(user_app_id=self.user_app_id)
+    all_concepts_infos = self.list_pages_generator(
+        self.STUB.ListConcepts,
+        service_pb2.ListConceptsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
+    for concept_info in all_concepts_infos:
+      concept_info['id'] = concept_info.pop('concept_id')
+      yield Concept(**concept_info)
 
   def create_dataset(self, dataset_id: str, **kwargs) -> Dataset:
     """Creates a dataset for the app.
 
     Args:
         dataset_id (str): The dataset ID for the dataset to create.
         **kwargs: Additional keyword arguments to be passed to the Dataset.
@@ -566,15 +637,17 @@
         Search: A Search object for the user and app ID.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
         >>> search_client = app.search(top_k=12, metric="euclidean")
     """
-    return Search(**kwargs)
+    user_id = kwargs.get("user_id", self.user_app_id.user_id)
+    app_id = kwargs.get("app_id", self.user_app_id.app_id)
+    return Search(user_id=user_id, app_id=app_id, **kwargs)
 
   def __getattr__(self, name):
     return getattr(self.app_info, name)
 
   def __str__(self):
     init_params = [param for param in self.kwargs.keys()]
     attribute_strings = [
```

### Comparing `clarifai-9.9.2/clarifai/client/auth/helper.py` & `clarifai-9.9.3/clarifai/client/auth/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,24 +224,14 @@
         user_id: CLARIFAI_USER_ID env var.
         app_id: CLARIFAI_APP_ID env var.
         one of:
           token: CLARIFAI_SESSION_TOKEN env var.
           pat: CLARIFAI_PAT env var.
         base: CLARIFAI_API_BASE env var.
     """
-    error_description = """
-Please check the following required vars are in your env:
- - 'CLARIFAI_USER_ID': the user ID accessing the module.
- - 'CLARIFAI_APP_ID': the app the module is being accessed from.
- - 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT': to authenticate the calling user with a session token or personal access token.
-
-Additionally, these optional params are supported:
- - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
- - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
-"""
     user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
     token = os.environ.get("CLARIFAI_SESSION_TOKEN", "")
     pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
     return cls(user_id, app_id, pat, token, base, ui, validate)
```

### Comparing `clarifai-9.9.2/clarifai/client/auth/register.py` & `clarifai-9.9.3/clarifai/client/auth/register.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/client/auth/stub.py` & `clarifai-9.9.3/clarifai/client/auth/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/client/base.py` & `clarifai-9.9.3/clarifai/client/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/client/dataset.py` & `clarifai-9.9.3/clarifai/client/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,19 @@
         chunk_size (int): chunk size for concurrent upload of inputs and annotations
 
     Example:
         >>> from clarifai.client.dataset import Dataset
         >>> dataset = Dataset(user_id = 'user_id', app_id = 'demo_app', dataset_id = 'demo_dataset')
         >>> dataset.upload_from_csv(csv_path='csv_path', input_type='text', csv_type='raw, labels=True)
 
-    Note: csv file should have either one(input) or two columns(input, labels).
+    Note:
+        CSV file supports 'inputid', 'input', 'concepts', 'metadata', 'geopoints' columns.
+        All the data in the CSV should be in double quotes.
+        metadata should be in single quotes format. Example: "{'key': 'value'}"
+        geopoints should be in "long,lat" format.
     """
     if input_type not in ['image', 'text', 'video', 'audio']:
       raise UserError('Invalid input type, it should be image,text,audio or video')
     if csv_type not in ['raw', 'url', 'file_path']:
       raise UserError('Invalid csv type, it should be raw, url or file_path')
     assert csv_path.endswith('.csv'), 'csv_path should be a csv file'
     if csv_type == 'raw' and input_type != 'text':
```

### Comparing `clarifai-9.9.2/clarifai/client/input.py` & `clarifai-9.9.3/clarifai/client/input.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import csv
+import json
 import os
 import time
 import uuid
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from multiprocessing import cpu_count
-from typing import List, Union
+from typing import Generator, List, Union
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2  # noqa: F401
 from clarifai_grpc.grpc.api.resources_pb2 import Annotation, Audio, Image, Input, Text, Video
 from clarifai_grpc.grpc.api.status import status_code_pb2, status_pb2
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.struct_pb2 import Struct
 from tqdm import tqdm
@@ -304,53 +305,92 @@
     Example:
         >>> from clarifai.client.input import Inputs
         >>> input_obj = Inputs()
         >>> input_protos = input_obj.get_inputs_from_csv(csv_path='filepath', input_type='text', csv_type='raw')
     """
     input_protos = []
     with open(csv_path) as _file:
-      reader = csv.reader(_file)
-      next(reader, None)  # skip header
+      reader = csv.DictReader(_file, delimiter=',', quotechar='"')
+      columns = reader.fieldnames
+      for column in columns:
+        if column not in ['inputid', 'input', 'concepts', 'metadata', 'geopoints']:
+          raise UserError(
+              "CSV file may have 'inputid', 'input', 'concepts', 'metadata', 'geopoints' columns. Does not support '{}' column".
+              format(column))
       for id, input in enumerate(reader):
         if labels:
-          assert len(input) == 2, "csv file should have two columns(input, labels)"
-          labels = input[1] if isinstance(input[1], list) else [input[1]]
+          labels_list = input['concepts'].split(',')
+          labels = labels_list if len(input['concepts']) > 0 else None
         else:
           labels = None
 
-        input_id = uuid.uuid4().hex
-        text = input[0] if input_type == 'text' else None
-        image = input[0] if input_type == 'image' else None
-        video = input[0] if input_type == 'video' else None
-        audio = input[0] if input_type == 'audio' else None
+        if 'metadata' in columns:
+          if len(input['metadata']) > 0:
+            metadata_str = input['metadata'].replace("'", '"')
+            try:
+              metadata_dict = json.loads(metadata_str)
+            except json.decoder.JSONDecodeError:
+              raise UserError("metadata column in CSV file should be a valid json")
+            metadata = Struct()
+            metadata.update(metadata_dict)
+          else:
+            metadata = None
+        else:
+          metadata = None
+
+        if 'geopoints' in columns:
+          if len(input['geopoints']) > 0:
+            geo_points = input['geopoints'].split(',')
+            geo_points = [float(geo_point) for geo_point in geo_points]
+            geo_info = geo_points if len(geo_points) == 2 else UserError(
+                "geopoints column in CSV file should have longitude,latitude")
+          else:
+            geo_info = None
+        else:
+          geo_info = None
+
+        input_id = input['inputid'] if 'inputid' in columns else uuid.uuid4().hex
+        text = input['input'] if input_type == 'text' else None
+        image = input['input'] if input_type == 'image' else None
+        video = input['input'] if input_type == 'video' else None
+        audio = input['input'] if input_type == 'audio' else None
 
         if csv_type == 'raw':
           input_protos.append(
               self.get_text_input(
-                  input_id=input_id, raw_text=text, dataset_id=dataset_id, labels=labels))
+                  input_id=input_id,
+                  raw_text=text,
+                  dataset_id=dataset_id,
+                  labels=labels,
+                  metadata=metadata,
+                  geo_info=geo_info))
         elif csv_type == 'url':
           input_protos.append(
               self.get_input_from_url(
                   input_id=input_id,
                   image_url=image,
                   text_url=text,
                   audio_url=audio,
                   video_url=video,
                   dataset_id=dataset_id,
-                  labels=labels))
+                  labels=labels,
+                  metadata=metadata,
+                  geo_info=geo_info))
         else:
           input_protos.append(
               self.get_input_from_file(
                   input_id=input_id,
                   image_file=image,
                   text_file=text,
                   audio_file=audio,
                   video_file=video,
                   dataset_id=dataset_id,
-                  labels=labels))
+                  labels=labels,
+                  metadata=metadata,
+                  geo_info=geo_info))
 
     return input_protos
 
   def get_text_inputs_from_folder(self,
                                   folder_path: str,
                                   dataset_id: str = None,
                                   labels: bool = False) -> List[Text]:  #text specific
@@ -611,15 +651,15 @@
     request = service_pb2.PostAnnotationsRequest(
         user_app_id=self.user_app_id, annotations=batch_annot)
     response = self._grpc_request(self.STUB.PostAnnotations, request)
     if response.status.code != status_code_pb2.SUCCESS:
       try:
         self.logger.warning(
             f"Post annotations failed, status: {response.annotations[0].status.details}")
-      except:
+      except Exception:
         self.logger.warning(f"Post annotations failed, status: {response.status.details}")
       finally:
         retry_upload.extend(batch_annot)
     else:
       if show_log:
         self.logger.info("\nAnnotations Uploaded\n%s", response.status)
     return retry_upload
@@ -644,43 +684,113 @@
 
     Args:
         input_ids (Input): List of input objects to delete.
 
     Example:
         >>> from clarifai.client.user import User
         >>> input_obj = User(user_id="user_id").app(app_id="app_id").inputs()
-        >>> input_obj.delete_inputs(input_obj.list_inputs())
+        >>> input_obj.delete_inputs(list(input_obj.list_inputs()))
     """
     if not isinstance(inputs, list):
       raise UserError("input_ids must be a list of input ids")
     inputs_ids = [input.id for input in inputs]
     request = service_pb2.DeleteInputsRequest(user_app_id=self.user_app_id, ids=inputs_ids)
     response = self._grpc_request(self.STUB.DeleteInputs, request)
     if response.status.code != status_code_pb2.SUCCESS:
       raise Exception(response.status)
     self.logger.info("\nInputs Deleted\n%s", response.status)
 
-  def list_inputs(self) -> List[Input]:  # TODO: update lister
+  def list_inputs(self,
+                  dataset_id: str = None,
+                  page_no: int = None,
+                  per_page: int = None,
+                  input_type: str = None) -> Generator[Input, None, None]:
     """Lists all the inputs for the app.
 
-    Returns:
-        list of Input: A list of Input objects for the app.
+    Args:
+        dataset_id (str): The dataset ID for the dataset to list inputs from.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+        input_type (str): The type of input to list. Options: 'image', 'video', 'audio', 'text'.
+
+    Yields:
+        Input: Input objects for the app.
 
     Example:
         >>> from clarifai.client.user import User
         >>> input_obj = User(user_id="user_id").app(app_id="app_id").inputs()
-        >>> input_obj.list_inputs()
+        >>> all_inputs = list(input_obj.list_inputs(input_type='image'))
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size)
-    all_inputs_info = list(
-        self.list_all_pages_generator(self.STUB.ListInputs, service_pb2.ListInputsRequest,
-                                      request_data))
+    if input_type not in ['image', 'text', 'video', 'audio', None]:
+      raise UserError('Invalid input type, it should be image,text,audio or video')
+    if dataset_id:
+      request_data = dict(user_app_id=self.user_app_id, dataset_id=dataset_id)
+      all_inputs_info = self.list_pages_generator(
+          self.STUB.ListDatasetInputs,
+          service_pb2.ListDatasetInputsRequest,
+          request_data,
+          per_page=per_page,
+          page_no=page_no)
+    else:
+      request_data = dict(user_app_id=self.user_app_id)
+      all_inputs_info = self.list_pages_generator(
+          self.STUB.ListInputs,
+          service_pb2.ListInputsRequest,
+          request_data,
+          per_page=per_page,
+          page_no=page_no)
     for input_info in all_inputs_info:
-      input_info['id'] = input_info.pop('input_id')
-    return [resources_pb2.Input(**input_info) for input_info in all_inputs_info]
+      input_info['id'] = input_info.pop('dataset_input_id') if dataset_id else input_info.pop(
+          'input_id')
+      if input_type:
+        if input_type not in input_info['data'].keys():
+          continue
+      yield resources_pb2.Input(**input_info)
+
+  def list_annotations(self,
+                       batch_input: List[Input] = None,
+                       page_no: int = None,
+                       per_page: int = None) -> Generator[Annotation, None, None]:
+    """Lists all the annotations for the app.
+
+    Args:
+        batch_input (List[Input]): The input objects to list annotations from.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Annotation: Annotation objects for the app.
+
+    Example:
+        >>> from clarifai.client.user import User
+        >>> input_obj = User(user_id="user_id").app(app_id="app_id").inputs()
+        >>> all_inputs = list(input_obj.list_inputs(input_type='image'))
+        >>> all_annotations = list(input_obj.list_annotations(batch_input=all_inputs))
+
+    Note:
+        If batch_input is not given, then lists all the annotations for the app.
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(
+        user_app_id=self.user_app_id,
+        input_ids=[input.id for input in batch_input] if batch_input else None)
+    all_annotations_info = self.list_pages_generator(
+        self.STUB.ListAnnotations,
+        service_pb2.ListAnnotationsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
+    for annotations_info in all_annotations_info:
+      annotations_info['id'] = annotations_info.pop('annotation_id')
+      yield Annotation(**annotations_info)
 
   def _bulk_upload(self, inputs: List[Input], chunk_size: int = 128) -> None:
     """Uploads process for large number of inputs.
 
     Args:
         inputs (List[Input]): input protos
         chunk_size (int): chunk size for each request
```

### Comparing `clarifai-9.9.2/clarifai/client/lister.py` & `clarifai-9.9.3/clarifai/client/lister.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,47 @@
 
 class Lister(BaseClient):
   """Lister class for obtaining paginated results from the Clarifai API."""
 
   def __init__(self, page_size: int = 16):
     self.default_page_size = page_size
 
-  def list_all_pages_generator(
-      self, endpoint: Callable, proto_message: Any,
-      request_data: Dict[str, Any]) -> Generator[Dict[str, Any], None, None]:
-    """Lists all pages of a resource.
+  def list_pages_generator(self,
+                           endpoint: Callable,
+                           proto_message: Any,
+                           request_data: Dict[str, Any],
+                           page_no: int = None,
+                           per_page: int = None) -> Generator[Dict[str, Any], None, None]:
+    """Lists pages of a resource.
 
     Args:
         endpoint (Callable): The endpoint to call.
         proto_message (Any): The proto message to use.
         request_data (dict): The request data to use.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
     Yields:
         response_dict: The next item in the listing.
     """
-    page = 1
+    page = 1 if not page_no else page_no
+    if page_no and not per_page:
+      per_page = self.default_page_size
     while True:
       request_data['page'] = page
+      request_data['per_page'] = per_page
       response = self._grpc_request(endpoint, proto_message(**request_data))
       dict_response = MessageToDict(response, preserving_proto_field_name=True)
       if response.status.code != status_code_pb2.SUCCESS:
         raise Exception(f"Listing failed with response {response!r}")
       if len(list(dict_response.keys())) == 1:
         break
       else:
         listing_resource = list(dict_response.keys())[1]
         for item in dict_response[listing_resource]:
-          yield self.process_response_keys(item, listing_resource[:-1])
+          if listing_resource == "dataset_inputs":
+            yield self.process_response_keys(item["input"], listing_resource[:-1])
+          else:
+            yield self.process_response_keys(item, listing_resource[:-1])
+      if page_no is not None or per_page is not None:
+        break
       page += 1
```

### Comparing `clarifai-9.9.2/clarifai/client/model.py` & `clarifai-9.9.3/clarifai/client/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-from typing import Dict, List
+from typing import Dict, Generator, List
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from clarifai_grpc.grpc.api.resources_pb2 import Input
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from google.protobuf.json_format import MessageToDict
 
 from clarifai.client.base import BaseClient
@@ -86,44 +86,51 @@
 
     kwargs.update({'app_id': self.app_id, 'user_id': self.user_id})
     dict_response = MessageToDict(response, preserving_proto_field_name=True)
     kwargs = self.process_response_keys(dict_response['model'], 'model')
 
     return Model(**kwargs)
 
-  def list_versions(self) -> List['Model']:
+  def list_versions(self, page_no: int = None,
+                    per_page: int = None) -> Generator['Model', None, None]:
     """Lists all the versions for the model.
 
-    Returns:
-        List[Model]: A list of Model objects for the versions of the model.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Model: Model objects for the versions of the model.
 
     Example:
         >>> from clarifai.client.model import Model
         >>> model = Model("model_url") # Example URL: https://clarifai.com/clarifai/main/models/general-image-recognition
                     or
         >>> model = Model(model_id='model_id', user_id='user_id', app_id='app_id')
-        >>> all_model_versions = model.list_versions()
+        >>> all_model_versions = list(model.list_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
     request_data = dict(
         user_app_id=self.user_app_id,
         model_id=self.id,
-        per_page=self.default_page_size,
     )
-    all_model_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListModelVersions,
-                                      service_pb2.ListModelVersionsRequest, request_data))
+    all_model_versions_info = self.list_pages_generator(
+        self.STUB.ListModelVersions,
+        service_pb2.ListModelVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
     for model_version_info in all_model_versions_info:
       model_version_info['id'] = model_version_info['model_version_id']
       del model_version_info['model_version_id']
-
-    return [
-        Model(model_id=self.id, **dict(self.kwargs, model_version=model_version_info))
-        for model_version_info in all_model_versions_info
-    ]
+      yield Model(model_id=self.id, **dict(self.kwargs, model_version=model_version_info))
 
   def predict(self, inputs: List[Input]):
     """Predicts the model based on the given inputs.
 
     Args:
         inputs (list[Input]): The inputs to predict, must be less than 128.
     """
@@ -240,45 +247,14 @@
           data=resources_pb2.Data(video=resources_pb2.Video(url=url)))
     elif input_type == "audio":
       input_proto = resources_pb2.Input(
           data=resources_pb2.Data(audio=resources_pb2.Audio(url=url)))
 
     return self.predict(inputs=[input_proto])
 
-  def list_versions(self) -> List['Model']:
-    """Lists all the versions for the model.
-
-    Returns:
-        List[Model]: A list of Model objects for the versions of the model.
-
-    Example:
-        >>> from clarifai.client.model import Model
-        >>> model = Model("model_url") # Example URL: https://clarifai.com/clarifai/main/models/general-image-recognition
-                    or
-        >>> model = Model(model_id='model_id', user_id='user_id', app_id='app_id')
-        >>> all_model_versions = model.list_versions()
-    """
-    request_data = dict(
-        user_app_id=self.user_app_id,
-        model_id=self.id,
-        per_page=self.default_page_size,
-    )
-    all_model_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListModelVersions,
-                                      service_pb2.ListModelVersionsRequest, request_data))
-
-    for model_version_info in all_model_versions_info:
-      model_version_info['id'] = model_version_info['model_version_id']
-      del model_version_info['model_version_id']
-
-    return [
-        Model(model_id=self.id, **dict(self.kwargs, model_version=model_version_info))
-        for model_version_info in all_model_versions_info
-    ]
-
   def __getattr__(self, name):
     return getattr(self.model_info, name)
 
   def __str__(self):
     init_params = [param for param in self.kwargs.keys()]
     attribute_strings = [
         f"{param}={getattr(self.model_info, param)}" for param in init_params
```

### Comparing `clarifai-9.9.2/clarifai/client/module.py` & `clarifai-9.9.3/clarifai/client/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List
+from typing import Dict, Generator
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 
 from clarifai.client.base import BaseClient
 from clarifai.client.lister import Lister
 from clarifai.errors import UserError
 from clarifai.urls.helper import ClarifaiUrlHelper
@@ -39,42 +39,49 @@
 
     self.kwargs = {**kwargs, 'id': module_id, 'module_version': module_version}
     self.module_info = resources_pb2.Module(**self.kwargs)
     self.logger = get_logger(logger_level="INFO")
     BaseClient.__init__(self, user_id=self.user_id, app_id=self.app_id, base=base_url)
     Lister.__init__(self)
 
-  def list_versions(self) -> List['Module']:
+  def list_versions(self, page_no: int = None,
+                    per_page: int = None) -> Generator['Module', None, None]:
     """Lists all the module versions for the module.
 
-        Returns:
-            List[Moudle]: A list of Module objects for versions of the module.
-
-        Example:
-            >>> from clarifai.client.module import Module
-            >>> module = Module(module_id='module_id', user_id='user_id', app_id='app_id')
-            >>> all_Module_versions = module.list_versions()
-        """
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Moudle: Module objects for versions of the module.
+
+    Example:
+        >>> from clarifai.client.module import Module
+        >>> module = Module(module_id='module_id', user_id='user_id', app_id='app_id')
+        >>> all_Module_versions = list(module.list_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
     request_data = dict(
         user_app_id=self.user_app_id,
         module_id=self.id,
-        per_page=self.default_page_size,
     )
-    all_module_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListModuleVersions,
-                                      service_pb2.ListModuleVersionsRequest, request_data))
+    all_module_versions_info = self.list_pages_generator(
+        self.STUB.ListModuleVersions,
+        service_pb2.ListModuleVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
     for module_version_info in all_module_versions_info:
       module_version_info['id'] = module_version_info['module_version_id']
       del module_version_info['module_version_id']
-
-    return [
-        Module(module_id=self.id, **dict(self.kwargs, module_version=module_version_info))
-        for module_version_info in all_module_versions_info
-    ]
+      yield Module(module_id=self.id, **dict(self.kwargs, module_version=module_version_info))
 
   def __getattr__(self, name):
     return getattr(self.module_info, name)
 
   def __str__(self):
     init_params = [param for param in self.kwargs.keys()]
     attribute_strings = [
```

### Comparing `clarifai-9.9.2/clarifai/client/runner.py` & `clarifai-9.9.3/clarifai/client/runner.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/client/search.py` & `clarifai-9.9.3/clarifai/client/search.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/client/user.py` & `clarifai-9.9.3/clarifai/client/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List
+from typing import Any, Dict, Generator, List
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from google.protobuf.json_format import MessageToDict
 
 from clarifai.client.app import App
 from clarifai.client.base import BaseClient
@@ -25,54 +25,75 @@
     """
     self.kwargs = {**kwargs, 'id': user_id}
     self.user_info = resources_pb2.User(**self.kwargs)
     self.logger = get_logger(logger_level="INFO", name=__name__)
     BaseClient.__init__(self, user_id=self.id, app_id="", base=base_url)
     Lister.__init__(self)
 
-  def list_apps(self, filter_by: Dict[str, Any] = {}) -> List[App]:
+  def list_apps(self, filter_by: Dict[str, Any] = {}, page_no: int = None,
+                per_page: int = None) -> Generator[App, None, None]:
     """Lists all the apps for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to be applied to the list of apps.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        list of App: A list of App objects for the user.
+    Yields:
+        App: App objects for the user.
 
     Example:
         >>> from clarifai.client.user import User
-        >>> apps = User("user_id").list_apps()
-    """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_apps_info = list(
-        self.list_all_pages_generator(self.STUB.ListApps, service_pb2.ListAppsRequest,
-                                      request_data))
+        >>> apps = list(User("user_id").list_apps())
 
-    return [App(**app_info) for app_info in all_apps_info]
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_apps_info = self.list_pages_generator(
+        self.STUB.ListApps,
+        service_pb2.ListAppsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
+    for app_info in all_apps_info:
+      yield App(**app_info)
 
-  def list_runners(self, filter_by: Dict[str, Any] = {}) -> List[Runner]:
+  def list_runners(self, filter_by: Dict[str, Any] = {}, page_no: int = None,
+                   per_page: int = None) -> Generator[Runner, None, None]:
     """List all runners for the user
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of runners.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Runner]: A list of Runner objects for the runners.
+    Yields:
+        Runner: Runner objects for the runners.
 
     Example:
         >>> from clarifai.client.user import User
         >>> client = User(user_id="user_id")
-        >>> all_runners= client.list_runners()
+        >>> all_runners= list(client.list_runners())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_runners_info = list(
-        self.list_all_pages_generator(self.STUB.ListRunners, service_pb2.ListRunnersRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_runners_info = self.list_pages_generator(
+        self.STUB.ListRunners,
+        service_pb2.ListRunnersRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    return [Runner(check_runner_exists=False, **runner_info) for runner_info in all_runners_info]
+    for runner_info in all_runners_info:
+      yield Runner(check_runner_exists=False, **runner_info)
 
   def create_app(self, app_id: str, base_workflow: str = 'Language-Understanding',
                  **kwargs) -> App:
     """Creates an app for the user.
 
     Args:
         app_id (str): The app ID for the app to create.
```

### Comparing `clarifai-9.9.2/clarifai/client/workflow.py` & `clarifai-9.9.3/clarifai/client/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Dict, List
+from typing import Dict, Generator, List
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from clarifai_grpc.grpc.api.resources_pb2 import Input
 from clarifai_grpc.grpc.api.status import status_code_pb2
 
 from clarifai.client.base import BaseClient
 from clarifai.client.lister import Lister
@@ -152,42 +152,49 @@
           data=resources_pb2.Data(video=resources_pb2.Video(url=url)))
     elif input_type == "audio":
       input_proto = resources_pb2.Input(
           data=resources_pb2.Data(audio=resources_pb2.Audio(url=url)))
 
     return self.predict(inputs=[input_proto])
 
-  def list_versions(self) -> List['Workflow']:
+  def list_versions(self, page_no: int = None,
+                    per_page: int = None) -> Generator['Workflow', None, None]:
     """Lists all the versions of the workflow.
 
-    Returns:
-        list[Workflow]: A list of Workflow objects.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Workflow: Workflow objects for versions of the workflow.
 
     Example:
         >>> from clarifai.client.workflow import Workflow
         >>> workflow = Workflow(user_id='user_id', app_id='app_id', workflow_id='workflow_id')
-        >>> workflow_versions = workflow.list_versions()
+        >>> workflow_versions = list(workflow.list_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
     request_data = dict(
         user_app_id=self.user_app_id,
         workflow_id=self.id,
-        per_page=self.default_page_size,
     )
-    all_workflow_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListWorkflowVersions,
-                                      service_pb2.ListWorkflowVersionsRequest, request_data))
+    all_workflow_versions_info = self.list_pages_generator(
+        self.STUB.ListWorkflowVersions,
+        service_pb2.ListWorkflowVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
     for workflow_version_info in all_workflow_versions_info:
       workflow_version_info['id'] = workflow_version_info['workflow_version_id']
       del workflow_version_info['workflow_version_id']
-
-    return [
-        Workflow(workflow_id=self.id, **dict(self.kwargs, version=workflow_version_info))
-        for workflow_version_info in all_workflow_versions_info
-    ]
+      yield Workflow(workflow_id=self.id, **dict(self.kwargs, version=workflow_version_info))
 
   def export(self, out_path: str):
     """Exports the workflow to a yaml file.
 
     Args:
         out_path (str): The path to save the yaml file to.
```

### Comparing `clarifai-9.9.2/clarifai/datasets/export/inputs_annotations.py` & `clarifai-9.9.3/clarifai/datasets/export/inputs_annotations.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/base.py` & `clarifai-9.9.3/clarifai/datasets/upload/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/README.md` & `clarifai-9.9.3/clarifai/datasets/upload/examples/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,11 +32,15 @@
     return data
 
   def __getitem__(self, index):
     item = self.data[index]
     return VisualClassificationFeatures(
         image_path=os.path.join(os.path.dirname(__file__), item[0]),
         label=item[1],
-        id=os.path.basename(item[0]).split(".")[0])
+        id=os.path.basename(item[0]).split(".")[0],
+        metadata={
+            "split": self.split,
+            "image_path": item[0]
+        })
 
   def __len__(self):
     return len(self.data)
```

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg` & `clarifai-9.9.3/clarifai/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,20 @@
     self.load_data()
 
   def load_data(self):
     with open(self.data_dirs[self.split]) as _file:
       reader = csv.reader(_file)
       next(reader, None)  # skip header
       for review in reader:
-        self.data.append({"text": review[0], "labels": review[1], "id": None})
+        self.data.append({
+            "text": review[0],
+            "labels": review[1],
+            "id": None,
+            "metadata": dict(split=self.split)
+        })
 
   def __getitem__(self, idx):
     item = self.data[idx]
     return TextFeatures(text=item["text"], labels=item["labels"], id=item["id"])
 
   def __len__(self):
     return len(self.data)
```

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/test.csv` & `clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/test.csv`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/examples/text_classification/imdb_dataset/train.csv` & `clarifai-9.9.3/clarifai/datasets/upload/examples/text_classification/imdb_dataset/train.csv`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/features.py` & `clarifai-9.9.3/clarifai/datasets/upload/features.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,40 @@
 
 @dataclass
 class TextFeatures:
   """Text classification datasets preprocessing output features."""
   text: str
   labels: List[Union[str, int]]  # List[str or int] to cater for multi-class tasks
   id: Optional[int] = None  # text_id
+  metadata: Optional[dict] = None
 
 
 @dataclass
 class VisualClassificationFeatures:
   """Image classification datasets preprocessing output features."""
   image_path: str
   label: Union[str, int]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
+  metadata: Optional[dict] = None
 
 
 @dataclass
 class VisualDetectionFeatures:
   """Image Detection datasets preprocessing output features."""
   image_path: str
   classes: List[Union[str, int]]
   bboxes: List[List[float]]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
+  metadata: Optional[dict] = None
 
 
 @dataclass
 class VisualSegmentationFeatures:
   """Image Segmentation datasets preprocessing output features."""
   image_path: str
   classes: List[Union[str, int]]
   polygons: List[List[List[float]]]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
+  metadata: Optional[dict] = None
```

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/image.py` & `clarifai-9.9.3/clarifai/datasets/upload/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,18 @@
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       image_path = datagen_item.image_path
       label = datagen_item.label if isinstance(datagen_item.label,
                                                list) else [datagen_item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
       geo_info = datagen_item.geo_info
-      metadata.update({"filename": os.path.basename(image_path), "split": self.split})
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"filename": os.path.basename(image_path), "split": self.split})
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_input_from_file(
               input_id=input_id,
               image_file=image_path,
               dataset_id=self.dataset_id,
@@ -71,16 +74,19 @@
 
     def process_datagen_item(id):
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       image = datagen_item.image_path
       labels = datagen_item.classes  # list:[l1,...,ln]
       bboxes = datagen_item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
-      input_id = f"{self.dataset_id}-{self.split}-{i}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
-      metadata.update({"filename": os.path.basename(image), "split": self.split})
+      input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = datagen_item.geo_info
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_input_from_file(
               input_id=input_id,
               image_file=image,
@@ -121,16 +127,19 @@
 
     def process_datagen_item(id):
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       image = datagen_item.image_path
       labels = datagen_item.classes
       _polygons = datagen_item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
-      input_id = f"{self.dataset_id}-{self.split}-{i}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
-      metadata.update({"filename": os.path.basename(image), "split": self.split})
+      input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = datagen_item.geo_info
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_input_from_file(
               input_id=input_id,
               image_file=image,
```

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/loaders/README.md` & `clarifai-9.9.3/clarifai/datasets/upload/loaders/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/loaders/coco_captions.py` & `clarifai-9.9.3/clarifai/datasets/upload/loaders/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/loaders/coco_detection.py` & `clarifai-9.9.3/clarifai/datasets/upload/loaders/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/loaders/coco_segmentation.py` & `clarifai-9.9.3/clarifai/datasets/upload/loaders/coco_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,22 +123,22 @@
     image_height, image_width = cv2.imread(image_path).shape[:2]
     for cat_id in labels:
       annot_ids = self.coco.getAnnIds(imgIds=_id, catIds=[cat_id])
       if len(annot_ids) > 0:
         img_annotations = self.coco.loadAnns(annot_ids)
         for ann in img_annotations:
           # get polygons
-          if type(ann['segmentation']) == list:
+          if isinstance(ann['segmentation'], list):
             for seg in ann['segmentation']:
               poly = np.array(seg).reshape((int(len(seg) / 2), 2))
               poly[:, 0], poly[:, 1] = poly[:, 0] / image_width, poly[:, 1] / image_height
               annots.append(poly.tolist())  #[[x=col, y=row],...]
               class_names.append(self.cat_id_map[cat_id])
           else:  # seg: {"counts":[...]}
-            if type(ann['segmentation']['counts']) == list:
+            if isinstance(ann['segmentation']['counts'], list):
               rle = maskUtils.frPyObjects([ann['segmentation']], image_height, image_width)
             else:
               rle = ann['segmentation']
             mask = maskUtils.decode(rle)  #binary mask
             #convert mask to polygons and add to annots
             contours, _ = cv2.findContours(mask, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             polygons = []
```

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/loaders/imagenet_classification.py` & `clarifai-9.9.3/clarifai/datasets/upload/loaders/imagenet_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             "".join(("".join((label.rstrip().lstrip().split(" ")))).split("'"))
             for label in _id[_id.find(" ") + 1:].split(",")
         })
 
     for _folder in os.listdir(os.path.join(self.data_dir, self.split)):
       try:
         concept = self.label_map[_folder]  #concepts
-      except:
+      except Exception:
         continue
       folder_path = os.path.join(self.data_dir, self.split) + "/" + _folder
       for _img in os.listdir(folder_path):
         if _img.lower().endswith(('.png', '.jpg', '.jpeg', '.tiff')):
           self.concepts.append(concept)
           self.image_paths.append(folder_path + "/" + _img)
```

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/loaders/xview_detection.py` & `clarifai-9.9.3/clarifai/datasets/upload/loaders/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/text.py` & `clarifai-9.9.3/clarifai/datasets/upload/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,18 @@
     def process_datagen_item(id):
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       text = datagen_item.text
       labels = datagen_item.labels if isinstance(
           datagen_item.labels, list) else [datagen_item.labels]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
-      metadata.update({"split": self.split})
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"split": self.split})
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_text_input(
               input_id=input_id,
               raw_text=text,
               dataset_id=self.dataset_id,
```

### Comparing `clarifai-9.9.2/clarifai/datasets/upload/utils.py` & `clarifai-9.9.3/clarifai/datasets/upload/utils.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/errors.py` & `clarifai-9.9.3/clarifai/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     current_ts_str = str(time.time())
 
     msg = """%(method)s %(resource)s FAILED(%(time_ts)s).  error_code: %(error_code)s, error_description: %(error_desc)s, error_details: %(error_details)s
  >> Python client %(client_version)s with Python %(python_version)s on %(os_version)s
  >> %(method)s %(resource)s
  >> REQUEST(%(time_ts)s) %(request)s
  >> RESPONSE(%(time_ts)s) %(response)s""" % {
-        'baseurl': '%s/v2/' % _base_url(self.resource),
         'method': method,
         'resource': resource,
         'error_code': self.error_code,
         'error_desc': self.error_desc,
         'error_details': self.error_details,
         'request': json.dumps(params, indent=2),
         'response': response_json,
@@ -74,15 +73,15 @@
 def _base_url(url: str) -> str:
   """
   Extracts the base URL from the url, which is everything before the 4th slash character.
   https://www.clarifai.com/v2/models/1/output -> https://www.clarifai.com/v2/
   """
   try:
     return url[:_find_nth(url, '/', 4) + 1]
-  except:
+  except Exception:
     return ''
 
 
 def _find_nth(haystack: str, needle: str, n: int) -> int:
   start = haystack.find(needle)
   while start >= 0 and n > 1:
     start = haystack.find(needle, start + len(needle))
```

### Comparing `clarifai-9.9.2/clarifai/models/api.py` & `clarifai-9.9.3/clarifai/models/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/README.md` & `clarifai-9.9.3/clarifai/models/model_serving/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/__init__.py` & `clarifai-9.9.3/clarifai/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/cli/__init__.py` & `clarifai-9.9.3/clarifai/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/cli/deploy_cli.py` & `clarifai-9.9.3/clarifai/models/model_serving/cli/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/cli/model_zip.py` & `clarifai-9.9.3/clarifai/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/cli/repository.py` & `clarifai-9.9.3/clarifai/models/model_serving/cli/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
       help=f"Clarifai supported model types.\n Model-types-map: {MODEL_TYPES}",
   )
   parser.add_argument(
       "--image_shape",
       type=dims_type,
       default="[-1, -1]",
       required=False,
-      help=
-      f"(H, W) dims for models with an image input type. H and W each have a max value of 1024",
+      help="(H, W) dims for models with an image input type. H and W each have a max value of 1024",
   )
   parser.add_argument(
       "--repo_dir",
       type=str,
       default=".",
       required=True,
       help="Directory to create triton repository.")
```

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/docs/custom_config.md` & `clarifai-9.9.3/clarifai/models/model_serving/docs/custom_config.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/docs/dependencies.md` & `clarifai-9.9.3/clarifai/models/model_serving/docs/dependencies.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/docs/model_types.md` & `clarifai-9.9.3/clarifai/models/model_serving/docs/model_types.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/docs/output.md` & `clarifai-9.9.3/clarifai/models/model_serving/docs/output.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/README.md` & `clarifai-9.9.3/clarifai/models/model_serving/examples/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json` & `clarifai-9.9.3/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/README.md` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/README.md` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/model.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/README.md` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/labels.txt` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_detection/yolov5x/labels.txt`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/model.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py` & `clarifai-9.9.3/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/model_config/__init__.py` & `clarifai-9.9.3/clarifai/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/model_config/config.py` & `clarifai-9.9.3/clarifai/models/model_serving/model_config/config.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/model_config/model_types_config/visual-detector.yaml` & `clarifai-9.9.3/clarifai/models/model_serving/model_config/model_types_config/visual-detector.yaml`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/model_config/serializer.py` & `clarifai-9.9.3/clarifai/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/models/__init__.py` & `clarifai-9.9.3/clarifai/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/models/default_test.py` & `clarifai-9.9.3/clarifai/models/model_serving/models/default_test.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/models/inference.py` & `clarifai-9.9.3/clarifai/models/model_serving/models/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/models/model_types.py` & `clarifai-9.9.3/clarifai/models/model_serving/models/model_types.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/models/output.py` & `clarifai-9.9.3/clarifai/models/model_serving/models/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
           scores-dims: {self.predicted_scores.ndim} instead."
     assert self.predicted_bboxes.shape[0] == self.predicted_labels.shape[0] == \
       self.predicted_scores.shape[0], f"The Number of predicted bounding boxes, \
         predicted labels and predicted scores MUST match. Got {len(self.predicted_bboxes)}, \
           {self.predicted_labels.shape[0]}, {self.predicted_scores.shape[0]} instead."
 
     if len(self.predicted_labels) > 0:
-      assert self.predicted_bboxes.shape[1] == 4, f"Box coordinates must have a length of 4."
+      assert self.predicted_bboxes.shape[
+          1] == 4, f"Box coordinates must have a length of 4. Actual:{self.predicted_bboxes.shape[1]}"
       assert np.all(np.logical_and(0 <= self.predicted_bboxes, self.predicted_bboxes <= 1)), \
        "Bounding box coordinates must be between 0 and 1"
 
 
 @dataclass
 class ClassifierOutput:
   """
```

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/models/pb_model.py` & `clarifai-9.9.3/clarifai/models/model_serving/models/pb_model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/models/test.py` & `clarifai-9.9.3/clarifai/models/model_serving/models/test.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/models/model_serving/pb_model_repository.py` & `clarifai-9.9.3/clarifai/models/model_serving/pb_model_repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/modules/css.py` & `clarifai-9.9.3/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/modules/pages.py` & `clarifai-9.9.3/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/modules/style.css` & `clarifai-9.9.3/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/runners/example.py` & `clarifai-9.9.3/clarifai/runners/example.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/schema/search.py` & `clarifai-9.9.3/clarifai/schema/search.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/urls/helper.py` & `clarifai-9.9.3/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/utils/logging.py` & `clarifai-9.9.3/clarifai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/utils/misc.py` & `clarifai-9.9.3/clarifai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/workflows/export.py` & `clarifai-9.9.3/clarifai/workflows/export.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/workflows/utils.py` & `clarifai-9.9.3/clarifai/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai/workflows/validate.py` & `clarifai-9.9.3/clarifai/workflows/validate.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai.egg-info/PKG-INFO` & `clarifai-9.9.3/clarifai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.9.2
+Version: 9.9.3
 Summary: Clarifai Python SDK
 Home-page: https://github.com/Clarifai/clarifai-python
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
@@ -21,36 +21,26 @@
 <h2 align="center">
 Clarifai Python SDK</a>
 </h2>
 
 
 
 <p align="center">
-  <a href="https://clarifaicommunity.slack.com/" target="_blank"> <img src="https://img.shields.io/badge/slack-chat-green.svg?logo=slack&color=4ec528" alt="Slack">
+  <a href="https://discord.gg/M32V7a7a" target="_blank"> <img src="https://img.shields.io/badge/discord-chat-green.svg?logo=discord&color=4ec528" alt="Discord">
+  </a>
+  <a href="https://pypi.org/project/clarifai" target="_blank"> <img src="https://img.shields.io/pypi/dm/clarifai" alt="PyPI - Downloads">
   </a>
-
 </p>
 
 
 
 
 This is the official Python client for interacting with our powerful [API](https://docs.clarifai.com). The Clarifai Python SDK offers a comprehensive set of tools to integrate Clarifai's AI platform to leverage computer vision capabiities like classification , detection ,segementation and natural language capabilities like classification , summarisation , generation , Q&A ,etc into your applications. With just a few lines of code, you can leverage cutting-edge artificial intelligence to unlock valuable insights from visual and textual content.
 
----
-**Website**: [https://www.clarifai.com](https://www.clarifai.com/)
-
-**Demo**: [https://clarifai.com/demo](https://clarifai.com/demo)
-
-**Sign up for a free Account**: [https://clarifai.com/signup](https://clarifai.com/signup)
-
-**Developer Guide**: [https://docs.clarifai.com](https://docs.clarifai.com/)
-
-**Clarifai Community**: [https://clarifai.com/explore](https://clarifai.com/explore)
-
-**Python SDK Docs**: [https://docs.clarifai.com/python-sdk/api-reference](https://docs.clarifai.com/python-sdk/api-reference)
+[Website](https://www.clarifai.com/) | [Demo](https://clarifai.com/demo) | [Signup for a Free Account](https://clarifai.com/signup) | [API Docs](https://docs.clarifai.com/) | [Clarifai Community](https://clarifai.com/explore) | [Python SDK Docs](https://docs.clarifai.com/python-sdk/api-reference) | [Examples](https://github.com/Clarifai/examples) | [Colab Notebooks](https://github.com/Clarifai/colab-notebooks)
 
 
 ---
 
 ## Installation
 
 
@@ -84,15 +74,16 @@
 
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.user import User
 client = User(user_id="user_id")
 
 # Get all apps
-apps = client.list_apps()
+apps_generator = client.list_apps()
+apps = list(apps_generator)
 ```
 
 ### Interacting with Datasets
 
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
@@ -114,33 +105,45 @@
 # Note: clarifai-data-protobuf.zip is acquired through exporting datasets within the Clarifai Platform.
 Dataset().export(save_path='output.zip', local_archive_path='clarifai-data-protobuf.zip')
 ```
 
 
 ### Interacting with Inputs
 
+#### Input upload
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.user import User
 app = User(user_id="user_id").app(app_id="app_id")
 input_obj = app.inputs()
 
 #input upload from url
 input_obj.upload_from_url(input_id = 'demo', image_url='https://samples.clarifai.com/metro-north.jpg')
 
 #input upload from filename
 input_obj.upload_from_file(input_id = 'demo', video_file='demo.mp4')
 
-#listing inputs
-input_obj.list_inputs()
-
 # text upload
 input_obj.upload_text(input_id = 'demo', raw_text = 'This is a test')
 ```
 
+#### Input listing
+```python
+#listing inputs
+input_generator = input_obj.list_inputs(page_no=1,per_page=10,input_type='image')
+inputs_list = list(input_generator)
+
+#listing annotations
+annotation_generator = input_obj.list_annotations(batch_input=inputs_list)
+annotations_list = list(annotation_generator)
+
+#listing concepts
+all_concepts = list(app.list_concepts())
+```
+
 
 ### Interacting with Models
 
 #### Model Predict
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.model import Model
@@ -161,25 +164,26 @@
 model_prediction = model.predict_by_url(url="VIDEO_URL", input_type="video")
 ```
 #### Models Listing
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
 # List all model versions
-all_model_versions = model.list_versions()
+all_model_versions = list(model.list_versions())
 
 # Go to specific model version
 model_v1 = client.app("app_id").model(model_id="model_id", model_version_id="model_version_id")
 
 # List all models in an app
-all_models = app.list_models()
+all_models = list(app.list_models())
 
 # List all models in community filtered by model_type, description
 all_llm_community_models = App().list_models(filter_by={"query": "LLM",
                                                         "model_type_id": "text-to-text"}, only_in_app=False)
+all_llm_community_models = list(all_llm_community_models)
 ```
 
 ### Interacting with Workflows
 
 #### Workflow Predict
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
@@ -196,24 +200,25 @@
 ```
 
 #### Workflows Listing
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 
 # List all workflow versions
-all_workflow_versions = workflow.list_versions()
+all_workflow_versions = list(workflow.list_versions())
 
 # Go to specific workflow version
 workflow_v1 = Workflow(workflow_id="workflow_id", workflow_version=dict(id="workflow_version_id"), app_id="app_id", user_id="user_id")
 
 # List all workflow in an app
-all_workflow = app.list_workflow()
+all_workflow = list(app.list_workflow())
 
 # List all workflow in community filtered by description
 all_face_community_workflows = App().list_workflows(filter_by={"query": "face"}, only_in_app=False) # Get all face related workflows
+all_face_community_workflows = list(all_face_community_workflows)
 ```
 #### Workflow Create
 Create a new workflow specified by a yaml config file.
 ```python
 # Note: CLARIFAI_PAT must be set as env variable.
 from clarifai.client.app import App
 app = App(app_id="app_id", user_id="user_id")
```

#### html2text {}

```diff
@@ -1,104 +1,111 @@
-Metadata-Version: 2.1 Name: clarifai Version: 9.9.2 Summary: Clarifai Python
+Metadata-Version: 2.1 Name: clarifai Version: 9.9.3 Summary: Clarifai Python
 SDK Home-page: https://github.com/Clarifai/clarifai-python Author: Clarifai
 Author-email: support@clarifai.com License: Apache 2.0 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                            ************ _[[_CC_ll_aa_rr_ii_ff_aa_ii_]] ************
                         ********** CCllaarriiffaaii PPyytthhoonn SSDDKK **********
-                                    _[_S_l_a_c_k_]
+                          _[_D_i_s_c_o_r_d_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]
 This is the official Python client for interacting with our powerful [API]
 (https://docs.clarifai.com). The Clarifai Python SDK offers a comprehensive set
 of tools to integrate Clarifai's AI platform to leverage computer vision
 capabiities like classification , detection ,segementation and natural language
 capabilities like classification , summarisation , generation , Q&A ,etc into
 your applications. With just a few lines of code, you can leverage cutting-edge
 artificial intelligence to unlock valuable insights from visual and textual
-content. --- **Website**: [https://www.clarifai.com](https://www.clarifai.com/
-) **Demo**: [https://clarifai.com/demo](https://clarifai.com/demo) **Sign up
-for a free Account**: [https://clarifai.com/signup](https://clarifai.com/
-signup) **Developer Guide**: [https://docs.clarifai.com](https://
-docs.clarifai.com/) **Clarifai Community**: [https://clarifai.com/explore]
-(https://clarifai.com/explore) **Python SDK Docs**: [https://docs.clarifai.com/
-python-sdk/api-reference](https://docs.clarifai.com/python-sdk/api-reference) -
--- ## Installation Install from PyPi: ```bash pip install -U clarifai ```
-Install from Source: ```bash git clone https://github.com/Clarifai/clarifai-
-python.git cd clarifai-python python3 -m venv env source env/bin/activate pip3
-install -r requirements.txt ``` ## Getting started Clarifai uses **Personal
-Access Tokens(PATs)** to validate requests. You can create and manage PATs
-under your Clarifai account security settings. Export your PAT as an
-environment variable. Then, import and initialize the API Client. ```cmd export
-CLARIFAI_PAT={your personal access token} ``` ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.user import User client =
-User(user_id="user_id") # Get all apps apps = client.list_apps() ``` ###
-Interacting with Datasets ```python # Note: CLARIFAI_PAT must be set as env
-variable. # Create app and dataset app = client.create_app(app_id="demo_app",
-base_workflow="Universal") dataset = app.create_dataset
-(dataset_id="demo_dataset") # execute data upload to Clarifai app dataset
-dataset.upload_dataset(task='visual_segmentation', split="train",
+content. [Website](https://www.clarifai.com/) | [Demo](https://clarifai.com/
+demo) | [Signup for a Free Account](https://clarifai.com/signup) | [API Docs]
+(https://docs.clarifai.com/) | [Clarifai Community](https://clarifai.com/
+explore) | [Python SDK Docs](https://docs.clarifai.com/python-sdk/api-
+reference) | [Examples](https://github.com/Clarifai/examples) | [Colab
+Notebooks](https://github.com/Clarifai/colab-notebooks) --- ## Installation
+Install from PyPi: ```bash pip install -U clarifai ``` Install from Source:
+```bash git clone https://github.com/Clarifai/clarifai-python.git cd clarifai-
+python python3 -m venv env source env/bin/activate pip3 install -
+r requirements.txt ``` ## Getting started Clarifai uses **Personal Access
+Tokens(PATs)** to validate requests. You can create and manage PATs under your
+Clarifai account security settings. Export your PAT as an environment variable.
+Then, import and initialize the API Client. ```cmd export CLARIFAI_PAT={your
+personal access token} ``` ```python # Note: CLARIFAI_PAT must be set as env
+variable. from clarifai.client.user import User client = User
+(user_id="user_id") # Get all apps apps_generator = client.list_apps() apps =
+list(apps_generator) ``` ### Interacting with Datasets ```python # Note:
+CLARIFAI_PAT must be set as env variable. # Create app and dataset app =
+client.create_app(app_id="demo_app", base_workflow="Universal") dataset =
+app.create_dataset(dataset_id="demo_dataset") # execute data upload to Clarifai
+app dataset dataset.upload_dataset(task='visual_segmentation', split="train",
 dataset_loader='coco_segmentation') #upload text from csv
 dataset.upload_from_csv(csv_path='csv_path', input_type='text', csv_type='raw',
 labels=True) #upload data from folder dataset.upload_from_folder
 (folder_path='folder_path', input_type='text', labels=True) # Export Dataset
 from clarifai.client.dataset import Dataset # Note: clarifai-data-protobuf.zip
 is acquired through exporting datasets within the Clarifai Platform. Dataset
 ().export(save_path='output.zip', local_archive_path='clarifai-data-
-protobuf.zip') ``` ### Interacting with Inputs ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.user import User app = User
-(user_id="user_id").app(app_id="app_id") input_obj = app.inputs() #input upload
-from url input_obj.upload_from_url(input_id = 'demo', image_url='https://
-samples.clarifai.com/metro-north.jpg') #input upload from filename
-input_obj.upload_from_file(input_id = 'demo', video_file='demo.mp4') #listing
-inputs input_obj.list_inputs() # text upload input_obj.upload_text(input_id =
-'demo', raw_text = 'This is a test') ``` ### Interacting with Models #### Model
-Predict ```python # Note: CLARIFAI_PAT must be set as env variable. from
-clarifai.client.model import Model # Model Predict model_prediction = Model
-("https://clarifai.com/anthropic/completion/models/claude-v2").predict_by_bytes
-(b"Write a tweet on future of AI", "text") model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id") model_prediction = model.predict_by_url
-(url="url", input_type="image") # Supports image, text, audio, video #
-Customizing Model Inference Output model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id", output_config={"min_value": 0.98}) #
-Return predictions having prediction confidence > 0.98 model_prediction =
-model.predict_by_filepath(filepath="local_filepath", input_type="text") #
-Supports image, text, audio, video model = Model(user_id="user_id",
-app_id="app_id", model_id="model_id", output_config={"sample_ms": 2000}) #
-Return predictions for specified interval model_prediction =
-model.predict_by_url(url="VIDEO_URL", input_type="video") ``` #### Models
-Listing ```python # Note: CLARIFAI_PAT must be set as env variable. # List all
-model versions all_model_versions = model.list_versions() # Go to specific
-model version model_v1 = client.app("app_id").model(model_id="model_id",
-model_version_id="model_version_id") # List all models in an app all_models =
-app.list_models() # List all models in community filtered by model_type,
-description all_llm_community_models = App().list_models(filter_by={"query":
-"LLM", "model_type_id": "text-to-text"}, only_in_app=False) ``` ### Interacting
-with Workflows #### Workflow Predict ```python # Note: CLARIFAI_PAT must be set
-as env variable. from clarifai.client.workflow import Workflow # Workflow
-Predict workflow = Workflow("workflow_url") # Example: https://clarifai.com/
-clarifai/main/workflows/Face-Sentiment workflow_prediction =
-workflow.predict_by_url(url="url", input_type="image") # Supports image, text,
-audio, video # Customizing Workflow Inference Output workflow = Workflow
-(user_id="user_id", app_id="app_id", workflow_id="workflow_id", output_config=
+protobuf.zip') ``` ### Interacting with Inputs #### Input upload ```python #
+Note: CLARIFAI_PAT must be set as env variable. from clarifai.client.user
+import User app = User(user_id="user_id").app(app_id="app_id") input_obj =
+app.inputs() #input upload from url input_obj.upload_from_url(input_id =
+'demo', image_url='https://samples.clarifai.com/metro-north.jpg') #input upload
+from filename input_obj.upload_from_file(input_id = 'demo',
+video_file='demo.mp4') # text upload input_obj.upload_text(input_id = 'demo',
+raw_text = 'This is a test') ``` #### Input listing ```python #listing inputs
+input_generator = input_obj.list_inputs
+(page_no=1,per_page=10,input_type='image') inputs_list = list(input_generator)
+#listing annotations annotation_generator = input_obj.list_annotations
+(batch_input=inputs_list) annotations_list = list(annotation_generator)
+#listing concepts all_concepts = list(app.list_concepts()) ``` ### Interacting
+with Models #### Model Predict ```python # Note: CLARIFAI_PAT must be set as
+env variable. from clarifai.client.model import Model # Model Predict
+model_prediction = Model("https://clarifai.com/anthropic/completion/models/
+claude-v2").predict_by_bytes(b"Write a tweet on future of AI", "text") model =
+Model(user_id="user_id", app_id="app_id", model_id="model_id") model_prediction
+= model.predict_by_url(url="url", input_type="image") # Supports image, text,
+audio, video # Customizing Model Inference Output model = Model
+(user_id="user_id", app_id="app_id", model_id="model_id", output_config=
 {"min_value": 0.98}) # Return predictions having prediction confidence > 0.98
-workflow_prediction = workflow.predict_by_filepath(filepath="local_filepath",
-input_type="text") # Supports image, text, audio, video ``` #### Workflows
-Listing ```python # Note: CLARIFAI_PAT must be set as env variable. # List all
-workflow versions all_workflow_versions = workflow.list_versions() # Go to
-specific workflow version workflow_v1 = Workflow(workflow_id="workflow_id",
+model_prediction = model.predict_by_filepath(filepath="local_filepath",
+input_type="text") # Supports image, text, audio, video model = Model
+(user_id="user_id", app_id="app_id", model_id="model_id", output_config=
+{"sample_ms": 2000}) # Return predictions for specified interval
+model_prediction = model.predict_by_url(url="VIDEO_URL", input_type="video")
+``` #### Models Listing ```python # Note: CLARIFAI_PAT must be set as env
+variable. # List all model versions all_model_versions = list
+(model.list_versions()) # Go to specific model version model_v1 = client.app
+("app_id").model(model_id="model_id", model_version_id="model_version_id") #
+List all models in an app all_models = list(app.list_models()) # List all
+models in community filtered by model_type, description
+all_llm_community_models = App().list_models(filter_by={"query": "LLM",
+"model_type_id": "text-to-text"}, only_in_app=False) all_llm_community_models =
+list(all_llm_community_models) ``` ### Interacting with Workflows #### Workflow
+Predict ```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.workflow import Workflow # Workflow Predict workflow = Workflow
+("workflow_url") # Example: https://clarifai.com/clarifai/main/workflows/Face-
+Sentiment workflow_prediction = workflow.predict_by_url(url="url",
+input_type="image") # Supports image, text, audio, video # Customizing Workflow
+Inference Output workflow = Workflow(user_id="user_id", app_id="app_id",
+workflow_id="workflow_id", output_config={"min_value": 0.98}) # Return
+predictions having prediction confidence > 0.98 workflow_prediction =
+workflow.predict_by_filepath(filepath="local_filepath", input_type="text") #
+Supports image, text, audio, video ``` #### Workflows Listing ```python # Note:
+CLARIFAI_PAT must be set as env variable. # List all workflow versions
+all_workflow_versions = list(workflow.list_versions()) # Go to specific
+workflow version workflow_v1 = Workflow(workflow_id="workflow_id",
 workflow_version=dict(id="workflow_version_id"), app_id="app_id",
-user_id="user_id") # List all workflow in an app all_workflow =
-app.list_workflow() # List all workflow in community filtered by description
+user_id="user_id") # List all workflow in an app all_workflow = list
+(app.list_workflow()) # List all workflow in community filtered by description
 all_face_community_workflows = App().list_workflows(filter_by={"query":
-"face"}, only_in_app=False) # Get all face related workflows ``` #### Workflow
-Create Create a new workflow specified by a yaml config file. ```python # Note:
-CLARIFAI_PAT must be set as env variable. from clarifai.client.app import App
-app = App(app_id="app_id", user_id="user_id") workflow = app.create_workflow
-(config_filepath="config.yml") ``` #### Workflow Export Export an existing
-workflow from Clarifai as a local yaml file. ```python # Note: CLARIFAI_PAT
-must be set as env variable. from clarifai.client.workflow import Workflow
-workflow = Workflow("https://clarifai.com/clarifai/main/workflows/
-Demographics") workflow.export('demographics_workflow.yml') ``` ## More
-Examples See many more code examples in this [repo](https://github.com/
-Clarifai/examples). Also see the official [Python SDK docs](https://clarifai-
-python.readthedocs.io/en/latest/index.html)
+"face"}, only_in_app=False) # Get all face related workflows
+all_face_community_workflows = list(all_face_community_workflows) ``` ####
+Workflow Create Create a new workflow specified by a yaml config file.
+```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.app import App app = App(app_id="app_id", user_id="user_id")
+workflow = app.create_workflow(config_filepath="config.yml") ``` #### Workflow
+Export Export an existing workflow from Clarifai as a local yaml file.
+```python # Note: CLARIFAI_PAT must be set as env variable. from
+clarifai.client.workflow import Workflow workflow = Workflow("https://
+clarifai.com/clarifai/main/workflows/Demographics") workflow.export
+('demographics_workflow.yml') ``` ## More Examples See many more code examples
+in this [repo](https://github.com/Clarifai/examples). Also see the official
+[Python SDK docs](https://clarifai-python.readthedocs.io/en/latest/index.html)
```

### Comparing `clarifai-9.9.2/clarifai.egg-info/SOURCES.txt` & `clarifai-9.9.3/clarifai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/auth/helper.py` & `clarifai-9.9.3/clarifai_utils/auth/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,24 +224,14 @@
         user_id: CLARIFAI_USER_ID env var.
         app_id: CLARIFAI_APP_ID env var.
         one of:
           token: CLARIFAI_SESSION_TOKEN env var.
           pat: CLARIFAI_PAT env var.
         base: CLARIFAI_API_BASE env var.
     """
-    error_description = """
-Please check the following required vars are in your env:
- - 'CLARIFAI_USER_ID': the user ID accessing the module.
- - 'CLARIFAI_APP_ID': the app the module is being accessed from.
- - 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT': to authenticate the calling user with a session token or personal access token.
-
-Additionally, these optional params are supported:
- - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
- - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
-"""
     user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
     token = os.environ.get("CLARIFAI_SESSION_TOKEN", "")
     pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
     return cls(user_id, app_id, pat, token, base, ui, validate)
```

### Comparing `clarifai-9.9.2/clarifai_utils/auth/register.py` & `clarifai-9.9.3/clarifai_utils/auth/register.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/auth/stub.py` & `clarifai-9.9.3/clarifai_utils/auth/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/client/__init__.py` & `clarifai-9.9.3/clarifai_utils/client/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/client/app.py` & `clarifai-9.9.3/clarifai_utils/client/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import uuid
-from typing import Any, Dict, List
+from typing import Any, Dict, Generator
 
 import yaml
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
+from clarifai_grpc.grpc.api.resources_pb2 import Concept
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from google.protobuf.json_format import MessageToDict
 
 from clarifai.client.base import BaseClient
 from clarifai.client.dataset import Dataset
 from clarifai.client.input import Inputs
 from clarifai.client.lister import Lister
@@ -47,159 +48,229 @@
       kwargs = {'user_id': user_id}
     self.kwargs = {**kwargs, 'id': app_id}
     self.app_info = resources_pb2.App(**self.kwargs)
     self.logger = get_logger(logger_level="INFO", name=__name__)
     BaseClient.__init__(self, user_id=self.user_id, app_id=self.id, base=base_url)
     Lister.__init__(self)
 
-  def list_datasets(self) -> List[Dataset]:
+  def list_datasets(self, page_no: int = None,
+                    per_page: int = None) -> Generator[Dataset, None, None]:
     """Lists all the datasets for the app.
 
-    Returns:
-        List[Dataset]: A list of Dataset objects for the datasets in the app.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Dataset: Dataset objects for the datasets in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_datasets = app.list_datasets()
+        >>> all_datasets = list(app.list_datasets())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(
-        user_app_id=self.user_app_id,
-        per_page=self.default_page_size,
-    )
-    all_datasets_info = list(
-        self.list_all_pages_generator(self.STUB.ListDatasets, service_pb2.ListDatasetsRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id,)
+    all_datasets_info = self.list_pages_generator(
+        self.STUB.ListDatasets,
+        service_pb2.ListDatasetsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
     for dataset_info in all_datasets_info:
       if 'version' in list(dataset_info.keys()):
         del dataset_info['version']['metrics']
+      yield Dataset(**dataset_info)
 
-    return [Dataset(**dataset_info) for dataset_info in all_datasets_info]
-
-  def list_models(self, filter_by: Dict[str, Any] = {}, only_in_app: bool = True) -> List[Model]:
+  def list_models(self,
+                  filter_by: Dict[str, Any] = {},
+                  only_in_app: bool = True,
+                  page_no: int = None,
+                  per_page: int = None) -> Generator[Model, None, None]:
     """Lists all the available models for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of models.
         only_in_app (bool): If True, only return models that are in the app.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Model]: A list of Model objects for the models in the app.
+    Yields:
+        Model: Model objects for the models in the app.
 
     Example:
         >>> from clarifai.client.user import User
         >>> app = User(user_id="user_id").app(app_id="app_id")
-        >>> all_models = app.list_models()
-    """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_models_info = list(
-        self.list_all_pages_generator(self.STUB.ListModels, service_pb2.ListModelsRequest,
-                                      request_data))
+        >>> all_models = list(app.list_models())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_models_info = self.list_pages_generator(
+        self.STUB.ListModels,
+        service_pb2.ListModelsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    filtered_models_info = []
     for model_info in all_models_info:
       if 'model_version' not in list(model_info.keys()):
         continue
       if only_in_app:
         if model_info['app_id'] != self.id:
           continue
-      filtered_models_info.append(model_info)
-
-    return [Model(**model_info) for model_info in filtered_models_info]
+      yield Model(**model_info)
 
-  def list_workflows(self, filter_by: Dict[str, Any] = {},
-                     only_in_app: bool = True) -> List[Workflow]:
+  def list_workflows(self,
+                     filter_by: Dict[str, Any] = {},
+                     only_in_app: bool = True,
+                     page_no: int = None,
+                     per_page: int = None) -> Generator[Workflow, None, None]:
     """Lists all the available workflows for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of workflows.
         only_in_app (bool): If True, only return workflows that are in the app.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Workflow]: A list of Workflow objects for the workflows in the app.
+    Yields:
+        Workflow: Workflow objects for the workflows in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_workflows = app.list_workflows()
+        >>> all_workflows = list(app.list_workflows())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_workflows_info = list(
-        self.list_all_pages_generator(self.STUB.ListWorkflows, service_pb2.ListWorkflowsRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_workflows_info = self.list_pages_generator(
+        self.STUB.ListWorkflows,
+        service_pb2.ListWorkflowsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    filtered_workflows_info = []
     for workflow_info in all_workflows_info:
       if only_in_app:
         if workflow_info['app_id'] != self.id:
           continue
-      filtered_workflows_info.append(workflow_info)
-
-    return [Workflow(**workflow_info) for workflow_info in all_workflows_info]
+      yield Workflow(**workflow_info)
 
-  def list_modules(self, filter_by: Dict[str, Any] = {}, only_in_app: bool = True) -> List[Module]:
+  def list_modules(self,
+                   filter_by: Dict[str, Any] = {},
+                   only_in_app: bool = True,
+                   page_no: int = None,
+                   per_page: int = None) -> Generator[Module, None, None]:
     """Lists all the available modules for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of modules.
         only_in_app (bool): If True, only return modules that are in the app.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Module]: A list of Module objects for the modules in the app.
+    Yields:
+        Module: Module objects for the modules in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_modules = app.list_modules()
+        >>> all_modules = list(app.list_modules())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_modules_info = list(
-        self.list_all_pages_generator(self.STUB.ListModules, service_pb2.ListModulesRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_modules_info = self.list_pages_generator(
+        self.STUB.ListModules,
+        service_pb2.ListModulesRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    filtered_modules_info = []
     for module_info in all_modules_info:
       if only_in_app:
         if module_info['app_id'] != self.id:
           continue
-      filtered_modules_info.append(module_info)
+      yield Module(**module_info)
 
-    return [Module(**module_info) for module_info in filtered_modules_info]
-
-  def list_installed_module_versions(self, filter_by: Dict[str, Any] = {}) -> List[Module]:
+  def list_installed_module_versions(self,
+                                     filter_by: Dict[str, Any] = {},
+                                     page_no: int = None,
+                                     per_page: int = None) -> Generator[Module, None, None]:
     """Lists all installed module versions in the app.
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of installed module versions.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Module]: A list of Module objects for the installed module versions in the app.
+    Yields:
+        Module: Module objects for the installed module versions in the app.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
-        >>> all_installed_module_versions = app.list_installed_module_versions()
+        >>> all_installed_module_versions = list(app.list_installed_module_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_imv_infos = list(
-        self.list_all_pages_generator(self.STUB.ListInstalledModuleVersions,
-                                      service_pb2.ListInstalledModuleVersionsRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_imv_infos = self.list_pages_generator(
+        self.STUB.ListInstalledModuleVersions,
+        service_pb2.ListInstalledModuleVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
     for imv_info in all_imv_infos:
       del imv_info['deploy_url']
       del imv_info['installed_module_version_id']  # TODO: remove this after the backend fix
+      yield Module(module_id=imv_info['module_version']['module_id'], **imv_info)
+
+  def list_concepts(self, page_no: int = None,
+                    per_page: int = None) -> Generator[Concept, None, None]:
+    """Lists all the concepts for the app.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    return [
-        Module(module_id=imv_info['module_version']['module_id'], **imv_info)
-        for imv_info in all_imv_infos
-    ]
-
-  def list_concepts(self):
-    """Lists all the concepts for the app."""
-    pass  # TODO
+    Yields:
+        Concept: Concepts in the app.
+
+    Example:
+        >>> from clarifai.client.app import App
+        >>> app = App(app_id="app_id", user_id="user_id")
+        >>> all_concepts = list(app.list_concepts())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(user_app_id=self.user_app_id)
+    all_concepts_infos = self.list_pages_generator(
+        self.STUB.ListConcepts,
+        service_pb2.ListConceptsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
+    for concept_info in all_concepts_infos:
+      concept_info['id'] = concept_info.pop('concept_id')
+      yield Concept(**concept_info)
 
   def create_dataset(self, dataset_id: str, **kwargs) -> Dataset:
     """Creates a dataset for the app.
 
     Args:
         dataset_id (str): The dataset ID for the dataset to create.
         **kwargs: Additional keyword arguments to be passed to the Dataset.
@@ -566,15 +637,17 @@
         Search: A Search object for the user and app ID.
 
     Example:
         >>> from clarifai.client.app import App
         >>> app = App(app_id="app_id", user_id="user_id")
         >>> search_client = app.search(top_k=12, metric="euclidean")
     """
-    return Search(**kwargs)
+    user_id = kwargs.get("user_id", self.user_app_id.user_id)
+    app_id = kwargs.get("app_id", self.user_app_id.app_id)
+    return Search(user_id=user_id, app_id=app_id, **kwargs)
 
   def __getattr__(self, name):
     return getattr(self.app_info, name)
 
   def __str__(self):
     init_params = [param for param in self.kwargs.keys()]
     attribute_strings = [
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/auth/helper.py` & `clarifai-9.9.3/clarifai_utils/client/auth/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,24 +224,14 @@
         user_id: CLARIFAI_USER_ID env var.
         app_id: CLARIFAI_APP_ID env var.
         one of:
           token: CLARIFAI_SESSION_TOKEN env var.
           pat: CLARIFAI_PAT env var.
         base: CLARIFAI_API_BASE env var.
     """
-    error_description = """
-Please check the following required vars are in your env:
- - 'CLARIFAI_USER_ID': the user ID accessing the module.
- - 'CLARIFAI_APP_ID': the app the module is being accessed from.
- - 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT': to authenticate the calling user with a session token or personal access token.
-
-Additionally, these optional params are supported:
- - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
- - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
-"""
     user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
     token = os.environ.get("CLARIFAI_SESSION_TOKEN", "")
     pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
     return cls(user_id, app_id, pat, token, base, ui, validate)
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/auth/register.py` & `clarifai-9.9.3/clarifai_utils/client/auth/register.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/client/auth/stub.py` & `clarifai-9.9.3/clarifai_utils/client/auth/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/client/base.py` & `clarifai-9.9.3/clarifai_utils/client/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/client/dataset.py` & `clarifai-9.9.3/clarifai_utils/client/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,19 @@
         chunk_size (int): chunk size for concurrent upload of inputs and annotations
 
     Example:
         >>> from clarifai.client.dataset import Dataset
         >>> dataset = Dataset(user_id = 'user_id', app_id = 'demo_app', dataset_id = 'demo_dataset')
         >>> dataset.upload_from_csv(csv_path='csv_path', input_type='text', csv_type='raw, labels=True)
 
-    Note: csv file should have either one(input) or two columns(input, labels).
+    Note:
+        CSV file supports 'inputid', 'input', 'concepts', 'metadata', 'geopoints' columns.
+        All the data in the CSV should be in double quotes.
+        metadata should be in single quotes format. Example: "{'key': 'value'}"
+        geopoints should be in "long,lat" format.
     """
     if input_type not in ['image', 'text', 'video', 'audio']:
       raise UserError('Invalid input type, it should be image,text,audio or video')
     if csv_type not in ['raw', 'url', 'file_path']:
       raise UserError('Invalid csv type, it should be raw, url or file_path')
     assert csv_path.endswith('.csv'), 'csv_path should be a csv file'
     if csv_type == 'raw' and input_type != 'text':
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/input.py` & `clarifai-9.9.3/clarifai_utils/client/input.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import csv
+import json
 import os
 import time
 import uuid
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from multiprocessing import cpu_count
-from typing import List, Union
+from typing import Generator, List, Union
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2  # noqa: F401
 from clarifai_grpc.grpc.api.resources_pb2 import Annotation, Audio, Image, Input, Text, Video
 from clarifai_grpc.grpc.api.status import status_code_pb2, status_pb2
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.struct_pb2 import Struct
 from tqdm import tqdm
@@ -304,53 +305,92 @@
     Example:
         >>> from clarifai.client.input import Inputs
         >>> input_obj = Inputs()
         >>> input_protos = input_obj.get_inputs_from_csv(csv_path='filepath', input_type='text', csv_type='raw')
     """
     input_protos = []
     with open(csv_path) as _file:
-      reader = csv.reader(_file)
-      next(reader, None)  # skip header
+      reader = csv.DictReader(_file, delimiter=',', quotechar='"')
+      columns = reader.fieldnames
+      for column in columns:
+        if column not in ['inputid', 'input', 'concepts', 'metadata', 'geopoints']:
+          raise UserError(
+              "CSV file may have 'inputid', 'input', 'concepts', 'metadata', 'geopoints' columns. Does not support '{}' column".
+              format(column))
       for id, input in enumerate(reader):
         if labels:
-          assert len(input) == 2, "csv file should have two columns(input, labels)"
-          labels = input[1] if isinstance(input[1], list) else [input[1]]
+          labels_list = input['concepts'].split(',')
+          labels = labels_list if len(input['concepts']) > 0 else None
         else:
           labels = None
 
-        input_id = uuid.uuid4().hex
-        text = input[0] if input_type == 'text' else None
-        image = input[0] if input_type == 'image' else None
-        video = input[0] if input_type == 'video' else None
-        audio = input[0] if input_type == 'audio' else None
+        if 'metadata' in columns:
+          if len(input['metadata']) > 0:
+            metadata_str = input['metadata'].replace("'", '"')
+            try:
+              metadata_dict = json.loads(metadata_str)
+            except json.decoder.JSONDecodeError:
+              raise UserError("metadata column in CSV file should be a valid json")
+            metadata = Struct()
+            metadata.update(metadata_dict)
+          else:
+            metadata = None
+        else:
+          metadata = None
+
+        if 'geopoints' in columns:
+          if len(input['geopoints']) > 0:
+            geo_points = input['geopoints'].split(',')
+            geo_points = [float(geo_point) for geo_point in geo_points]
+            geo_info = geo_points if len(geo_points) == 2 else UserError(
+                "geopoints column in CSV file should have longitude,latitude")
+          else:
+            geo_info = None
+        else:
+          geo_info = None
+
+        input_id = input['inputid'] if 'inputid' in columns else uuid.uuid4().hex
+        text = input['input'] if input_type == 'text' else None
+        image = input['input'] if input_type == 'image' else None
+        video = input['input'] if input_type == 'video' else None
+        audio = input['input'] if input_type == 'audio' else None
 
         if csv_type == 'raw':
           input_protos.append(
               self.get_text_input(
-                  input_id=input_id, raw_text=text, dataset_id=dataset_id, labels=labels))
+                  input_id=input_id,
+                  raw_text=text,
+                  dataset_id=dataset_id,
+                  labels=labels,
+                  metadata=metadata,
+                  geo_info=geo_info))
         elif csv_type == 'url':
           input_protos.append(
               self.get_input_from_url(
                   input_id=input_id,
                   image_url=image,
                   text_url=text,
                   audio_url=audio,
                   video_url=video,
                   dataset_id=dataset_id,
-                  labels=labels))
+                  labels=labels,
+                  metadata=metadata,
+                  geo_info=geo_info))
         else:
           input_protos.append(
               self.get_input_from_file(
                   input_id=input_id,
                   image_file=image,
                   text_file=text,
                   audio_file=audio,
                   video_file=video,
                   dataset_id=dataset_id,
-                  labels=labels))
+                  labels=labels,
+                  metadata=metadata,
+                  geo_info=geo_info))
 
     return input_protos
 
   def get_text_inputs_from_folder(self,
                                   folder_path: str,
                                   dataset_id: str = None,
                                   labels: bool = False) -> List[Text]:  #text specific
@@ -611,15 +651,15 @@
     request = service_pb2.PostAnnotationsRequest(
         user_app_id=self.user_app_id, annotations=batch_annot)
     response = self._grpc_request(self.STUB.PostAnnotations, request)
     if response.status.code != status_code_pb2.SUCCESS:
       try:
         self.logger.warning(
             f"Post annotations failed, status: {response.annotations[0].status.details}")
-      except:
+      except Exception:
         self.logger.warning(f"Post annotations failed, status: {response.status.details}")
       finally:
         retry_upload.extend(batch_annot)
     else:
       if show_log:
         self.logger.info("\nAnnotations Uploaded\n%s", response.status)
     return retry_upload
@@ -644,43 +684,113 @@
 
     Args:
         input_ids (Input): List of input objects to delete.
 
     Example:
         >>> from clarifai.client.user import User
         >>> input_obj = User(user_id="user_id").app(app_id="app_id").inputs()
-        >>> input_obj.delete_inputs(input_obj.list_inputs())
+        >>> input_obj.delete_inputs(list(input_obj.list_inputs()))
     """
     if not isinstance(inputs, list):
       raise UserError("input_ids must be a list of input ids")
     inputs_ids = [input.id for input in inputs]
     request = service_pb2.DeleteInputsRequest(user_app_id=self.user_app_id, ids=inputs_ids)
     response = self._grpc_request(self.STUB.DeleteInputs, request)
     if response.status.code != status_code_pb2.SUCCESS:
       raise Exception(response.status)
     self.logger.info("\nInputs Deleted\n%s", response.status)
 
-  def list_inputs(self) -> List[Input]:  # TODO: update lister
+  def list_inputs(self,
+                  dataset_id: str = None,
+                  page_no: int = None,
+                  per_page: int = None,
+                  input_type: str = None) -> Generator[Input, None, None]:
     """Lists all the inputs for the app.
 
-    Returns:
-        list of Input: A list of Input objects for the app.
+    Args:
+        dataset_id (str): The dataset ID for the dataset to list inputs from.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+        input_type (str): The type of input to list. Options: 'image', 'video', 'audio', 'text'.
+
+    Yields:
+        Input: Input objects for the app.
 
     Example:
         >>> from clarifai.client.user import User
         >>> input_obj = User(user_id="user_id").app(app_id="app_id").inputs()
-        >>> input_obj.list_inputs()
+        >>> all_inputs = list(input_obj.list_inputs(input_type='image'))
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size)
-    all_inputs_info = list(
-        self.list_all_pages_generator(self.STUB.ListInputs, service_pb2.ListInputsRequest,
-                                      request_data))
+    if input_type not in ['image', 'text', 'video', 'audio', None]:
+      raise UserError('Invalid input type, it should be image,text,audio or video')
+    if dataset_id:
+      request_data = dict(user_app_id=self.user_app_id, dataset_id=dataset_id)
+      all_inputs_info = self.list_pages_generator(
+          self.STUB.ListDatasetInputs,
+          service_pb2.ListDatasetInputsRequest,
+          request_data,
+          per_page=per_page,
+          page_no=page_no)
+    else:
+      request_data = dict(user_app_id=self.user_app_id)
+      all_inputs_info = self.list_pages_generator(
+          self.STUB.ListInputs,
+          service_pb2.ListInputsRequest,
+          request_data,
+          per_page=per_page,
+          page_no=page_no)
     for input_info in all_inputs_info:
-      input_info['id'] = input_info.pop('input_id')
-    return [resources_pb2.Input(**input_info) for input_info in all_inputs_info]
+      input_info['id'] = input_info.pop('dataset_input_id') if dataset_id else input_info.pop(
+          'input_id')
+      if input_type:
+        if input_type not in input_info['data'].keys():
+          continue
+      yield resources_pb2.Input(**input_info)
+
+  def list_annotations(self,
+                       batch_input: List[Input] = None,
+                       page_no: int = None,
+                       per_page: int = None) -> Generator[Annotation, None, None]:
+    """Lists all the annotations for the app.
+
+    Args:
+        batch_input (List[Input]): The input objects to list annotations from.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Annotation: Annotation objects for the app.
+
+    Example:
+        >>> from clarifai.client.user import User
+        >>> input_obj = User(user_id="user_id").app(app_id="app_id").inputs()
+        >>> all_inputs = list(input_obj.list_inputs(input_type='image'))
+        >>> all_annotations = list(input_obj.list_annotations(batch_input=all_inputs))
+
+    Note:
+        If batch_input is not given, then lists all the annotations for the app.
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(
+        user_app_id=self.user_app_id,
+        input_ids=[input.id for input in batch_input] if batch_input else None)
+    all_annotations_info = self.list_pages_generator(
+        self.STUB.ListAnnotations,
+        service_pb2.ListAnnotationsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
+    for annotations_info in all_annotations_info:
+      annotations_info['id'] = annotations_info.pop('annotation_id')
+      yield Annotation(**annotations_info)
 
   def _bulk_upload(self, inputs: List[Input], chunk_size: int = 128) -> None:
     """Uploads process for large number of inputs.
 
     Args:
         inputs (List[Input]): input protos
         chunk_size (int): chunk size for each request
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/lister.py` & `clarifai-9.9.3/clarifai_utils/client/lister.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,47 @@
 
 class Lister(BaseClient):
   """Lister class for obtaining paginated results from the Clarifai API."""
 
   def __init__(self, page_size: int = 16):
     self.default_page_size = page_size
 
-  def list_all_pages_generator(
-      self, endpoint: Callable, proto_message: Any,
-      request_data: Dict[str, Any]) -> Generator[Dict[str, Any], None, None]:
-    """Lists all pages of a resource.
+  def list_pages_generator(self,
+                           endpoint: Callable,
+                           proto_message: Any,
+                           request_data: Dict[str, Any],
+                           page_no: int = None,
+                           per_page: int = None) -> Generator[Dict[str, Any], None, None]:
+    """Lists pages of a resource.
 
     Args:
         endpoint (Callable): The endpoint to call.
         proto_message (Any): The proto message to use.
         request_data (dict): The request data to use.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
     Yields:
         response_dict: The next item in the listing.
     """
-    page = 1
+    page = 1 if not page_no else page_no
+    if page_no and not per_page:
+      per_page = self.default_page_size
     while True:
       request_data['page'] = page
+      request_data['per_page'] = per_page
       response = self._grpc_request(endpoint, proto_message(**request_data))
       dict_response = MessageToDict(response, preserving_proto_field_name=True)
       if response.status.code != status_code_pb2.SUCCESS:
         raise Exception(f"Listing failed with response {response!r}")
       if len(list(dict_response.keys())) == 1:
         break
       else:
         listing_resource = list(dict_response.keys())[1]
         for item in dict_response[listing_resource]:
-          yield self.process_response_keys(item, listing_resource[:-1])
+          if listing_resource == "dataset_inputs":
+            yield self.process_response_keys(item["input"], listing_resource[:-1])
+          else:
+            yield self.process_response_keys(item, listing_resource[:-1])
+      if page_no is not None or per_page is not None:
+        break
       page += 1
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/model.py` & `clarifai-9.9.3/clarifai_utils/client/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-from typing import Dict, List
+from typing import Dict, Generator, List
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from clarifai_grpc.grpc.api.resources_pb2 import Input
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from google.protobuf.json_format import MessageToDict
 
 from clarifai.client.base import BaseClient
@@ -86,44 +86,51 @@
 
     kwargs.update({'app_id': self.app_id, 'user_id': self.user_id})
     dict_response = MessageToDict(response, preserving_proto_field_name=True)
     kwargs = self.process_response_keys(dict_response['model'], 'model')
 
     return Model(**kwargs)
 
-  def list_versions(self) -> List['Model']:
+  def list_versions(self, page_no: int = None,
+                    per_page: int = None) -> Generator['Model', None, None]:
     """Lists all the versions for the model.
 
-    Returns:
-        List[Model]: A list of Model objects for the versions of the model.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Model: Model objects for the versions of the model.
 
     Example:
         >>> from clarifai.client.model import Model
         >>> model = Model("model_url") # Example URL: https://clarifai.com/clarifai/main/models/general-image-recognition
                     or
         >>> model = Model(model_id='model_id', user_id='user_id', app_id='app_id')
-        >>> all_model_versions = model.list_versions()
+        >>> all_model_versions = list(model.list_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
     request_data = dict(
         user_app_id=self.user_app_id,
         model_id=self.id,
-        per_page=self.default_page_size,
     )
-    all_model_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListModelVersions,
-                                      service_pb2.ListModelVersionsRequest, request_data))
+    all_model_versions_info = self.list_pages_generator(
+        self.STUB.ListModelVersions,
+        service_pb2.ListModelVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
     for model_version_info in all_model_versions_info:
       model_version_info['id'] = model_version_info['model_version_id']
       del model_version_info['model_version_id']
-
-    return [
-        Model(model_id=self.id, **dict(self.kwargs, model_version=model_version_info))
-        for model_version_info in all_model_versions_info
-    ]
+      yield Model(model_id=self.id, **dict(self.kwargs, model_version=model_version_info))
 
   def predict(self, inputs: List[Input]):
     """Predicts the model based on the given inputs.
 
     Args:
         inputs (list[Input]): The inputs to predict, must be less than 128.
     """
@@ -240,45 +247,14 @@
           data=resources_pb2.Data(video=resources_pb2.Video(url=url)))
     elif input_type == "audio":
       input_proto = resources_pb2.Input(
           data=resources_pb2.Data(audio=resources_pb2.Audio(url=url)))
 
     return self.predict(inputs=[input_proto])
 
-  def list_versions(self) -> List['Model']:
-    """Lists all the versions for the model.
-
-    Returns:
-        List[Model]: A list of Model objects for the versions of the model.
-
-    Example:
-        >>> from clarifai.client.model import Model
-        >>> model = Model("model_url") # Example URL: https://clarifai.com/clarifai/main/models/general-image-recognition
-                    or
-        >>> model = Model(model_id='model_id', user_id='user_id', app_id='app_id')
-        >>> all_model_versions = model.list_versions()
-    """
-    request_data = dict(
-        user_app_id=self.user_app_id,
-        model_id=self.id,
-        per_page=self.default_page_size,
-    )
-    all_model_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListModelVersions,
-                                      service_pb2.ListModelVersionsRequest, request_data))
-
-    for model_version_info in all_model_versions_info:
-      model_version_info['id'] = model_version_info['model_version_id']
-      del model_version_info['model_version_id']
-
-    return [
-        Model(model_id=self.id, **dict(self.kwargs, model_version=model_version_info))
-        for model_version_info in all_model_versions_info
-    ]
-
   def __getattr__(self, name):
     return getattr(self.model_info, name)
 
   def __str__(self):
     init_params = [param for param in self.kwargs.keys()]
     attribute_strings = [
         f"{param}={getattr(self.model_info, param)}" for param in init_params
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/module.py` & `clarifai-9.9.3/clarifai_utils/client/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List
+from typing import Dict, Generator
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 
 from clarifai.client.base import BaseClient
 from clarifai.client.lister import Lister
 from clarifai.errors import UserError
 from clarifai.urls.helper import ClarifaiUrlHelper
@@ -39,42 +39,49 @@
 
     self.kwargs = {**kwargs, 'id': module_id, 'module_version': module_version}
     self.module_info = resources_pb2.Module(**self.kwargs)
     self.logger = get_logger(logger_level="INFO")
     BaseClient.__init__(self, user_id=self.user_id, app_id=self.app_id, base=base_url)
     Lister.__init__(self)
 
-  def list_versions(self) -> List['Module']:
+  def list_versions(self, page_no: int = None,
+                    per_page: int = None) -> Generator['Module', None, None]:
     """Lists all the module versions for the module.
 
-        Returns:
-            List[Moudle]: A list of Module objects for versions of the module.
-
-        Example:
-            >>> from clarifai.client.module import Module
-            >>> module = Module(module_id='module_id', user_id='user_id', app_id='app_id')
-            >>> all_Module_versions = module.list_versions()
-        """
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Moudle: Module objects for versions of the module.
+
+    Example:
+        >>> from clarifai.client.module import Module
+        >>> module = Module(module_id='module_id', user_id='user_id', app_id='app_id')
+        >>> all_Module_versions = list(module.list_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
     request_data = dict(
         user_app_id=self.user_app_id,
         module_id=self.id,
-        per_page=self.default_page_size,
     )
-    all_module_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListModuleVersions,
-                                      service_pb2.ListModuleVersionsRequest, request_data))
+    all_module_versions_info = self.list_pages_generator(
+        self.STUB.ListModuleVersions,
+        service_pb2.ListModuleVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
     for module_version_info in all_module_versions_info:
       module_version_info['id'] = module_version_info['module_version_id']
       del module_version_info['module_version_id']
-
-    return [
-        Module(module_id=self.id, **dict(self.kwargs, module_version=module_version_info))
-        for module_version_info in all_module_versions_info
-    ]
+      yield Module(module_id=self.id, **dict(self.kwargs, module_version=module_version_info))
 
   def __getattr__(self, name):
     return getattr(self.module_info, name)
 
   def __str__(self):
     init_params = [param for param in self.kwargs.keys()]
     attribute_strings = [
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/runner.py` & `clarifai-9.9.3/clarifai_utils/client/runner.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/client/search.py` & `clarifai-9.9.3/clarifai_utils/client/search.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/client/user.py` & `clarifai-9.9.3/clarifai_utils/client/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List
+from typing import Any, Dict, Generator, List
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from google.protobuf.json_format import MessageToDict
 
 from clarifai.client.app import App
 from clarifai.client.base import BaseClient
@@ -25,54 +25,75 @@
     """
     self.kwargs = {**kwargs, 'id': user_id}
     self.user_info = resources_pb2.User(**self.kwargs)
     self.logger = get_logger(logger_level="INFO", name=__name__)
     BaseClient.__init__(self, user_id=self.id, app_id="", base=base_url)
     Lister.__init__(self)
 
-  def list_apps(self, filter_by: Dict[str, Any] = {}) -> List[App]:
+  def list_apps(self, filter_by: Dict[str, Any] = {}, page_no: int = None,
+                per_page: int = None) -> Generator[App, None, None]:
     """Lists all the apps for the user.
 
     Args:
         filter_by (dict): A dictionary of filters to be applied to the list of apps.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        list of App: A list of App objects for the user.
+    Yields:
+        App: App objects for the user.
 
     Example:
         >>> from clarifai.client.user import User
-        >>> apps = User("user_id").list_apps()
-    """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_apps_info = list(
-        self.list_all_pages_generator(self.STUB.ListApps, service_pb2.ListAppsRequest,
-                                      request_data))
+        >>> apps = list(User("user_id").list_apps())
 
-    return [App(**app_info) for app_info in all_apps_info]
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
+    """
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_apps_info = self.list_pages_generator(
+        self.STUB.ListApps,
+        service_pb2.ListAppsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
+    for app_info in all_apps_info:
+      yield App(**app_info)
 
-  def list_runners(self, filter_by: Dict[str, Any] = {}) -> List[Runner]:
+  def list_runners(self, filter_by: Dict[str, Any] = {}, page_no: int = None,
+                   per_page: int = None) -> Generator[Runner, None, None]:
     """List all runners for the user
 
     Args:
         filter_by (dict): A dictionary of filters to apply to the list of runners.
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
 
-    Returns:
-        List[Runner]: A list of Runner objects for the runners.
+    Yields:
+        Runner: Runner objects for the runners.
 
     Example:
         >>> from clarifai.client.user import User
         >>> client = User(user_id="user_id")
-        >>> all_runners= client.list_runners()
+        >>> all_runners= list(client.list_runners())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
-    request_data = dict(user_app_id=self.user_app_id, per_page=self.default_page_size, **filter_by)
-    all_runners_info = list(
-        self.list_all_pages_generator(self.STUB.ListRunners, service_pb2.ListRunnersRequest,
-                                      request_data))
+    request_data = dict(user_app_id=self.user_app_id, **filter_by)
+    all_runners_info = self.list_pages_generator(
+        self.STUB.ListRunners,
+        service_pb2.ListRunnersRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
-    return [Runner(check_runner_exists=False, **runner_info) for runner_info in all_runners_info]
+    for runner_info in all_runners_info:
+      yield Runner(check_runner_exists=False, **runner_info)
 
   def create_app(self, app_id: str, base_workflow: str = 'Language-Understanding',
                  **kwargs) -> App:
     """Creates an app for the user.
 
     Args:
         app_id (str): The app ID for the app to create.
```

### Comparing `clarifai-9.9.2/clarifai_utils/client/workflow.py` & `clarifai-9.9.3/clarifai_utils/client/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Dict, List
+from typing import Dict, Generator, List
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from clarifai_grpc.grpc.api.resources_pb2 import Input
 from clarifai_grpc.grpc.api.status import status_code_pb2
 
 from clarifai.client.base import BaseClient
 from clarifai.client.lister import Lister
@@ -152,42 +152,49 @@
           data=resources_pb2.Data(video=resources_pb2.Video(url=url)))
     elif input_type == "audio":
       input_proto = resources_pb2.Input(
           data=resources_pb2.Data(audio=resources_pb2.Audio(url=url)))
 
     return self.predict(inputs=[input_proto])
 
-  def list_versions(self) -> List['Workflow']:
+  def list_versions(self, page_no: int = None,
+                    per_page: int = None) -> Generator['Workflow', None, None]:
     """Lists all the versions of the workflow.
 
-    Returns:
-        list[Workflow]: A list of Workflow objects.
+    Args:
+        page_no (int): The page number to list.
+        per_page (int): The number of items per page.
+
+    Yields:
+        Workflow: Workflow objects for versions of the workflow.
 
     Example:
         >>> from clarifai.client.workflow import Workflow
         >>> workflow = Workflow(user_id='user_id', app_id='app_id', workflow_id='workflow_id')
-        >>> workflow_versions = workflow.list_versions()
+        >>> workflow_versions = list(workflow.list_versions())
+
+    Note:
+        Defaults to 16 per page if page_no is specified and per_page is not specified.
+        If both page_no and per_page are None, then lists all the resources.
     """
     request_data = dict(
         user_app_id=self.user_app_id,
         workflow_id=self.id,
-        per_page=self.default_page_size,
     )
-    all_workflow_versions_info = list(
-        self.list_all_pages_generator(self.STUB.ListWorkflowVersions,
-                                      service_pb2.ListWorkflowVersionsRequest, request_data))
+    all_workflow_versions_info = self.list_pages_generator(
+        self.STUB.ListWorkflowVersions,
+        service_pb2.ListWorkflowVersionsRequest,
+        request_data,
+        per_page=per_page,
+        page_no=page_no)
 
     for workflow_version_info in all_workflow_versions_info:
       workflow_version_info['id'] = workflow_version_info['workflow_version_id']
       del workflow_version_info['workflow_version_id']
-
-    return [
-        Workflow(workflow_id=self.id, **dict(self.kwargs, version=workflow_version_info))
-        for workflow_version_info in all_workflow_versions_info
-    ]
+      yield Workflow(workflow_id=self.id, **dict(self.kwargs, version=workflow_version_info))
 
   def export(self, out_path: str):
     """Exports the workflow to a yaml file.
 
     Args:
         out_path (str): The path to save the yaml file to.
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/export/inputs_annotations.py` & `clarifai-9.9.3/clarifai_utils/datasets/export/inputs_annotations.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/base.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/README.md` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,11 +32,15 @@
     return data
 
   def __getitem__(self, index):
     item = self.data[index]
     return VisualClassificationFeatures(
         image_path=os.path.join(os.path.dirname(__file__), item[0]),
         label=item[1],
-        id=os.path.basename(item[0]).split(".")[0])
+        id=os.path.basename(item[0]).split(".")[0],
+        metadata={
+            "split": self.split,
+            "image_path": item[0]
+        })
 
   def __len__(self):
     return len(self.data)
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_700.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_701.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_702.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_703.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_704.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_705.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_706.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_707.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_708.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/cifar10/images/test_batch_709.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/1420783.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3287885.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/3617075.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/38052.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/beignets/39147.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/139558.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/1636096.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/2480925.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3385808.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/hamburger/3647386.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/259212.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/1545393.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/2427642.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/3520891.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/377566.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/image_classification/food-101/images/ramen/503504.jpg`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,20 @@
     self.load_data()
 
   def load_data(self):
     with open(self.data_dirs[self.split]) as _file:
       reader = csv.reader(_file)
       next(reader, None)  # skip header
       for review in reader:
-        self.data.append({"text": review[0], "labels": review[1], "id": None})
+        self.data.append({
+            "text": review[0],
+            "labels": review[1],
+            "id": None,
+            "metadata": dict(split=self.split)
+        })
 
   def __getitem__(self, idx):
     item = self.data[idx]
     return TextFeatures(text=item["text"], labels=item["labels"], id=item["id"])
 
   def __len__(self):
     return len(self.data)
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/test.csv` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/test.csv`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/train.csv` & `clarifai-9.9.3/clarifai_utils/datasets/upload/examples/text_classification/imdb_dataset/train.csv`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/features.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/features.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,40 @@
 
 @dataclass
 class TextFeatures:
   """Text classification datasets preprocessing output features."""
   text: str
   labels: List[Union[str, int]]  # List[str or int] to cater for multi-class tasks
   id: Optional[int] = None  # text_id
+  metadata: Optional[dict] = None
 
 
 @dataclass
 class VisualClassificationFeatures:
   """Image classification datasets preprocessing output features."""
   image_path: str
   label: Union[str, int]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
+  metadata: Optional[dict] = None
 
 
 @dataclass
 class VisualDetectionFeatures:
   """Image Detection datasets preprocessing output features."""
   image_path: str
   classes: List[Union[str, int]]
   bboxes: List[List[float]]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
+  metadata: Optional[dict] = None
 
 
 @dataclass
 class VisualSegmentationFeatures:
   """Image Segmentation datasets preprocessing output features."""
   image_path: str
   classes: List[Union[str, int]]
   polygons: List[List[List[float]]]
   geo_info: Optional[List[float]] = None  #[Longitude, Latitude]
   id: Optional[int] = None  # image_id
+  metadata: Optional[dict] = None
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/image.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,18 @@
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       image_path = datagen_item.image_path
       label = datagen_item.label if isinstance(datagen_item.label,
                                                list) else [datagen_item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
       geo_info = datagen_item.geo_info
-      metadata.update({"filename": os.path.basename(image_path), "split": self.split})
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"filename": os.path.basename(image_path), "split": self.split})
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_input_from_file(
               input_id=input_id,
               image_file=image_path,
               dataset_id=self.dataset_id,
@@ -71,16 +74,19 @@
 
     def process_datagen_item(id):
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       image = datagen_item.image_path
       labels = datagen_item.classes  # list:[l1,...,ln]
       bboxes = datagen_item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
-      input_id = f"{self.dataset_id}-{self.split}-{i}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
-      metadata.update({"filename": os.path.basename(image), "split": self.split})
+      input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = datagen_item.geo_info
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_input_from_file(
               input_id=input_id,
               image_file=image,
@@ -121,16 +127,19 @@
 
     def process_datagen_item(id):
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       image = datagen_item.image_path
       labels = datagen_item.classes
       _polygons = datagen_item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
-      input_id = f"{self.dataset_id}-{self.split}-{i}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
-      metadata.update({"filename": os.path.basename(image), "split": self.split})
+      input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = datagen_item.geo_info
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_input_from_file(
               input_id=input_id,
               image_file=image,
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/README.md` & `clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/coco_captions.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/coco_detection.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/coco_segmentation.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/coco_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,22 +123,22 @@
     image_height, image_width = cv2.imread(image_path).shape[:2]
     for cat_id in labels:
       annot_ids = self.coco.getAnnIds(imgIds=_id, catIds=[cat_id])
       if len(annot_ids) > 0:
         img_annotations = self.coco.loadAnns(annot_ids)
         for ann in img_annotations:
           # get polygons
-          if type(ann['segmentation']) == list:
+          if isinstance(ann['segmentation'], list):
             for seg in ann['segmentation']:
               poly = np.array(seg).reshape((int(len(seg) / 2), 2))
               poly[:, 0], poly[:, 1] = poly[:, 0] / image_width, poly[:, 1] / image_height
               annots.append(poly.tolist())  #[[x=col, y=row],...]
               class_names.append(self.cat_id_map[cat_id])
           else:  # seg: {"counts":[...]}
-            if type(ann['segmentation']['counts']) == list:
+            if isinstance(ann['segmentation']['counts'], list):
               rle = maskUtils.frPyObjects([ann['segmentation']], image_height, image_width)
             else:
               rle = ann['segmentation']
             mask = maskUtils.decode(rle)  #binary mask
             #convert mask to polygons and add to annots
             contours, _ = cv2.findContours(mask, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             polygons = []
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/imagenet_classification.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/imagenet_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             "".join(("".join((label.rstrip().lstrip().split(" ")))).split("'"))
             for label in _id[_id.find(" ") + 1:].split(",")
         })
 
     for _folder in os.listdir(os.path.join(self.data_dir, self.split)):
       try:
         concept = self.label_map[_folder]  #concepts
-      except:
+      except Exception:
         continue
       folder_path = os.path.join(self.data_dir, self.split) + "/" + _folder
       for _img in os.listdir(folder_path):
         if _img.lower().endswith(('.png', '.jpg', '.jpeg', '.tiff')):
           self.concepts.append(concept)
           self.image_paths.append(folder_path + "/" + _img)
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/loaders/xview_detection.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/loaders/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/text.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,18 @@
     def process_datagen_item(id):
       datagen_item = self.datagen_object[id]
       metadata = Struct()
       text = datagen_item.text
       labels = datagen_item.labels if isinstance(
           datagen_item.labels, list) else [datagen_item.labels]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{id}" if datagen_item.id is None else f"{self.dataset_id}-{self.split}-{str(datagen_item.id)}"
-      metadata.update({"split": self.split})
+      if datagen_item.metadata is not None:
+        metadata.update(datagen_item.metadata)
+      else:
+        metadata.update({"split": self.split})
 
       self.all_input_ids[id] = input_id
       input_protos.append(
           self.input_object.get_text_input(
               input_id=input_id,
               raw_text=text,
               dataset_id=self.dataset_id,
```

### Comparing `clarifai-9.9.2/clarifai_utils/datasets/upload/utils.py` & `clarifai-9.9.3/clarifai_utils/datasets/upload/utils.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/errors.py` & `clarifai-9.9.3/clarifai_utils/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     current_ts_str = str(time.time())
 
     msg = """%(method)s %(resource)s FAILED(%(time_ts)s).  error_code: %(error_code)s, error_description: %(error_desc)s, error_details: %(error_details)s
  >> Python client %(client_version)s with Python %(python_version)s on %(os_version)s
  >> %(method)s %(resource)s
  >> REQUEST(%(time_ts)s) %(request)s
  >> RESPONSE(%(time_ts)s) %(response)s""" % {
-        'baseurl': '%s/v2/' % _base_url(self.resource),
         'method': method,
         'resource': resource,
         'error_code': self.error_code,
         'error_desc': self.error_desc,
         'error_details': self.error_details,
         'request': json.dumps(params, indent=2),
         'response': response_json,
@@ -74,15 +73,15 @@
 def _base_url(url: str) -> str:
   """
   Extracts the base URL from the url, which is everything before the 4th slash character.
   https://www.clarifai.com/v2/models/1/output -> https://www.clarifai.com/v2/
   """
   try:
     return url[:_find_nth(url, '/', 4) + 1]
-  except:
+  except Exception:
     return ''
 
 
 def _find_nth(haystack: str, needle: str, n: int) -> int:
   start = haystack.find(needle)
   while start >= 0 and n > 1:
     start = haystack.find(needle, start + len(needle))
```

### Comparing `clarifai-9.9.2/clarifai_utils/models/api.py` & `clarifai-9.9.3/clarifai_utils/models/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/README.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/__init__.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/cli/__init__.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/cli/deploy_cli.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/cli/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/cli/model_zip.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/cli/repository.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/cli/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
       help=f"Clarifai supported model types.\n Model-types-map: {MODEL_TYPES}",
   )
   parser.add_argument(
       "--image_shape",
       type=dims_type,
       default="[-1, -1]",
       required=False,
-      help=
-      f"(H, W) dims for models with an image input type. H and W each have a max value of 1024",
+      help="(H, W) dims for models with an image input type. H and W each have a max value of 1024",
   )
   parser.add_argument(
       "--repo_dir",
       type=str,
       default=".",
       required=True,
       help="Directory to create triton repository.")
```

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/docs/custom_config.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/docs/custom_config.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/docs/dependencies.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/docs/dependencies.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/docs/model_types.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/docs/model_types.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/docs/output.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/docs/output.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/README.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/README.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_image/sd-v1.5/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/README.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/README.md` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/labels.txt` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/labels.txt`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/__init__.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/config.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/config.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/model_types_config/visual-detector.yaml` & `clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/model_types_config/visual-detector.yaml`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/model_config/serializer.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/models/__init__.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/models/default_test.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/models/default_test.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/models/inference.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/models/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/models/model_types.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/models/model_types.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/models/output.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/models/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
           scores-dims: {self.predicted_scores.ndim} instead."
     assert self.predicted_bboxes.shape[0] == self.predicted_labels.shape[0] == \
       self.predicted_scores.shape[0], f"The Number of predicted bounding boxes, \
         predicted labels and predicted scores MUST match. Got {len(self.predicted_bboxes)}, \
           {self.predicted_labels.shape[0]}, {self.predicted_scores.shape[0]} instead."
 
     if len(self.predicted_labels) > 0:
-      assert self.predicted_bboxes.shape[1] == 4, f"Box coordinates must have a length of 4."
+      assert self.predicted_bboxes.shape[
+          1] == 4, f"Box coordinates must have a length of 4. Actual:{self.predicted_bboxes.shape[1]}"
       assert np.all(np.logical_and(0 <= self.predicted_bboxes, self.predicted_bboxes <= 1)), \
        "Bounding box coordinates must be between 0 and 1"
 
 
 @dataclass
 class ClassifierOutput:
   """
```

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/models/pb_model.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/models/pb_model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/models/test.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/models/test.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/models/model_serving/pb_model_repository.py` & `clarifai-9.9.3/clarifai_utils/models/model_serving/pb_model_repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/modules/css.py` & `clarifai-9.9.3/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/modules/pages.py` & `clarifai-9.9.3/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/modules/style.css` & `clarifai-9.9.3/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/runners/example.py` & `clarifai-9.9.3/clarifai_utils/runners/example.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/schema/search.py` & `clarifai-9.9.3/clarifai_utils/schema/search.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/urls/helper.py` & `clarifai-9.9.3/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/utils/logging.py` & `clarifai-9.9.3/clarifai_utils/utils/logging.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/utils/misc.py` & `clarifai-9.9.3/clarifai_utils/utils/misc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/workflows/export.py` & `clarifai-9.9.3/clarifai_utils/workflows/export.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/workflows/utils.py` & `clarifai-9.9.3/clarifai_utils/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/clarifai_utils/workflows/validate.py` & `clarifai-9.9.3/clarifai_utils/workflows/validate.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/tests/test_app.py` & `clarifai-9.9.3/tests/test_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,40 +44,40 @@
     - model
     - workflow
 
     Note: Update to be added later.
     """
 
   def test_list_models(self, app):
-    all_models = app.list_models()
-    assert len(all_models) > 0
+    all_models = list(app.list_models(page_no=2))
+    assert len(all_models) == 16  #default per_page is 16
 
   def test_list_workflows(self, app):
-    all_workflows = app.list_workflows()
-    assert len(all_workflows) > 0
+    all_workflows = list(app.list_workflows(page_no=1, per_page=10))
+    assert len(all_workflows) == 10
 
   def test_list_apps(self, client):
-    all_apps = client.list_apps()
+    all_apps = list(client.list_apps())
     assert len(all_apps) > 0
 
   def test_get_model(self, client):
     model = client.app(app_id=MAIN_APP_ID).model(model_id=GENERAL_MODEL_ID)
     assert model.id == GENERAL_MODEL_ID and model.app_id == MAIN_APP_ID and model.user_id == MAIN_APP_USER_ID
 
   def test_get_workflow(self, client):
     workflow = client.app(app_id=MAIN_APP_ID).workflow(workflow_id=General_Workflow_ID)
     assert workflow.id == General_Workflow_ID and workflow.app_id == MAIN_APP_ID and workflow.user_id == MAIN_APP_USER_ID
 
   def test_create_app(self):
     app = User(user_id=CREATE_APP_USER_ID).create_app(app_id=CREATE_APP_ID)
     assert app.id == CREATE_APP_ID and app.user_id == CREATE_APP_USER_ID
 
-  def test_create_dataset(self, create_app):
+  def test_create_search(self, create_app):
     search = create_app.search()
-    assert search.page_size == DEFAULT_TOP_K and search.metric_distance == "COSINE_DISTANCE"
+    assert search.default_page_size == DEFAULT_TOP_K and search.metric_distance == "COSINE_DISTANCE"
 
   def test_create_dataset(self, create_app):
     dataset = create_app.create_dataset(CREATE_DATASET_ID)
     assert dataset.id == CREATE_DATASET_ID and dataset.app_id == CREATE_APP_ID and dataset.user_id == CREATE_APP_USER_ID
 
   def test_create_model(self, create_app):
     model = create_app.create_model(CREATE_MODEL_ID)
@@ -89,14 +89,22 @@
 
   def test_create_runner(self, client):
     client = User(user_id=CREATE_APP_USER_ID)
     runner = client.create_runner(
         CREATE_RUNNER_ID, labels=["ci runner"], description="CI test runner")
     assert runner.id == CREATE_RUNNER_ID and runner.user_id == CREATE_APP_USER_ID
 
+  def test_get_dataset(self, create_app):
+    dataset = create_app.dataset(dataset_id=CREATE_DATASET_ID)
+    assert dataset.id == CREATE_DATASET_ID and dataset.app_id == CREATE_APP_ID and dataset.user_id == CREATE_APP_USER_ID
+
+  def test_list_datasets(self, create_app):
+    all_datasets = list(create_app.list_datasets())
+    assert len(all_datasets) == 1
+
   def test_delete_dataset(self, create_app, caplog):
     with caplog.at_level(logging.INFO):
       create_app.delete_dataset(CREATE_DATASET_ID)
       assert "SUCCESS" in caplog.text
 
   def test_delete_model(self, create_app, caplog):
     with caplog.at_level(logging.INFO):
@@ -114,13 +122,7 @@
       client.delete_runner(CREATE_RUNNER_ID)
       assert "SUCCESS" in caplog.text
 
   def test_delete_app(self, caplog):
     with caplog.at_level(logging.INFO):
       User(user_id=CREATE_APP_USER_ID).delete_app(CREATE_APP_ID)
       assert "SUCCESS" in caplog.text
-
-  def test_get_dataset(self):
-    pass  # TODO
-
-  def test_list_datasets(self):
-    pass  # TODO
```

### Comparing `clarifai-9.9.2/tests/test_auth.py` & `clarifai-9.9.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/tests/test_data_upload.py` & `clarifai-9.9.3/tests/test_data_upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import logging
 import os
+from datetime import datetime
 
 from clarifai.client.user import User
 
 CREATE_APP_USER_ID = os.environ["CLARIFAI_USER_ID"]
-CREATE_APP_ID = "ci_input_app"
+NOW = str(int(datetime.now().timestamp()))
+CREATE_APP_ID = f"ci_input_app_{NOW}"
 CREATE_DATASET_ID = "ci_input_test_dataset"
 
 #assets
 IMAGE_URL = "https://samples.clarifai.com/metro-north.jpg"
 VIDEO_URL = "https://samples.clarifai.com/beer.mp4"
 TEXT_URL = "https://samples.clarifai.com/featured-models/Llama2_Conversational-agent.txt"
 AUDIO_URL = "https://samples.clarifai.com/english_audio_sample.mp3"
 IMAGE_FILE_PATH = os.path.dirname(__file__) + "/assets/red-truck.png"
 VIDEO_FILE_PATH = os.path.dirname(__file__) + "/assets/sample.mp4"
 TEXT_FILE_PATH = os.path.dirname(__file__) + "/assets/sample.txt"
 AUDIO_FILE_PATH = os.path.dirname(__file__) + "/assets/sample.mp3"
 CSV_FILE_PATH = os.path.dirname(__file__) + "/assets/sample.csv"
 FOLDER_PATH = os.path.dirname(__file__) + "/assets/test"
+MODULE_DIR = os.path.dirname(__file__) + "/assets/voc"
 
 
 def create_app():
   client = User(user_id=CREATE_APP_USER_ID)
   return client.create_app(app_id=CREATE_APP_ID, base_workflow="Empty")
 
 
@@ -37,14 +40,15 @@
   - url
   - filepath
   - rawtext
   - CSV
   - Folder
   """
 
+  @classmethod
   def setup_class(self):
     self.app = create_app()
     self.input_object = self.app.inputs()
     self.dataset = self.app.create_dataset(dataset_id=CREATE_DATASET_ID)
 
   def test_upload_image_url(self, caplog):
     with caplog.at_level(logging.INFO):
@@ -87,36 +91,55 @@
       assert "SUCCESS" in caplog.text
 
   def test_upload_rawtext(self, caplog):
     with caplog.at_level(logging.INFO):
       self.input_object.upload_text(input_id='input_9', raw_text='This is a test text')
       assert "SUCCESS" in caplog.text
 
+  def test_list_inputs(self):
+    paginated_inputs = list(self.input_object.list_inputs(page_no=1, per_page=5))
+    image_filterd_inputs = list(self.input_object.list_inputs(input_type='image'))
+    assert len(paginated_inputs) == 5
+    assert len(image_filterd_inputs) == 2  # 2 images uploaded in the above tests
+
   def test_aggregate_inputs(self, caplog):
-    uploaded_inputs = self.input_object.list_inputs()
+    uploaded_inputs = list(self.input_object.list_inputs())
     with caplog.at_level(logging.INFO):
       self.input_object.delete_inputs(uploaded_inputs)
       assert "Inputs Deleted" in caplog.text  # Testing delete inputs action
     assert len(uploaded_inputs) == 9  # 9 inputs uploaded in the above tests
 
   def test_upload_csv(self, caplog):
     self.dataset.upload_from_csv(
         csv_path=CSV_FILE_PATH, input_type='text', csv_type='raw', labels=True)
-    uploaded_inputs = self.input_object.list_inputs()
+    uploaded_inputs = list(self.input_object.list_inputs(dataset_id=CREATE_DATASET_ID))
+    concepts = list(self.app.list_concepts())
     with caplog.at_level(logging.INFO):
       self.input_object.delete_inputs(uploaded_inputs)
       assert "Inputs Deleted" in caplog.text  # Testing delete inputs action
     assert uploaded_inputs[0].data.concepts[0].name == 'neg'  # label of the first input in the CSV file
     assert len(uploaded_inputs) == 5  # 5 inputs are uploaded from the CSV file
+    assert len(concepts) == 2  # Test for list concepts
 
   def test_upload_folder(self, caplog):
     self.dataset.upload_from_folder(folder_path=FOLDER_PATH, input_type='image', labels=True)
-    uploaded_inputs = self.input_object.list_inputs()
+    uploaded_inputs = list(self.input_object.list_inputs())
     with caplog.at_level(logging.INFO):
       self.input_object.delete_inputs(uploaded_inputs)
       assert "Inputs Deleted" in caplog.text  # Testing delete inputs action
     assert uploaded_inputs[0].data.concepts[0].name == 'test'  # label of the first input in the folder
     assert len(uploaded_inputs) == 3  # 3 inputs are uploaded from the folder
 
+  def test_upload_dataset(self, caplog):
+    self.dataset.upload_dataset(task="visual_detection", split="train", module_dir=MODULE_DIR)
+    uploaded_inputs = list(self.input_object.list_inputs())
+    annotations = list(self.input_object.list_annotations(batch_input=uploaded_inputs))
+    with caplog.at_level(logging.INFO):
+      self.input_object.delete_inputs(uploaded_inputs)
+      assert "Inputs Deleted" in caplog.text  # Testing delete inputs action
+    assert len(uploaded_inputs) == 10  # 3 inputs are uploaded from the folder
+    assert len(annotations) == 28  # Test for list annotatoins
+
+  @classmethod
   def teardown_class(self):
     self.app.delete_dataset(dataset_id=CREATE_DATASET_ID)
     User(user_id=CREATE_APP_USER_ID).delete_app(app_id=CREATE_APP_ID)
```

### Comparing `clarifai-9.9.2/tests/test_model_predict.py` & `clarifai-9.9.3/tests/test_model_predict.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/tests/test_modules.py` & `clarifai-9.9.3/tests/test_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
       model_id,
       model_version_id,
   ) = ClarifaiUrlHelper.split_clarifai_url(url)
   assert user_id == "clarifai"
   assert app_id == "main"
   assert resource_type == "models"
   assert model_id == "model_1"
-  assert model_version_id == None
+  assert model_version_id is None
 
   new = ClarifaiUrlHelper(auth).clarifai_url(user_id, app_id, resource_type, model_id,
                                              model_version_id)
   assert new == url
 
 
 def test_bad_resource_type_in_clarifai_url():
```

### Comparing `clarifai-9.9.2/tests/test_search.py` & `clarifai-9.9.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.9.2/tests/test_stub.py` & `clarifai-9.9.3/tests/test_stub.py`

 * *Files identical despite different names*

