# Comparing `tmp/nonebot_plugin_cnrail-0.2.2.dev1.tar.gz` & `tmp/nonebot_plugin_cnrail-0.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cnrail-0.2.2.dev1.tar", last modified: Thu Apr  4 17:10:15 2024, max compression
+gzip compressed data, was "nonebot_plugin_cnrail-0.2.2.post1.tar", last modified: Fri May  3 11:29:43 2024, max compression
```

## Comparing `nonebot_plugin_cnrail-0.2.2.dev1.tar` & `nonebot_plugin_cnrail-0.2.2.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/LICENSE
--rw-r--r--   0        0        0     4601 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/README.md
--rw-r--r--   0        0        0      686 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__init__.py
--rw-r--r--   0        0        0     3938 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__main__.py
--rw-r--r--   0        0        0      308 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/config.py
--rw-r--r--   0        0        0     5526 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/data_source.py
--rw-r--r--   0        0        0     4830 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/models.py
--rw-r--r--   0        0        0    15513 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/templates/train_table.html.jinja
--rw-r--r--   0        0        0      813 2024-04-04 17:10:15.252575 nonebot_plugin_cnrail-0.2.2.dev1/pyproject.toml
--rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-03 11:29:29.950398 nonebot_plugin_cnrail-0.2.2.post1/LICENSE
+-rw-r--r--   0        0        0     4604 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/README.md
+-rw-r--r--   0        0        0      687 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__init__.py
+-rw-r--r--   0        0        0     4233 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__main__.py
+-rw-r--r--   0        0        0      308 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/config.py
+-rw-r--r--   0        0        0     5526 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/data_source.py
+-rw-r--r--   0        0        0     4830 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/models.py
+-rw-r--r--   0        0        0    15513 2024-05-03 11:29:29.954398 nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/templates/train_table.html.jinja
+-rw-r--r--   0        0        0      814 2024-05-03 11:29:43.098519 nonebot_plugin_cnrail-0.2.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.2.post1/PKG-INFO
```

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/LICENSE` & `nonebot_plugin_cnrail-0.2.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/README.md` & `nonebot_plugin_cnrail-0.2.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -110,46 +110,48 @@
 
 ## 🎉 使用
 
 使用指令 `train -h` 查看帮助
 
 ### 效果图
 
-![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png)
+<details>
+
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/t301.png)
+
+</details>
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
-### [海兰德小助手](https://qun.qq.com/qunpro/robot/qunshare?robot_uin=3889001607) & [Train-QQbot 插件](https://github.com/staytomorrow/FindTrain)
+### [海兰德小助手](https://qun.qq.com/qunpro/robot/qunshare?robot_uin=3889001607) & [Train-QQBot 插件](https://github.com/staytomorrow/FindTrain)
 
 灵感来源
 
-### [12306](https://www.12306.cn)
+### [MoeFactory 提供的查询 API](https://train.moefactory.com/)
 
 数据来源
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
+## 📝 更新日志
 
-  </details>
+### 0.2.2
 
-## 📝 更新日志
+- 修复列车行驶进度条计算问题（fix by [@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)）
 
 ### 0.2.1
 
 - 适配 [MoeFactory API](https://train.moefactory.com)
 - 新增配置项 `CNRAIL_ACG_IMAGE_URL`
 
 ### 0.2.0
```

#### html2text {}

```diff
@@ -14,27 +14,27 @@
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_cnrail" ] ``` ## âï¸ éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼
 | è¯´æ | | :--------------------: | :--: | :-------------------------------:
 | :----------------------------: | | `CNRAIL_ACG_IMAGE_URL` | å¦ | `https://
 www.loliapi.com/acg/pe/` | ç¨äºæä»¤è¿åå¾çèæ¯çå¾ç URL | ##
 ð ä½¿ç¨ ä½¿ç¨æä»¤ `train -h` æ¥çå¸®å© ### ææå¾ ![ææå¾]
-(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png) ##
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/t301.png) ##
 ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [æµ·å°å¾·å°å©æ](https://qun.qq.com/qunpro/
-robot/qunshare?robot_uin=3889001607) & [Train-QQbot æä»¶](https://github.com/
-staytomorrow/FindTrain) çµææ¥æº ### [12306](https://www.12306.cn)
-æ°æ®æ¥æº ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.1 - éé [MoeFactory API]
-(https://train.moefactory.com) - æ°å¢éç½®é¡¹ `CNRAIL_ACG_IMAGE_URL` ###
-0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ### 0.1.7 -
-æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ - bug fix
-### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 - ä¿®å¤ `-
-h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº ### 0.1.3 -
-fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/issues/2) ###
-0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~ åååæ¥ï¼
-### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢ ### 0.1.0 - ð
-Create this project
+robot/qunshare?robot_uin=3889001607) & [Train-QQBot æä»¶](https://github.com/
+staytomorrow/FindTrain) çµææ¥æº ### [MoeFactory æä¾çæ¥è¯¢ API]
+(https://train.moefactory.com/) æ°æ®æ¥æº ## ð° èµå© **[èµå©æ]
+(https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.2 - ä¿®å¤åè½¦è¡é©¶è¿åº¦æ¡è®¡ç®é®é¢ï¼fix by
+[@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)ï¼ ### 0.2.1 - éé
+[MoeFactory API](https://train.moefactory.com) - æ°å¢éç½®é¡¹
+`CNRAIL_ACG_IMAGE_URL` ### 0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ###
+0.1.7 - æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ -
+bug fix ### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 -
+ä¿®å¤ `-h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº
+### 0.1.3 - fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/
+issues/2) ### 0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~
+åååæ¥ï¼ ### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢
+### 0.1.0 - ð Create this project
```

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__init__.py` & `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.2.dev1"
+__version__ = "0.2.2.post1"
 __plugin_meta__ = PluginMetadata(
     name="CNRail",
     description="查询 12306 列车时刻表",
     usage="使用指令 train -h 查看帮助",
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__main__.py` & `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import string
 from contextlib import suppress
-from datetime import date, datetime
+from datetime import date, datetime, timedelta
 from typing import Optional
 
 from arclet.alconna import Alconna, Args, Arparma, CommandMeta
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from httpx import TimeoutException
 from nonebot import logger
 from nonebot_plugin_alconna import AlconnaMatcher, CommandResult, on_alconna
@@ -27,17 +27,25 @@
     def parse(df: str) -> Optional[date]:
         with suppress(ValueError):
             parsed = (
                 datetime.strptime(date_str, df)
                 .replace(year=today_date.year)
                 .date()  # noqa: DTZ007
             )
-            if parsed < today_date:
-                parsed = parsed.replace(year=today_date.year + 1)
-            return parsed
+            for parsed_date in [
+                parsed,
+                parsed.replace(year=today_date.year - 1),
+                parsed.replace(year=today_date.year + 1),
+            ]:
+                if (
+                    (today_date - timedelta(days=2))
+                    <= parsed_date
+                    <= (today_date + timedelta(days=14))
+                ):
+                    return parsed_date
         return None
 
     date_formats = ("%m/%d", "%m-%d", "%m月%d日", "%m月%d号", "%m月%d")
     if r := next((parse(x) for x in date_formats if parse(x)), None):
         return r
     raise ValueError
```

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/data_source.py` & `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/models.py` & `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/templates/train_table.html.jinja` & `nonebot_plugin_cnrail-0.2.2.post1/nonebot_plugin_cnrail/templates/train_table.html.jinja`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -329,16 +329,16 @@
         <div class="bottom-title">经停站</div>
         <div class="station-table-wrapper">
           <table class="station-table">
             <thead>
               <tr>
                 <th></th>
                 <th>停靠站</th>
-                <th>开点</th>
                 <th>到点</th>
+                <th>开点</th>
                 <th>停留</th>
                 <th>车次</th>
               </tr>
             </thead>
             <tbody>
               {% for station in detail.via_stations -%}
               <tr>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 担当路局：{{ detail.company_name }}
 {%- if sn -%}
 车组号：{{ sn }}
 {%- else -%}
 列车型号：{{ detail.routing.train_model }}
 {%- endif %}
 经停站
- ?停?靠?站                  ?开?点                     ?到?点                     ?停?留                   ?车?次
+ ?停?靠?站                  ?到?点                     ?开?点                     ?停?留                   ?车?次
                                                                     {% if loop.first
  {                    {% if loop.first %}-{% {% if loop.last %}-{%  %}始发站{% elif         {
  {                    else %}{               else %}{               loop.last %}终点站{%    {
  station.station_name {                      {                      else %}{             station.train_number
  }}                   station.arrival_time}} station.departure_time {                    }}
                       {% endif %}            }}{% endif %}          station.stop_minutes
                                                                     }} 分{% endif %}
```

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/pyproject.toml` & `nonebot_plugin_cnrail-0.2.2.post1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "nonebot-plugin-alconna>=0.40.1",
     "nonebot-plugin-htmlrender>=0.2.2",
     "jinja2>=3.1.2",
     "pytz>=2023.3.post1",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.2.dev1"
+version = "0.2.2.post1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail"
```

### Comparing `nonebot_plugin_cnrail-0.2.2.dev1/PKG-INFO` & `nonebot_plugin_cnrail-0.2.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cnrail
-Version: 0.2.2.dev1
+Version: 0.2.2.post1
 Summary: NoneBot2 plugin for query the train time table
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Author-Email: student_2333 <lgc2333@126.com>, XieXiLin <support@xiexilin.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
@@ -127,46 +127,48 @@
 
 ## 🎉 使用
 
 使用指令 `train -h` 查看帮助
 
 ### 效果图
 
-![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png)
+<details>
+
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/t301.png)
+
+</details>
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
-### [海兰德小助手](https://qun.qq.com/qunpro/robot/qunshare?robot_uin=3889001607) & [Train-QQbot 插件](https://github.com/staytomorrow/FindTrain)
+### [海兰德小助手](https://qun.qq.com/qunpro/robot/qunshare?robot_uin=3889001607) & [Train-QQBot 插件](https://github.com/staytomorrow/FindTrain)
 
 灵感来源
 
-### [12306](https://www.12306.cn)
+### [MoeFactory 提供的查询 API](https://train.moefactory.com/)
 
 数据来源
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
+## 📝 更新日志
 
-  </details>
+### 0.2.2
 
-## 📝 更新日志
+- 修复列车行驶进度条计算问题（fix by [@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)）
 
 ### 0.2.1
 
 - 适配 [MoeFactory API](https://train.moefactory.com)
 - 新增配置项 `CNRAIL_ACG_IMAGE_URL`
 
 ### 0.2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.2.dev1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.2.post1 Summary:
 NoneBot2 plugin for query the train time table Home-page: https://github.com/
 lgc-NB2Dev/nonebot-plugin-cnrail Author-Email: student_2333
 126.com>, XieXiLin
 xiexilin.com> License: MIT Project-URL: Homepage, https://github.com/lgc-
 NB2Dev/nonebot-plugin-cnrail Requires-Python: <4.0,>=3.9 Requires-Dist:
 nonebot2>=2.2.0 Requires-Dist: httpx>=0.24 Requires-Dist: nonebot-plugin-
 alconna>=0.40.1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.2 Requires-Dist:
@@ -24,27 +24,27 @@
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_cnrail" ] ``` ## âï¸ éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼
 | è¯´æ | | :--------------------: | :--: | :-------------------------------:
 | :----------------------------: | | `CNRAIL_ACG_IMAGE_URL` | å¦ | `https://
 www.loliapi.com/acg/pe/` | ç¨äºæä»¤è¿åå¾çèæ¯çå¾ç URL | ##
 ð ä½¿ç¨ ä½¿ç¨æä»¤ `train -h` æ¥çå¸®å© ### ææå¾ ![ææå¾]
-(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/g3720.png) ##
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cnrail/t301.png) ##
 ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [æµ·å°å¾·å°å©æ](https://qun.qq.com/qunpro/
-robot/qunshare?robot_uin=3889001607) & [Train-QQbot æä»¶](https://github.com/
-staytomorrow/FindTrain) çµææ¥æº ### [12306](https://www.12306.cn)
-æ°æ®æ¥æº ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.1 - éé [MoeFactory API]
-(https://train.moefactory.com) - æ°å¢éç½®é¡¹ `CNRAIL_ACG_IMAGE_URL` ###
-0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ### 0.1.7 -
-æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ - bug fix
-### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 - ä¿®å¤ `-
-h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº ### 0.1.3 -
-fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/issues/2) ###
-0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~ åååæ¥ï¼
-### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢ ### 0.1.0 - ð
-Create this project
+robot/qunshare?robot_uin=3889001607) & [Train-QQBot æä»¶](https://github.com/
+staytomorrow/FindTrain) çµææ¥æº ### [MoeFactory æä¾çæ¥è¯¢ API]
+(https://train.moefactory.com/) æ°æ®æ¥æº ## ð° èµå© **[èµå©æ]
+(https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.2 - ä¿®å¤åè½¦è¡é©¶è¿åº¦æ¡è®¡ç®é®é¢ï¼fix by
+[@This-is-XiaoDeng](https://github.com/This-is-XiaoDeng)ï¼ ### 0.2.1 - éé
+[MoeFactory API](https://train.moefactory.com) - æ°å¢éç½®é¡¹
+`CNRAIL_ACG_IMAGE_URL` ### 0.2.0 - éé Pydantic V1 & V2 - æ ·å¼å¾®è° ###
+0.1.7 - æ·»å è½¦ç»å·æ¾ç¤ºï¼æ æ³æ¾ç¤ºæªæ¥æ¥æçè½¦ç»å·ä¿¡æ¯ï¼ -
+bug fix ### 0.1.6 - æ·»å æå½è·¯å±æ¾ç¤º & æ¹æ¬¡åè½¦æ¥è¯¢ ### 0.1.5 -
+ä¿®å¤ `-h` åæ°æ æçé®é¢ ### 0.1.4 - ç°å¨ç¼ºå°åæ°ä¼æç¤ºäº
+### 0.1.3 - fix [#2](https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail/
+issues/2) ### 0.1.2 - æ¯æéæ©æ¥ææ¥è¯¢ï¼æ¥æèå´ä¸ºåäºæ¥ ~
+åååæ¥ï¼ ### 0.1.1 - ä¿®å¤æ¥è¯¢å°å¤ä¸ªè½¦æ¬¡ä¸ä¼æç¤ºçé®é¢
+### 0.1.0 - ð Create this project
```

