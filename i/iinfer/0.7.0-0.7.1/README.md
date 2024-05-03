# Comparing `tmp/iinfer-0.7.0.tar.gz` & `tmp/iinfer-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iinfer-0.7.0.tar", last modified: Mon Apr 29 11:29:40 2024, max compression
+gzip compressed data, was "iinfer-0.7.1.tar", last modified: Fri May  3 09:31:47 2024, max compression
```

## Comparing `iinfer-0.7.0.tar` & `iinfer-0.7.1.tar`

### file list

```diff
@@ -1,191 +1,213 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.516207 iinfer-0.7.0/
--rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     5553 2024-04-29 11:29:40.514207 iinfer-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.843204 iinfer-0.7.0/iinfer/
--rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/__init__.py
--rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.893203 iinfer-0.7.0/iinfer/app/
--rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.0/iinfer/app/__init__.py
--rw-rw-rw-   0        0        0    49119 2024-04-28 12:19:10.000000 iinfer-0.7.0/iinfer/app/app.py
--rw-rw-rw-   0        0        0    33060 2024-04-28 13:16:47.000000 iinfer-0.7.0/iinfer/app/client.py
--rw-rw-rw-   0        0        0    13214 2024-04-28 13:45:06.000000 iinfer-0.7.0/iinfer/app/common.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.902202 iinfer-0.7.0/iinfer/app/commons/
--rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.0/iinfer/app/commons/convert.py
--rw-rw-rw-   0        0        0     7466 2024-03-30 02:49:07.000000 iinfer-0.7.0/iinfer/app/commons/module.py
--rw-rw-rw-   0        0        0     3508 2024-04-28 01:45:44.000000 iinfer-0.7.0/iinfer/app/gui.py
--rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.0/iinfer/app/injection.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.939203 iinfer-0.7.0/iinfer/app/injections/
--rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.0/iinfer/app/injections/after_cls_jadge_injection.py
--rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.0/iinfer/app/injections/after_csv_injection.py
--rw-rw-rw-   0        0        0     6515 2024-04-07 06:56:33.000000 iinfer-0.7.0/iinfer/app/injections/after_det_filter_injection.py
--rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.0/iinfer/app/injections/after_det_jadge_injection.py
--rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.0/iinfer/app/injections/after_http_injection.py
--rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.0/iinfer/app/injections/after_seg_bbox_injection.py
--rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.0/iinfer/app/injections/after_seg_filter_injection.py
--rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.0/iinfer/app/injections/before_grayimg_injection.py
--rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.7.0/iinfer/app/install.py
--rw-rw-rw-   0        0        0     4811 2024-03-10 08:54:06.000000 iinfer-0.7.0/iinfer/app/postprocess.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.984207 iinfer-0.7.0/iinfer/app/postprocesses/
--rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/app/postprocesses/cls_jadge.py
--rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.0/iinfer/app/postprocesses/csv.py
--rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_clip.py
--rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_face_store.py
--rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_filter.py
--rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_jadge.py
--rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.0/iinfer/app/postprocesses/httpreq.py
--rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.0/iinfer/app/postprocesses/seg_bbox.py
--rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.0/iinfer/app/postprocesses/seg_filter.py
--rw-rw-rw-   0        0        0     6077 2024-02-24 13:15:38.000000 iinfer-0.7.0/iinfer/app/predict.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.024206 iinfer-0.7.0/iinfer/app/predicts/
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/app/predicts/__init__.py
--rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.7.0/iinfer/app/predicts/insightface_det.py
--rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.7.0/iinfer/app/predicts/mmdet_det_YoloX.py
--rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.7.0/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.7.0/iinfer/app/predicts/mmpretrain_cls_swin.py
--rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.7.0/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
--rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.7.0/iinfer/app/predicts/mmrotate_det_ReDet.py
--rw-rw-rw-   0        0        0     5712 2024-04-05 13:16:32.000000 iinfer-0.7.0/iinfer/app/predicts/mmseg_seg_PSPNet.py
--rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.0/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
--rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
--rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_TinyYoloV3.py
--rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloV3.py
--rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX.py
--rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/app/redis.py
--rw-rw-rw-   0        0        0    51249 2024-04-29 07:04:17.000000 iinfer-0.7.0/iinfer/app/server.py
--rw-rw-rw-   0        0        0    76790 2024-04-29 10:40:51.000000 iinfer-0.7.0/iinfer/app/web.py
--rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/config.yml
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.041204 iinfer-0.7.0/iinfer/docker/
--rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.7.0/iinfer/docker/Dockerfile
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/docker/__init__.py
--rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/docker/build.sh
--rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/docker/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.787210 iinfer-0.7.0/iinfer/extensions/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.080206 iinfer-0.7.0/iinfer/extensions/injection/
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.0/iinfer/extensions/injection/after_cls_jadge_injection.json
--rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.0/iinfer/extensions/injection/after_csv_injection.json
--rw-rw-rw-   0        0        0      129 2024-04-07 04:03:58.000000 iinfer-0.7.0/iinfer/extensions/injection/after_det_filter_injection.json
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.0/iinfer/extensions/injection/after_det_jadge_injection.json
--rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.0/iinfer/extensions/injection/after_http_injection.json
--rw-rw-rw-   0        0        0      107 2024-04-07 03:43:59.000000 iinfer-0.7.0/iinfer/extensions/injection/after_seg_bbox_injection.json
--rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.0/iinfer/extensions/injection/after_seg_filter_injection.json
--rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.0/iinfer/extensions/injection/before_gray_injection.json
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.341204 iinfer-0.7.0/iinfer/licenses/
--rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
--rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
--rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
--rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
--rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
--rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
--rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
--rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
--rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
--rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
--rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
--rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
--rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
--rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
--rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
--rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
--rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
--rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
--rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
--rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
--rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
--rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
--rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
--rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
--rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
--rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
--rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
--rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
--rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
--rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/files.txt
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_client.yml
--rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_gui.yml
--rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_install.yml
--rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_postprocess.yml
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_redis.yml
--rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_server.yml
--rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.0/iinfer/logconf_web.yml
--rw-rw-rw-   0        0        0     1010 2024-04-29 10:52:21.000000 iinfer-0.7.0/iinfer/version.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.344207 iinfer-0.7.0/iinfer/web/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.793205 iinfer-0.7.0/iinfer/web/assets/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.366204 iinfer-0.7.0/iinfer/web/assets/bootstrap/
--rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
--rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
--rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
--rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.397205 iinfer-0.7.0/iinfer/web/assets/iinfer/
--rw-rw-rw-   0        0        0     5664 2024-04-23 14:00:17.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/filer_modal.js
--rw-rw-rw-   0        0        0    16723 2024-04-28 01:44:14.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/list_cmd.js
--rw-rw-rw-   0        0        0     6675 2024-04-28 01:46:33.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/list_pipe.js
--rw-rw-rw-   0        0        0     5581 2024-04-23 14:04:49.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/main.js
--rw-rw-rw-   0        0        0      439 2024-04-23 14:05:01.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/open_capture.js
--rw-rw-rw-   0        0        0      459 2024-04-23 14:05:10.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/open_output_json.js
--rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/svfiler.css
--rw-rw-rw-   0        0        0    24976 2024-04-23 14:07:35.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/svfiler.js
--rw-rw-rw-   0        0        0     1246 2024-04-23 14:07:58.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/view_raw.js
--rw-rw-rw-   0        0        0     4543 2024-04-23 14:08:58.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/view_result.js
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.401205 iinfer-0.7.0/iinfer/web/assets/jquery/
--rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery/jquery.min.3.2.0.js
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.404204 iinfer-0.7.0/iinfer/web/assets/jquery-resizable/
--rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.442206 iinfer-0.7.0/iinfer/web/assets/jquery-ui/
--rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/AUTHORS.txt
--rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.473201 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/
--rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.css
--rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.js
--rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
--rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
--rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/package.json
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.793205 iinfer-0.7.0/iinfer/web/assets/lightbox2/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.476203 iinfer-0.7.0/iinfer/web/assets/lightbox2/css/
--rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/css/lightbox.min.css
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.490207 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/
--rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/close.png
--rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/loading.gif
--rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/next.png
--rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/prev.png
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.493205 iinfer-0.7.0/iinfer/web/assets/lightbox2/js/
--rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/js/lightbox.min.js
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.795208 iinfer-0.7.0/iinfer/web/assets/tree-menu/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.496205 iinfer-0.7.0/iinfer/web/assets/tree-menu/css/
--rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/css/tree-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.508205 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/
--rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/file.png
--rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/folder-close.png
--rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/folder-open.png
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.512207 iinfer-0.7.0/iinfer/web/assets/tree-menu/js/
--rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/js/tree-menu.js
--rw-rw-rw-   0        0        0    31056 2024-04-21 10:24:46.000000 iinfer-0.7.0/iinfer/web/gui.html
-drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.858204 iinfer-0.7.0/iinfer.egg-info/
--rw-rw-rw-   0        0        0     5553 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7238 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:29:40.516207 iinfer-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     2185 2024-04-06 23:22:57.000000 iinfer-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.314041 iinfer-0.7.1/
+-rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     5553 2024-05-03 09:31:47.312451 iinfer-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.824564 iinfer-0.7.1/iinfer/
+-rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/__init__.py
+-rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.944697 iinfer-0.7.1/iinfer/app/
+-rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.1/iinfer/app/__init__.py
+-rw-rw-rw-   0        0        0    50217 2024-05-03 09:09:11.000000 iinfer-0.7.1/iinfer/app/app.py
+-rw-rw-rw-   0        0        0    34473 2024-05-03 08:22:57.000000 iinfer-0.7.1/iinfer/app/client.py
+-rw-rw-rw-   0        0        0    14034 2024-05-03 09:11:44.000000 iinfer-0.7.1/iinfer/app/common.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.955222 iinfer-0.7.1/iinfer/app/commons/
+-rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.1/iinfer/app/commons/convert.py
+-rw-rw-rw-   0        0        0     7466 2024-05-03 09:25:05.000000 iinfer-0.7.1/iinfer/app/commons/module.py
+-rw-rw-rw-   0        0        0     3613 2024-05-03 05:30:54.000000 iinfer-0.7.1/iinfer/app/gui.py
+-rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.1/iinfer/app/injection.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.117723 iinfer-0.7.1/iinfer/app/injections/
+-rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.1/iinfer/app/injections/after_cls_jadge_injection.py
+-rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.1/iinfer/app/injections/after_csv_injection.py
+-rw-rw-rw-   0        0        0     6735 2024-05-02 03:57:31.000000 iinfer-0.7.1/iinfer/app/injections/after_det_filter_injection.py
+-rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.1/iinfer/app/injections/after_det_jadge_injection.py
+-rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.1/iinfer/app/injections/after_http_injection.py
+-rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.1/iinfer/app/injections/after_seg_bbox_injection.py
+-rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.1/iinfer/app/injections/after_seg_filter_injection.py
+-rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.1/iinfer/app/injections/before_grayimg_injection.py
+-rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.7.1/iinfer/app/install.py
+-rw-rw-rw-   0        0        0     5309 2024-05-02 02:25:26.000000 iinfer-0.7.1/iinfer/app/postprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.329360 iinfer-0.7.1/iinfer/app/postprocesses/
+-rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/app/postprocesses/cls_jadge.py
+-rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.1/iinfer/app/postprocesses/csv.py
+-rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_clip.py
+-rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_face_store.py
+-rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_filter.py
+-rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_jadge.py
+-rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.1/iinfer/app/postprocesses/httpreq.py
+-rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.1/iinfer/app/postprocesses/seg_bbox.py
+-rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.1/iinfer/app/postprocesses/seg_filter.py
+-rw-rw-rw-   0        0        0     6082 2024-05-03 06:19:11.000000 iinfer-0.7.1/iinfer/app/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.407932 iinfer-0.7.1/iinfer/app/predicts/
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/app/predicts/__init__.py
+-rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.7.1/iinfer/app/predicts/insightface_det.py
+-rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.7.1/iinfer/app/predicts/mmdet_det_YoloX.py
+-rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.7.1/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.7.1/iinfer/app/predicts/mmpretrain_cls_swin.py
+-rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.7.1/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
+-rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.7.1/iinfer/app/predicts/mmrotate_det_ReDet.py
+-rw-rw-rw-   0        0        0     5712 2024-05-03 05:32:49.000000 iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_PSPNet.py
+-rw-rw-rw-   0        0        0      377 2024-05-02 14:44:28.000000 iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_San.py
+-rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
+-rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
+-rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_TinyYoloV3.py
+-rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloV3.py
+-rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX.py
+-rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/app/redis.py
+-rw-rw-rw-   0        0        0    51835 2024-05-03 06:22:29.000000 iinfer-0.7.1/iinfer/app/server.py
+-rw-rw-rw-   0        0        0    76670 2024-05-03 07:50:31.000000 iinfer-0.7.1/iinfer/app/web.py
+-rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/config.yml
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.455043 iinfer-0.7.1/iinfer/docker/
+-rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.7.1/iinfer/docker/Dockerfile
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/docker/__init__.py
+-rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/docker/build.sh
+-rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/docker/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.726621 iinfer-0.7.1/iinfer/extensions/
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.726096 iinfer-0.7.1/iinfer/extensions/configs/
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.475101 iinfer-0.7.1/iinfer/extensions/configs/mmdet/
+-rw-rw-rw-   0        0        0      273 2024-05-03 08:33:49.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     7908 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1883 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1276 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_tta.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.501672 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/
+-rw-rw-rw-   0        0        0      252 2024-05-03 08:36:21.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      253 2024-05-03 08:36:59.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      231 2024-05-03 08:35:35.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
+-rw-rw-rw-   0        0        0      236 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.557196 iinfer-0.7.1/iinfer/extensions/configs/mmseg/
+-rw-rw-rw-   0        0        0      139 2024-03-16 14:01:11.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      277 2024-03-11 12:50:08.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      299 2024-03-11 13:57:39.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0     2543 2024-05-03 02:44:50.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0     1065 2024-05-02 14:40:03.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0      614 2024-03-30 02:18:25.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      361 2024-03-30 02:17:37.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      501 2024-03-23 13:10:40.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0     1752 2024-03-23 13:24:30.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.592200 iinfer-0.7.1/iinfer/extensions/injection/
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.1/iinfer/extensions/injection/after_cls_jadge_injection.json
+-rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.1/iinfer/extensions/injection/after_csv_injection.json
+-rw-rw-rw-   0        0        0      149 2024-05-02 13:46:36.000000 iinfer-0.7.1/iinfer/extensions/injection/after_det_filter_injection.json
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.1/iinfer/extensions/injection/after_det_jadge_injection.json
+-rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.1/iinfer/extensions/injection/after_http_injection.json
+-rw-rw-rw-   0        0        0      106 2024-05-02 14:15:04.000000 iinfer-0.7.1/iinfer/extensions/injection/after_seg_bbox_injection.json
+-rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.1/iinfer/extensions/injection/after_seg_filter_injection.json
+-rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.1/iinfer/extensions/injection/before_gray_injection.json
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:46.828969 iinfer-0.7.1/iinfer/licenses/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
+-rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
+-rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
+-rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
+-rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
+-rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
+-rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
+-rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
+-rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
+-rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
+-rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
+-rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
+-rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
+-rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
+-rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
+-rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
+-rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
+-rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
+-rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
+-rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
+-rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/files.txt
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_client.yml
+-rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_gui.yml
+-rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_install.yml
+-rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_postprocess.yml
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_redis.yml
+-rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_server.yml
+-rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.1/iinfer/logconf_web.yml
+-rw-rw-rw-   0        0        0     1009 2024-05-03 09:30:13.000000 iinfer-0.7.1/iinfer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:46.839969 iinfer-0.7.1/iinfer/web/
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.735800 iinfer-0.7.1/iinfer/web/assets/
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:46.898106 iinfer-0.7.1/iinfer/web/assets/bootstrap/
+-rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
+-rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
+-rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
+-rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.017638 iinfer-0.7.1/iinfer/web/assets/iinfer/
+-rw-rw-rw-   0        0        0     5664 2024-04-23 14:00:17.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/filer_modal.js
+-rw-rw-rw-   0        0        0    16585 2024-04-30 13:36:02.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/list_cmd.js
+-rw-rw-rw-   0        0        0     6537 2024-04-30 13:37:34.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/list_pipe.js
+-rw-rw-rw-   0        0        0     5958 2024-05-01 13:45:13.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/main.js
+-rw-rw-rw-   0        0        0      421 2024-04-30 13:38:58.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/open_capture.js
+-rw-rw-rw-   0        0        0      441 2024-04-30 13:39:09.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/open_output_json.js
+-rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/svfiler.css
+-rw-rw-rw-   0        0        0    24976 2024-04-23 14:07:35.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/svfiler.js
+-rw-rw-rw-   0        0        0     1246 2024-04-23 14:07:58.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/view_raw.js
+-rw-rw-rw-   0        0        0     6154 2024-05-02 12:27:53.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/view_result.js
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.041919 iinfer-0.7.1/iinfer/web/assets/jquery/
+-rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery/jquery.min.3.2.0.js
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.049921 iinfer-0.7.1/iinfer/web/assets/jquery-resizable/
+-rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.164118 iinfer-0.7.1/iinfer/web/assets/jquery-ui/
+-rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.214746 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/
+-rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.css
+-rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.js
+-rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
+-rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
+-rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/package.json
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.734650 iinfer-0.7.1/iinfer/web/assets/lightbox2/
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.228307 iinfer-0.7.1/iinfer/web/assets/lightbox2/css/
+-rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/css/lightbox.min.css
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.259333 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/
+-rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/close.png
+-rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/loading.gif
+-rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/next.png
+-rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/prev.png
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.273337 iinfer-0.7.1/iinfer/web/assets/lightbox2/js/
+-rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/js/lightbox.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.736657 iinfer-0.7.1/iinfer/web/assets/tree-menu/
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.280334 iinfer-0.7.1/iinfer/web/assets/tree-menu/css/
+-rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/css/tree-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.297258 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/
+-rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/file.png
+-rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/folder-close.png
+-rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/folder-open.png
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.310782 iinfer-0.7.1/iinfer/web/assets/tree-menu/js/
+-rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/js/tree-menu.js
+-rw-rw-rw-   0        0        0    31056 2024-05-02 03:04:28.000000 iinfer-0.7.1/iinfer/web/gui.html
+drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.871292 iinfer-0.7.1/iinfer.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8562 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 09:31:47.314550 iinfer-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     2181 2024-05-03 08:40:54.000000 iinfer-0.7.1/setup.py
```

### Comparing `iinfer-0.7.0/LICENSE` & `iinfer-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/PKG-INFO` & `iinfer-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.0
+Version: 0.7.1
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.0/README.md` & `iinfer-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/app.py` & `iinfer-0.7.1/iinfer/app/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 
 def main(args_list:list=None):
     app = IinferApp()
     return app.main(args_list)[0]
 
 class IinferApp:
+    def __init__(self):
+        self.sv = None
+        self.cl = None
+        self.web = None
+        common.copy_sample()
+
     def main(self, args_list:list=None, file_dict:dict=dict()):
         """
         コマンドライン引数を処理し、サーバーまたはクライアントを起動し、コマンドを実行する。
         """
         parser = argparse.ArgumentParser(prog='iinfer', description='This application generates modules to set up the application system.')
         parser.add_argument('--version', help='show version infomation.', action='store_true')
         parser.add_argument('--host', help='Setting the redis server host.', default=os.environ.get('REDIS_HOST', 'localhost'))
@@ -40,16 +46,16 @@
                                     'deploy', 'deploy_list', 'undeploy', 'predict', 'predict_type_list', 'capture', # client mode
                                     'file_list', 'file_mkdir', 'file_rmdir', 'file_download', 'file_upload', 'file_remove', # client mode
                                     'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter', # postprocess mode
                                     ])
         parser.add_argument('-T','--use_track', help='Setting the multi object tracking enable for Object Detection.', action='store_true')
         parser.add_argument('--model_img_width', help='Setting the cmd deploy model_img_width.', type=int)
         parser.add_argument('--model_img_height', help='Setting the cmd deploy model_img_height.', type=int)
-        parser.add_argument('--model_file', help='Setting the cmd deploy model_file file.')
-        parser.add_argument('--model_conf_file', help='Setting the cmd deploy model_conf_file file.', action='append')
+        parser.add_argument('--model_file', help='Setting the cmd deploy model_file file path or download url.')
+        parser.add_argument('--model_conf_file', help='Setting the cmd deploy model_conf_file file path or download url.', action='append')
         parser.add_argument('--predict_type', help='Setting the cmd deploy predict_type. If Custom, custom_predict_py must be specified.',
                             choices=['Custom'] + list(common.BASE_MODELS.keys()))
         parser.add_argument('--custom_predict_py', help='Setting the cmd deploy custom_predict.py file.')
         parser.add_argument('--label_file', help='Setting the cmd deploy label_txt file.')
         parser.add_argument('--color_file', help='Setting the cmd deploy color_txt file.')
         parser.add_argument('--before_injection_type', help='Setting the cmd deploy before_injection_type.', action='append',
                             choices=list(common.BASE_BREFORE_INJECTIONS.keys()))
@@ -234,15 +240,15 @@
         install_insightface = common.getopt(opt, 'install_insightface', preval=args_dict, withset=True)
         install_tag = common.getopt(opt, 'install_tag', preval=args_dict, withset=True)
         install_use_gpu = common.getopt(opt, 'install_use_gpu', preval=args_dict, withset=True)
 
         allow_host = common.getopt(opt, 'allow_host', preval=args_dict, withset=True)
         listen_port = common.getopt(opt, 'listen_port', preval=args_dict, withset=True)
 
-        tm = time.time()
+        tm = time.perf_counter()
         ret = {"success":f"Start command. {args}"}
 
         if args.saveopt:
             if args.useopt is None:
                 msg = {"warn":f"Please specify the --useopt option."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
@@ -330,15 +336,14 @@
             logger, _ = common.load_config(mode)
             if svname is None:
                 msg = {"warn":f"Please specify the --svname option."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
             self.cl = client.Client(logger, redis_host=host, redis_port=port, redis_password=password, svname=svname)
             if cmd == 'deploy':
-                model_file = Path(model_file) if model_file is not None else None
                 if model_conf_file is not None:
                     model_conf_file = [Path(f) for f in model_conf_file if f is not None and f != '']
                 if before_injection_py is not None:
                     before_injection_py = [Path(f) for f in before_injection_py if f is not None and f != '']
                 if after_injection_py is not None:
                     after_injection_py = [Path(f) for f in after_injection_py if f is not None and f != '']
                 custom_predict_py = Path(custom_predict_py) if custom_predict_py is not None else None
@@ -384,33 +389,33 @@
                     if input_file is not None:
                         ret = self.cl.predict(name, image_file=input_file, image_type=image_type,
                                                 output_image_file=output_image, output_preview=output_preview,
                                                 nodraw=nodraw, timeout=timeout)
                         if type(ret) is list:
                             for r in ret:
                                 common.print_format(r, format, tm, output_json, output_json_append)
-                                tm = time.time()
+                                tm = time.perf_counter()
                                 output_json_append = True
                         else:
                             common.print_format(ret, format, tm, output_json, output_json_append)
                     elif stdin:
                         if image_type is None:
                             msg = {"warn":f"Please specify the --image_type option."}
                             common.print_format(msg, format, tm, output_json, output_json_append)
                             return 1, msg
                         if image_type == 'capture':
                             for line in sys.stdin:
                                 ret = self.cl.predict(name, image=line, image_type=image_type, output_image_file=output_image, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
                                 common.print_format(ret, format, tm, output_json, output_json_append)
-                                tm = time.time()
+                                tm = time.perf_counter()
                                 output_json_append = True
                         else:
                             ret = self.cl.predict(name, image=sys.stdin.buffer.read(), image_type=image_type, output_image_file=output_image, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
                             common.print_format(ret, format, tm, output_json, output_json_append)
-                            tm = time.time()
+                            tm = time.perf_counter()
                     else:
                         msg = {"warn":f"Image file or stdin is empty."}
                         common.print_format(msg, format, tm, output_json, output_json_append)
                         return 1, msg
                 finally:
                     try:
                         cv2.destroyWindow('preview')
@@ -454,16 +459,16 @@
                 common.print_format(ret, format, tm, output_json, output_json_append)
                 if 'success' not in ret:
                     return 1, ret
 
             elif cmd == 'predict_type_list':
                 type_list = [dict(predict_type=key, site=val['site'], image_width=val['image_width'], image_height=val['image_height'],
                                 required_model_conf=val['required_model_conf'], required_model_weight=val['required_model_weight']) for key,val in common.BASE_MODELS.items()]
-                type_list.append(dict(predict_type='Custom', site='Custom', image_width=None, image_height=None))
-                ret = type_list
+                type_list.append(dict(predict_type='Custom', site='Custom', image_width=None, image_height=None, required_model_conf=None, required_model_weight=None))
+                ret = dict(success=type_list)
                 common.print_format(ret, format, tm, output_json, output_json_append)
 
             elif cmd == 'capture':
                 count = 0
                 append = False
                 try:
                     for t,b64,h,w,c,fn in self.cl.capture(capture_device=capture_device, image_type=image_type,
@@ -471,15 +476,15 @@
                                         output_preview=output_preview):
                         ret = f"{t},"+b64+f",{h},{w},{c},{fn}"
                         if output_csv is not None:
                             with open(output_csv, 'a' if append else 'w', encoding="utf-8") as f:
                                 print(ret, file=f)
                                 append = True
                         else: common.print_format(ret, False, tm, None, False)
-                        tm = time.time()
+                        tm = time.perf_counter()
                         count += 1
                         if capture_count > 0 and count >= capture_count:
                             break
                 finally:
                     try:
                         cv2.destroyWindow('preview')
                     except:
@@ -488,47 +493,51 @@
             else:
                 msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
 
         elif mode == 'postprocess':
             logger, _ = common.load_config(mode)
-            def _to_proc(f, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append, output_csv=None):
+            def _to_proc(f, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append,
+                         output_image_file=None, output_csv=None):
                 try:
                     for line in f:
                         line = line.rstrip()
                         if line == "":
                             continue
                         try:
                             json_session, img_session, text_session = proc.create_session(json_connectstr, img_connectstr, text_connectstr)
-                            ret = proc.postprocess(json_session, img_session, text_session, line, timeout=timeout)
+                            ret = proc.postprocess(json_session, img_session, text_session, line, output_image_file=output_image_file, timeout=timeout)
                             if output_csv is not None:
                                 with open(output_csv, 'a' if output_json_append else 'w', encoding="utf-8") as f:
                                     txt = common.print_format(ret, format, tm, output_json, output_json_append, stdout=False)
                                     print(txt.strip(), file=f)
                             else: common.print_format(ret, format, tm, output_json, output_json_append)
                         except Exception as e:
                             msg = {"warn":f"Invalid input. {e}"}
                             common.print_format(msg, format, tm, output_json, output_json_append)
                             ret = msg
-                        tm = time.time()
+                        tm = time.perf_counter()
                         output_json_append = True
                     return ret
                 finally:
                     try:
                         cv2.destroyWindow('preview')
                     except:
                         pass
 
-            def _exec_proc(input_file, stdin, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append, output_csv=None):
+            def _exec_proc(input_file, stdin, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm,
+                           output_json, output_json_append, output_image_file=None, output_csv=None):
                 if input_file is not None:
                     with open(input_file, 'r', encoding="UTF-8") as f:
-                        ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
+                        ret = _to_proc(f, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append,
+                                       output_image_file=output_image_file, output_csv=output_csv)
                 elif stdin:
-                    ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
+                    ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append,
+                                   output_image_file=output_image_file, output_csv=output_csv)
                 else:
                     msg = {"warn":f"Image file or stdin is empty."}
                     common.print_format(msg, format, tm, output_json, output_json_append)
                     return 1, msg
                 return 0, ret
 
             if cmd == 'cls_jadge':
@@ -536,99 +545,108 @@
                     proc = cls_jadge.ClaJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
                                             ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
                                             ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
                                             nodraw=nodraw, output_preview=output_preview)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm,
+                                       output_json, output_json_append, output_image_file=output_image)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'csv':
                 try:
                     proc = csv.Csv(logger, out_headers=out_headers, noheader=noheader)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm,
+                                       None, False, output_image_file=None, output_csv=output_csv)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'det_clip':
                 try:
                     proc = det_clip.DetClip(logger, image_type=image_type, clip_margin=clip_margin)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm,
+                                       None, False, output_image_file=None, output_csv=output_csv)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'det_face_store':
                 try:
                     proc = det_face_store.DetFaceStore(logger, face_threshold=face_threshold, image_type=image_type, clip_margin=clip_margin)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, output_json, output_json_append)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm,
+                                       output_json, output_json_append, output_image_file=None)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'det_filter':
                 try:
                     proc = det_filter.DetFilter(logger, score_th=score_th, width_th=width_th, height_th=height_th, classes=classes, labels=labels, nodraw=nodraw, output_preview=output_preview)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm,
+                                       output_json, output_json_append, output_image_file=output_image)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'det_jadge':
                 try:
                     proc = det_jadge.DetJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
                                             ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
                                             ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
                                             nodraw=nodraw, output_preview=output_preview)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm,
+                                       output_json, output_json_append, output_image_file=output_image)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'httpreq':
                 try:
                     proc = httpreq.Httpreq(logger, fileup_name=fileup_name)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, None, False)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm,
+                                       None, False, output_image_file=None)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'seg_bbox':
                 try:
                     proc = seg_bbox.SegBBox(logger, del_segments=del_segments, nodraw=nodraw, nodraw_bbox=nodraw_bbox, nodraw_rbbox=nodraw_rbbox,
                                             output_preview=output_preview)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm,
+                                       output_json, output_json_append, output_image_file=output_image)
                 if code != 0:
                     return code, ret
 
             elif cmd == 'seg_filter':
                 try:
                     proc = seg_filter.SegFilter(logger, logits_th=logits_th, classes=classes, labels=labels, nodraw=nodraw, del_logits=del_logits)
                 except Exception as e:
                     common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                     return 1, msg
-                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm,
+                                       output_json, output_json_append, output_image_file=output_image)
                 if code != 0:
                     return code, ret
 
             else:
                 msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
```

### Comparing `iinfer-0.7.0/iinfer/app/client.py` & `iinfer-0.7.1/iinfer/app/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,37 +61,38 @@
             params (List[str]): コマンドのパラメータ
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             dict: Redisサーバーからの応答
         """
         try:
+            sreqtime = time.perf_counter()
             self.check_server()
             reskey = common.random_string()
             self.redis_cli.rpush(key, f"{cmd} {reskey} {' '.join([str(p) for p in params])}")
             self.is_running = True
             stime = time.time()
             while self.is_running:
                 ctime = time.time()
                 if ctime - stime > timeout:
                     raise Exception(f"Response timed out.")
                 res = self.redis_cli.blpop([reskey], timeout=1)
                 if res is None or len(res) <= 0:
                     time.sleep(1)
                     continue
-                return self._response(reskey, res)
+                return self._response(reskey, res, sreqtime)
             raise KeyboardInterrupt(f"Stop command.")
         except KeyboardInterrupt as e:
-            self.logger.error(f"Stop command. cmd={cmd}, params={params}", exc_info=True)
-            return {"error": f"Stop command. cmd={cmd}, params={params}"}
+            self.logger.error(f"Stop command. cmd={cmd}", exc_info=True)
+            return {"error": f"Stop command. cmd={cmd}"}
         except Exception as e:
-            self.logger.error(f"fail to execute command. cmd={cmd}, params={params}, msg={e}", exc_info=True)
-            return {"error": f"fail to execute command. cmd={cmd}, params={params}, msg={e}"}
+            self.logger.error(f"fail to execute command. cmd={cmd}, msg={e}", exc_info=True)
+            return {"error": f"fail to execute command. cmd={cmd}, msg={e}"}
 
-    def _response(self, reskey:str, res_msg:List[str]):
+    def _response(self, reskey:str, res_msg:List[str], sreqtime:float):
         """
         Redisサーバーからの応答を解析する
 
         Args:
             reskey (str): Redisサーバーからの応答のキー
             res_msg (List[str]): Redisサーバーからの応答
 
@@ -112,28 +113,34 @@
             msg_json["output_image"] = "binary"
         if "error" in res_json:
             self.logger.error(str(msg_json))
         if "warn" in res_json:
             self.logger.warn(str(msg_json))
         if "success" in res_json:
             self.logger.info(str(msg_json))
+            if type(res_json["success"]) is not dict:
+                res_json["success"] = dict(data=res_json["success"])
+            if "performance" not in res_json["success"]:
+                res_json["success"]["performance"] = []
+            performance = res_json["success"]["performance"]
+            performance.append(dict(key="cl_svreqest", val=f"{time.perf_counter()-sreqtime:.3f}s"))
         return res_json
 
-    def deploy(self, name:str, model_img_width:int, model_img_height:int, model_file:Path, model_conf_file:List[Path], predict_type:str,
+    def deploy(self, name:str, model_img_width:int, model_img_height:int, model_file:str, model_conf_file:List[Path], predict_type:str,
                custom_predict_py:Path, label_file:Path, color_file:Path,
                before_injection_conf:Path, before_injection_type:List[str], before_injection_py:List[Path],
                after_injection_conf:Path, after_injection_type:List[str], after_injection_py:List[Path], overwrite:bool, timeout:int = 60):
         """
         モデルをRedisサーバーにデプロイする
 
         Args:
             name (str): モデル名
             model_img_width (int): 画像の幅
             model_img_height (int): 画像の高さ
-            model_file (Path): モデルファイルのパス
+            model_file (str): モデルファイルのパス又はURL
             model_conf_file (List[Path]): モデル設定ファイルのパス
             predict_type (str): 推論方法のタイプ
             custom_predict_py (Path): 推論スクリプトのパス
             label_file (Path): ラベルファイルのパス
             color_file (Path): 色ファイルのパス
             before_injection_conf (Path): 推論前処理設定ファイルのパス
             before_injection_type (List[str]): 推論前処理タイプ
@@ -203,15 +210,16 @@
         if not ret: return label_file_b64
         ret, color_file_b64 = _conf_b64("color_file", color_file)
         if not ret: return color_file_b64
         ret, before_injection_conf_b64 = _conf_b64("before_injection_conf", before_injection_conf)
         if not ret: return before_injection_conf_b64
         ret, after_injection_conf_b64 = _conf_b64("after_injection_conf", after_injection_conf)
         if not ret: return after_injection_conf_b64
-        if model_file is not None:
+        if model_file is not None and not model_file.startswith("http"):
+            model_file = Path(model_file)
             if model_file.exists():
                 with open(model_file, "rb") as mf:
                     model_bytes_b64 = base64.b64encode(mf.read()).decode('utf-8')
             else:
                 self.logger.error(f"model_file {model_file} does not exist")
                 return {"error": f"model_file {model_file} does not exist"}
         else:
@@ -232,15 +240,16 @@
         ret, model_conf_file_name, model_conf_bytes_b64 = _name_b64("model_conf_file", model_conf_file)
         if not ret: return model_conf_file_name
         ret, before_injection_py_name, before_injection_py_b64 = _name_b64("before_injection_py", before_injection_py)
         if not ret: return before_injection_py_name
         ret, after_injection_py_name, after_injection_py_b64 = _name_b64("after_injection_py", after_injection_py)
         if not ret: return after_injection_py_name
         res_json = self._proc(self.svname, 'deploy', [name, str(model_img_width), str(model_img_height), predict_type,
-                                                   model_file.name, model_bytes_b64, model_conf_file_name, model_conf_bytes_b64,
+                                                   model_file.name if isinstance(model_file, Path) else model_file, model_bytes_b64,
+                                                   model_conf_file_name, model_conf_bytes_b64,
                                                    custom_predict_py_b64, label_file_b64, color_file_b64,
                                                    before_injection_conf_b64, before_injection_type, before_injection_py_name, before_injection_py_b64,
                                                    after_injection_conf_b64, after_injection_type, after_injection_py_name, after_injection_py_b64, overwrite], timeout=timeout)
         return res_json
 
     def deploy_list(self, timeout:int = 60):
         """
@@ -322,42 +331,44 @@
         return res_json
 
 
     def stop_server(self, timeout:int = 60):
         res_json = self._proc(self.svname, 'stop_server', [], timeout=timeout)
         return res_json
 
-    def predict(self, name:str, image = None, image_file = None, image_file_enable:bool=True, image_type:str = 'jpeg', output_image_file:Path = None, output_preview:bool=False, nodraw:bool=False, timeout:int = 60):
+    def predict(self, name:str, image = None, image_file = None, image_file_enable:bool=True, image_type:str = 'jpeg', output_image_file:str = None, output_preview:bool=False, nodraw:bool=False, timeout:int = 60):
         """
         画像をRedisサーバーに送信し、推論結果を取得する
 
         Args:
             name (str): モデル名
             image (np.ndarray | bytes, optional): 画像データ. Defaults to None. np.ndarray型の場合はデコードしない(RGBであること).
             image_file (str|file-like object, optional): 画像ファイルのパス. Defaults to None.
             image_file_enable (bool, optional): 画像ファイルを使用するかどうか. Defaults to True. image_fileがNoneでなく、このパラメーターがTrueの場合はimage_fileを使用する.
             image_type (str, optional): 画像の形式. Defaults to 'jpeg'.
-            output_image_file (Path, optional): 予測結果の画像ファイルのパス. Defaults to None.
+            output_image_file (str, optional): 予測結果の画像ファイルのパス. Defaults to None.
             output_preview (bool, optional): 予測結果の画像をプレビューするかどうか. Defaults to False.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             dict: Redisサーバーからの応答
         """
+        spredtime = time.perf_counter()
         if self.password is None or self.password == "":
             self.logger.error(f"password is empty.")
             return {"error": f"password is empty."}
         if name is None or name == "":
             self.logger.error(f"name is empty.")
             return {"error": f"name is empty."}
         if image is None and image_file is None:
             self.logger.error(f"image and image_file is empty.")
             return {"error": f"image and image_file is empty."}
         npy_b64 = None
+        simgloadtime = time.perf_counter()
         if image_file is not None and image_file_enable:
             if type(image_file) == str:
                 if not Path(image_file).exists():
                     self.logger.error(f"Not found image_file. {image_file}.")
                     return {"error": f"Not found image_file. {image_file}."}
             if image_type == 'jpeg' or image_type == 'png' or image_type == 'bmp':
                 f = None
@@ -451,18 +462,19 @@
                 image_file_enable = False
             else:
                 self.logger.error(f"image_type is invalid. {image_type}.")
                 return {"error": f"image_type is invalid. {image_type}."}
 
         npy_b64 = convert.npy2b64str(img_npy)
         #img_npy2 = np.frombuffer(base64.b64decode(npy_b64), dtype='uint8').reshape(img_npy.shape)
-
+        eimgloadtime = time.perf_counter()
         res_json = self._proc(self.svname, 'predict',
                               [name, npy_b64, str(nodraw), str(img_npy.shape[0]), str(img_npy.shape[1]),
                                str(img_npy.shape[2] if len(img_npy.shape) > 2 else '-1'), image_file], timeout=timeout)
+        soutputtime = time.perf_counter()
         if "output_image" in res_json and "output_image_shape" in res_json:
             #byteio = BytesIO(base64.b64decode(res_json["output_image"]))
             #img_npy = np.load(byteio)
             img_npy = convert.b64str2npy(res_json["output_image"], res_json["output_image_shape"])
             if output_image_file is not None:
                 exp = Path(output_image_file).suffix
                 exp = exp[1:] if exp[0] == '.' else exp
@@ -470,14 +482,23 @@
             if output_preview:
                 # RGB画像をBGR画像に変換
                 try:
                     cv2.imshow('preview', convert.bgr2rgb(img_npy))
                     cv2.waitKey(1)
                 except KeyboardInterrupt:
                     pass
+        eoutputtime = time.perf_counter()
+        epredtime = time.perf_counter()
+        if "success" in res_json:
+            if "performance" not in res_json["success"]:
+                res_json["success"]["performance"] = []
+            performance = res_json["success"]["performance"]
+            performance.append(dict(key="cl_imgload", val=f"{eimgloadtime-simgloadtime:.3f}s"))
+            performance.append(dict(key="cl_output", val=f"{eoutputtime-soutputtime:.3f}s"))
+            performance.append(dict(key="cl_pred", val=f"{epredtime-spredtime:.3f}s"))
         return res_json
     
     def file_list(self, svpath:str, timeout:int = 60):
         """
         サーバー上のファイルリストを取得する
 
         Args:
@@ -594,20 +615,21 @@
             capture_frame_height (int): キャプチャするビデオのフレーム高さ, by default None
             capture_fps (int): キャプチャするビデオのフレームレート, by default 10
             output_preview (bool, optional): 予測結果の画像をプレビューするかどうか. Defaults to False.
         """
         if capture_device.isdecimal():
             capture_device = int(capture_device)
         cap = cv2.VideoCapture(capture_device)
+        cap.set(cv2.CAP_PROP_BUFFERSIZE, 0)
+        cap.set(cv2.CAP_PROP_FPS, 30)
+        cap.set(cv2.CAP_PROP_FOURCC, cv2.VideoWriter_fourcc('H', '2', '6', '4'))
         if capture_frame_width is not None:
             cap.set(cv2.CAP_PROP_FRAME_WIDTH, capture_frame_width)
         if capture_frame_height is not None:
             cap.set(cv2.CAP_PROP_FRAME_HEIGHT, capture_frame_height)
-        if capture_fps is not None:
-            cap.set(cv2.CAP_PROP_FPS, capture_fps)
         try:
             interval = float(1 / capture_fps)
             self.is_running = True
             while self.is_running:
                 start = time.perf_counter()
                 ret, frame = cap.read()
                 output_image_name = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
```

### Comparing `iinfer-0.7.0/iinfer/app/common.py` & `iinfer-0.7.1/iinfer/app/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 import tempfile
 import time
 import yaml
 
 APP_ID = 'iinfer'
 HOME_DIR = Path(os.path.expanduser("~"))
 
+def copy_sample(dst:Path=Path.cwd()/'sample'):
+    if dst.exists():
+        return
+    src = Path(__file__).parent.parent / 'extensions'
+    shutil.copytree(src, dst)
+
 def load_config(mode:str) -> Tuple[logging.Logger, dict]:
     """
     指定されたモードのロガーと設定を読み込みます。
 
     Args:
         mode (str): モード名
 
@@ -196,29 +202,38 @@
         stdout (bool, optional): 標準出力に出力するかどうか. Defaults to True.
         tablefmt (str, optional): テーブルのフォーマット. Defaults to 'github'.
     Returns:
         str: 生成された文字列
     """
     txt = ''
     if format:
-        if 'success' in data and type(data['success']) == list:
-            txt = tabulate(data['success'], headers='keys', tablefmt=tablefmt)
-        elif 'success' in data and type(data['success']) == dict:
-            txt = tabulate([data['success']], headers='keys', tablefmt=tablefmt)
+        if 'success' in data:
+            data = data['success']['data'] if 'data' in data['success'] else data['success']
+            if type(data) == list:
+                txt = tabulate(data, headers='keys', tablefmt=tablefmt)
+            elif type(data) == dict:
+                txt = tabulate([data], headers='keys', tablefmt=tablefmt)
+            else:
+                txt = str(data)
         elif type(data) == list:
             txt = tabulate(data, headers='keys', tablefmt=tablefmt)
         else:
             txt = tabulate([data], headers='keys', tablefmt=tablefmt)
         if stdout:
             try:
                 print(txt)
-                print(f"{time.time() - tm:.03f} seconds.")
+                print(f"{time.perf_counter() - tm:.03f}s.")
             except BrokenPipeError:
                 pass
     else:
+        if 'success' in data and type(data['success']) == dict:
+            if "performance" not in data["success"]:
+                data["success"]["performance"] = []
+            performance = data["success"]["performance"]
+            performance.append(dict(key="app_proc", val=f"{time.perf_counter() - tm:.03f}s"))
         try:
             if type(data) == dict:
                 txt = json.dumps(data, default=default_json_enc, ensure_ascii=False)
             else:
                 txt = data
         except:
             txt = data
@@ -310,38 +325,41 @@
         b = np.where(m, color[2], 0).astype(np.uint8)
         mask = cv2.merge([r, g, b])
         masked_image = cv2.addWeighted(masked_image, 1, mask[0], 1, 0)
     img_npy = cv2.addWeighted(img_npy, 0.5, masked_image, 0.5, 0)
     img_npy = cv2.cvtColor(img_npy, cv2.COLOR_BGR2RGB)
     return img_npy
 
-def draw_boxes(image:Image.Image, boxes:List[List[float]], scores:List[float], classes:List[int], ids:List[str]=None, labels:List[str]=None, colors:List[Tuple[int]]=None,
+def draw_boxes(image:Image.Image, boxes:List[List[float]], scores:List[float], classes:List[int], ids:List[str]=None,
+               labels:List[str]=None, colors:List[Tuple[int]]=None, tracks:List[int]=None,
                nodraw:bool=False, nolookup:bool=False) -> Tuple[Image.Image, List[str]]:
     """
     画像にバウンディングボックスを描画します。
 
     Args:
         image (Image.Image): 描画する画像
         boxes (List[List[float]]): バウンディングボックスの座標リスト
         scores (List[float]): 各バウンディングボックスのスコアリスト
         classes (List[int]): 各バウンディングボックスのクラスリスト
         ids (List[str]): 各バウンディングボックスのIDリスト
         labels (List[str], optional): クラスのラベルリスト. Defaults to None.
         colors (List[Tuple[int]], optional): クラスごとの色のリスト. Defaults to None.
+        tracks (List[int], optional): トラックIDリスト. Defaults to None.
         nodraw (bool, optional): 描画しない場合はTrue. Defaults to False.
         nolookup (bool, optional): ラベル及び色をクラスIDから取得しない場合はTrue. Defaults to False.
 
     Returns:
         Image: バウンディングボックスが描画された画像
         List[str]: 各バウンディングボックスのラベルリスト
     """
     draw = ImageDraw.Draw(image)
     ids = ids if ids is not None else [None] * len(boxes)
+    tracks = tracks if tracks is not None else [None] * len(boxes)
     output_labels = []
-    for i, (box, score, cl, id) in enumerate(zip(boxes, scores, classes, ids)):
+    for i, (box, score, cl, id, trc) in enumerate(zip(boxes, scores, classes, ids, tracks)):
         y1, x1, y2, x2 = box
         x1 = max(0, np.floor(x1 + 0.5).astype(int))
         y1 = max(0, np.floor(y1 + 0.5).astype(int))
         x2 = min(image.width, np.floor(x2 + 0.5).astype(int))
         y2 = min(image.height, np.floor(y2 + 0.5).astype(int))
         if not nolookup:
             color = colors[int(cl)] if colors is not None and len(colors) > cl else make_color(str(int(cl)))
@@ -350,15 +368,15 @@
             color = colors[i] if colors is not None and len(colors) > i else make_color(str(int(cl)))
             label = str(labels[i]) if labels is not None and len(labels) > i else None
         if not nodraw:
             if x2 - x1 > 0 and y2 - y1 > 0:
                 draw.rectangle(((x1, y1), (x2, y2)), outline=color)
                 if label is not None:
                     draw.rectangle(((x1, y1), (x2, y1+10)), outline=color, fill=color)
-                    draw.text((x1, y1), label, tuple([int(255-c) for c in color]))
+                    draw.text((x1, y1), f"{label}:{score}", tuple([int(255-c) for c in color]))
         output_labels.append(label)
 
     return image, output_labels
 
 def make_color(idstr:str) -> Tuple[int]:
     if len(idstr) < 3:
         idstr = idstr.zfill(3)
```

### Comparing `iinfer-0.7.0/iinfer/app/commons/convert.py` & `iinfer-0.7.1/iinfer/app/commons/convert.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/commons/module.py` & `iinfer-0.7.1/iinfer/app/commons/module.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/gui.py` & `iinfer-0.7.1/iinfer/app/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,12 +114,15 @@
     
     def callback_return_cmd_exec_func(self, title, output:dict):
         eel.js_return_cmd_exec_func(title, output)
 
     def callback_return_pipe_exec_func(self, title, output):
         eel.js_return_pipe_exec_func(title, output)
 
+    def callback_return_stream_log_func(self, output):
+        eel.js_return_stream_log_func(output)
+
     def stop(self, route, websockets):
         self.bbforce_cmd()
         self.logger.info(f"Stop eel web. {route}")
         exit(0)
```

### Comparing `iinfer-0.7.0/iinfer/app/injection.py` & `iinfer-0.7.1/iinfer/app/injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/injections/after_cls_jadge_injection.py` & `iinfer-0.7.1/iinfer/app/injections/after_cls_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/injections/after_csv_injection.py` & `iinfer-0.7.1/iinfer/app/injections/after_csv_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/injections/after_det_filter_injection.py` & `iinfer-0.7.1/iinfer/app/injections/after_det_filter_injection.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,44 +74,47 @@
         labels = self.get_config('labels', [])
 
         if 'success' not in outputs or type(outputs['success']) != dict:
             raise Exception('Invalid outputs. outputs[\'success\'] must be dict.')
         data = outputs['success']
         if 'output_scores' not in data or 'output_classes' not in data:
             raise Exception('Invalid outputs. outputs[\'success\'][\'output_scores\'] and outputs[\'success\'][\'output_classes\'] must be set.')
-        output_boxes = []
+        output_ids = []
         output_scores = []
         output_classes = []
         output_labels = []
+        output_boxes = []
         output_tracks = []
         for i, score in enumerate(data['output_scores']):
             if score < score_th:
                 continue
             width = data['output_boxes'][i][2] - data['output_boxes'][i][0]
             height = data['output_boxes'][i][3] - data['output_boxes'][i][1]
             if width < width_th or height < height_th:
                 continue
             if classes is not None and len(classes) > 0 and 'output_classes' in data:
                 if data['output_classes'][i] not in classes:
                     continue
             if labels is not None and len(labels) > 0 and 'output_labels' in data:
                 if data['output_labels'][i] not in labels:
                     continue
-            output_boxes.append(data['output_boxes'][i])
+            output_ids.append(data['output_ids'][i])
             output_scores.append(score)
             output_classes.append(data['output_classes'][i])
             if 'output_labels' in data:
                 output_labels.append(data['output_labels'][i])
+            output_boxes.append(data['output_boxes'][i])
             if 'output_tracks' in data:
                 output_tracks.append(data['output_tracks'][i])
-        data['output_boxes'] = output_boxes
+        data['output_ids'] = output_ids
         data['output_scores'] = output_scores
         data['output_classes'] = output_classes
         if 'output_labels' in data:
             data['output_labels'] = output_labels
+        data['output_boxes'] = output_boxes
         if 'output_tracks' in data:
             data['output_tracks'] = output_tracks
 
         return outputs
 
     def post_img(self, outputs:Dict[str, Any], output_image:Image.Image) -> Image.Image:
         """
@@ -124,13 +127,14 @@
         """
         if 'success' not in outputs or type(outputs['success']) != dict:
             raise Exception(outputs, 'Invalid outputs. outputs[\'success\'] must be dict.')
 
         nodraw = self.get_config('nodraw', False)
 
         data = outputs['success']
+        output_ids = data["output_ids"] if "output_ids" in data else None
         output_labels = data["output_labels"] if "output_labels" in data else None
-        output_tracks = data["output_tracks"] if "output_tracks" in data else None
+        output_tracks = data["output_tracks"] if "output_tracks" in data else output_ids
         image, output_labels = common.draw_boxes(output_image, data["output_boxes"], data["output_scores"], data["output_classes"],
-                                                 ids=output_labels, labels=output_tracks, nodraw=nodraw, nolookup=True)
+                                                 ids=output_ids, labels=output_labels, tracks=output_tracks, nodraw=nodraw, nolookup=True)
 
         return image
```

### Comparing `iinfer-0.7.0/iinfer/app/injections/after_det_jadge_injection.py` & `iinfer-0.7.1/iinfer/app/injections/after_det_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/injections/after_http_injection.py` & `iinfer-0.7.1/iinfer/app/injections/after_http_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/injections/after_seg_bbox_injection.py` & `iinfer-0.7.1/iinfer/app/injections/after_seg_bbox_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/injections/after_seg_filter_injection.py` & `iinfer-0.7.1/iinfer/app/injections/after_seg_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/injections/before_grayimg_injection.py` & `iinfer-0.7.1/iinfer/app/injections/before_grayimg_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/install.py` & `iinfer-0.7.1/iinfer/app/install.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocess.py` & `iinfer-0.7.1/iinfer/app/postprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from iinfer.app.commons import convert
+from pathlib import Path
 from PIL import Image
 from typing import Dict, Any
 import logging
 import json
 
 class Postprocess(object):
     def __init__(self, logger:logging.Logger):
@@ -11,23 +12,24 @@
         後処理クラスはこのクラスを継承してください。
         
         Args:
             logger (logging.Logger): ロガー
         """
         self.logger = logger
 
-    def postprocess(self, json_session, img_session, text_session, res_str:str, timeout:int=60) -> Dict[str, Any]:
+    def postprocess(self, json_session, img_session, text_session, res_str:str, output_image_file:str=None, timeout:int=60) -> Dict[str, Any]:
             """
             ポストプロセスを実行します。
 
             Args:
                 json_session (任意): JSONセッション
                 img_session (任意): 画像セッション
                 text_session (任意): テキストセッション
                 res_str (str): 推論結果の文字列
+                output_image_file (str, optional): 出力画像ファイル名。デフォルトはNone。
                 timeout (int, optional): タイムアウト時間（秒）。デフォルトは60。
 
             Returns:
                 Dict[str, Any]: 処理結果(処理後の画像含む)
             """
             if text_session is not None:
                 result = self.post_text(text_session, res_str)
@@ -44,15 +46,20 @@
                 result = self.post_json(json_session, outputs, output_image)
 
                 if img_session is not None:
                     if type(result) == dict and output_image is not None:
                         output_image = self.post_img(img_session, result, output_image)
                         output_image_npy = convert.img2npy(output_image)
                         output_image_b64 = convert.npy2b64str(output_image_npy)
+                        if output_image_file is not None:
+                            exp = Path(output_image_file).suffix
+                            exp = exp[1:] if exp[0] == '.' else exp
+                            convert.npy2imgfile(output_image_npy, output_image_file=output_image_file, image_type=exp)
                         return dict(success=result, output_image=output_image_b64, output_image_shape=output_image_npy.shape, output_image_name=outputs["output_image_name"])
+                    
             if type(result) == str:
                 return result
             return dict(success=result)
 
     def create_session(self, json_connectstr:str, img_connectstr:str, text_connectstr:str):
         """
         後処理のセッションを作成する関数です。
```

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/cls_jadge.py` & `iinfer-0.7.1/iinfer/app/postprocesses/cls_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/csv.py` & `iinfer-0.7.1/iinfer/app/postprocesses/csv.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/det_clip.py` & `iinfer-0.7.1/iinfer/app/postprocesses/det_clip.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/det_face_store.py` & `iinfer-0.7.1/iinfer/app/postprocesses/det_face_store.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/det_filter.py` & `iinfer-0.7.1/iinfer/app/postprocesses/det_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/det_jadge.py` & `iinfer-0.7.1/iinfer/app/postprocesses/det_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/httpreq.py` & `iinfer-0.7.1/iinfer/app/postprocesses/httpreq.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/seg_bbox.py` & `iinfer-0.7.1/iinfer/app/postprocesses/seg_bbox.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/postprocesses/seg_filter.py` & `iinfer-0.7.1/iinfer/app/postprocesses/seg_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predict.py` & `iinfer-0.7.1/iinfer/app/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 from PIL import Image
 from typing import List, Tuple, Dict, Any
 import logging
 
+
 class Predict(object):
     def __init__(self, logger:logging.Logger) -> None:
         """
         このクラスのインスタンスを初期化します。
         継承時は、このコンストラクタを呼び出すようにしてください。
             super().__init__(logger)
         Args:
@@ -126,12 +127,13 @@
             gpu_id (int, optional): GPU ID. Defaults to None.
         Returns:
             bool: GPUが利用可能かどうか
         """
         try:
             import torch
             ret = torch.cuda.is_available()
-            self.logger.info(f'GPU is available: True')
+            self.logger.info(f'GPU is available: {ret}')
             return ret
         except:
             self.logger.info(f'GPU is available: False')
             return False
+
```

### Comparing `iinfer-0.7.0/iinfer/app/predicts/insightface_det.py` & `iinfer-0.7.1/iinfer/app/predicts/insightface_det.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/mmdet_det_YoloX.py` & `iinfer-0.7.1/iinfer/app/predicts/mmdet_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/mmpretrain_cls_swin.py` & `iinfer-0.7.1/iinfer/app/predicts/mmpretrain_cls_swin.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/mmrotate_det_ReDet.py` & `iinfer-0.7.1/iinfer/app/predicts/mmrotate_det_ReDet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/mmseg_seg_PSPNet.py` & `iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_PSPNet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py` & `iinfer-0.7.1/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/onnx_det_TinyYoloV3.py` & `iinfer-0.7.1/iinfer/app/predicts/onnx_det_TinyYoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloV3.py` & `iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX.py` & `iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX_Lite.py` & `iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX_Lite.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/redis.py` & `iinfer-0.7.1/iinfer/app/redis.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/app/server.py` & `iinfer-0.7.1/iinfer/app/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import datetime
 import logging
 import json
 import numpy as np
 import redis
 import shutil
 import time
+import urllib
 
 
 class Server(object):
     RESP_SCCESS:int = 0
     RESP_WARN:int = 1
     RESP_ERROR:int = 2
     def __init__(self, data_dir: Path, logger: logging.Logger, redis_host: str = "localhost", redis_port: int = 6379, redis_password: str = None, svname: str = 'server'):
@@ -322,14 +323,18 @@
             after_injection_bin (List[bytes]): 推論後処理のPythonスクリプト
             overwrite (bool): 上書きするかどうか
         """
         if name is None or name == "":
             self.logger.warn(f"Name is empty.")
             self.responce(reskey, {"warn": f"Name is empty."})
             return self.RESP_WARN
+        if model_file is None or model_file == "":
+            self.logger.warn(f"model_file is empty.")
+            self.responce(reskey, {"warn": f"model_file is empty."})
+            return self.RESP_WARN
         if model_img_width is None or model_img_width <= 0:
             self.logger.warn(f"Image width is invalid.")
             self.responce(reskey, {"warn": f"Image width is invalid."})
             return self.RESP_WARN
         if model_img_height is None or model_img_height <= 0:
             self.logger.warn(f"Image height is invalid.")
             self.responce(reskey, {"warn": f"Image height is invalid."})
@@ -360,18 +365,23 @@
                 return False, None
             file = deploy_dir / file
             with open(file, "wb") as f:
                 f.write(data)
                 self.logger.info(f"Save {file} to {str(deploy_dir)}")
             return True, file
 
-        if common.BASE_MODELS[predict_type]['required_model_weight']==True and (model_file is None or model_bin is None):
-            self.logger.warn(f"model_file is None.")
-            self.responce(reskey, {"warn": f"model_file is None."})
-            return self.RESP_WARN
+        if model_file.startswith("http") and (model_bin is None or model_bin == ''):
+            model_path = deploy_dir / urllib.parse.urlparse(model_file).path.split('/')[-1]
+            if not model_path.exists():
+                self.logger.info(f"Downloading. {model_file}")
+                urllib.request.urlretrieve(model_file, model_path)
+                self.logger.info(f"Save {model_path}")
+            else:
+                self.logger.info(f"Already exists. {model_path}")
+            model_file = model_path
         else:
             ret, model_file = _save_s(model_file, model_bin)
 
         ret, before_injection_conf = _save_s("before_injection_conf.json", before_injection_conf)
         ret, after_injection_conf = _save_s("after_injection_conf.json", after_injection_conf)
 
         def _save_m(name:str, files:List[str], datas:List[bytes]):
@@ -732,31 +742,31 @@
             predict_end = time.perf_counter()
             if session['tracker'] is not None:
                 if 'output_boxes' in outputs and 'output_scores' in outputs and 'output_classes' in outputs:
                     detections = [Detection(box, score, cls) for box, score, cls in zip(outputs['output_boxes'], outputs['output_scores'], outputs['output_classes'])]
                     session['tracker'].step(detections=detections)
                     tracks = session['tracker'].active_tracks()
                     outputs['output_tracks'] = [t.id for t in tracks]
-                    if image is not None:
+                    if image is not None and not nodraw:
                         image = common.draw_boxes(image, outputs['output_boxes'], outputs['output_scores'], outputs['output_classes'], ids=outputs['output_tracks'])
             tracker_end = time.perf_counter()
 
             def _after_injection(reskey:str, name:str, output:dict, output_image:Image.Image, session:dict):
                 if session['after_injections'] is not None:
                     injections:List[injection.AfterInjection] = session['after_injections']
                     for inject in injections:
                         output, output_image = inject.action(reskey, name, output, output_image, session)
                 return output, output_image
 
             def _set_perftime(output, predict_process_start, before_injections_end, predict_end, tracker_end, after_injections_end, predict_process_end):
-                performance = f"before={(before_injections_end-predict_process_start):.3f}s" \
-                              f", predict={(predict_end-before_injections_end):.3f}s" \
-                              f", track={(tracker_end-predict_end):.3f}s" \
-                              f", after={(after_injections_end-tracker_end):.3f}s" \
-                              f", process={(predict_process_end-predict_process_start):.3f}s"
+                performance = [dict(key="sv_before", val=f"{(before_injections_end-predict_process_start):.3f}s"),
+                               dict(key="sv_predict", val=f"{(predict_end-before_injections_end):.3f}s"),
+                               dict(key="sv_track", val=f"{(tracker_end-predict_end):.3f}s"),
+                               dict(key="sv_after", val=f"{(after_injections_end-tracker_end):.3f}s"),
+                               dict(key="sv_process", val=f"{(predict_process_end-predict_process_start):.3f}s")]
                 if 'success' in output:
                     output['success']['performance'] = performance
 
             if output_image is not None:
                 output = dict(success=outputs, output_image_name=output_image_name)
                 # 後処理を実行
                 output, output_image = _after_injection(reskey, name, output, output_image, session)
```

### Comparing `iinfer-0.7.0/iinfer/app/web.py` & `iinfer-0.7.1/iinfer/app/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from iinfer import version
 from iinfer.app import app, common
 from iinfer.app.commons import convert
 from pathlib import Path
 import bottle
 import datetime
 import glob
+import gevent
 import html
 import iinfer
 import io
 import json
 import logging
 import os
 import re
@@ -68,15 +69,15 @@
                     dict(opt="before_injection_type", type="str", default="", required=False, multi=True, hide=True, choise=['']+[key for key in common.BASE_BREFORE_INJECTIONS.keys()]),
                     dict(opt="before_injection_conf", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="in"),
                     dict(opt="before_injection_py", type="file", default="", required=False, multi=True, hide=True, choise=None, fileio="in"),
                     dict(opt="after_injection_type", type="str", default="", required=False, multi=True, hide=True, choise=['']+[key for key in common.BASE_AFTER_INJECTIONS.keys()]),
                     dict(opt="after_injection_conf", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="in"),
                     dict(opt="after_injection_py", type="file", default="", required=False, multi=True, hide=True, choise=None, fileio="in"),
                     dict(opt="overwrite", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False]),
-                    dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
+                    dict(opt="timeout", type="int", default="120", required=False, multi=False, hide=True, choise=None),
                     dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out"),
                     dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                     dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False]),
                     dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False])
                 ]
             elif cmd == "deploy_list":
                 return [
@@ -304,14 +305,15 @@
                     dict(opt="ext_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
                     dict(opt="ext_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
                     dict(opt="ext_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
                     dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out"),
                     dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                    dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out"),
                     dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                     dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False])
                 ]
             elif cmd == "csv":
                 return [
                     dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="in"),
                     dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
@@ -352,14 +354,15 @@
                     dict(opt="height_th", type="int", default="0", required=False, multi=False, hide=False, choise=None),
                     dict(opt="classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
                     dict(opt="labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
                     dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out"),
                     dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                    dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out"),
                     dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                     dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False])
                 ]
             elif cmd == "det_jadge":
                 return [
                     dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="in"),
                     dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
@@ -372,14 +375,15 @@
                     dict(opt="ext_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
                     dict(opt="ext_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
                     dict(opt="ext_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
                     dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out"),
                     dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                    dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out"),
                     dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                     dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False])
                 ]
             elif cmd == "httpreq":
                 return [
                     dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="in"),
                     dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
@@ -396,14 +400,15 @@
                     dict(opt="del_segments", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="nodraw_bbox", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="nodraw_rbbox", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out"),
                     dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                    dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out"),
                     dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                     dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False])
                 ]
             elif cmd == "seg_filter":
                 return [
                     dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="in"),
                     dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
@@ -411,14 +416,15 @@
                     dict(opt="classes", type="int", default="", required=False, multi=True, hide=True, choise=None),
                     dict(opt="labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
                     dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="del_logits", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                     dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out"),
                     dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                    dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="out"),
                     dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                     dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False])
                 ]
             return []
         elif mode == "redis":
             if cmd == "docker_run":
                 return [
@@ -657,15 +663,15 @@
                 self.callback_return_cmd_exec_func(title, ret)
             except:
                 if nothread:
                     return output
                 self.callback_return_cmd_exec_func(title, output)
         if nothread:
             return _exec_cmd(self.container['iinfer_app'], title, opt, True)
-        th = threading.Thread(target=_exec_cmd, args=(self.container['iinfer_app'], title, opt))
+        th = threading.Thread(target=_exec_cmd, args=(self.container['iinfer_app'], title, opt, False))
         th.start()
         return [dict(warn='start_cmd')]
     
     def callback_console_modal_log_func(self, output:dict):
         raise NotImplementedError('callback_console_modal_log_func is not implemented.')
     
     def callback_return_cmd_exec_func(self, title, output:dict):
@@ -673,15 +679,15 @@
 
     def raw_cmd(self, title:str, opt:dict):
         self.logger.info(f"raw_cmd: title={title}, opt={opt}")
         opt_list, _ = self.mk_opt_list(opt)
         if 'stdout_log' in opt: del opt['stdout_log']
         if 'capture_stdout' in opt: del opt['capture_stdout']
         curl_cmd_file = self.mk_curl_fileup(opt)
-        return [dict(type='cmdline',raw=' '.join(['iinfer']+opt_list)),
+        return [dict(type='cmdline',raw=' '.join(['python','-m','iinfer']+opt_list)),
                 dict(type='optjson',raw=json.dumps(opt, default=common.default_json_enc)),
                 dict(type='curlcmd',raw=f'curl {curl_cmd_file} http://localhost:8081/exec_cmd/{title}')]
 
     def list_tree(self, current_path):
         current_path = Path.cwd() if current_path is None or current_path=='' else Path(current_path)
         current_path = current_path if current_path.is_dir() else current_path.parent
         path_tree = {}
@@ -740,14 +746,21 @@
         if kwd is None or kwd == '':
             kwd = '*'
         paths = glob.glob(str(self.data / f"pipe-{kwd}.json"))
         return [common.loadopt(path) for path in paths]
 
     def exec_pipe(self, title, opt, nothread=False):
         self.logger.info(f"exec_pipe: title={title}, opt={opt}")
+        def to_json(o):
+            res_json = json.loads(o)
+            if 'output_image' in res_json and 'output_image_shape' in res_json:
+                img_npy = convert.b64str2npy(res_json["output_image"], res_json["output_image_shape"])
+                img_bytes = convert.npy2imgfile(img_npy, image_type='png')
+                res_json["output_image"] = convert.bytes2b64str(img_bytes)
+            return res_json
         def _exec_pipe(title, opt, container, nothread=False):
             capture_stdout = True
             for i, cmd_title in enumerate(opt['pipe_cmd']):
                 if cmd_title == '':
                     continue
                 cmd_opt = self.load_cmd(cmd_title)
                 #cmd_ref = self.get_opt_opt(cmd_opt['mode'], cmd_opt['cmd'])
@@ -758,88 +771,69 @@
                 else:
                     capture_stdout = True
                 if 'output_csv' in cmd_opt and cmd_opt['output_csv'] != '':
                     output = dict(warn=f'The "output_csv" option is not supported in pipe. ({cmd_title})')
                     if nothread: return output
                     self.callback_return_pipe_exec_func(title, output)
                     return
-                """
-                if i>0 and chk_stdin and ('stdin' not in cmd_opt or not cmd_opt['stdin']):
-                    output = dict(warn=f'The "stdin" option must be specified for the second and subsequent commands. ({cmd_title})')
-                    if nothread: return output
-                    self.callback_return_pipe_exec_func(title, output)
-                    return
-                if i>0 and chk_input_file and 'input_file' in cmd_opt and cmd_opt['input_file'] != '':
-                    output = dict(warn=f'The "input_file" option must not be specified in a second or subsequent command. ({cmd_title})')
-                    if nothread: return output
-                    self.callback_return_pipe_exec_func(title, output)
-                    return
-                """
 
             cmdline = self.raw_pipe(title, opt)[0]['raw']
             try:
                 container['pipe_proc'] = subprocess.Popen(cmdline, shell=True, text=True, encoding='utf-8', 
                                                         stdout=(subprocess.PIPE if capture_stdout else None),
                                                         stderr=(subprocess.STDOUT if capture_stdout else None))
                 output = ""
                 output_size = 0
                 while container['pipe_proc'].poll() is None:
-                    time.sleep(0.1)
+                    gevent.sleep(0.1)
                     if capture_stdout:
-                        o = container['pipe_proc'].stdout.read()
-                        output += o.strip()
-                        output_size += len(o)
-                    if output_size > self.output_size_th:
-                        o = output.split('\n')
-                        if len(o) > 0:
-                            osize = len(o[0])
-                            oidx = int(self.output_size_th / osize)
-                            if oidx > 0:
-                                output = '\n'.join(o[-oidx:])
+                        o = container['pipe_proc'].stdout.readline().strip()
+                        if 0 >= len(o):
+                            continue
+                        try:
+                            if len(o) < self.output_size_th:
+                                o = to_json(o)
+                                self.callback_return_stream_log_func(o)
                             else:
-                                output = [dict(warn=f'The captured stdout was discarded because its size was larger than {self.output_size_th} bytes.')]
-                        else:
-                            output = [dict(warn=f'The captured stdout was discarded because its size was larger than {self.output_size_th} bytes.')]
-                        output_size = len(output)
+                                o = [dict(warn=f'The captured stdout was discarded because its size was larger than {self.output_size_th} bytes.')]
+                                self.callback_return_stream_log_func(o)
+                        except:
+                            o = [dict(warn=f'<pre>{html.escape(traceback.format_exc())}</pre>')]
+                            self.callback_return_stream_log_func(o)
                 if capture_stdout:
                     container['pipe_proc'].stdout.read() # 最後のストリームは読み捨て
                 else:
                     output = [dict(warn='capture_stdout is off.')]
             except Exception as e:
                 output = [dict(warn=f'<pre>{html.escape(traceback.format_exc())}</pre>')]
             if 'stdout_log' in opt and cmd_opt['stdout_log']:
                 self.callback_console_modal_log_func(output)
             try:
-                def to_json(o):
-                    res_json = json.loads(o)
-                    if 'output_image' in res_json and 'output_image_shape' in res_json:
-                        img_npy = convert.b64str2npy(res_json["output_image"], res_json["output_image_shape"])
-                        img_bytes = convert.npy2imgfile(img_npy, image_type='png')
-                        res_json["output_image"] = convert.bytes2b64str(img_bytes)
-                    return res_json
                 try:
                     ret = [to_json(o) for o in output.split('\n') if o.strip() != '']
                 except:
                     ret = to_json(output)
                 if nothread:
                     return ret
                 self.callback_return_pipe_exec_func(title, ret)
             except:
                 if nothread:
                     return output
                 self.callback_return_pipe_exec_func(title, output)
         if nothread:
             return _exec_pipe(title, opt, self.container, True)
-        th = threading.Thread(target=_exec_pipe, args=(title, opt, self.container))
-        th.start()
+        gevent.spawn(_exec_pipe, title, opt, self.container)
         return dict(success='start_pipe')
     
     def callback_return_pipe_exec_func(self, title, output):
         raise NotImplementedError('callback_return_pipe_exec_func is not implemented.')
-        
+
+    def callback_return_stream_log_func(self, output:dict):
+        pass
+
     def raw_pipe(self, title, opt):
         self.logger.info(f"raw_pipe: title={title}, opt={opt}")
         cmdlines = []
         errormsg = []
         curl_cmd_file = ""
         for i, cmd_title in enumerate(opt['pipe_cmd']):
             if cmd_title == '':
@@ -860,15 +854,15 @@
                 if 'request_files' in opt and len(opt['request_files']) > 0:
                     for fn in opt['request_files']:
                         if fn in cmd_opt:
                             cmd_opt[fn] = opt['request_files'][fn]
                 curl_cmd_file = self.mk_curl_fileup(cmd_opt)
 
             cmd_output = self.raw_cmd(cmd_title, cmd_opt)
-            cmdlines.append(f'python -m {cmd_output[0]["raw"]}')
+            cmdlines.append(cmd_output[0]["raw"])
 
         curl_opt = json.dumps(opt, default=common.default_json_enc)
         curl_opt = curl_opt.replace('"', '\\"')
         ret = [dict(type='cmdline', raw=' | '.join(cmdlines)),
                 dict(type='curlcmd', raw=f'curl {curl_cmd_file} http://localhost:8081/exec_pipe/{title}')]
         ret += [dict(type='warn', raw=em) for em in errormsg]
         return ret
@@ -998,22 +992,24 @@
             pid = os.getpid()
             f.write(str(pid))
             self.is_running = True
             server = _WSGIRefServer(host=self.allow_host, port=self.listen_port)
             th = threading.Thread(target=bottle.run, kwargs=dict(app=app, server=server))
             th.start()
             while self.is_running:
-                time.sleep(0.01)
+                gevent.sleep(0.01)
             server.srv.shutdown()
+        Path("iinfer_web.pid").unlink(missing_ok=True)
 
     def stop(self):
         with open("iinfer_web.pid", mode="r", encoding="utf-8") as f:
             pid = f.read()
             os.kill(int(pid), signal.CTRL_C_EVENT)
             self.logger.info(f"Stop bottle web. allow_host={self.allow_host} listen_port={self.listen_port}")
+        Path("iinfer_web.pid").unlink(missing_ok=True)
 
 class _WSGIRefServer(bottle.WSGIRefServer):
     """
     runメソッドでWSGIRefServerを起動する際に、make_serverの戻り値をインスタンス変数にするためのクラス
     """
     def __init__(self, host='127.0.0.1', port=8080, **options):
         super().__init__(host, port, **options)
```

### Comparing `iinfer-0.7.0/iinfer/docker/Dockerfile` & `iinfer-0.7.1/iinfer/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt` & `iinfer-0.7.1/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/licenses/files.txt` & `iinfer-0.7.1/iinfer/licenses/files.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/logconf_client.yml` & `iinfer-0.7.1/iinfer/logconf_client.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/logconf_gui.yml` & `iinfer-0.7.1/iinfer/logconf_gui.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/logconf_install.yml` & `iinfer-0.7.1/iinfer/logconf_install.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/logconf_postprocess.yml` & `iinfer-0.7.1/iinfer/logconf_postprocess.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/logconf_redis.yml` & `iinfer-0.7.1/iinfer/logconf_redis.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/logconf_server.yml` & `iinfer-0.7.1/iinfer/logconf_server.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/logconf_web.yml` & `iinfer-0.7.1/iinfer/logconf_web.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/version.py` & `iinfer-0.7.1/iinfer/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 
-dt_now = datetime.datetime(2024, 4, 29)
+dt_now = datetime.datetime(2024, 5, 3)
 __title__ = 'iinfer (Image Inference Application)'
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 __copyright__ = f'Copyright © 2023-{dt_now.strftime("%Y")} hamacom2004jp'
 __pypiurl__ = 'https://pypi.org/project/iinfer/'
 __srcurl__ = 'https://github.com/hamacom2004jp/iinfer'
 __docurl__ = 'https://hamacom2004jp.github.io/iinfer/index.html'
 __description__ = f'{__title__} {__version__}\n' + \
                   f'{__copyright__}\n' + \
                   f'Web Site: PyPi <{__pypiurl__}>\n' + \
```

### Comparing `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js` & `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js` & `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css` & `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css` & `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/iinfer/filer_modal.js` & `iinfer-0.7.1/iinfer/web/assets/iinfer/filer_modal.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/iinfer/list_cmd.js` & `iinfer-0.7.1/iinfer/web/assets/iinfer/list_cmd.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -273,54 +273,54 @@
     // コマンドファイルの保存
     $('#cmd_save').off('click').on('click', async () => {
         cmd_modal = $('#cmd_modal');
         var [title, opt] = get_param(cmd_modal);
         if (cmd_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
-        $('#loading').removeClass('d-none');
+        show_loading();
         result = await eel.save_cmd(title, opt)();
         await list_cmd_func();
         $('.cmd_card').off('click').on('click', cmd_card_func);
         if (result['success']) alert(result['success']);
         else if (result['warn']) alert(result['warn']);
-        $('#loading').addClass('d-none');
+        hide_loading();
     });
     // コマンドファイルの削除
     $('#cmd_del').off('click').on('click', async () => {
         cmd_modal = $('#cmd_modal');
         var title = cmd_modal.find('[name="title"]').val();
-        $('#loading').removeClass('d-none');
+        show_loading();
         if (window.confirm(`delete "${title}"?`)) {
             await eel.del_cmd(title)();
             cmd_modal.modal('hide');
             await list_cmd_func();
             $('.cmd_card').off('click').on('click', cmd_card_func);
         }
-        $('#loading').addClass('d-none');
+        hide_loading();
     });
     // コマンドファイルの実行
     $('#cmd_exec').off('click').on('click', async () => {
         cmd_modal = $('#cmd_modal');
         var [title, opt] = get_param(cmd_modal);
         if (cmd_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
-        $('#loading').removeClass('d-none');
+        show_loading();
         // コマンドの実行
         eel.exec_cmd(title, opt)().then((result) => {});
     });
     // RAW表示の実行
     $('#cmd_raw').off('click').on('click', async () => {
         cmd_modal = $('#cmd_modal');
         var [title, opt] = get_param(cmd_modal);
         if (cmd_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
-        $('#loading').removeClass('d-none');
+        show_loading();
         // コマンドの実行
         eel.raw_cmd(title, opt)().then((result) => {
             view_raw_func(title, result);
-            $('#loading').addClass('d-none');
+            hide_loading();
         });
     });
 };
```

### Comparing `iinfer-0.7.0/iinfer/web/assets/iinfer/list_pipe.js` & `iinfer-0.7.1/iinfer/web/assets/iinfer/list_pipe.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -87,55 +87,55 @@
     // パイプラインファイルの保存
     $('#pipe_save').off('click').on('click', async () => {
         pipe_modal = $('#pipe_modal');
         var [title, opt] = get_param(pipe_modal);
         if (pipe_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
-        $('#loading').removeClass('d-none');
+        show_loading();
         result = await eel.save_pipe(title, opt)();
         await list_pipe_func();
         $('.pipe_card').off('click').on('click', pipe_card_func);
         if (result['success']) alert(result['success']);
         else if (result['warn']) alert(result['warn']);
-        $('#loading').addClass('d-none');
+        hide_loading();
     });
     // パイプラインファイルの削除
     $('#pipe_del').off('click').on('click', async () => {
         pipe_modal = $('#pipe_modal');
         var title = pipe_modal.find('[name="title"]').val();
-        $('#loading').removeClass('d-none');
+        show_loading();
         if (window.confirm(`delete "${title}"?`)) {
             await eel.del_pipe(title)();
             pipe_modal.modal('hide');
             await list_pipe_func();
             $('.pipe_card').off('click').on('click', pipe_card_func);
         }
-        $('#loading').addClass('d-none');
+        hide_loading();
     });
     // パイプラインファイルの実行
     $('#pipe_exec').off('click').on('click', async () => {
         pipe_modal = $('#pipe_modal');
         var [title, opt] = get_param(pipe_modal);
         if (pipe_modal.find('.row_content').find('.is-invalid').length > 0) {
             return;
         }
-        $('#loading').removeClass('d-none');
+        show_loading();
         // コマンドの実行
         $('#loading').find('.bbforce').addClass('pipe_executed');
         eel.exec_pipe(title, opt)().then((result) => {});
     });
     // RAW表示の実行
     $('#pipe_raw').off('click').on('click', async () => {
         pipe_modal = $('#pipe_modal');
         var [title, opt] = get_param(pipe_modal);
         if (pipe_modal.find('.row_content').find('.is-invalid').length > 0) {
             return;
         }
-        $('#loading').removeClass('d-none');
+        show_loading();
         // コマンドの実行
         eel.raw_pipe(title, opt)().then((result) => {
             view_raw_func(title, result);
-            $('#loading').addClass('d-none');
+            hide_loading();
         });
     });
 };
```

### Comparing `iinfer-0.7.0/iinfer/web/assets/iinfer/main.js` & `iinfer-0.7.1/iinfer/web/assets/iinfer/main.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,21 @@
 change_dark_mode = (dark_mode) => {
     html = $('html');
     if (dark_mode) html.attr('data-bs-theme', 'dark');
     else if (html.attr('data-bs-theme') == 'dark') html.removeAttr('data-bs-theme');
     else html.attr('data-bs-theme', 'dark');
 }
+show_loading = () => {
+    elem = $('#loading');
+    elem.removeClass('d-none');
+}
+hide_loading = () => {
+    elem = $('#loading');
+    elem.addClass('d-none');
+}
 $(() => {
     // ダークモード対応
     change_dark_mode(window.matchMedia('(prefers-color-scheme: dark)').matches);
     // copyright情報取得
     copyright_func = async () => {
         copyright = await eel.copyright()();
         $('.copyright').text(copyright);
@@ -87,19 +95,19 @@
     });
     $('.btn_window_stack').css('margin-left', '0px').hide();
     $('.btn_window').css('margin-left', 'auto').show();
     $('.bbforce').off('click').on('click', async () => {
         if ($('#loading').find('.bbforce').hasClass('pipe_executed') &&
             window.confirm('パイプラインでこのアクションを実行すると、guiモード自体が停止します。実行しますか？')) {
             await eel.bbforce_cmd()();
-            $('#loading').addClass('d-none');
+            hide_loading();
             window.close();
         } else if (!$('#loading').find('.bbforce').hasClass('pipe_executed')) {
             await eel.bbforce_cmd()();
-            $('#loading').addClass('d-none');
+            hide_loading();
         }
     });
 
     // disable F5 and Ctrl+R
     $(document).on('keydown', (e) => {
         if ((e.which || e.keyCode) == 116) {
             return false;
@@ -121,18 +129,26 @@
     };
     eel.expose(js_return_cmd_exec_func);
 
     function js_return_cmd_exec_func(title, result) {
         cmd_modal = $('#cmd_modal');
         cmd_modal.modal('hide');
         view_result_func(title, result);
-        $('#loading').addClass('d-none');
+        hide_loading();
     }
     eel.expose(js_return_pipe_exec_func);
 
     function js_return_pipe_exec_func(title, result) {
         pipe_modal = $('#pipe_modal');
         pipe_modal.modal('hide');
         view_result_func(title, result);
-        $('#loading').addClass('d-none');
+        hide_loading();
     }
+    eel.expose(js_return_stream_log_func);
+
+    function js_return_stream_log_func(result) {
+        size_th = 1024 * 1024 * 5;
+        view_result_func('stream log', result);
+        result_modal = $('#result_modal');
+        result_modal.find('.btn_window').click();
+    };
 });
```

### Comparing `iinfer-0.7.0/iinfer/web/assets/iinfer/svfiler.js` & `iinfer-0.7.1/iinfer/web/assets/iinfer/svfiler.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/iinfer/view_raw.js` & `iinfer-0.7.1/iinfer/web/assets/iinfer/view_raw.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/iinfer/view_result.js` & `iinfer-0.7.1/iinfer/web/assets/iinfer/view_result.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,88 +1,121 @@
+cell_chop = (val) => {
+    if (val && val.length > 150) {
+        return `${val.substring(0, 150)}...`;
+    }
+    return val;
+}
 // 実行結果をモーダルダイアログに表示
 view_result_func = (title, result) => {
-    result_modal = $('#result_modal');
+    if (!result | Array.isArray(result) && result.length <= 0) return;
+    let result_modal = $('#result_modal');
     result_modal.find('.modal-title').text(title);
     result_modal.find('.modal-body').html('');
     mk_table_func = () => {
-        table = $('<table class="table table-bordered table-hover table-sm"></table>');
-        table_head = $('<thead class="table-dark bg-dark"></thead>');
-        table_body = $('<tbody></tbody>');
+        let table = $('<table class="table table-bordered table-hover table-sm"></table>');
+        let table_head = $('<thead class="table-dark bg-dark"></thead>');
+        let table_body = $('<tbody></tbody>');
         table.append(table_head);
         table.append(table_body);
         return table;
     }
-    result_modal.find('.modal-body').append(mk_table_func());
+    let table = mk_table_func();
+    result_modal.find('.modal-body').append(table);
     // list型の結果をテーブルに変換
     list2table = (data, table_head, table_body) => {
-        $.each(data, (i, row) => {
+        Object.keys(data).forEach(i => {
+            let row = data[i];
             if (row['success'] && typeof row['success'] == "object" && !Array.isArray(row['success'])) {
                 dict2table(row['success'], i == 0 ? table_head : null, table_body, row['output_image']);
                 return;
             }
             if (typeof row == 'string' || row instanceof String) {
-                tr = $('<tr></tr>');
+                let tr = $('<tr></tr>');
+                table_body.append(tr);
+                tr.append($(`<td>${row}</td>`));
+                return;
+            }
+            if (Array.isArray(row) && row.length > 0 && typeof row[0] != "object") {
+                let tr = $('<tr></tr>');
                 table_body.append(tr);
+                val = cell_chop(JSON.stringify(row));
                 tr.append($(`<td>${row}</td>`));
                 return;
             }
-            tr = $('<tr></tr>');
+            let tr = $('<tr></tr>');
             table_body.append(tr);
-            $.each(row, (key, val) => {
+            Object.keys(row).forEach(key => {
+                let val = row[key];
                 if (i == 0) {
-                    table_head.append($(`<th scope="col">${key}</th>`));
+                    table_head.append($(`<th scope="col" style="word-break:normal">${key}</th>`));
                 }
                 if (val && val['success'] && Array.isArray(val['success'])) {
-                    tbl = mk_table_func()
-                    td = $('<td></td>');
+                    let tbl = mk_table_func()
+                    let td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
                     list2table(val['success'], tbl.find('thead'), tbl.find('tbody'));
                 } else if (val && val['success'] && typeof val['success'] == "object") {
-                    tbl = mk_table_func()
-                    td = $('<td></td>');
+                    let tbl = mk_table_func()
+                    let td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
                     dict2table(val['success'], tbl.find('thead'), tbl.find('tbody'));
                 } else if (val && Array.isArray(val) && val.length > 0 && typeof val[0] == "object") {
-                    tbl = mk_table_func()
-                    td = $('<td></td>');
+                    let tbl = mk_table_func()
+                    let td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
                     list2table(val, tbl.find('thead'), tbl.find('tbody'));
                 } else {
                     tr.append($(`<td>${val}</td>`));
                 }
             });
         });
     }
     // dict型の結果をテーブルに変換
     dict2table = (data, table_head, table_body, output_image) => {
-        tr = $('<tr></tr>');
+        let tr = $('<tr></tr>');
         if (output_image) {
-            if (table_head) table_head.append($('<th scope="col">output_image</th>'));
-            img = $('<img class="img-thumbnail">').attr('src', `data:image/png;base64,${output_image}`);
+            if (table_head) table_head.append($('<th scope="col" style="word-break:normal">output_image</th>'));
+            let img = $('<img class="img-thumbnail">').attr('src', `data:image/png;base64,${output_image}`);
             img.css('width', '100px').css('height', 'auto');
-            anchor = $(`<a href="data:image/jpeg;base64,${output_image}" data-lightbox="output_image"></a>`).append(img);
+            let anchor = $(`<a href="data:image/jpeg;base64,${output_image}" data-lightbox="output_image"></a>`).append(img);
             tr.append($('<td></td>').append(anchor));
         }
-        $.each(data, (key, val) => {
-            if (table_head) table_head.append($(`<th scope="col">${key}</th>`));
+        table_body.append(tr);
+        Object.keys(data).forEach(key => {
+            let val = data[key];
+            if (table_head) table_head.append($(`<th scope="col" style="word-break:normal">${key}</th>`));
             if (key != 'warn' && val) {
-                if (typeof value === 'object' || Array.isArray(val)) {
-                    val = JSON.stringify(val);
-                }
-                if ((typeof val === 'string' || val instanceof String) && val.length > 150) {
-                    val = `${val.substring(0, 150)}...`;
+                if (Array.isArray(val)) {
+                    if (val.length > 0 && typeof val[0] == "object") {
+                        let tbl = mk_table_func()
+                        let td = $('<td></td>');
+                        td.append(tbl);
+                        list2table(val, tbl.find('thead'), tbl.find('tbody'));
+                        val = td.html();
+                    } else {
+                        val = cell_chop(JSON.stringify(val));
+                    }
+                } else if (typeof val == "object") {
+                    let tbl = mk_table_func()
+                    let td = $('<td></td>');
+                    td.append(tbl);
+                    dict2table(val, tbl.find('thead'), tbl.find('tbody'));
+                    val = td.html();
+                } else if ((typeof val === 'string' || val instanceof String) && val.length > 150) {
+                    val = cell_chop(val);
                 }
             }
-            tr.append($(`<td>${val}</td>`));
+            tr.append($(`<td style="overflow-wrap:break-word;word-break:break-all;">${val}</td>`));
         });
-        table_body.append(tr);
     }
+    let table_head = table.find('thead')
+    let table_body = table.find('tbody')
     // 結果をテーブルに変換
     if (result['success'] && Array.isArray(result['success'])) {
         list2table(result['success'], table_head, table_body);
     } else if (result['success'] && typeof result['success'] == "object") {
         dict2table(result['success'], table_head, table_body, result['output_image']);
     } else if (Array.isArray(result)) {
         list2table(result, table_head, table_body);
```

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery/jquery.min.3.2.0.js` & `iinfer-0.7.1/iinfer/web/assets/jquery/jquery.min.3.2.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js` & `iinfer-0.7.1/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/AUTHORS.txt` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/LICENSE.txt` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.css` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.js` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/jquery-ui/package.json` & `iinfer-0.7.1/iinfer/web/assets/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/lightbox2/css/lightbox.min.css` & `iinfer-0.7.1/iinfer/web/assets/lightbox2/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/lightbox2/images/loading.gif` & `iinfer-0.7.1/iinfer/web/assets/lightbox2/images/loading.gif`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/lightbox2/images/next.png` & `iinfer-0.7.1/iinfer/web/assets/lightbox2/images/next.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/lightbox2/images/prev.png` & `iinfer-0.7.1/iinfer/web/assets/lightbox2/images/prev.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/lightbox2/js/lightbox.min.js` & `iinfer-0.7.1/iinfer/web/assets/lightbox2/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/tree-menu/css/tree-menu.css` & `iinfer-0.7.1/iinfer/web/assets/tree-menu/css/tree-menu.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/assets/tree-menu/js/tree-menu.js` & `iinfer-0.7.1/iinfer/web/assets/tree-menu/js/tree-menu.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer/web/gui.html` & `iinfer-0.7.1/iinfer/web/gui.html`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.0/iinfer.egg-info/PKG-INFO` & `iinfer-0.7.1/iinfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.0
+Version: 0.7.1
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.0/iinfer.egg-info/SOURCES.txt` & `iinfer-0.7.1/iinfer.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -53,24 +53,42 @@
 iinfer/app/predicts/insightface_det.py
 iinfer/app/predicts/mmdet_det_YoloX.py
 iinfer/app/predicts/mmdet_det_YoloX_Lite.py
 iinfer/app/predicts/mmpretrain_cls_swin.py
 iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
 iinfer/app/predicts/mmrotate_det_ReDet.py
 iinfer/app/predicts/mmseg_seg_PSPNet.py
+iinfer/app/predicts/mmseg_seg_San.py
 iinfer/app/predicts/mmseg_seg_SwinUpernet.py
 iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
 iinfer/app/predicts/onnx_det_TinyYoloV3.py
 iinfer/app/predicts/onnx_det_YoloV3.py
 iinfer/app/predicts/onnx_det_YoloX.py
 iinfer/app/predicts/onnx_det_YoloX_Lite.py
 iinfer/docker/Dockerfile
 iinfer/docker/__init__.py
 iinfer/docker/build.sh
 iinfer/docker/docker-compose.yml
+iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
+iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
+iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
+iinfer/extensions/configs/mmdet/yolox_tta.py
+iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
+iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
+iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
+iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
+iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
+iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
+iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
 iinfer/extensions/injection/after_cls_jadge_injection.json
 iinfer/extensions/injection/after_csv_injection.json
 iinfer/extensions/injection/after_det_filter_injection.json
 iinfer/extensions/injection/after_det_jadge_injection.json
 iinfer/extensions/injection/after_http_injection.json
 iinfer/extensions/injection/after_seg_bbox_injection.json
 iinfer/extensions/injection/after_seg_filter_injection.json
```

### Comparing `iinfer-0.7.0/setup.py` & `iinfer-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 PACKAGES = [
     'iinfer',
     'iinfer.app',
     'iinfer.app.commons',
     'iinfer.app.injections',
     'iinfer.app.postprocesses',
     'iinfer.app.predicts',
-    'iinfer.datasets',
     'iinfer.docker',
     'iinfer.extensions'
 ]
 KEYWORDS = 'onnxruntime predict inference image ai model'
 CLASSIFIERS=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
@@ -46,15 +45,15 @@
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 with open('README.md', 'r', encoding='utf-8') as fp:
     readme = fp.read()
 LONG_DESCRIPTION = readme
 LONG_DESCRIPTION_CONTENT_TYPE = 'text/markdown'
-RESORCE_TEXT_FILES = dict(iinfer=['*.yml', 'extensions/*', 'extensions/*/*', 'docker/*', 'datasets/**', 'licenses/**', 'web/**', 'web/*/*', 'web/*/*/*', 'web/*/*/*/*'])
+RESORCE_TEXT_FILES = dict(iinfer=['*.yml', 'extensions/*', 'extensions/*/*', 'extensions/*/*/*', 'docker/*', 'licenses/*', 'web/*', 'web/*/*', 'web/*/*/*', 'web/*/*/*/*', 'web/*/*/*/*/*'])
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESCRIPTION_CONTENT_TYPE,
     python_requires=PYTHON_REQUIRES,
```

