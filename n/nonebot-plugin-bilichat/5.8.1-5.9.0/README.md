# Comparing `tmp/nonebot_plugin_bilichat-5.8.1.tar.gz` & `tmp/nonebot_plugin_bilichat-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.8.1.tar", last modified: Tue Apr 30 06:47:25 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.9.0.tar", last modified: Fri May  3 08:18:40 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.8.1.tar` & `nonebot_plugin_bilichat-5.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    34523 2024-04-30 06:47:21.640246 nonebot_plugin_bilichat-5.8.1/LICENSE
--rw-r--r--   0        0        0    17907 2024-04-30 06:47:21.640246 nonebot_plugin_bilichat-5.8.1/README.md
--rw-r--r--   0        0        0     2718 2024-04-30 06:47:21.660246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-30 06:47:21.660246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-30 06:47:21.660246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2176 2024-04-30 06:47:21.660246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1622 2024-04-30 06:47:21.660246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2655 2024-04-30 06:47:21.660246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7996 2024-04-30 06:47:21.660246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      942 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3848 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5196 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9227 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3130 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4227 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3958 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      494 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6142 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2346 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      366 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3379 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1136 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7275 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3187 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3091 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1701 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1739 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     3988 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      552 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      809 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      532 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3030 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1016 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0      596 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/const.py
--rw-r--r--   0        0        0     1163 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      291 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-30 06:47:21.664246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     3111 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7187 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    16423 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4894 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2243 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1578 2024-04-30 06:47:21.668246 nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1647 2024-04-30 06:47:25.052243 nonebot_plugin_bilichat-5.8.1/pyproject.toml
--rw-r--r--   0        0        0    19604 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-03 08:18:36.623330 nonebot_plugin_bilichat-5.9.0/LICENSE
+-rw-r--r--   0        0        0    18173 2024-05-03 08:18:36.623330 nonebot_plugin_bilichat-5.9.0/README.md
+-rw-r--r--   0        0        0     2718 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2176 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1622 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2655 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7996 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1280 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0     3916 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3848 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5196 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9296 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3210 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     5270 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     4033 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      494 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6142 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      366 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3379 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1136 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7275 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3187 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3091 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1701 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1739 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     3988 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      552 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      809 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      532 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3030 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1016 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0      596 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/const.py
+-rw-r--r--   0        0        0     1163 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      291 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     3111 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7187 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    16423 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4894 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2243 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1578 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1647 2024-05-03 08:18:40.095334 nonebot_plugin_bilichat-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0    19870 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.9.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.8.1/LICENSE` & `nonebot_plugin_bilichat-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/README.md` & `nonebot_plugin_bilichat-5.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,15 @@
 |  bilichat_cmd_remove_sub  | list[str] |     ["退订", "取关"]     |     "unsub"命令的别名     |
 |  bilichat_cmd_check_sub   | list[str] |   ["查看", "查看订阅"]   |     "check"命令的别名     |
 |  bilichat_cmd_reset_sub   | list[str] |   ["重置", "重置配置"]   |     "reset"命令的别名     |
 |    bilichat_cmd_at_all    | list[str] | ["全体成员", "at 全体"]  |     "atall"命令的别名     |
 |   bilichat_cmd_dynamic    | list[str] | ["动态通知", "动态订阅"] |    "dynamic"命令的别名    |
 |     bilichat_cmd_live     | list[str] | ["直播通知", "直播订阅"] |     "live"命令的别名      |
 | bilichat_cmd_checkdynamic | list[str] |       ["查看动态"]       | "checkdynamic" 命令的别名 |
+|    bilichat_cmd_fetch     | list[str] | ["获取内容", "解析内容"] |    "fetch" 命令的别名     |
 | bilichat_cmd_check_login  | list[str] |     ["查看登录账号"]     |  "checklogin" 命令的别名  |
 | bilichat_cmd_login_qrcode | list[str] |       ["扫码登录"]       |   "qrlogin" 命令的别名    |
 |    bilichat_cmd_logout    | list[str] |       ["登出账号"]       |    "logout" 命令的别名    |
 
 ### 基础信息配置项
 
 |            配置项            | 类型 | 默认值 |                        说明                        |
@@ -324,14 +325,15 @@
 |    unsub     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       |         移除订阅，all 时为全移除         |
 |    check     | 无限制 |  群聊  |       UP 主的昵称或 UID，或留空        |    查看本群订阅列表或指定 UP 主的配置    |
 |    reset     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       | 重置指定 UP 主的推送配置，all 时为全重置 |
 |    atall     |  主人  |  群聊  | UP 主的昵称或 UID `全局` `动态` `直播` |           设置是否 at 全体成员           |
 |   dynamic    |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的动态通知         |
 |     live     |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的直播通知         |
 | checkdynamic | 无限制 | 无限制 |           UP 主的昵称或 UID            |       查看指定 UP 主的最新一条动态       |
+|    fetch     | 无限制 | 无限制 | 视频或动态 ID，或回复包含此内容的消息  |       解析动态包含的图片或视频直链       |
 |  checklogin  |  主人  | 无限制 |                   无                   |         查看当前已登录的全部账号         |
 |   qrlogin    |  主人  | 无限制 |                   无                   |      使用二维码登录 B 站，防止风控       |
 |    logout    |  主人  | 无限制 |               账号的 UID               |              登出指定的账号              |
 
 ## 🙏 感谢
 
 在此感谢以下开发者(项目)对本项目做出的贡献：
```

#### html2text {}

```diff
@@ -82,22 +82,24 @@
 bilichat_cmd_check_sub | list[str] | ["æ¥ç", "æ¥çè®¢é"] |
 "check"å½ä»¤çå«å | | bilichat_cmd_reset_sub | list[str] | ["éç½®",
 "éç½®éç½®"] | "reset"å½ä»¤çå«å | | bilichat_cmd_at_all | list[str] |
 ["å¨ä½æå", "at å¨ä½"] | "atall"å½ä»¤çå«å | | bilichat_cmd_dynamic
 | list[str] | ["å¨æéç¥", "å¨æè®¢é"] | "dynamic"å½ä»¤çå«å | |
 bilichat_cmd_live | list[str] | ["ç´æ­éç¥", "ç´æ­è®¢é"] |
 "live"å½ä»¤çå«å | | bilichat_cmd_checkdynamic | list[str] |
-["æ¥çå¨æ"] | "checkdynamic" å½ä»¤çå«å | | bilichat_cmd_check_login
-| list[str] | ["æ¥çç»å½è´¦å·"] | "checklogin" å½ä»¤çå«å | |
-bilichat_cmd_login_qrcode | list[str] | ["æ«ç ç»å½"] | "qrlogin"
-å½ä»¤çå«å | | bilichat_cmd_logout | list[str] | ["ç»åºè´¦å·"] |
-"logout" å½ä»¤çå«å | ### åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å |
-é»è®¤å¼ | è¯´æ | | :--------------------------: | :--: | :----: | :--------
-----------------------------------------: | | bilichat_basic_info | bool | True
-| æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str | Auto |
+["æ¥çå¨æ"] | "checkdynamic" å½ä»¤çå«å | | bilichat_cmd_fetch | list
+[str] | ["è·ååå®¹", "è§£æåå®¹"] | "fetch" å½ä»¤çå«å | |
+bilichat_cmd_check_login | list[str] | ["æ¥çç»å½è´¦å·"] | "checklogin"
+å½ä»¤çå«å | | bilichat_cmd_login_qrcode | list[str] | ["æ«ç ç»å½"] |
+"qrlogin" å½ä»¤çå«å | | bilichat_cmd_logout | list[str] |
+["ç»åºè´¦å·"] | "logout" å½ä»¤çå«å | ### åºç¡ä¿¡æ¯éç½®é¡¹ |
+éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :--------------------------: | :--:
+| :----: | :------------------------------------------------: | |
+bilichat_basic_info | bool | True | æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | |
+bilichat_basic_info_style | str | Auto |
 è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
 bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
 bilichat_reply_to_basic_info | bool | True |
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) | |
 bilichat_dynamic | bool | True | æ¯å¦å¼å¯å¨æè§£æ | |
 bilichat_dynamic_style | str | Auto |
@@ -166,29 +168,30 @@
 UIDï¼æçç©º | æ¥çæ¬ç¾¤è®¢éåè¡¨ææå® UP ä¸»çéç½® | | reset |
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UIDï¼æ `all` | éç½®æå® UP
 ä¸»çæ¨ééç½®ï¼all æ¶ä¸ºå¨éç½® | | atall | ä¸»äºº | ç¾¤è | UP
 ä¸»çæµç§°æ UID `å¨å±` `å¨æ` `ç´æ­` | è®¾ç½®æ¯å¦ at å¨ä½æå |
 | dynamic | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ¯å¦å¼å¯è¯¥ UP
 çå¨æéç¥ | | live | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID |
 æ¯å¦å¼å¯è¯¥ UP çç´æ­éç¥ | | checkdynamic | æ éå¶ | æ éå¶ |
-UP ä¸»çæµç§°æ UID | æ¥çæå® UP ä¸»çææ°ä¸æ¡å¨æ | |
-checklogin | ä¸»äºº | æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· |
-| qrlogin | ä¸»äºº | æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B
-ç«ï¼é²æ­¢é£æ§ | | logout | ä¸»äºº | æ éå¶ | è´¦å·ç UID |
-ç»åºæå®çè´¦å· | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
-(é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
-BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
-SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
-åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [HarukaBot](https://github.com/SK-415/
-HarukaBot) åè½æ¥æº - [BBot-Graia](https://github.com/djkcyl/BBot-Graia)
-åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://github.com/
-djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [bilireq](https://
-github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili è¯·æ±åº - [nonebot-
-plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
-é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://github.com/Misaka-
-Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG ä¿®å¤åä»£ç åè - [hamo-
-reid](https://github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ -
-[dynamicrender](https://pypi.org/project/dynrender-skia/) æä¾ t2i
-åå¨ææ¸²æ - [ALC](https://github.com/nonebot/plugin-alconna)
-æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿ [![Stargazers over time](https://
-starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/
-nonebot-plugin-bilichat)
+UP ä¸»çæµç§°æ UID | æ¥çæå® UP ä¸»çææ°ä¸æ¡å¨æ | | fetch |
+æ éå¶ | æ éå¶ | è§é¢æå¨æ IDï¼æåå¤åå«æ­¤åå®¹çæ¶æ¯
+| è§£æå¨æåå«çå¾çæè§é¢ç´é¾ | | checklogin | ä¸»äºº |
+æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· | | qrlogin | ä¸»äºº |
+æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B ç«ï¼é²æ­¢é£æ§ | | logout |
+ä¸»äºº | æ éå¶ | è´¦å·ç UID | ç»åºæå®çè´¦å· | ## ð æè°¢
+å¨æ­¤æè°¢ä»¥ä¸å¼åè(é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT]
+(https://github.com/JimmyLv/BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-
+collect](https://github.com/SocialSisterYi/bilibili-API-collect)
+æå§æ¶éçåç§ BiliBili Api åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ -
+[HarukaBot](https://github.com/SK-415/HarukaBot) åè½æ¥æº - [BBot-Graia]
+(https://github.com/djkcyl/BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ -
+[ABot-Graia](https://github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot
+ð - [bilireq](https://github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili
+è¯·æ±åº - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-
+plugin-template): é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://
+github.com/Misaka-Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG
+ä¿®å¤åä»£ç åè - [hamo-reid](https://github.com/hamo-reid) ä¸º
+style_blue ç»å¶äºçé¢ - [dynamicrender](https://pypi.org/project/
+dynrender-skia/) æä¾ t2i åå¨ææ¸²æ - [ALC](https://github.com/nonebot/
+plugin-alconna) æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿ [![Stargazers over
+time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://
+starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 async def _pre_check(state: T_State, event: Event, bot: Bot, msg: UniMsg, target: MsgTarget):
     set_options(state, msg)
     return await _permission_check(bot, event, target, state) and await _bili_check(state, event, bot, msg)
 
 
 bilichat = on_message(
     block=plugin_config.bilichat_block,
-    priority=1,
+    priority=2,
     rule=Rule(_pre_check),
 )
 
 
 @bilichat.handle()
 async def content_info(event: Event, origin_msg: UniMsg, state: T_State):
     content: Column | Video | Dynamic = state["_content_"]
```

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     bilichat_cmd_remove_sub: list[str] = ["退订", "取关"]
     bilichat_cmd_check_sub: list[str] = ["查看", "查看订阅"]
     bilichat_cmd_reset_sub: list[str] = ["重置", "重置配置"]
     bilichat_cmd_at_all: list[str] = ["全体成员", "at全体"]
     bilichat_cmd_dynamic: list[str] = ["动态通知", "动态订阅"]
     bilichat_cmd_live: list[str] = ["直播通知", "直播订阅"]
     bilichat_cmd_checkdynamic: list[str] = ["查看动态"]
+    bilichat_cmd_fetch: list[str] = ["获取内容", "解析内容"]
     bilichat_cmd_check_login: list[str] = ["查看登录账号"]
     bilichat_cmd_login_qrcode: list[str] = ["扫码登录"]
     bilichat_cmd_logout: list[str] = ["登出账号"]
 
     # basic info
     bilichat_basic_info: bool = True
     bilichat_basic_info_style: Literal["bbot_default", "style_blue"] = Field(default="Auto")
```

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/column.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,7 +69,10 @@
         return content
 
     async def get_subtitle(self):
         return self.cache.content
 
     async def get_image(self, style: str):
         return await draw_column(cvid=self.id)
+    
+    async def fetch_content(self) -> list[bytes] | list[None]:
+        ...
```

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bilireq.exceptions import GrpcError, ResponseCodeError
 from bilireq.grpc.dynamic import grpc_get_dynamic_detail
 from bilireq.grpc.protos.bilibili.app.dynamic.v2.dynamic_pb2 import DynamicType, DynModuleType
 from google.protobuf.json_format import MessageToDict
 from nonebot.log import logger
 from pydantic import BaseModel
 
-from ..lib.bilibili_request import get_b23_url, get_dynamic
+from ..lib.bilibili_request import get_b23_url, get_dynamic, hc
 from ..lib.bilibili_request.auth import AuthManager
 from ..lib.draw.dynamic import draw_dynamic
 from ..model.exception import AbortError
 from ..optional import capture_exception
 
 
 class Dynamic(BaseModel):
@@ -20,15 +20,15 @@
     url: str
     """b23 链接"""
     dynamic_type: DynamicType.ValueType = DynamicType.dyn_none
     "动态类型"
     raw: dict = {}
     """动态的原始信息"""
     raw_type: Literal["web", "grpc", None] = None
-    
+
     @property
     def bili_id(self) -> str:
         return f"动态id: {self.id}"
 
     async def _grpc(self):
         logger.debug("正在使用 gRPC 获取动态信息")
         _dyn = await grpc_get_dynamic_detail(dynamic_id=self.id, auth=AuthManager.get_auth())
@@ -57,14 +57,16 @@
             self.dynamic_type = DynamicType.av
             aid = dyn["modules"]["module_dynamic"]["major"]["archive"]["aid"]
             self.url = await get_b23_url(f"https://www.bilibili.com/video/av{aid}")
         elif dyn["type"] == "DYNAMIC_TYPE_ARTICLE":
             self.dynamic_type = DynamicType.article
             cvid = dyn["modules"]["module_dynamic"]["major"]["article"]["id"]
             self.url = await get_b23_url(f"https://www.bilibili.com/read/cv{cvid}")
+        elif dyn["type"] == "DYNAMIC_TYPE_DRAW":
+            self.dynamic_type = DynamicType.draw
 
     @classmethod
     async def from_id(cls, bili_number: str):
         if not bili_number.isdigit():
             bili_number = bili_number.lstrip("qwertyuiopasdfghjklzxcvbnm/.")
 
         dynamic = cls(id=bili_number, url="")
@@ -90,11 +92,32 @@
                     if dynamic.raw:  # 如果存在动态内容，则很可能是数据结构变化了
                         logger.debug(dynamic.raw)
                         capture_exception(extra={"dynamic_data": dynamic.raw})
                 raise AbortError("动态查询信息异常，请查看控制台获取更多信息")
 
         if not dynamic.url:
             dynamic.url = await get_b23_url(f"https://t.bilibili.com/{bili_number}")
+        # with open("dynamic.json", "w", encoding="utf-8") as f:
+        #     import json
+        #     json.dump(dynamic.dict(), f, ensure_ascii=False)
         return dynamic
 
     async def get_image(self, style: str):
         return await draw_dynamic(dynid=self.id, raw=self.raw, raw_type=self.raw_type)
+
+    async def fetch_content(self) -> list[bytes] | list[None]:
+        result = []
+        # 获取图文动态中的图片
+        if self.dynamic_type == DynamicType.draw:
+            if self.raw_type == "web":
+                items = self.raw["modules"]["module_dynamic"]["major"]["draw"]["items"]
+            elif self.raw_type == "grpc":
+                for module in self.raw["modules"]:
+                    if module["module_type"] == "module_dynamic":
+                        items = module["dynDraw"]["items"]
+                        break
+            for item in items:
+                resq = await hc.get(item["src"])
+                result.append(resq.content)
+        else:
+            logger.debug(f"动态类型 {self.dynamic_type} 不是图文动态")
+        return result
```

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,7 +100,10 @@
         logger.debug(resp)
         try:
             summary = SummaryApiResponse(**resp)
         except ValidationError as e:
             capture_exception(extra={"response": resp})
             raise AbortError("获取官方视频总结失败") from e
         return summary
+
+    async def fetch_content(self) -> list[bytes] | list[None]:
+        ...
```

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/arguments.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/arguments.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/const.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/const.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.8.1/pyproject.toml` & `nonebot_plugin_bilichat-5.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.8.1"
+version = "5.9.0"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.13",
```

### Comparing `nonebot_plugin_bilichat-5.8.1/PKG-INFO` & `nonebot_plugin_bilichat-5.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.8.1
+Version: 5.9.0
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.10
 Requires-Dist: bilireq>=0.2.13
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -234,14 +234,15 @@
 |  bilichat_cmd_remove_sub  | list[str] |     ["退订", "取关"]     |     "unsub"命令的别名     |
 |  bilichat_cmd_check_sub   | list[str] |   ["查看", "查看订阅"]   |     "check"命令的别名     |
 |  bilichat_cmd_reset_sub   | list[str] |   ["重置", "重置配置"]   |     "reset"命令的别名     |
 |    bilichat_cmd_at_all    | list[str] | ["全体成员", "at 全体"]  |     "atall"命令的别名     |
 |   bilichat_cmd_dynamic    | list[str] | ["动态通知", "动态订阅"] |    "dynamic"命令的别名    |
 |     bilichat_cmd_live     | list[str] | ["直播通知", "直播订阅"] |     "live"命令的别名      |
 | bilichat_cmd_checkdynamic | list[str] |       ["查看动态"]       | "checkdynamic" 命令的别名 |
+|    bilichat_cmd_fetch     | list[str] | ["获取内容", "解析内容"] |    "fetch" 命令的别名     |
 | bilichat_cmd_check_login  | list[str] |     ["查看登录账号"]     |  "checklogin" 命令的别名  |
 | bilichat_cmd_login_qrcode | list[str] |       ["扫码登录"]       |   "qrlogin" 命令的别名    |
 |    bilichat_cmd_logout    | list[str] |       ["登出账号"]       |    "logout" 命令的别名    |
 
 ### 基础信息配置项
 
 |            配置项            | 类型 | 默认值 |                        说明                        |
@@ -364,14 +365,15 @@
 |    unsub     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       |         移除订阅，all 时为全移除         |
 |    check     | 无限制 |  群聊  |       UP 主的昵称或 UID，或留空        |    查看本群订阅列表或指定 UP 主的配置    |
 |    reset     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       | 重置指定 UP 主的推送配置，all 时为全重置 |
 |    atall     |  主人  |  群聊  | UP 主的昵称或 UID `全局` `动态` `直播` |           设置是否 at 全体成员           |
 |   dynamic    |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的动态通知         |
 |     live     |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的直播通知         |
 | checkdynamic | 无限制 | 无限制 |           UP 主的昵称或 UID            |       查看指定 UP 主的最新一条动态       |
+|    fetch     | 无限制 | 无限制 | 视频或动态 ID，或回复包含此内容的消息  |       解析动态包含的图片或视频直链       |
 |  checklogin  |  主人  | 无限制 |                   无                   |         查看当前已登录的全部账号         |
 |   qrlogin    |  主人  | 无限制 |                   无                   |      使用二维码登录 B 站，防止风控       |
 |    logout    |  主人  | 无限制 |               账号的 UID               |              登出指定的账号              |
 
 ## 🙏 感谢
 
 在此感谢以下开发者(项目)对本项目做出的贡献：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.8.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.9.0 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.10 Requires-Dist:
 bilireq>=0.2.13 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
@@ -106,22 +106,24 @@
 bilichat_cmd_check_sub | list[str] | ["æ¥ç", "æ¥çè®¢é"] |
 "check"å½ä»¤çå«å | | bilichat_cmd_reset_sub | list[str] | ["éç½®",
 "éç½®éç½®"] | "reset"å½ä»¤çå«å | | bilichat_cmd_at_all | list[str] |
 ["å¨ä½æå", "at å¨ä½"] | "atall"å½ä»¤çå«å | | bilichat_cmd_dynamic
 | list[str] | ["å¨æéç¥", "å¨æè®¢é"] | "dynamic"å½ä»¤çå«å | |
 bilichat_cmd_live | list[str] | ["ç´æ­éç¥", "ç´æ­è®¢é"] |
 "live"å½ä»¤çå«å | | bilichat_cmd_checkdynamic | list[str] |
-["æ¥çå¨æ"] | "checkdynamic" å½ä»¤çå«å | | bilichat_cmd_check_login
-| list[str] | ["æ¥çç»å½è´¦å·"] | "checklogin" å½ä»¤çå«å | |
-bilichat_cmd_login_qrcode | list[str] | ["æ«ç ç»å½"] | "qrlogin"
-å½ä»¤çå«å | | bilichat_cmd_logout | list[str] | ["ç»åºè´¦å·"] |
-"logout" å½ä»¤çå«å | ### åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å |
-é»è®¤å¼ | è¯´æ | | :--------------------------: | :--: | :----: | :--------
-----------------------------------------: | | bilichat_basic_info | bool | True
-| æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str | Auto |
+["æ¥çå¨æ"] | "checkdynamic" å½ä»¤çå«å | | bilichat_cmd_fetch | list
+[str] | ["è·ååå®¹", "è§£æåå®¹"] | "fetch" å½ä»¤çå«å | |
+bilichat_cmd_check_login | list[str] | ["æ¥çç»å½è´¦å·"] | "checklogin"
+å½ä»¤çå«å | | bilichat_cmd_login_qrcode | list[str] | ["æ«ç ç»å½"] |
+"qrlogin" å½ä»¤çå«å | | bilichat_cmd_logout | list[str] |
+["ç»åºè´¦å·"] | "logout" å½ä»¤çå«å | ### åºç¡ä¿¡æ¯éç½®é¡¹ |
+éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :--------------------------: | :--:
+| :----: | :------------------------------------------------: | |
+bilichat_basic_info | bool | True | æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | |
+bilichat_basic_info_style | str | Auto |
 è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
 bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
 bilichat_reply_to_basic_info | bool | True |
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) | |
 bilichat_dynamic | bool | True | æ¯å¦å¼å¯å¨æè§£æ | |
 bilichat_dynamic_style | str | Auto |
@@ -190,29 +192,30 @@
 UIDï¼æçç©º | æ¥çæ¬ç¾¤è®¢éåè¡¨ææå® UP ä¸»çéç½® | | reset |
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UIDï¼æ `all` | éç½®æå® UP
 ä¸»çæ¨ééç½®ï¼all æ¶ä¸ºå¨éç½® | | atall | ä¸»äºº | ç¾¤è | UP
 ä¸»çæµç§°æ UID `å¨å±` `å¨æ` `ç´æ­` | è®¾ç½®æ¯å¦ at å¨ä½æå |
 | dynamic | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ¯å¦å¼å¯è¯¥ UP
 çå¨æéç¥ | | live | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID |
 æ¯å¦å¼å¯è¯¥ UP çç´æ­éç¥ | | checkdynamic | æ éå¶ | æ éå¶ |
-UP ä¸»çæµç§°æ UID | æ¥çæå® UP ä¸»çææ°ä¸æ¡å¨æ | |
-checklogin | ä¸»äºº | æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· |
-| qrlogin | ä¸»äºº | æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B
-ç«ï¼é²æ­¢é£æ§ | | logout | ä¸»äºº | æ éå¶ | è´¦å·ç UID |
-ç»åºæå®çè´¦å· | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
-(é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
-BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
-SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
-åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [HarukaBot](https://github.com/SK-415/
-HarukaBot) åè½æ¥æº - [BBot-Graia](https://github.com/djkcyl/BBot-Graia)
-åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://github.com/
-djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [bilireq](https://
-github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili è¯·æ±åº - [nonebot-
-plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
-é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://github.com/Misaka-
-Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG ä¿®å¤åä»£ç åè - [hamo-
-reid](https://github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ -
-[dynamicrender](https://pypi.org/project/dynrender-skia/) æä¾ t2i
-åå¨ææ¸²æ - [ALC](https://github.com/nonebot/plugin-alconna)
-æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿ [![Stargazers over time](https://
-starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/
-nonebot-plugin-bilichat)
+UP ä¸»çæµç§°æ UID | æ¥çæå® UP ä¸»çææ°ä¸æ¡å¨æ | | fetch |
+æ éå¶ | æ éå¶ | è§é¢æå¨æ IDï¼æåå¤åå«æ­¤åå®¹çæ¶æ¯
+| è§£æå¨æåå«çå¾çæè§é¢ç´é¾ | | checklogin | ä¸»äºº |
+æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· | | qrlogin | ä¸»äºº |
+æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B ç«ï¼é²æ­¢é£æ§ | | logout |
+ä¸»äºº | æ éå¶ | è´¦å·ç UID | ç»åºæå®çè´¦å· | ## ð æè°¢
+å¨æ­¤æè°¢ä»¥ä¸å¼åè(é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT]
+(https://github.com/JimmyLv/BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-
+collect](https://github.com/SocialSisterYi/bilibili-API-collect)
+æå§æ¶éçåç§ BiliBili Api åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ -
+[HarukaBot](https://github.com/SK-415/HarukaBot) åè½æ¥æº - [BBot-Graia]
+(https://github.com/djkcyl/BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ -
+[ABot-Graia](https://github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot
+ð - [bilireq](https://github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili
+è¯·æ±åº - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-
+plugin-template): é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://
+github.com/Misaka-Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG
+ä¿®å¤åä»£ç åè - [hamo-reid](https://github.com/hamo-reid) ä¸º
+style_blue ç»å¶äºçé¢ - [dynamicrender](https://pypi.org/project/
+dynrender-skia/) æä¾ t2i åå¨ææ¸²æ - [ALC](https://github.com/nonebot/
+plugin-alconna) æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿ [![Stargazers over
+time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://
+starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

