# Comparing `tmp/nonebot_plugin_steam_info-0.2.0.tar.gz` & `tmp/nonebot_plugin_steam_info-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_steam_info-0.2.0.tar", last modified: Sat Apr 27 05:27:48 2024, max compression
+gzip compressed data, was "nonebot_plugin_steam_info-0.3.0.tar", last modified: Fri May  3 14:26:02 2024, max compression
```

## Comparing `nonebot_plugin_steam_info-0.2.0.tar` & `nonebot_plugin_steam_info-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1062 2024-04-27 05:27:23.457559 nonebot_plugin_steam_info-0.2.0/LICENSE
--rw-r--r--   0        0        0     2380 2024-04-27 05:27:23.457559 nonebot_plugin_steam_info-0.2.0/README.md
--rw-r--r--   0        0        0     9520 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/__init__.py
--rw-r--r--   0        0        0      152 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/config.py
--rw-r--r--   0        0        0     6254 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/data_source.py
--rw-r--r--   0        0        0    12428 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/draw.py
--rw-r--r--   0        0        0      572 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/models.py
--rw-r--r--   0        0        0      552 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/busy.png
--rw-r--r--   0        0        0     1847 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/friends_search.png
--rw-r--r--   0        0        0     7467 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/parent_status.png
--rw-r--r--   0        0        0     3409 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg
--rw-r--r--   0        0        0      533 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_gaming.png
--rw-r--r--   0        0        0      536 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_online.png
--rw-r--r--   0        0        0     1209 2024-04-27 05:27:23.613558 nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/steam.py
--rw-r--r--   0        0        0      580 2024-04-27 05:27:48.861264 nonebot_plugin_steam_info-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-03 14:25:36.848723 nonebot_plugin_steam_info-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2560 2024-05-03 14:25:36.848723 nonebot_plugin_steam_info-0.3.0/README.md
+-rw-r--r--   0        0        0    11166 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/config.py
+-rw-r--r--   0        0        0     6705 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/data_source.py
+-rw-r--r--   0        0        0    13658 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/draw.py
+-rw-r--r--   0        0        0      572 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/models.py
+-rw-r--r--   0        0        0      552 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/busy.png
+-rw-r--r--   0        0        0     1847 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/friends_search.png
+-rw-r--r--   0        0        0     8807 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/gaming.png
+-rw-r--r--   0        0        0     7467 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/parent_status.png
+-rw-r--r--   0        0        0     3409 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg
+-rw-r--r--   0        0        0      533 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_gaming.png
+-rw-r--r--   0        0        0      536 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_online.png
+-rw-r--r--   0        0        0     1209 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/steam.py
+-rw-r--r--   0        0        0      580 2024-05-03 14:26:02.824605 nonebot_plugin_steam_info-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_steam_info-0.2.0/LICENSE` & `nonebot_plugin_steam_info-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/README.md` & `nonebot_plugin_steam_info-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - [x] 群友状态变更播报
 - [x] 主动查询群友状态
 
 ## 预览
 仿照了 Steam 好友列表的样式
 
 ![image](./preview.png)
+![image](./preview_1.png)
 
 ## 使用
 | 命令 | 别名 |  说明 |
 | --- | --- | --- |
 | steambind [Steam ID 或 Steam好友代码] | 绑定steam | 绑定 Steam |
 | steamunbind | 解绑steam | 解绑 Steam |
 | steaminfo | steam信息 | 查看绑定信息 |
@@ -71,13 +72,14 @@
 在 .env 文件中配置以下内容
 
 | 配置项 | 默认值 | 说明 |
 | --- | --- | --- |
 | STEAM_API_KEY | 无 | Steam API Key，可在 [此处](https://partner.steamgames.com/doc/webapi_overview/auth) 获取 |
 | PROXY | 无 | 代理地址 |
 | STEAM_REQUEST_INTERVAL | 300 | Steam 请求间隔 & 播报间隔。单位为秒 |
+| STEAM_BROADCAST_TYPE | `"part"` | 播报类型。`"part"` 为部分播报(图 2)，`"all"` 为全部播报(图 1)，`"none"` 为只播报文字消息 |
 
 最后再把仓库中 `fonts` 文件夹下的字体文件放到 Bot 的 **运行目录** 下，配置就完毕啦
 
 > 这里使用了 MiSans 字体，感谢 [MiSans](https://hyperos.mi.com/font/zh/)
 
 >如果你希望使用其他字体，请在 `draw.py` 中，将 `font_regular_path`, `font_light_path` 和 `font_bold_path` 修改为你的字体文件路径
```

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/__init__.py` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 require("nonebot_plugin_apscheduler")
 
 import nonebot_plugin_localstore as store
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_alconna import Text, Image, UniMessage, Target
 
 from .config import Config
-from .models import PlayerSummaries
+from .models import PlayerSummaries, Player
 from .steam import get_steam_id, get_steam_users_info, STEAM_ID_OFFSET
 from .data_source import BindData, SteamInfoData, ParentData, DisableParentData
 from .draw import (
     check_font,
+    fetch_avatar,
     image_to_bytes,
+    draw_start_gaming,
     draw_friends_status,
     simplize_steam_player_data,
+    vertically_concatenate_images,
 )
 
 
 __plugin_meta__ = PluginMetadata(
     name="Steam Info",
     description="播报绑定的 Steam 好友状态",
     usage="绑定 Steam ID: steambind [Steam ID 或 Steam好友代码]\n解绑 Steam ID: steamunbind\n查看 Steam ID: steaminfo\n查看 Steam 好友状态: steamcheck\n启用 Steam 播报: steamenable\n禁用 Steam 播报: steamdisable\n更新群信息: steamupdate",
@@ -111,29 +114,57 @@
 
 async def broadcast_steam_info(parent_id: str, steam_info: PlayerSummaries):
     if disable_parent_data.is_disabled(parent_id):
         return None
 
     bot = nonebot.get_bot()
 
-    msg = steam_info_data.compare(parent_id, steam_info["response"])
+    play_data = steam_info_data.compare(parent_id, steam_info["response"])
+
+    msg = []
+    for entry in play_data:
+        player: Player = entry["player"]
+        old_player: Player = entry.get("old_player")
+
+        if entry["type"] == "start":
+            msg.append(f"{player['personaname']} 开始玩 {player['gameextrainfo']} 了")
+        elif entry["type"] == "stop":
+            msg.append(f"{player['personaname']} 停止玩 {old_player['gameextrainfo']} 了")
+        elif entry["type"] == "change":
+            msg.append(
+                f"{player['personaname']} 停止玩 {old_player['gameextrainfo']}，开始玩 {player['gameextrainfo']} 了"
+            )
+        elif entry["type"] == "error":
+            f"出现错误！{player['personaname']}\nNew: {player.get('gameextrainfo')}\nOld: {old_player.get('gameextrainfo')}"
+        else:
+            logger.error(f"未知的播报类型: {entry['type']}")
 
     if msg == []:
         return None
 
-    steam_status_data = [
-        await simplize_steam_player_data(player, config.proxy, avatar_path)
-        for player in steam_info["response"]["players"]
-    ]
-
-    parent_avatar, parent_name = parent_data.get(parent_id)
-
-    image = draw_friends_status(parent_avatar, parent_name, steam_status_data)
+    if config.steam_broadcast_type == "all":
+        steam_status_data = [
+            await simplize_steam_player_data(player, config.proxy, avatar_path)
+            for player in steam_info["response"]["players"]
+        ]
+
+        parent_avatar, parent_name = parent_data.get(parent_id)
+        image = draw_friends_status(parent_avatar, parent_name, steam_status_data)
+        uni_msg = UniMessage([Text("\n".join(msg)), Image(raw=image_to_bytes(image))])
+    elif config.steam_broadcast_type == "part":
+        images = [draw_start_gaming((await fetch_avatar(entry["player"], avatar_path, config.proxy)), entry["player"]["personaname"], entry["player"]["gameextrainfo"]) for entry in play_data if entry["type"] == "start"]
+        if images == []:
+            uni_msg = UniMessage([Text("\n".join(msg))])
+        else:
+            image = vertically_concatenate_images(images) if len(images) > 1 else images[0]
+            uni_msg = UniMessage([Text("\n".join(msg)), Image(raw=image_to_bytes(image))])
+    else:
+        uni_msg = UniMessage([Text("\n".join(msg))])
 
-    await UniMessage([Text("\n".join(msg)), Image(raw=image_to_bytes(image))]).send(
+    await uni_msg.send(
         Target(parent_id, parent_id, True, False, "", bot.adapter.get_name()), bot
     )
 
 
 @nonebot.get_driver().on_bot_connect
 async def init_steam_info():
     for parent_id in bind_data.content:
```

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/data_source.py` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             json.dump(self.content, f, indent=4)
 
     def add(self, parent_id: str, content: Dict[str, str]) -> None:
         if parent_id not in self.content:
             self.content[parent_id] = [content]
         else:
             self.content[parent_id].append(content)
-    
+
     def remove(self, parent_id: str, user_id: str) -> None:
         if parent_id not in self.content:
             return
         for data in self.content[parent_id]:
             if data["user_id"] == user_id:
                 self.content[parent_id].remove(data)
                 break
@@ -92,30 +92,46 @@
 
         for player in new_content["players"]:
             for old_player in old_content["players"]:
                 if player["steamid"] == old_player["steamid"]:
                     if player.get("gameextrainfo") != old_player.get("gameextrainfo"):
                         if player.get("gameextrainfo") is not None:
                             result.append(
-                                f"{player['personaname']} 开始玩 {player['gameextrainfo']} 了"
+                                {
+                                    "type": "start",
+                                    "player": player,
+                                    "old_player": old_player,
+                                }
                             )
                         elif old_player.get("gameextrainfo") is not None:
                             result.append(
-                                f"{player['personaname']} 停止玩 {old_player['gameextrainfo']} 了"
+                                {
+                                    "type": "stop",
+                                    "player": player,
+                                    "old_player": old_player,
+                                }
                             )
                         elif (
                             player.get("gameextrainfo") is not None
                             and old_player.get("gameextrainfo") is not None
                         ):
                             result.append(
-                                f"{player['personaname']} 停止玩 {old_player['gameextrainfo']}，开始玩 {player['gameextrainfo']} 了"
+                                {
+                                    "type": "change",
+                                    "player": player,
+                                    "old_player": old_player,
+                                }
                             )
                         else:
                             result.append(
-                                f"出现错误！{player['personaname']}\nNew: {player.get('gameextrainfo')}\nOld: {old_player.get('gameextrainfo')}"
+                                {
+                                    "type": "error",
+                                    "player": player,
+                                    "old_player": old_player,
+                                }
                             )
         return result
 
 
 class ParentData:
     def __init__(self, save_path: Path) -> None:
         self.content: Dict[str, str] = {}  # parent_id: name
```

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/draw.py` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/draw.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 unknown_avatar_path = Path(__file__).parent / "res/unknown_avatar.jpg"
 parent_status_path = Path(__file__).parent / "res/parent_status.png"
 friends_search_path = Path(__file__).parent / "res/friends_search.png"
 busy_path = Path(__file__).parent / "res/busy.png"
 zzz_online_path = Path(__file__).parent / "res/zzz_online.png"
 zzz_gaming_path = Path(__file__).parent / "res/zzz_gaming.png"
+gaming_path = Path(__file__).parent / "res/gaming.png"
 
 font_regular_path = (Path().cwd() / "fonts/MiSans-Regular.ttf").resolve().__str__()
 font_light_path = (Path().cwd() / "fonts/MiSans-Light.ttf").resolve().__str__()
 font_bold_path = (Path().cwd() / "fonts/MiSans-Bold.ttf").resolve().__str__()
 
 
 def check_font():
@@ -30,36 +31,42 @@
         raise FileNotFoundError(f"Font file {font_regular_path} not found.")
     if not Path(font_light_path).exists():
         raise FileNotFoundError(f"Font file {font_light_path} not found.")
     if not Path(font_bold_path).exists():
         raise FileNotFoundError(f"Font file {font_bold_path} not found.")
 
 
-async def fetch_avatar(avatar_url: str, proxy: str = None) -> Image.Image:
+async def _fetch_avatar(avatar_url: str, proxy: str = None) -> Image.Image:
     async with aiohttp.ClientSession() as session:
         async with session.get(avatar_url, proxy=proxy) as resp:
             if resp.status != 200:
                 return Image.open(unknown_avatar_path)
             return Image.open(BytesIO(await resp.read()))
 
 
-async def simplize_steam_player_data(
-    player: Player, proxy: str = None, avatar_dir: Path = None
-) -> Dict[str, str]:
+async def fetch_avatar(player: Player, avatar_dir: Path, proxy: str = None) -> Image.Image:
     if avatar_dir is not None:
         avatar_path = avatar_dir / f"avatar_{player['steamid']}.png"
 
         if avatar_path.exists():
             avatar = Image.open(avatar_path)
         else:
-            avatar = await fetch_avatar(player["avatarfull"], proxy)
+            avatar = await _fetch_avatar(player["avatarfull"], proxy)
 
             avatar.save(avatar_path)
     else:
-        avatar = await fetch_avatar(player["avatarfull"], proxy)
+        avatar = await _fetch_avatar(player["avatarfull"], proxy)
+    
+    return avatar
+
+
+async def simplize_steam_player_data(
+    player: Player, proxy: str = None, avatar_dir: Path = None
+) -> Dict[str, str]:
+    avatar = await fetch_avatar(player, avatar_dir, proxy)
 
     if player["personastate"] == 0:
         if not player.get("lastlogoff"):
             status = "离线"
         else:
             time_logged_off = player["lastlogoff"]  # Unix timestamp
             time_to_now = calendar.timegm(time.gmtime()) - time_logged_off
@@ -75,23 +82,19 @@
                 status = f"上次在线 {time_to_now // 86400} 天前"
             elif time_to_now < 31536000:
                 status = f"上次在线 {time_to_now // 2592000} 个月前"
             else:
                 status = f"上次在线 {time_to_now // 31536000} 年前"
     elif player["personastate"] in [1, 2, 4]:
         status = (
-            "在线"
-            if player.get("gameextrainfo") is None
-            else player["gameextrainfo"]
+            "在线" if player.get("gameextrainfo") is None else player["gameextrainfo"]
         )
     elif player["personastate"] == 3:
         status = (
-            "离开"
-            if player.get("gameextrainfo") is None
-            else player["gameextrainfo"]
+            "离开" if player.get("gameextrainfo") is None else player["gameextrainfo"]
         )
     elif player["personastate"] in [5, 6]:
         status = "在线"
     else:
         status = "未知"
 
     return {
@@ -119,14 +122,46 @@
     3: (hex_to_rgb("45778e"), hex_to_rgb("365969")),
     4: (hex_to_rgb("6dcef5"), hex_to_rgb("4c91ac")),
     5: (hex_to_rgb("6dcef5"), hex_to_rgb("4c91ac")),
     6: (hex_to_rgb("6dcef5"), hex_to_rgb("4c91ac")),
 }
 
 
+def vertically_concatenate_images(images: List[Image.Image]) -> Image.Image:
+    widths, heights = zip(*(i.size for i in images))
+    total_width = max(widths)
+    total_height = sum(heights)
+
+    new_image = Image.new("RGB", (total_width, total_height))
+
+    y_offset = 0
+    for image in images:
+        new_image.paste(image, (0, y_offset))
+        y_offset += image.size[1]
+
+    return new_image
+
+
+def draw_start_gaming(avatar: Image.Image, friend_name: str, game_name: str):
+    canvas = Image.open(gaming_path)
+    canvas.paste(avatar.resize((66, 66), Image.BICUBIC), (15, 20))
+
+    # 绘制名称
+    draw = ImageDraw.Draw(canvas)
+    draw.text((104, 14), friend_name, font=ImageFont.truetype(font_regular_path, 19), fill=hex_to_rgb("e3ffc2"))
+
+    # 绘制"正在玩"
+    draw.text((103, 42), "正在玩", font=ImageFont.truetype(font_regular_path, 17), fill=hex_to_rgb("969696"))
+
+    # 绘制游戏名称
+    draw.text((104, 66), game_name, font=ImageFont.truetype(font_bold_path, 14), fill=hex_to_rgb("91c257"))
+
+    return canvas
+
+
 def draw_parent_status(parent_avatar: Image.Image, parent_name: str) -> Image.Image:
     parent_avatar = parent_avatar.resize(
         (PARENT_AVATAR_SIZE, PARENT_AVATAR_SIZE), Image.BICUBIC
     )
 
     canvas = Image.open(parent_status_path).resize((WIDTH, 120), Image.BICUBIC)
```

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/models.py` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/busy.png` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/busy.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/friends_search.png` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/friends_search.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/parent_status.png` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/parent_status.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_gaming.png` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_gaming.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/res/zzz_online.png` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_online.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/nonebot_plugin_steam_info/steam.py` & `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.2.0/pyproject.toml` & `nonebot_plugin_steam_info-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-steam-info"
-version = "0.2.0"
+version = "0.3.0"
 description = "Default template for PDM package"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
     "nonebot-plugin-alconna>=0.37.0",
```

### Comparing `nonebot_plugin_steam_info-0.2.0/PKG-INFO` & `nonebot_plugin_steam_info-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-steam-info
-Version: 0.2.0
+Version: 0.3.0
 Summary: Default template for PDM package
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: nonebot-plugin-alconna>=0.37.0
 Requires-Dist: aiohttp>=3.9.3
@@ -21,14 +21,15 @@
 - [x] 群友状态变更播报
 - [x] 主动查询群友状态
 
 ## 预览
 仿照了 Steam 好友列表的样式
 
 ![image](./preview.png)
+![image](./preview_1.png)
 
 ## 使用
 | 命令 | 别名 |  说明 |
 | --- | --- | --- |
 | steambind [Steam ID 或 Steam好友代码] | 绑定steam | 绑定 Steam |
 | steamunbind | 解绑steam | 解绑 Steam |
 | steaminfo | steam信息 | 查看绑定信息 |
@@ -86,13 +87,14 @@
 在 .env 文件中配置以下内容
 
 | 配置项 | 默认值 | 说明 |
 | --- | --- | --- |
 | STEAM_API_KEY | 无 | Steam API Key，可在 [此处](https://partner.steamgames.com/doc/webapi_overview/auth) 获取 |
 | PROXY | 无 | 代理地址 |
 | STEAM_REQUEST_INTERVAL | 300 | Steam 请求间隔 & 播报间隔。单位为秒 |
+| STEAM_BROADCAST_TYPE | `"part"` | 播报类型。`"part"` 为部分播报(图 2)，`"all"` 为全部播报(图 1)，`"none"` 为只播报文字消息 |
 
 最后再把仓库中 `fonts` 文件夹下的字体文件放到 Bot 的 **运行目录** 下，配置就完毕啦
 
 > 这里使用了 MiSans 字体，感谢 [MiSans](https://hyperos.mi.com/font/zh/)
 
 >如果你希望使用其他字体，请在 `draw.py` 中，将 `font_regular_path`, `font_light_path` 和 `font_bold_path` 修改为你的字体文件路径
```

