# Comparing `tmp/nonebot_plugin_nai3-0.1.7.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.7.tar` & `nonebot_plugin_nai3-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.7/LICENSE
--rw-r--r--   0        0        0    13247 2024-05-03 14:28:08.535553 nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      803 2024-05-02 12:22:13.415920 nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-05-03 14:32:03.773065 nonebot_plugin_nai3-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5363 2024-05-02 12:22:18.486293 nonebot_plugin_nai3-0.1.7/README.md
--rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.8/LICENSE
+-rw-r--r--   0        0        0    13202 2024-05-03 14:53:25.721129 nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      803 2024-05-02 12:22:13.415920 nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-05-03 14:48:40.750023 nonebot_plugin_nai3-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5363 2024-05-02 12:22:18.486293 nonebot_plugin_nai3-0.1.8/README.md
+-rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.7/LICENSE` & `nonebot_plugin_nai3-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,22 +110,18 @@
         pass
 
     # 更新冷却时间和次数
     now_time = time.time()
     try:
         cd[gid]["user"][uid]["limit"]
     except KeyError:
-        cd[gid] = {
-            "cool_time": now_time - nai3_config.nai3_cooltime_group,
-        }
-        cd[gid]["user"] = {
-            uid: {
-                "limit": 999 if event.get_user_id() in bot.config.superusers else nai3_config.nai3_limit,
-                "cool_time": now_time - nai3_config.nai3_cooltime_user,
-            }
+        cd[gid] = {"cool_time": now_time - nai3_config.nai3_cooltime_group, "user": {}}
+        cd[gid]["user"][uid] = {
+            "limit": 999 if event.get_user_id() in bot.config.superusers else nai3_config.nai3_limit,
+            "cool_time": now_time - nai3_config.nai3_cooltime_user,
         }
 
     # 判断冷却时间并阻断
     if event.get_user_id() not in bot.config.superusers:
         logger.debug(event.get_user_id())
         logger.debug(bot.config.superusers)
         if now_time - cd[gid]["cool_time"] < nai3_config.nai3_cooltime_group:
@@ -235,15 +231,15 @@
                             await bot.call_api(
                                 "send_msg",
                                 **{
                                     "message": f"群: {gid}, 用户: {uid}, 画了一张涩图!\n{file.url}",
                                     "user_id": superuser,
                                 },
                             )
-                            asyncio.sleep(1)
+                            await asyncio.sleep(1)
                     return
             await nai3.send(f"种子: {seed}\n" + MessageSegment.image(Path("./data/nai3/temp.png")), at_sender=True)
             return
     except Exception as e:
         await nai3.finish(f"出现错误: {e}", at_sender=True)
```

### Comparing `nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.7/pyproject.toml` & `nonebot_plugin_nai3-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.7"
+version = "0.1.8"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.7/README.md` & `nonebot_plugin_nai3-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.7/PKG-INFO` & `nonebot_plugin_nai3-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.7
+Version: 0.1.8
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.7 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.8 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
```

