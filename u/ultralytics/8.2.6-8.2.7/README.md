# Comparing `tmp/ultralytics-8.2.6.tar.gz` & `tmp/ultralytics-8.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.2.6.tar", last modified: Wed May  1 14:01:24 2024, max compression
+gzip compressed data, was "ultralytics-8.2.7.tar", last modified: Fri May  3 01:27:24 2024, max compression
```

## Comparing `ultralytics-8.2.6.tar` & `ultralytics-8.2.7.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.348546 ultralytics-8.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-01 13:59:50.000000 ultralytics-8.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-05-01 14:01:24.348546 ultralytics-8.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36782 2024-05-01 13:59:50.000000 ultralytics-8.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-01 13:59:50.000000 ultralytics-8.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:01:24.348546 ultralytics-8.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.312546 ultralytics-8.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-01 13:59:50.000000 ultralytics-8.2.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-01 13:59:50.000000 ultralytics-8.2.6/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-01 13:59:50.000000 ultralytics-8.2.6/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-01 13:59:50.000000 ultralytics-8.2.6/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-01 13:59:50.000000 ultralytics-8.2.6/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    23135 2024-05-01 13:59:50.000000 ultralytics-8.2.6/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.312546 ultralytics-8.2.6/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.312546 ultralytics-8.2.6/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.312546 ultralytics-8.2.6/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.316546 ultralytics-8.2.6/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.308546 ultralytics-8.2.6/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.320546 ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.320546 ultralytics-8.2.6/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.320546 ultralytics-8.2.6/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.320546 ultralytics-8.2.6/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.320546 ultralytics-8.2.6/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.324546 ultralytics-8.2.6/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.324546 ultralytics-8.2.6/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.324546 ultralytics-8.2.6/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.324546 ultralytics-8.2.6/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.324546 ultralytics-8.2.6/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    30879 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.328546 ultralytics-8.2.6/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54600 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34987 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.328546 ultralytics-8.2.6/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.328546 ultralytics-8.2.6/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.328546 ultralytics-8.2.6/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.328546 ultralytics-8.2.6/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.328546 ultralytics-8.2.6/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.332546 ultralytics-8.2.6/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.332546 ultralytics-8.2.6/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.332546 ultralytics-8.2.6/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.332546 ultralytics-8.2.6/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.332546 ultralytics-8.2.6/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.332546 ultralytics-8.2.6/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.332546 ultralytics-8.2.6/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.336546 ultralytics-8.2.6/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.336546 ultralytics-8.2.6/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.336546 ultralytics-8.2.6/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.336546 ultralytics-8.2.6/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.336546 ultralytics-8.2.6/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.336546 ultralytics-8.2.6/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/parking_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.340546 ultralytics-8.2.6/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.340546 ultralytics-8.2.6/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.344546 ultralytics-8.2.6/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    39286 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    23470 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.344546 ultralytics-8.2.6/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    48315 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-01 13:59:50.000000 ultralytics-8.2.6/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:01:24.344546 ultralytics-8.2.6/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-05-01 14:01:24.000000 ultralytics-8.2.6/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-05-01 14:01:24.000000 ultralytics-8.2.6/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:01:24.000000 ultralytics-8.2.6/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 14:01:24.000000 ultralytics-8.2.6/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-01 14:01:24.000000 ultralytics-8.2.6/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 14:01:24.000000 ultralytics-8.2.6/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.954858 ultralytics-8.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-03 01:26:01.000000 ultralytics-8.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40624 2024-05-03 01:27:24.954858 ultralytics-8.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36782 2024-05-03 01:26:01.000000 ultralytics-8.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-03 01:26:01.000000 ultralytics-8.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 01:27:24.954858 ultralytics-8.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.918857 ultralytics-8.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-03 01:26:01.000000 ultralytics-8.2.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-03 01:26:01.000000 ultralytics-8.2.7/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-03 01:26:01.000000 ultralytics-8.2.7/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-03 01:26:01.000000 ultralytics-8.2.7/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-03 01:26:01.000000 ultralytics-8.2.7/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23135 2024-05-03 01:26:01.000000 ultralytics-8.2.7/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.918857 ultralytics-8.2.7/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.918857 ultralytics-8.2.7/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.918857 ultralytics-8.2.7/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.922857 ultralytics-8.2.7/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.914857 ultralytics-8.2.7/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.922857 ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.922857 ultralytics-8.2.7/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.926857 ultralytics-8.2.7/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.926857 ultralytics-8.2.7/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.926857 ultralytics-8.2.7/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.926857 ultralytics-8.2.7/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.926857 ultralytics-8.2.7/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.930858 ultralytics-8.2.7/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.930858 ultralytics-8.2.7/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.930858 ultralytics-8.2.7/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30879 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.930858 ultralytics-8.2.7/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54606 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34987 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.934857 ultralytics-8.2.7/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.934857 ultralytics-8.2.7/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.934857 ultralytics-8.2.7/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.934857 ultralytics-8.2.7/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.934857 ultralytics-8.2.7/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.934857 ultralytics-8.2.7/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.938857 ultralytics-8.2.7/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.938857 ultralytics-8.2.7/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.938857 ultralytics-8.2.7/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.938857 ultralytics-8.2.7/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.938857 ultralytics-8.2.7/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.938857 ultralytics-8.2.7/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.938857 ultralytics-8.2.7/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.942858 ultralytics-8.2.7/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.942858 ultralytics-8.2.7/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.942858 ultralytics-8.2.7/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.942858 ultralytics-8.2.7/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.942858 ultralytics-8.2.7/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/parking_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.946858 ultralytics-8.2.7/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.946858 ultralytics-8.2.7/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.950858 ultralytics-8.2.7/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39284 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23470 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.950858 ultralytics-8.2.7/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28077 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48315 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-03 01:26:01.000000 ultralytics-8.2.7/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:27:24.950858 ultralytics-8.2.7/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40624 2024-05-03 01:27:24.000000 ultralytics-8.2.7/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-05-03 01:27:24.000000 ultralytics-8.2.7/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:27:24.000000 ultralytics-8.2.7/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 01:27:24.000000 ultralytics-8.2.7/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-03 01:27:24.000000 ultralytics-8.2.7/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 01:27:24.000000 ultralytics-8.2.7/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.2.6/LICENSE` & `ultralytics-8.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/PKG-INFO` & `ultralytics-8.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.6
+Version: 8.2.7
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
@@ -59,14 +59,15 @@
 Requires-Dist: mkdocs-ultralytics-plugin>=0.0.44; extra == "dev"
 Provides-Extra: export
 Requires-Dist: onnx>=1.12.0; extra == "export"
 Requires-Dist: coremltools>=7.0; (platform_system != "Windows" and python_version <= "3.11") and extra == "export"
 Requires-Dist: openvino>=2024.0.0; extra == "export"
 Requires-Dist: tensorflow<=2.13.1; python_version <= "3.11" and extra == "export"
 Requires-Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
+Requires-Dist: flatbuffers<100,>=23.5.26; platform_machine == "aarch64" and extra == "export"
 Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra == "export"
 Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra == "export"
 Provides-Extra: explorer
 Requires-Dist: lancedb; extra == "explorer"
 Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 Provides-Extra: logging
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.6 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.7 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
@@ -35,24 +35,25 @@
 mkdocs-redirects; extra == "dev" Requires-Dist: mkdocs-ultralytics-
 plugin>=0.0.44; extra == "dev" Provides-Extra: export Requires-Dist:
 onnx>=1.12.0; extra == "export" Requires-Dist: coremltools>=7.0;
 (platform_system != "Windows" and python_version <= "3.11") and extra ==
 "export" Requires-Dist: openvino>=2024.0.0; extra == "export" Requires-Dist:
 tensorflow<=2.13.1; python_version <= "3.11" and extra == "export" Requires-
 Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
-Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra ==
-"export" Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra
-== "export" Provides-Extra: explorer Requires-Dist: lancedb; extra ==
-"explorer" Requires-Dist: duckdb<=0.9.2; extra == "explorer" Requires-Dist:
-streamlit; extra == "explorer" Provides-Extra: logging Requires-Dist: comet;
-extra == "logging" Requires-Dist: tensorboard>=2.13.0; extra == "logging"
-Requires-Dist: dvclive>=2.12.0; extra == "logging" Provides-Extra: extra
-Requires-Dist: hub-sdk>=0.0.5; extra == "extra" Requires-Dist: ipython; extra
-== "extra" Requires-Dist: albumentations>=1.0.3; extra == "extra" Requires-
-Dist: pycocotools>=2.0.7; extra == "extra"
+Requires-Dist: flatbuffers<100,>=23.5.26; platform_machine == "aarch64" and
+extra == "export" Requires-Dist: numpy==1.23.5; platform_machine == "aarch64"
+and extra == "export" Requires-Dist: h5py!=3.11.0; platform_machine ==
+"aarch64" and extra == "export" Provides-Extra: explorer Requires-Dist:
+lancedb; extra == "explorer" Requires-Dist: duckdb<=0.9.2; extra == "explorer"
+Requires-Dist: streamlit; extra == "explorer" Provides-Extra: logging Requires-
+Dist: comet; extra == "logging" Requires-Dist: tensorboard>=2.13.0; extra ==
+"logging" Requires-Dist: dvclive>=2.12.0; extra == "logging" Provides-Extra:
+extra Requires-Dist: hub-sdk>=0.0.5; extra == "extra" Requires-Dist: ipython;
+extra == "extra" Requires-Dist: albumentations>=1.0.3; extra == "extra"
+Requires-Dist: pycocotools>=2.0.7; extra == "extra"
                              _[_Y_O_L_O_ _V_i_s_i_o_n_ _b_a_n_n_e_r_]
        [ä¸­æ](https://docs.ultralytics.com/zh/) | [íêµ­ì´](https://
  docs.ultralytics.com/ko/) | [æ¥æ¬èª](https://docs.ultralytics.com/ja/) |
     [Ð ÑÑÑÐºÐ¸Ð¹](https://docs.ultralytics.com/ru/) | [Deutsch](https://
  docs.ultralytics.com/de/) | [FranÃ§ais](https://docs.ultralytics.com/fr/) |
      [EspaÃ±ol](https://docs.ultralytics.com/es/) | [PortuguÃªs](https://
   docs.ultralytics.com/pt/) | [TÃ¼rkÃ§e](https://docs.ultralytics.com/tr/) |
```

### Comparing `ultralytics-8.2.6/README.md` & `ultralytics-8.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/pyproject.toml` & `ultralytics-8.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 ]
 export = [
     "onnx>=1.12.0", # ONNX export
     "coremltools>=7.0; platform_system != 'Windows' and python_version <= '3.11'", # CoreML supported on macOS and Linux
     "openvino>=2024.0.0", # OpenVINO export
     "tensorflow<=2.13.1; python_version <= '3.11'", # TF bug https://github.com/ultralytics/ultralytics/issues/5161
     "tensorflowjs>=3.9.0; python_version <= '3.11'", # TF.js export, automatically installs tensorflow
-    # "flatbuffers>=23.5.26,<100", # update old 'flatbuffers' included inside tensorflow package: WARNING Dockerfile error https://github.com/ultralytics/ultralytics/actions/runs/8715942435/job/23908971614
+    "flatbuffers>=23.5.26,<100; platform_machine == 'aarch64'", # update old 'flatbuffers' included inside tensorflow package
     "numpy==1.23.5; platform_machine == 'aarch64'", # fix error: `np.bool` was a deprecated alias for the builtin `bool` when using TensorRT models on NVIDIA Jetson
     "h5py!=3.11.0; platform_machine == 'aarch64'", # fix h5py build issues due to missing aarch64 wheels in 3.11 release
 ]
 explorer = [
     "lancedb", # vector search
     "duckdb<=0.9.2", # SQL queries, duckdb==0.10.0 bug https://github.com/ultralytics/ultralytics/pull/8181
     "streamlit", # visualizing with GUI
```

### Comparing `ultralytics-8.2.6/tests/test_cli.py` & `ultralytics-8.2.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/tests/test_cuda.py` & `ultralytics-8.2.7/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/tests/test_engine.py` & `ultralytics-8.2.7/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/tests/test_explorer.py` & `ultralytics-8.2.7/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/tests/test_integrations.py` & `ultralytics-8.2.7/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/tests/test_python.py` & `ultralytics-8.2.7/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/__init__.py` & `ultralytics-8.2.7/ultralytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.2.6"
+__version__ = "8.2.7"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `ultralytics-8.2.6/ultralytics/assets/bus.jpg` & `ultralytics-8.2.7/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/assets/zidane.jpg` & `ultralytics-8.2.7/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/__init__.py` & `ultralytics-8.2.7/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/Argoverse.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/DOTAv1.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/ImageNet.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/Objects365.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/SKU-110K.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/VOC.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/VisDrone.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/african-wildlife.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/african-wildlife.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/brain-tumor.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/brain-tumor.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/carparts-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/coco-pose.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/coco.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/coco128-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/coco128.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/coco8-pose.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/coco8-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/coco8.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/crack-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/dota8.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/lvis.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/lvis.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/open-images-v7.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/package-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/tiger-pose.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/datasets/xView.yaml` & `ultralytics-8.2.7/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/default.yaml` & `ultralytics-8.2.7/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v3/yolov3.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v5/yolov5.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v6/yolov6.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-world.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-world.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8-worldv2.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8-worldv2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v8/yolov8.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9c-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9c-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9c.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9c.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9e-seg.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9e-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/models/v9/yolov9e.yaml` & `ultralytics-8.2.7/ultralytics/cfg/models/v9/yolov9e.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/trackers/botsort.yaml` & `ultralytics-8.2.7/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/cfg/trackers/bytetrack.yaml` & `ultralytics-8.2.7/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/__init__.py` & `ultralytics-8.2.7/ultralytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/annotator.py` & `ultralytics-8.2.7/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/augment.py` & `ultralytics-8.2.7/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/base.py` & `ultralytics-8.2.7/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/build.py` & `ultralytics-8.2.7/ultralytics/data/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     LoadScreenshots,
     LoadStreams,
     LoadTensor,
     SourceTypes,
     autocast_list,
 )
 from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS
-from ultralytics.utils import RANK, colorstr
+from ultralytics.utils import NUM_THREADS, RANK, colorstr
 from ultralytics.utils.checks import check_file
 
 from .dataset import GroundingDataset, YOLODataset, YOLOMultiModalDataset
 from .utils import PIN_MEMORY
 
 
 class InfiniteDataLoader(dataloader.DataLoader):
@@ -77,14 +77,15 @@
 
 
 def seed_worker(worker_id):  # noqa
     """Set dataloader worker seed https://pytorch.org/docs/stable/notes/randomness.html#dataloader."""
     worker_seed = torch.initial_seed() % 2**32
     np.random.seed(worker_seed)
     random.seed(worker_seed)
+    os.sched_setaffinity(0, range(NUM_THREADS))  # fix https://github.com/ultralytics/ultralytics/pull/11195
 
 
 def build_yolo_dataset(cfg, img_path, batch, data, mode="train", rect=False, stride=32, multi_modal=False):
     """Build YOLO Dataset."""
     dataset = YOLOMultiModalDataset if multi_modal else YOLODataset
     return dataset(
         img_path=img_path,
```

### Comparing `ultralytics-8.2.6/ultralytics/data/converter.py` & `ultralytics-8.2.7/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/dataset.py` & `ultralytics-8.2.7/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/explorer/explorer.py` & `ultralytics-8.2.7/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/explorer/gui/dash.py` & `ultralytics-8.2.7/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/explorer/utils.py` & `ultralytics-8.2.7/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/loaders.py` & `ultralytics-8.2.7/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/split_dota.py` & `ultralytics-8.2.7/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/data/utils.py` & `ultralytics-8.2.7/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/engine/exporter.py` & `ultralytics-8.2.7/ultralytics/engine/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,15 @@
 
         onnx.save(model_onnx, f)
         return f, model_onnx
 
     @try_export
     def export_openvino(self, prefix=colorstr("OpenVINO:")):
         """YOLOv8 OpenVINO export."""
-        check_requirements("openvino>=2024.0.0")  # requires openvino: https://pypi.org/project/openvino/
+        check_requirements(f'openvino{"<=2024.0.0" if ARM64 else ">=2024.0.0"}')  # fix OpenVINO issue on ARM64
         import openvino as ov
 
         LOGGER.info(f"\n{prefix} starting export with openvino {ov.__version__}...")
         assert TORCH_1_13, f"OpenVINO export requires torch>=1.13.0 but torch=={torch.__version__} is installed"
         ov_model = ov.convert_model(
             self.model.cpu(),
             input=None if self.args.dynamic else [self.im.shape],
```

### Comparing `ultralytics-8.2.6/ultralytics/engine/model.py` & `ultralytics-8.2.7/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/engine/predictor.py` & `ultralytics-8.2.7/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/engine/results.py` & `ultralytics-8.2.7/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/engine/trainer.py` & `ultralytics-8.2.7/ultralytics/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/engine/tuner.py` & `ultralytics-8.2.7/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/engine/validator.py` & `ultralytics-8.2.7/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/hub/__init__.py` & `ultralytics-8.2.7/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/hub/auth.py` & `ultralytics-8.2.7/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/hub/session.py` & `ultralytics-8.2.7/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/hub/utils.py` & `ultralytics-8.2.7/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/fastsam/model.py` & `ultralytics-8.2.7/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/fastsam/predict.py` & `ultralytics-8.2.7/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/fastsam/prompt.py` & `ultralytics-8.2.7/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/fastsam/utils.py` & `ultralytics-8.2.7/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/fastsam/val.py` & `ultralytics-8.2.7/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/nas/model.py` & `ultralytics-8.2.7/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/nas/predict.py` & `ultralytics-8.2.7/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/nas/val.py` & `ultralytics-8.2.7/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/rtdetr/model.py` & `ultralytics-8.2.7/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/rtdetr/predict.py` & `ultralytics-8.2.7/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/rtdetr/train.py` & `ultralytics-8.2.7/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/rtdetr/val.py` & `ultralytics-8.2.7/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/amg.py` & `ultralytics-8.2.7/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/build.py` & `ultralytics-8.2.7/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/model.py` & `ultralytics-8.2.7/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/modules/decoders.py` & `ultralytics-8.2.7/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/modules/encoders.py` & `ultralytics-8.2.7/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/modules/sam.py` & `ultralytics-8.2.7/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/modules/tiny_encoder.py` & `ultralytics-8.2.7/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/modules/transformer.py` & `ultralytics-8.2.7/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/sam/predict.py` & `ultralytics-8.2.7/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/utils/loss.py` & `ultralytics-8.2.7/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/utils/ops.py` & `ultralytics-8.2.7/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/classify/predict.py` & `ultralytics-8.2.7/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/classify/train.py` & `ultralytics-8.2.7/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/classify/val.py` & `ultralytics-8.2.7/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/detect/predict.py` & `ultralytics-8.2.7/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/detect/train.py` & `ultralytics-8.2.7/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/detect/val.py` & `ultralytics-8.2.7/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/model.py` & `ultralytics-8.2.7/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/obb/predict.py` & `ultralytics-8.2.7/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/obb/train.py` & `ultralytics-8.2.7/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/obb/val.py` & `ultralytics-8.2.7/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/pose/predict.py` & `ultralytics-8.2.7/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/pose/train.py` & `ultralytics-8.2.7/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/pose/val.py` & `ultralytics-8.2.7/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/segment/predict.py` & `ultralytics-8.2.7/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/segment/train.py` & `ultralytics-8.2.7/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/segment/val.py` & `ultralytics-8.2.7/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/world/train.py` & `ultralytics-8.2.7/ultralytics/models/yolo/world/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/models/yolo/world/train_world.py` & `ultralytics-8.2.7/ultralytics/models/yolo/world/train_world.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/__init__.py` & `ultralytics-8.2.7/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/autobackend.py` & `ultralytics-8.2.7/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/modules/__init__.py` & `ultralytics-8.2.7/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/modules/block.py` & `ultralytics-8.2.7/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/modules/conv.py` & `ultralytics-8.2.7/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/modules/head.py` & `ultralytics-8.2.7/ultralytics/nn/modules/head.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,53 +94,51 @@
 
     def __init__(self, nc=80, nm=32, npr=256, ch=()):
         """Initialize the YOLO model attributes such as the number of masks, prototypes, and the convolution layers."""
         super().__init__(nc, ch)
         self.nm = nm  # number of masks
         self.npr = npr  # number of protos
         self.proto = Proto(ch[0], self.npr, self.nm)  # protos
-        self.detect = Detect.forward
 
         c4 = max(ch[0] // 4, self.nm)
         self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.nm, 1)) for x in ch)
 
     def forward(self, x):
         """Return model outputs and mask coefficients if training, otherwise return outputs and mask coefficients."""
         p = self.proto(x[0])  # mask protos
         bs = p.shape[0]  # batch size
 
         mc = torch.cat([self.cv4[i](x[i]).view(bs, self.nm, -1) for i in range(self.nl)], 2)  # mask coefficients
-        x = self.detect(self, x)
+        x = Detect.forward(self, x)
         if self.training:
             return x, mc, p
         return (torch.cat([x, mc], 1), p) if self.export else (torch.cat([x[0], mc], 1), (x[1], mc, p))
 
 
 class OBB(Detect):
     """YOLOv8 OBB detection head for detection with rotation models."""
 
     def __init__(self, nc=80, ne=1, ch=()):
         """Initialize OBB with number of classes `nc` and layer channels `ch`."""
         super().__init__(nc, ch)
         self.ne = ne  # number of extra parameters
-        self.detect = Detect.forward
 
         c4 = max(ch[0] // 4, self.ne)
         self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.ne, 1)) for x in ch)
 
     def forward(self, x):
         """Concatenates and returns predicted bounding boxes and class probabilities."""
         bs = x[0].shape[0]  # batch size
         angle = torch.cat([self.cv4[i](x[i]).view(bs, self.ne, -1) for i in range(self.nl)], 2)  # OBB theta logits
         # NOTE: set `angle` as an attribute so that `decode_bboxes` could use it.
         angle = (angle.sigmoid() - 0.25) * math.pi  # [-pi/4, 3pi/4]
         # angle = angle.sigmoid() * math.pi / 2  # [0, pi/2]
         if not self.training:
             self.angle = angle
-        x = self.detect(self, x)
+        x = Detect.forward(self, x)
         if self.training:
             return x, angle
         return torch.cat([x, angle], 1) if self.export else (torch.cat([x[0], angle], 1), (x[1], angle))
 
     def decode_bboxes(self, bboxes, anchors):
         """Decode rotated bounding boxes."""
         return dist2rbox(bboxes, self.angle, anchors, dim=1)
@@ -150,24 +148,23 @@
     """YOLOv8 Pose head for keypoints models."""
 
     def __init__(self, nc=80, kpt_shape=(17, 3), ch=()):
         """Initialize YOLO network with default parameters and Convolutional Layers."""
         super().__init__(nc, ch)
         self.kpt_shape = kpt_shape  # number of keypoints, number of dims (2 for x,y or 3 for x,y,visible)
         self.nk = kpt_shape[0] * kpt_shape[1]  # number of keypoints total
-        self.detect = Detect.forward
 
         c4 = max(ch[0] // 4, self.nk)
         self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.nk, 1)) for x in ch)
 
     def forward(self, x):
         """Perform forward pass through YOLO model and return predictions."""
         bs = x[0].shape[0]  # batch size
         kpt = torch.cat([self.cv4[i](x[i]).view(bs, self.nk, -1) for i in range(self.nl)], -1)  # (bs, 17*3, h*w)
-        x = self.detect(self, x)
+        x = Detect.forward(self, x)
         if self.training:
             return x, kpt
         pred_kpt = self.kpts_decode(bs, kpt)
         return torch.cat([x, pred_kpt], 1) if self.export else (torch.cat([x[0], pred_kpt], 1), (x[1], kpt))
 
     def kpts_decode(self, bs, kpts):
         """Decodes keypoints."""
```

### Comparing `ultralytics-8.2.6/ultralytics/nn/modules/transformer.py` & `ultralytics-8.2.7/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/modules/utils.py` & `ultralytics-8.2.7/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/nn/tasks.py` & `ultralytics-8.2.7/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/solutions/ai_gym.py` & `ultralytics-8.2.7/ultralytics/solutions/ai_gym.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/solutions/distance_calculation.py` & `ultralytics-8.2.7/ultralytics/solutions/distance_calculation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/solutions/heatmap.py` & `ultralytics-8.2.7/ultralytics/solutions/heatmap.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/solutions/object_counter.py` & `ultralytics-8.2.7/ultralytics/solutions/object_counter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/solutions/parking_management.py` & `ultralytics-8.2.7/ultralytics/solutions/parking_management.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/solutions/queue_management.py` & `ultralytics-8.2.7/ultralytics/solutions/queue_management.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/solutions/speed_estimation.py` & `ultralytics-8.2.7/ultralytics/solutions/speed_estimation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/trackers/basetrack.py` & `ultralytics-8.2.7/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/trackers/bot_sort.py` & `ultralytics-8.2.7/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/trackers/byte_tracker.py` & `ultralytics-8.2.7/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/trackers/track.py` & `ultralytics-8.2.7/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/trackers/utils/gmc.py` & `ultralytics-8.2.7/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/trackers/utils/kalman_filter.py` & `ultralytics-8.2.7/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/trackers/utils/matching.py` & `ultralytics-8.2.7/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/__init__.py` & `ultralytics-8.2.7/ultralytics/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 # Other Constants
 ARGV = sys.argv or ["", ""]  # sometimes sys.argv = []
 FILE = Path(__file__).resolve()
 ROOT = FILE.parents[1]  # YOLO
 ASSETS = ROOT / "assets"  # default images
 DEFAULT_CFG_PATH = ROOT / "cfg/default.yaml"
-NUM_THREADS = min(8, max(1, os.cpu_count() - 1))  # number of YOLOv5 multiprocessing threads
+NUM_THREADS = min(8, max(1, os.cpu_count() - 1))  # number of YOLO multiprocessing threads
 AUTOINSTALL = str(os.getenv("YOLO_AUTOINSTALL", True)).lower() == "true"  # global auto-install mode
 VERBOSE = str(os.getenv("YOLO_VERBOSE", True)).lower() == "true"  # global verbose mode
 TQDM_BAR_FORMAT = "{l_bar}{bar:10}{r_bar}" if VERBOSE else None  # tqdm bar format
 LOGGING_NAME = "ultralytics"
 MACOS, LINUX, WINDOWS = (platform.system() == x for x in ["Darwin", "Linux", "Windows"])  # environment booleans
 ARM64 = platform.machine() in {"arm64", "aarch64"}  # ARM64 booleans
 PYTHON_VERSION = platform.python_version()
```

### Comparing `ultralytics-8.2.6/ultralytics/utils/autobatch.py` & `ultralytics-8.2.7/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/benchmarks.py` & `ultralytics-8.2.7/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/base.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/clearml.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/comet.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/dvc.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/hub.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/mlflow.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/neptune.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/raytune.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/tensorboard.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/callbacks/wb.py` & `ultralytics-8.2.7/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/checks.py` & `ultralytics-8.2.7/ultralytics/utils/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,22 @@
     https://github.com/pytorch/vision#installation.
 
     The compatibility table is a dictionary where the keys are PyTorch versions and the values are lists of compatible
     Torchvision versions.
     """
 
     # Compatibility table
-    compatibility_table = {"2.0": ["0.15"], "1.13": ["0.14"], "1.12": ["0.13"]}
+    compatibility_table = {
+        "2.3": ["0.18"],
+        "2.2": ["0.17"],
+        "2.1": ["0.16"],
+        "2.0": ["0.15"],
+        "1.13": ["0.14"],
+        "1.12": ["0.13"],
+    }
 
     # Extract only the major and minor versions
     v_torch = ".".join(torch.__version__.split("+")[0].split(".")[:2])
     v_torchvision = ".".join(TORCHVISION_VERSION.split("+")[0].split(".")[:2])
 
     if v_torch in compatibility_table:
         compatible_versions = compatibility_table[v_torch]
```

### Comparing `ultralytics-8.2.6/ultralytics/utils/dist.py` & `ultralytics-8.2.7/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/downloads.py` & `ultralytics-8.2.7/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/errors.py` & `ultralytics-8.2.7/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/files.py` & `ultralytics-8.2.7/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/instance.py` & `ultralytics-8.2.7/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/loss.py` & `ultralytics-8.2.7/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/metrics.py` & `ultralytics-8.2.7/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/ops.py` & `ultralytics-8.2.7/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/patches.py` & `ultralytics-8.2.7/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/plotting.py` & `ultralytics-8.2.7/ultralytics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/tal.py` & `ultralytics-8.2.7/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/torch_utils.py` & `ultralytics-8.2.7/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/triton.py` & `ultralytics-8.2.7/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics/utils/tuner.py` & `ultralytics-8.2.7/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.2.7/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.6
+Version: 8.2.7
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
@@ -59,14 +59,15 @@
 Requires-Dist: mkdocs-ultralytics-plugin>=0.0.44; extra == "dev"
 Provides-Extra: export
 Requires-Dist: onnx>=1.12.0; extra == "export"
 Requires-Dist: coremltools>=7.0; (platform_system != "Windows" and python_version <= "3.11") and extra == "export"
 Requires-Dist: openvino>=2024.0.0; extra == "export"
 Requires-Dist: tensorflow<=2.13.1; python_version <= "3.11" and extra == "export"
 Requires-Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
+Requires-Dist: flatbuffers<100,>=23.5.26; platform_machine == "aarch64" and extra == "export"
 Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra == "export"
 Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra == "export"
 Provides-Extra: explorer
 Requires-Dist: lancedb; extra == "explorer"
 Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 Provides-Extra: logging
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.6 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.7 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
@@ -35,24 +35,25 @@
 mkdocs-redirects; extra == "dev" Requires-Dist: mkdocs-ultralytics-
 plugin>=0.0.44; extra == "dev" Provides-Extra: export Requires-Dist:
 onnx>=1.12.0; extra == "export" Requires-Dist: coremltools>=7.0;
 (platform_system != "Windows" and python_version <= "3.11") and extra ==
 "export" Requires-Dist: openvino>=2024.0.0; extra == "export" Requires-Dist:
 tensorflow<=2.13.1; python_version <= "3.11" and extra == "export" Requires-
 Dist: tensorflowjs>=3.9.0; python_version <= "3.11" and extra == "export"
-Requires-Dist: numpy==1.23.5; platform_machine == "aarch64" and extra ==
-"export" Requires-Dist: h5py!=3.11.0; platform_machine == "aarch64" and extra
-== "export" Provides-Extra: explorer Requires-Dist: lancedb; extra ==
-"explorer" Requires-Dist: duckdb<=0.9.2; extra == "explorer" Requires-Dist:
-streamlit; extra == "explorer" Provides-Extra: logging Requires-Dist: comet;
-extra == "logging" Requires-Dist: tensorboard>=2.13.0; extra == "logging"
-Requires-Dist: dvclive>=2.12.0; extra == "logging" Provides-Extra: extra
-Requires-Dist: hub-sdk>=0.0.5; extra == "extra" Requires-Dist: ipython; extra
-== "extra" Requires-Dist: albumentations>=1.0.3; extra == "extra" Requires-
-Dist: pycocotools>=2.0.7; extra == "extra"
+Requires-Dist: flatbuffers<100,>=23.5.26; platform_machine == "aarch64" and
+extra == "export" Requires-Dist: numpy==1.23.5; platform_machine == "aarch64"
+and extra == "export" Requires-Dist: h5py!=3.11.0; platform_machine ==
+"aarch64" and extra == "export" Provides-Extra: explorer Requires-Dist:
+lancedb; extra == "explorer" Requires-Dist: duckdb<=0.9.2; extra == "explorer"
+Requires-Dist: streamlit; extra == "explorer" Provides-Extra: logging Requires-
+Dist: comet; extra == "logging" Requires-Dist: tensorboard>=2.13.0; extra ==
+"logging" Requires-Dist: dvclive>=2.12.0; extra == "logging" Provides-Extra:
+extra Requires-Dist: hub-sdk>=0.0.5; extra == "extra" Requires-Dist: ipython;
+extra == "extra" Requires-Dist: albumentations>=1.0.3; extra == "extra"
+Requires-Dist: pycocotools>=2.0.7; extra == "extra"
                              _[_Y_O_L_O_ _V_i_s_i_o_n_ _b_a_n_n_e_r_]
        [ä¸­æ](https://docs.ultralytics.com/zh/) | [íêµ­ì´](https://
  docs.ultralytics.com/ko/) | [æ¥æ¬èª](https://docs.ultralytics.com/ja/) |
     [Ð ÑÑÑÐºÐ¸Ð¹](https://docs.ultralytics.com/ru/) | [Deutsch](https://
  docs.ultralytics.com/de/) | [FranÃ§ais](https://docs.ultralytics.com/fr/) |
      [EspaÃ±ol](https://docs.ultralytics.com/es/) | [PortuguÃªs](https://
   docs.ultralytics.com/pt/) | [TÃ¼rkÃ§e](https://docs.ultralytics.com/tr/) |
```

### Comparing `ultralytics-8.2.6/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.2.7/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.6/ultralytics.egg-info/requires.txt` & `ultralytics-8.2.7/ultralytics.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 streamlit
 
 [export]
 onnx>=1.12.0
 openvino>=2024.0.0
 
 [export:platform_machine == "aarch64"]
+flatbuffers<100,>=23.5.26
 numpy==1.23.5
 h5py!=3.11.0
 
 [export:platform_system != "Windows" and python_version <= "3.11"]
 coremltools>=7.0
 
 [export:python_version <= "3.11"]
```

