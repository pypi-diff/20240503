# Comparing `tmp/nonebot_plugin_nai3-0.1.6.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.7.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.6.tar` & `nonebot_plugin_nai3-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.6/LICENSE
--rw-r--r--   0        0        0    13262 2024-04-16 05:23:40.318589 nonebot_plugin_nai3-0.1.6/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      803 2024-04-16 05:26:48.482731 nonebot_plugin_nai3-0.1.6/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.6/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-04-16 05:27:30.543045 nonebot_plugin_nai3-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5371 2024-04-16 05:27:02.695171 nonebot_plugin_nai3-0.1.6/README.md
--rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.7/LICENSE
+-rw-r--r--   0        0        0    13247 2024-05-03 14:28:08.535553 nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      803 2024-05-02 12:22:13.415920 nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-05-03 14:32:03.773065 nonebot_plugin_nai3-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5363 2024-05-02 12:22:18.486293 nonebot_plugin_nai3-0.1.7/README.md
+-rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.7/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.6/LICENSE` & `nonebot_plugin_nai3-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.6/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,20 +112,20 @@
     # 更新冷却时间和次数
     now_time = time.time()
     try:
         cd[gid]["user"][uid]["limit"]
     except KeyError:
         cd[gid] = {
             "cool_time": now_time - nai3_config.nai3_cooltime_group,
-            "user": {
-                uid: {
-                    "limit": 999 if event.get_user_id() in bot.config.superusers else nai3_config.nai3_limit,
-                    "cool_time": now_time - nai3_config.nai3_cooltime_user,
-                }
-            },
+        }
+        cd[gid]["user"] = {
+            uid: {
+                "limit": 999 if event.get_user_id() in bot.config.superusers else nai3_config.nai3_limit,
+                "cool_time": now_time - nai3_config.nai3_cooltime_user,
+            }
         }
 
     # 判断冷却时间并阻断
     if event.get_user_id() not in bot.config.superusers:
         logger.debug(event.get_user_id())
         logger.debug(bot.config.superusers)
         if now_time - cd[gid]["cool_time"] < nai3_config.nai3_cooltime_group:
```

### Comparing `nonebot_plugin_nai3-0.1.6/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.6/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.7/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.6/pyproject.toml` & `nonebot_plugin_nai3-0.1.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.6"
+version = "0.1.7"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.6/README.md` & `nonebot_plugin_nai3-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 <summary>conda</summary>
 
     conda install nonebot-plugin-nai3
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot_plugin_hoshino_sign"]
+    plugins = ["nonebot_plugin_nai3"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
```

#### html2text {}

```diff
@@ -11,20 +11,20 @@
 ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-nai3
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-nai3 pdm pdm add nonebot-plugin-nai3 poetry
 poetry add nonebot-plugin-nai3 conda conda install nonebot-plugin-nai3 æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_hoshino_sign"] ## âï¸ éç½®
-å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
-| å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
-| | nai3_token | æ¯ | str | "xxx" | è¯·æ±å¤´ä¸­å¿éç token | |
-nai3_negative | å¦ | str | "nsfw,..." | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
-int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_nai3"] ## âï¸ éç½® å¨
+nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
+å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
+nai3_token | æ¯ | str | "xxx" | è¯·æ±å¤´ä¸­å¿éç token | | nai3_negative
+| å¦ | str | "nsfw,..." | è´é¢æç¤ºè¯ | | nai3_limit | å¦ | int | 10 |
+æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
 post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
 æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
 nai3_send_to_group | å¦ | bool | True |
 æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | False |
 æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str | "./data/
```

### Comparing `nonebot_plugin_nai3-0.1.6/PKG-INFO` & `nonebot_plugin_nai3-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.6
+Version: 0.1.7
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -73,15 +73,15 @@
 <summary>conda</summary>
 
     conda install nonebot-plugin-nai3
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot_plugin_hoshino_sign"]
+    plugins = ["nonebot_plugin_nai3"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.6 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.7 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
@@ -21,20 +21,20 @@
 ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-nai3
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-nai3 pdm pdm add nonebot-plugin-nai3 poetry
 poetry add nonebot-plugin-nai3 conda conda install nonebot-plugin-nai3 æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_hoshino_sign"] ## âï¸ éç½®
-å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
-| å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
-| | nai3_token | æ¯ | str | "xxx" | è¯·æ±å¤´ä¸­å¿éç token | |
-nai3_negative | å¦ | str | "nsfw,..." | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
-int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_nai3"] ## âï¸ éç½® å¨
+nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
+å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
+nai3_token | æ¯ | str | "xxx" | è¯·æ±å¤´ä¸­å¿éç token | | nai3_negative
+| å¦ | str | "nsfw,..." | è´é¢æç¤ºè¯ | | nai3_limit | å¦ | int | 10 |
+æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
 post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
 æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
 nai3_send_to_group | å¦ | bool | True |
 æ¯å¦åè®¸å°å¾çé¾æ¥åéå°ç¾¤ | | nai3_save | å¦ | bool | False |
 æ¯å¦å°ç¨æ·çæçå¾çä¿å­ | | nai3_save_path | å¦ | str | "./data/
```

