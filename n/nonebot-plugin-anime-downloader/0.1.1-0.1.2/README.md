# Comparing `tmp/nonebot_plugin_anime_downloader-0.1.1.tar.gz` & `tmp/nonebot_plugin_anime_downloader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_anime_downloader-0.1.1.tar", last modified: Fri May  3 08:29:59 2024, max compression
+gzip compressed data, was "nonebot_plugin_anime_downloader-0.1.2.tar", last modified: Fri May  3 08:43:26 2024, max compression
```

## Comparing `nonebot_plugin_anime_downloader-0.1.1.tar` & `nonebot_plugin_anime_downloader-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/LICENSE
--rw-r--r--   0        0        0     3606 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/README.md
--rw-r--r--   0        0        0    11798 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/__init__.py
--rw-r--r--   0        0        0     4761 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/acgrip/__init__.py
--rw-r--r--   0        0        0      654 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/config.py
--rw-r--r--   0        0        0      698 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/data_source.py
--rw-r--r--   0        0        0     1609 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/downloader/__init__.py
--rw-r--r--   0        0        0     1214 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/downloader/models.py
--rw-r--r--   0        0        0      175 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/models.py
--rw-r--r--   0        0        0     1472 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/routes.py
--rw-r--r--   0        0        0      761 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/tasks.py
--rw-r--r--   0        0        0      316 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/templates/index.html
--rw-r--r--   0        0        0      897 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/test.py
--rw-r--r--   0        0        0     2659 2024-05-03 08:29:26.439142 nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/utils.py
--rw-r--r--   0        0        0      730 2024-05-03 08:29:59.387234 nonebot_plugin_anime_downloader-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3606 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/README.md
+-rw-r--r--   0        0        0    12137 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/__init__.py
+-rw-r--r--   0        0        0     4761 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/acgrip/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/config.py
+-rw-r--r--   0        0        0      698 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/data_source.py
+-rw-r--r--   0        0        0     1609 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/__init__.py
+-rw-r--r--   0        0        0     1214 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/models.py
+-rw-r--r--   0        0        0      175 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/models.py
+-rw-r--r--   0        0        0     1398 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/routes.py
+-rw-r--r--   0        0        0      761 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/tasks.py
+-rw-r--r--   0        0        0      316 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/templates/index.html
+-rw-r--r--   0        0        0      897 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/test.py
+-rw-r--r--   0        0        0     2659 2024-05-03 08:42:50.969004 nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/utils.py
+-rw-r--r--   0        0        0      730 2024-05-03 08:43:26.589354 nonebot_plugin_anime_downloader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_anime_downloader-0.1.1/LICENSE` & `nonebot_plugin_anime_downloader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/README.md` & `nonebot_plugin_anime_downloader-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,33 @@
 
 if hasattr(nonebot, "get_plugin_config"):
     plugin_config = nonebot.get_plugin_config(Config)
 else:
     plugin_config = Config.parse_obj(nonebot.get_driver().config)
 
 
+download_path = Path(plugin_config.download_path)
+
+if not download_path.exists():
+    try:
+        download_path.mkdir(parents=True)
+    except PermissionError:
+        download_path = store.get_data_dir("nonebot_plugin_anime_downloader")
+        logger.warning(f"无法创建下载目录！请自行创建下载目录后重启 NoneBot. 本次下载目录为: {download_path}")
+
 tasks_file = store.get_data_file("nonebot_plugin_anime_downloader", "tasks.json")
 
 task_manager = TaskManager(tasks_file)
-video_manager = VideoManager(nonebot.get_app(), Path(plugin_config.download_path))
+video_manager = VideoManager(nonebot.get_app(), download_path)
 
 torrent_downloader = TorrentDownloader(
     plugin_config.qbittorrent_host,
     plugin_config.qbittorrent_username,
     plugin_config.qbittorrent_password,
-    Path(plugin_config.download_path),
+    download_path,
 )
 
 acg_rip_file = store.get_data_file("nonebot_plugin_anime_downloader", "acgrip.db")
 user_file = store.get_data_file("nonebot_plugin_anime_downloader", "users.db")
 video_file = store.get_data_file("nonebot_plugin_anime_downloader", "videos.db")
 
 acg_rip_engine = create_engine(f"sqlite:///{acg_rip_file.resolve()}")
```

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/acgrip/__init__.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/acgrip/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/config.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/data_source.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/downloader/models.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/downloader/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/routes.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 
 class VideoManager:
     def __init__(self, app: FastAPI, download_path: Path):
         if not isinstance(app, FastAPI):
             raise TypeError("app must be an instance of FastAPI.")
 
-        if not download_path.exists():
-            download_path.mkdir()
-
         self.ids: List[int] = []
         self.app = app
         self.download_path = download_path
         self.templates = Jinja2Templates(
             directory=(Path(__file__).parent / "templates").resolve()
         )
```

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/tasks.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/tasks.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/test.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/test.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/nonebot_plugin_anime_downloader/utils.py` & `nonebot_plugin_anime_downloader-0.1.2/nonebot_plugin_anime_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.1/pyproject.toml` & `nonebot_plugin_anime_downloader-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-anime-downloader"
-version = "0.1.1"
+version = "0.1.2"
 description = "✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "aiohttp>=3.9.5",
```

### Comparing `nonebot_plugin_anime_downloader-0.1.1/PKG-INFO` & `nonebot_plugin_anime_downloader-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-anime-downloader
-Version: 0.1.1
+Version: 0.1.2
 Summary: ✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: aiohttp>=3.9.5
 Requires-Dist: qbittorrent-api>=2024.3.60
```

