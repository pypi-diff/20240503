# Comparing `tmp/dghs_imgutils-0.4.2.tar.gz` & `tmp/dghs_imgutils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs_imgutils-0.4.2.tar", last modified: Thu May  2 15:51:45 2024, max compression
+gzip compressed data, was "dghs_imgutils-0.4.3.tar", last modified: Fri May  3 17:38:27 2024, max compression
```

## Comparing `dghs_imgutils-0.4.2.tar` & `dghs_imgutils-0.4.3.tar`

### file list

```diff
@@ -1,126 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.806495 dghs_imgutils-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 15:50:56.000000 dghs_imgutils-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 15:50:56.000000 dghs_imgutils-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19054 2024-05-02 15:51:45.806495 dghs_imgutils-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-02 15:50:56.000000 dghs_imgutils-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19054 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/ascii/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ascii/drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/censor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/eye.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/halfbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/hand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/generic/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/generic/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21967 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/ccip.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/dbaesthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/recognize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/censor_.py
--rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/emoji_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/heart_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/imgcensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/smile_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/squeeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/dwpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/restore/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/nafnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/scunet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/sd/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/sd/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/sd/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/onnxruntime.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/tqdm_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/aicheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/bangumi_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/completeness.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/dbrating.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/nsfw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/portrait.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/real.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/style_age.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/teen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-model.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:51:45.806495 dghs_imgutils-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.903425 dghs_imgutils-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 17:37:43.000000 dghs_imgutils-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 17:37:43.000000 dghs_imgutils-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-03 17:38:27.903425 dghs_imgutils-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-03 17:37:43.000000 dghs_imgutils-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.883425 dghs_imgutils-0.4.3/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.883425 dghs_imgutils-0.4.3/imgutils/ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ascii/drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.883425 dghs_imgutils-0.4.3/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/censor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/halfbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/hand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/generic/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23332 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/ccip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/dbaesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/recognize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/censor_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/emoji_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/heart_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/imgcensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/smile_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/squeeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/dwpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/resource/background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/restore/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/nafnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/scunet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/sd/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/sd/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/onnxruntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/tqdm_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/aicheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/bangumi_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/dbrating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/nsfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/portrait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/style_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/teen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-model.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:38:27.903425 dghs_imgutils-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/setup.py
```

### Comparing `dghs_imgutils-0.4.2/LICENSE` & `dghs_imgutils-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/PKG-INFO` & `dghs_imgutils-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.2
+Version: 0.4.3
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,14 +31,16 @@
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: emoji>=2.5.0
 Requires-Dist: pilmoji>=1.3.0
 Requires-Dist: shapely
 Requires-Dist: pyclipper
 Requires-Dist: deprecation>=2.0.0
+Requires-Dist: hfutils>=0.2.3
+Requires-Dist: filelock
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
 Requires-Dist: pytest~=6.2.5; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
```

### Comparing `dghs_imgutils-0.4.2/README.md` & `dghs_imgutils-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/dghs_imgutils.egg-info/PKG-INFO` & `dghs_imgutils-0.4.3/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.2
+Version: 0.4.3
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,14 +31,16 @@
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: emoji>=2.5.0
 Requires-Dist: pilmoji>=1.3.0
 Requires-Dist: shapely
 Requires-Dist: pyclipper
 Requires-Dist: deprecation>=2.0.0
+Requires-Dist: hfutils>=0.2.3
+Requires-Dist: filelock
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
 Requires-Dist: pytest~=6.2.5; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
```

### Comparing `dghs_imgutils-0.4.2/dghs_imgutils.egg-info/SOURCES.txt` & `dghs_imgutils-0.4.3/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 imgutils/edge/lineart_anime.py
 imgutils/generic/__init__.py
 imgutils/generic/classify.py
 imgutils/metrics/__init__.py
 imgutils/metrics/aesthetic.py
 imgutils/metrics/ccip.py
 imgutils/metrics/dbaesthetic.py
+imgutils/metrics/laplacian.py
 imgutils/metrics/lpips.py
 imgutils/metrics/psnr_.py
 imgutils/ocr/__init__.py
 imgutils/ocr/detect.py
 imgutils/ocr/entry.py
 imgutils/ocr/recognize.py
 imgutils/operate/__init__.py
@@ -60,14 +61,16 @@
 imgutils/operate/imgcensor.py
 imgutils/operate/smile_censor.png
 imgutils/operate/squeeze.py
 imgutils/pose/__init__.py
 imgutils/pose/dwpose.py
 imgutils/pose/format.py
 imgutils/pose/visual.py
+imgutils/resource/__init__.py
+imgutils/resource/background.py
 imgutils/restore/__init__.py
 imgutils/restore/adversarial.py
 imgutils/restore/nafnet.py
 imgutils/restore/scunet.py
 imgutils/sd/__init__.py
 imgutils/sd/metadata.py
 imgutils/sd/model.py
@@ -82,14 +85,15 @@
 imgutils/tagging/mldanbooru.py
 imgutils/tagging/order.py
 imgutils/tagging/overlap.py
 imgutils/tagging/wd14.py
 imgutils/utils/__init__.py
 imgutils/utils/area.py
 imgutils/utils/onnxruntime.py
+imgutils/utils/storage.py
 imgutils/utils/tqdm_.py
 imgutils/validate/__init__.py
 imgutils/validate/aicheck.py
 imgutils/validate/bangumi_char.py
 imgutils/validate/classify.py
 imgutils/validate/color.py
 imgutils/validate/completeness.py
```

### Comparing `dghs_imgutils-0.4.2/dghs_imgutils.egg-info/requires.txt` & `dghs_imgutils-0.4.3/dghs_imgutils.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 pandas
 scipy
 emoji>=2.5.0
 pilmoji>=1.3.0
 shapely
 pyclipper
 deprecation>=2.0.0
+hfutils>=0.2.3
+filelock
 
 [doc]
 Jinja2~=3.0.0
 sphinx>=3.2.0
 sphinx_rtd_theme>=0.4.3
 enum_tools~=0.9.0
 sphinx-toolbox
```

### Comparing `dghs_imgutils-0.4.2/imgutils/ascii/drawing.py` & `dghs_imgutils-0.4.3/imgutils/ascii/drawing.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/config/meta.py` & `dghs_imgutils-0.4.3/imgutils/config/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.4.2'
+__VERSION__ = '0.4.3'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d7'
```

### Comparing `dghs_imgutils-0.4.2/imgutils/data/background.py` & `dghs_imgutils-0.4.3/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/data/decode.py` & `dghs_imgutils-0.4.3/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/data/encode.py` & `dghs_imgutils-0.4.3/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/data/image.py` & `dghs_imgutils-0.4.3/imgutils/data/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     return hasattr(obj, 'read') and hasattr(obj, 'seek')
 
 
 ImageTyping = Union[str, PathLike, bytes, bytearray, BinaryIO, Image.Image]
 MultiImagesTyping = Union[ImageTyping, List[ImageTyping], Tuple[ImageTyping, ...]]
 
 
+def _has_alpha_channel(image: Image.Image) -> bool:
+    return any(band in {'A', 'a', 'P'} for band in image.getbands())
+
+
 def load_image(image: ImageTyping, mode=None, force_background: Optional[str] = 'white'):
     """
     Loads the image from the provided source and applies necessary transformations.
 
     The function supports loading images from various sources, such as file paths, binary data, or file-like objects.
     It opens the image using the PIL library and converts it to the specified mode if required.
     If the image has an RGBA (4-channel) format and a ``force_background`` value is provided, a background of
@@ -43,15 +47,15 @@
     if isinstance(image, (str, PathLike, bytes, bytearray, BinaryIO)) or _is_readable(image):
         image = Image.open(image)
     elif isinstance(image, Image.Image):
         pass  # just do nothing
     else:
         raise TypeError(f'Unknown image type - {image!r}.')
 
-    if force_background is not None:
+    if _has_alpha_channel(image) and force_background is not None:
         image = add_background_for_rgba(image, force_background)
 
     if mode is not None and image.mode != mode:
         image = image.convert(mode)
 
     return image
```

### Comparing `dghs_imgutils-0.4.2/imgutils/data/layer.py` & `dghs_imgutils-0.4.3/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/__init__.py` & `dghs_imgutils-0.4.3/imgutils/detect/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/_yolo.py` & `dghs_imgutils-0.4.3/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/censor.py` & `dghs_imgutils-0.4.3/imgutils/detect/censor.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/eye.py` & `dghs_imgutils-0.4.3/imgutils/detect/eye.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/face.py` & `dghs_imgutils-0.4.3/imgutils/detect/face.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/halfbody.py` & `dghs_imgutils-0.4.3/imgutils/detect/halfbody.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/hand.py` & `dghs_imgutils-0.4.3/imgutils/detect/hand.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/head.py` & `dghs_imgutils-0.4.3/imgutils/detect/head.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/person.py` & `dghs_imgutils-0.4.3/imgutils/detect/person.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/text.py` & `dghs_imgutils-0.4.3/imgutils/detect/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     :return: List of detected text bounding boxes, labels, and scores.
     :rtype: List[Tuple[Tuple[int, int, int, int], str, float]]
 
     .. warning::
         This function is deprecated, and it will be removed from imgutils in the future.
         Please migrate to :func:`imgutils.ocr.detect_text_with_ocr` as soon as possible.
     """
-    image = load_image(image)
+    image = load_image(image, mode='RGB')
     if max_area_size is not None and image.width * image.height >= max_area_size ** 2:
         r = ((image.width * image.height) / (max_area_size ** 2)) ** 0.5
         new_width, new_height = int(image.width / r), int(image.height / r)
         image = image.resize((new_width, new_height))
     else:
         r = 1.0
```

### Comparing `dghs_imgutils-0.4.2/imgutils/detect/visual.py` & `dghs_imgutils-0.4.3/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/edge/__init__.py` & `dghs_imgutils-0.4.3/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/edge/_base.py` & `dghs_imgutils-0.4.3/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/edge/canny.py` & `dghs_imgutils-0.4.3/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/edge/lineart.py` & `dghs_imgutils-0.4.3/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/edge/lineart_anime.py` & `dghs_imgutils-0.4.3/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/generic/classify.py` & `dghs_imgutils-0.4.3/imgutils/generic/classify.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/metrics/aesthetic.py` & `dghs_imgutils-0.4.3/imgutils/metrics/aesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/metrics/ccip.py` & `dghs_imgutils-0.4.3/imgutils/metrics/ccip.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     'ccip_difference',
     'ccip_same',
     'ccip_batch_differences',
     'ccip_batch_same',
 
     'ccip_default_clustering_params',
     'ccip_clustering',
+
+    'ccip_merge',
 ]
 
 
 def _normalize(data, mean=(0.48145466, 0.4578275, 0.40821073), std=(0.26862954, 0.26130258, 0.27577711)):
     mean, std = np.asarray(mean), np.asarray(std)
     return (data - mean[:, None, None]) / std[:, None, None]
 
@@ -513,7 +515,43 @@
         clustering = DBSCAN(eps=eps, min_samples=min_samples, metric=_metric).fit(samples)
     elif 'optics' in method:
         clustering = OPTICS(max_eps=eps, min_samples=min_samples, metric=_metric).fit(samples)
     else:
         assert False, f'Unknown mode for CCIP clustering - {method!r}.'  # pragma: no cover
 
     return clustering.labels_.tolist()
+
+
+def ccip_merge(images: Union[List[_FeatureOrImage], np.ndarray],
+               size: int = 384, model: str = _DEFAULT_MODEL_NAMES) -> np.ndarray:
+    """
+    Merge multiple feature vectors into a single vector.
+
+    :param images: The feature vectors or images to merge.
+    :type images: Union[List[_FeatureOrImage], numpy.ndarray]
+    :param size: The size of the image. (default: 384)
+    :type size: int
+    :param model: The name of the model. (default: ``ccip-caformer-24-randaug-pruned``)
+    :type model: str
+    :return: The merged feature vector.
+    :rtype: numpy.ndarray
+
+    Examples::
+        >>> from imgutils.metrics import ccip_merge, ccip_batch_differences
+        >>>
+        >>> images = [f'ccip/{i}.jpg' for i in range(1, 4)]
+        >>>
+        >>> merged = ccip_merge(images)
+        >>> merged.shape
+        (768,)
+        >>>
+        >>> diffs = ccip_batch_differences([merged, *images])[0, 1:]
+        >>> diffs
+        array([0.07437477, 0.0356068 , 0.04396922], dtype=float32)
+        >>> diffs.mean()
+        0.05131693
+    """
+    embs = np.stack([_p_feature(img, size, model) for img in images]).astype(np.float32)
+    lengths = np.linalg.norm(embs, axis=-1)
+    embs = embs / lengths.reshape(-1, 1)
+    ret_embedding = embs.mean(axis=0)
+    return ret_embedding / np.linalg.norm(ret_embedding) * lengths.mean()
```

### Comparing `dghs_imgutils-0.4.2/imgutils/metrics/dbaesthetic.py` & `dghs_imgutils-0.4.3/imgutils/metrics/dbaesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/metrics/lpips.py` & `dghs_imgutils-0.4.3/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/metrics/psnr_.py` & `dghs_imgutils-0.4.3/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/ocr/__init__.py` & `dghs_imgutils-0.4.3/imgutils/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/ocr/detect.py` & `dghs_imgutils-0.4.3/imgutils/ocr/detect.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/ocr/entry.py` & `dghs_imgutils-0.4.3/imgutils/ocr/entry.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/ocr/recognize.py` & `dghs_imgutils-0.4.3/imgutils/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/operate/align.py` & `dghs_imgutils-0.4.3/imgutils/operate/align.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/operate/censor_.py` & `dghs_imgutils-0.4.3/imgutils/operate/censor_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/operate/emoji_censor.png` & `dghs_imgutils-0.4.3/imgutils/operate/emoji_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/operate/heart_censor.png` & `dghs_imgutils-0.4.3/imgutils/operate/heart_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/operate/imgcensor.py` & `dghs_imgutils-0.4.3/imgutils/operate/imgcensor.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/operate/smile_censor.png` & `dghs_imgutils-0.4.3/imgutils/operate/smile_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/operate/squeeze.py` & `dghs_imgutils-0.4.3/imgutils/operate/squeeze.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/pose/dwpose.py` & `dghs_imgutils-0.4.3/imgutils/pose/dwpose.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/pose/format.py` & `dghs_imgutils-0.4.3/imgutils/pose/format.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/pose/visual.py` & `dghs_imgutils-0.4.3/imgutils/pose/visual.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/restore/adversarial.py` & `dghs_imgutils-0.4.3/imgutils/restore/adversarial.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/restore/nafnet.py` & `dghs_imgutils-0.4.3/imgutils/restore/nafnet.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/restore/scunet.py` & `dghs_imgutils-0.4.3/imgutils/restore/scunet.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/sd/metadata.py` & `dghs_imgutils-0.4.3/imgutils/sd/metadata.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/sd/model.py` & `dghs_imgutils-0.4.3/imgutils/sd/model.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/segment/isnetis.py` & `dghs_imgutils-0.4.3/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/__init__.py` & `dghs_imgutils-0.4.3/imgutils/tagging/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/blacklist.py` & `dghs_imgutils-0.4.3/imgutils/tagging/blacklist.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/character.py` & `dghs_imgutils-0.4.3/imgutils/tagging/character.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/deepdanbooru.py` & `dghs_imgutils-0.4.3/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/format.py` & `dghs_imgutils-0.4.3/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/match.py` & `dghs_imgutils-0.4.3/imgutils/tagging/match.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/mldanbooru.py` & `dghs_imgutils-0.4.3/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/order.py` & `dghs_imgutils-0.4.3/imgutils/tagging/order.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/overlap.py` & `dghs_imgutils-0.4.3/imgutils/tagging/overlap.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/tagging/wd14.py` & `dghs_imgutils-0.4.3/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/utils/area.py` & `dghs_imgutils-0.4.3/imgutils/utils/area.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/utils/onnxruntime.py` & `dghs_imgutils-0.4.3/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/utils/tqdm_.py` & `dghs_imgutils-0.4.3/imgutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/aicheck.py` & `dghs_imgutils-0.4.3/imgutils/validate/aicheck.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/bangumi_char.py` & `dghs_imgutils-0.4.3/imgutils/validate/bangumi_char.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/classify.py` & `dghs_imgutils-0.4.3/imgutils/validate/classify.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/color.py` & `dghs_imgutils-0.4.3/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/completeness.py` & `dghs_imgutils-0.4.3/imgutils/validate/completeness.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/dbrating.py` & `dghs_imgutils-0.4.3/imgutils/validate/dbrating.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/monochrome.py` & `dghs_imgutils-0.4.3/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/nsfw.py` & `dghs_imgutils-0.4.3/imgutils/validate/nsfw.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/portrait.py` & `dghs_imgutils-0.4.3/imgutils/validate/portrait.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/rating.py` & `dghs_imgutils-0.4.3/imgutils/validate/rating.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/real.py` & `dghs_imgutils-0.4.3/imgutils/validate/real.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/safe.py` & `dghs_imgutils-0.4.3/imgutils/validate/safe.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/style_age.py` & `dghs_imgutils-0.4.3/imgutils/validate/style_age.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/teen.py` & `dghs_imgutils-0.4.3/imgutils/validate/teen.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/imgutils/validate/truncate.py` & `dghs_imgutils-0.4.3/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.2/setup.py` & `dghs_imgutils-0.4.3/setup.py`

 * *Files identical despite different names*

