# Comparing `tmp/nonebot_plugin_anime_downloader-0.1.3.tar.gz` & `tmp/nonebot_plugin_anime_downloader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_anime_downloader-0.1.3.tar", last modified: Fri May  3 08:56:52 2024, max compression
+gzip compressed data, was "nonebot_plugin_anime_downloader-0.1.4.tar", last modified: Fri May  3 12:03:27 2024, max compression
```

## Comparing `nonebot_plugin_anime_downloader-0.1.3.tar` & `nonebot_plugin_anime_downloader-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/LICENSE
--rw-r--r--   0        0        0     3606 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/README.md
--rw-r--r--   0        0        0    12118 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/__init__.py
--rw-r--r--   0        0        0     4761 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/acgrip/__init__.py
--rw-r--r--   0        0        0      654 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/config.py
--rw-r--r--   0        0        0      698 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/data_source.py
--rw-r--r--   0        0        0     1609 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/__init__.py
--rw-r--r--   0        0        0     1214 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/models.py
--rw-r--r--   0        0        0      175 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/models.py
--rw-r--r--   0        0        0     1398 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/routes.py
--rw-r--r--   0        0        0      761 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/tasks.py
--rw-r--r--   0        0        0      316 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/templates/index.html
--rw-r--r--   0        0        0      897 2024-05-03 08:56:21.875944 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/test.py
--rw-r--r--   0        0        0     2659 2024-05-03 08:56:21.879945 nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/utils.py
--rw-r--r--   0        0        0      730 2024-05-03 08:56:52.848129 nonebot_plugin_anime_downloader-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3751 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/README.md
+-rw-r--r--   0        0        0    12262 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/__init__.py
+-rw-r--r--   0        0        0     4761 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/acgrip/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/config.py
+-rw-r--r--   0        0        0      698 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/data_source.py
+-rw-r--r--   0        0        0     1609 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/downloader/__init__.py
+-rw-r--r--   0        0        0     1214 2024-05-03 12:02:57.953767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/downloader/models.py
+-rw-r--r--   0        0        0      175 2024-05-03 12:02:57.957767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/models.py
+-rw-r--r--   0        0        0     1398 2024-05-03 12:02:57.957767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/routes.py
+-rw-r--r--   0        0        0      761 2024-05-03 12:02:57.957767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/tasks.py
+-rw-r--r--   0        0        0      316 2024-05-03 12:02:57.957767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/templates/index.html
+-rw-r--r--   0        0        0      897 2024-05-03 12:02:57.957767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/test.py
+-rw-r--r--   0        0        0     2659 2024-05-03 12:02:57.957767 nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/utils.py
+-rw-r--r--   0        0        0      730 2024-05-03 12:03:27.577879 nonebot_plugin_anime_downloader-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_anime_downloader-0.1.3/LICENSE` & `nonebot_plugin_anime_downloader-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/README.md` & `nonebot_plugin_anime_downloader-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 ## 使用
 | 命令 | 别名 | 说明 | 示例 |
 | --- | --- | --- | --- |
 | sub | 订阅 | 通过 Tag 订阅番剧 | `sub Up to 21°C Nijiyon Animation 2 MP4` |
 | unsub | 取消订阅 | 通过 Tag 取消订阅番剧 | `unsub Up to 21°C Nijiyon Animation 2 MP4` |
 | listsub | sublist, 订阅列表 | 查看当前用户/群组的订阅列表 | `sublist` |
 
+这里的 Tag 就是用来在 ACG.RIP 搜索的关键词，番剧名、分辨率、字幕组等等，只要能在 ACG.RIP 搜索到的都可以
+
 > 记得加上你的命令头哦
 
 ## 效果
 
 **user**: `/sub Up to 21°C Nijiyon Animation 2 MP4`
 
 **bot**: 订阅成功！
```

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,52 +137,52 @@
                         {
                             "id": user.id,
                             "content": torrent_info,
                             "torrent_id": int(entry["id"]),
                         }
                     )
 
-                # set a scheduler to check if the video is downloaded
-                async def check_video_downloaded(
-                    title: str, torrent_id: int, user_id: str
-                ):
-                    logger.info(
-                        f"Checking whether {title} is downloaded for {user_id}..."
-                    )
-                    if torrent_id in video_manager.ids:
+                    # set a scheduler to check if the video is downloaded
+                    async def check_video_downloaded(
+                        title: str, torrent_id: int, user_id: str
+                    ):
                         logger.info(
-                            f"{title} is downloaded for {user_id}! Sending message..."
-                        )
-                        # send message to user
-                        msg = (
-                            f"{title} 现在可以观看了！\n"
-                            + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{torrent_id}"
-                        )
-                        chat_type = str(user_id).split("_")[0]
-                        id_ = str(user_id).split("_")[-1]
-                        target = Target(
-                            id=id_,
-                            parent_id=id_ if chat_type == "group" else "",
-                            channel=chat_type == "group",
-                            private=chat_type == "private",
+                            f"Checking whether {title} is downloaded for {user_id}..."
                         )
-                        await UniMessage(msg).send(target)
-                        logger.info(f"Message sent to {user_id}!")
-
-                        scheduler.remove_job(f"{title}_{user_id}")
-                    else:
-                        logger.info(f"{title} is not downloaded yet for {user_id}.")
-
-                scheduler.add_job(
-                    check_video_downloaded,
-                    "interval",
-                    seconds=10,
-                    args=(entry["title"], int(entry["id"]), user.id),
-                    id=f"{entry['title']}_{user.id}",
-                )
+                        if torrent_id in video_manager.ids:
+                            logger.info(
+                                f"{title} is downloaded for {user_id}! Sending message..."
+                            )
+                            # send message to user
+                            msg = (
+                                f"{title} 现在可以观看了！\n"
+                                + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{torrent_id}"
+                            )
+                            chat_type = str(user_id).split("_")[0]
+                            id_ = str(user_id).split("_")[-1]
+                            target = Target(
+                                id=id_,
+                                parent_id=id_ if chat_type == "group" else "",
+                                channel=chat_type == "group",
+                                private=chat_type == "private",
+                            )
+                            await UniMessage(msg).send(target)
+                            logger.info(f"Message sent to {user_id}!")
+
+                            scheduler.remove_job(f"{title}_{user_id}")
+                        else:
+                            logger.info(f"{title} is not downloaded yet for {user_id}.")
+
+                    scheduler.add_job(
+                        check_video_downloaded,
+                        "interval",
+                        seconds=10,
+                        args=(entry["title"], int(entry["id"]), user.id),
+                        id=f"{entry['title']}_{user.id}",
+                    )
 
 
 @scheduler.scheduled_job("interval", seconds=60)
 async def check_for_tasks():
     tasks = task_manager.get()
 
     for task in tasks:
```

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/acgrip/__init__.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/acgrip/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/config.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/data_source.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/downloader/models.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/downloader/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/routes.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/routes.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/tasks.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/tasks.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/test.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/test.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/nonebot_plugin_anime_downloader/utils.py` & `nonebot_plugin_anime_downloader-0.1.4/nonebot_plugin_anime_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.3/pyproject.toml` & `nonebot_plugin_anime_downloader-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-anime-downloader"
-version = "0.1.3"
+version = "0.1.4"
 description = "✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "aiohttp>=3.9.5",
```

### Comparing `nonebot_plugin_anime_downloader-0.1.3/PKG-INFO` & `nonebot_plugin_anime_downloader-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-anime-downloader
-Version: 0.1.3
+Version: 0.1.4
 Summary: ✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: aiohttp>=3.9.5
 Requires-Dist: qbittorrent-api>=2024.3.60
@@ -33,14 +33,16 @@
 ## 使用
 | 命令 | 别名 | 说明 | 示例 |
 | --- | --- | --- | --- |
 | sub | 订阅 | 通过 Tag 订阅番剧 | `sub Up to 21°C Nijiyon Animation 2 MP4` |
 | unsub | 取消订阅 | 通过 Tag 取消订阅番剧 | `unsub Up to 21°C Nijiyon Animation 2 MP4` |
 | listsub | sublist, 订阅列表 | 查看当前用户/群组的订阅列表 | `sublist` |
 
+这里的 Tag 就是用来在 ACG.RIP 搜索的关键词，番剧名、分辨率、字幕组等等，只要能在 ACG.RIP 搜索到的都可以
+
 > 记得加上你的命令头哦
 
 ## 效果
 
 **user**: `/sub Up to 21°C Nijiyon Animation 2 MP4`
 
 **bot**: 订阅成功！
```

