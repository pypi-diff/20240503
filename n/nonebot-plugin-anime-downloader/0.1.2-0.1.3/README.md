# Comparing `tmp/nonebot_plugin_anime_downloader-0.1.2.tar.gz` & `tmp/nonebot_plugin_anime_downloader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_anime_downloader-0.1.2.tar", last modified: Fri May  3 08:43:26 2024, max compression
+gzip compressed data, was "nonebot_plugin_anime_downloader-0.1.3.tar", last modified: Fri May  3 08:56:52 2024, max compression
```

## Comparing `nonebot_plugin_anime_downloader-0.1.2.tar` & `nonebot_plugin_anime_downloader-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/LICENSE
--rw-r--r--   0        0        0     3606 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/README.md
--rw-r--r--   0        0        0    12137 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/__init__.py
--rw-r--r--   0        0        0     4761 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/acgrip/__init__.py
--rw-r--r--   0        0        0      654 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/config.py
--rw-r--r--   0        0        0      698 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/data_source.py
--rw-r--r--   0        0        0     1609 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/__init__.py
--rw-r--r--   0        0        0     1214 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/models.py
--rw-r--r--   0        0        0      175 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/models.py
--rw-r--r--   0        0        0     1398 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/routes.py
--rw-r--r--   0        0        0      761 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/tasks.py
--rw-r--r--   0        0        0      316 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/templates/index.html
--rw-r--r--   0        0        0      897 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/test.py
--rw-r--r--   0        0        0     2659 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/utils.py
--rw-r--r--   0        0        0      730 2024-05-03 08:43:26.589354 nonebot_plugin_anime_downloader-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3606 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/README.md
+-rw-r--r--   0        0        0    12118 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/__init__.py
+-rw-r--r--   0        0        0     4761 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/acgrip/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/config.py
+-rw-r--r--   0        0        0      698 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/data_source.py
+-rw-r--r--   0        0        0     1609 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/__init__.py
+-rw-r--r--   0        0        0     1214 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/models.py
+-rw-r--r--   0        0        0      175 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/models.py
+-rw-r--r--   0        0        0     1398 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/routes.py
+-rw-r--r--   0        0        0      761 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/tasks.py
+-rw-r--r--   0        0        0      316 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/templates/index.html
+-rw-r--r--   0        0        0      897 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/test.py
+-rw-r--r--   0        0        0     2659 2024-05-03 08:56:21.879945 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/utils.py
+-rw-r--r--   0        0        0      730 2024-05-03 08:56:52.848129 nonebot_plugin_anime_downloader-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_anime_downloader-0.1.2/LICENSE` & `nonebot_plugin_anime_downloader-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/README.md` & `nonebot_plugin_anime_downloader-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     extract_data,
     fetch_torrent_data,
     replace_html_entities,
 )
 
 
 __plugin_meta__ = PluginMetadata(
-    name="nonebot_plugin_anime_downloader",
+    name="番剧下载",
     description="基于 qBittorrent Web UI 的番剧下载 NoneBot 插件",
     usage="/sub 订阅 Tag\n/unsub 取消订阅 Tag\n/listsub 查看订阅列表",
     type="application",
     homepage="https://github.com/zhaomaoniu/nonebot-plugin-anime-downloader",
     config=Config,
     supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
 )
```

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/acgrip/__init__.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/acgrip/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/config.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/data_source.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/models.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/routes.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/routes.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/tasks.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/tasks.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/test.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/test.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/utils.py` & `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.2/pyproject.toml` & `nonebot_plugin_anime_downloader-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-anime-downloader"
-version = "0.1.2"
+version = "0.1.3"
 description = "✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "aiohttp>=3.9.5",
```

### Comparing `nonebot_plugin_anime_downloader-0.1.2/PKG-INFO` & `nonebot_plugin_anime_downloader-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-anime-downloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: ✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: aiohttp>=3.9.5
 Requires-Dist: qbittorrent-api>=2024.3.60
```

