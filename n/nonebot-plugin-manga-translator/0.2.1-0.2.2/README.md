# Comparing `tmp/nonebot_plugin_manga_translator-0.2.1.tar.gz` & `tmp/nonebot_plugin_manga_translator-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_manga_translator-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_manga_translator-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_manga_translator-0.2.1.tar` & `nonebot_plugin_manga_translator-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-28 11:34:18.648225 nonebot_plugin_manga_translator-0.2.1/LICENSE
--rw-r--r--   0        0        0     9353 2024-04-28 11:34:18.648225 nonebot_plugin_manga_translator-0.2.1/README.md
--rw-r--r--   0        0        0     6922 2024-04-28 11:34:18.648225 nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/__init__.py
--rw-r--r--   0        0        0      309 2024-04-28 11:34:18.652225 nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/config.py
--rw-r--r--   0        0        0    10693 2024-04-28 11:34:18.652225 nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/utils.py
--rw-r--r--   0        0        0      524 2024-04-28 11:34:18.652225 nonebot_plugin_manga_translator-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10157 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-03 05:53:45.795697 nonebot_plugin_manga_translator-0.2.2/LICENSE
+-rw-r--r--   0        0        0     9408 2024-05-03 05:53:45.795697 nonebot_plugin_manga_translator-0.2.2/README.md
+-rw-r--r--   0        0        0     6881 2024-05-03 05:53:45.795697 nonebot_plugin_manga_translator-0.2.2/nonebot_plugin_manga_translator/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-03 05:53:45.795697 nonebot_plugin_manga_translator-0.2.2/nonebot_plugin_manga_translator/config.py
+-rw-r--r--   0        0        0    11639 2024-05-03 05:53:45.795697 nonebot_plugin_manga_translator-0.2.2/nonebot_plugin_manga_translator/utils.py
+-rw-r--r--   0        0        0      524 2024-05-03 05:53:45.795697 nonebot_plugin_manga_translator-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10212 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_manga_translator-0.2.1/LICENSE` & `nonebot_plugin_manga_translator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.2.1/README.md` & `nonebot_plugin_manga_translator-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,20 +106,20 @@
 (该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
 
    1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
    2. 安装好依赖后，在仓库目录下运行
 
       ```python
       python -m manga_translator -v --mode web --use-cuda
-      # the demo will be serving on http://127.0.0.1:5003
+      # the demo will be serving on http://127.0.0.1:5003，此时会提供一个网页，可以点击打开
       ```
 
    3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
 
-   4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
+   4. 你可以访问控制台给出的网址，**尝试先本地翻译一张图片**，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
    5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
    6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
 
 </details>
 
 ## 🎉命令
```

#### html2text {}

```diff
@@ -53,19 +53,20 @@
 åå«æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶ ç¦»çº¿ç¿»è¯
 (è¯¥æ¹æ¡å¯¹è®¾å¤éç½®è¦æ±è¾é«ï¼å»ºè®®å¨æè¶³å¤çç¡¬çç©ºé´ãåå­ãæ¾å­ï¼ææä¸å°è½ä¸ºbotå¤çè¯·æ±çæå¡å¨æ¶èèä½¿ç¨è¯¥æ¹æ¡)
 1. åè[manga-image-translator](https://github.com/zyddnys/manga-image-
 translator)çè¯´æï¼åéä»åºï¼å¹¶å®è£ç¸å³ä¾èµ
 (å¯è½éè¦é¢å¤å®è£`pydensecrf`) 2.
 å®è£å¥½ä¾èµåï¼å¨ä»åºç®å½ä¸è¿è¡ ```python python -
 m manga_translator -v --mode web --use-cuda # the demo will be serving on http:
-//127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
+//127.0.0.1:5003ï¼æ­¤æ¶ä¼æä¾ä¸ä¸ªç½é¡µï¼å¯ä»¥ç¹å»æå¼ ``` 3.
+å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
 (è¦æ±pytorchççæ¬åcudaå¯¹åºï¼ä¸å¯¹åºè¯·éè£)ï¼è¯·å»æåæ°`--
 use-cuda`ï¼å¦æå¾çå¤çè¿ç¨ä¸­çæ¾å­ï¼è¯·æ¹æ`--use-cuda-
 limited` 4.
-ä½ å¯ä»¥è®¿é®æ§å¶å°ç»åºçç½åï¼å°è¯åæ¬å°ç¿»è¯ä¸å¼ å¾çï¼æ­¤æ¶ä¼æ ¹æ®éé¡¹ä¸è½½éè¦çæ¨¡å
+ä½ å¯ä»¥è®¿é®æ§å¶å°ç»åºçç½åï¼**å°è¯åæ¬å°ç¿»è¯ä¸å¼ å¾ç**ï¼æ­¤æ¶ä¼æ ¹æ®éé¡¹ä¸è½½éè¦çæ¨¡å
 (ä¸ºé²æ­¢ä¸è½½å¤±è´¥ï¼ä¹å¯ä»¥æåæå¨ä¸è½½) 5.
 å¦æbotåç¿»è¯å¨å¨åä¸å°è®¾å¤ï¼é£ä¹.envå¡«å`offline_url="http://
 127.0.0.1:
 5003"`å³å¯ï¼å¦æä¸å¨åä¸å°è®¾å¤ï¼ä½ **å¯è½**è¿éè¦æ¾è¡é²ç«å¢ãç«¯å£è½¬åç­ï¼å¹¶ä¸å¡«ååå®¹ä¹ä¼ææåå
 6.
 æåä½ **å¯è½**è¿éè¦ä¿®æ¹ä¸ä¸æ¬æä»¶çä»£ç ï¼æ¾å°æ¬æä»¶`utils.py`ç`offline`å½æ°ï¼æ ¹æ®æ³¨éå
 [ææ¡£](https://github.com/zyddnys/manga-image-translator/blob/main/
```

### Comparing `nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/__init__.py` & `nonebot_plugin_manga_translator-0.2.2/nonebot_plugin_manga_translator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from nonebot.exception import MatcherException
-from nonebot.params import CommandArg, Arg, ArgPlainText
+from nonebot.params import CommandArg, ArgPlainText
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot import on_command, logger, get_plugin_config, require
 from nonebot.adapters import Message, Event, Bot
 from datetime import datetime
 from typing import List
 
 require("nonebot_plugin_alconna")
 
 from nonebot_plugin_alconna import CustomNode, Image, Reference, UniMessage
 from nonebot_plugin_alconna.uniseg.tools import image_fetch, reply_fetch
 from nonebot_plugin_alconna.uniseg import UniMsg, Reply
-from .utils import MangaTranslator, BytesIO
+from .utils import MangaTranslator
 from .config import Config
 
 
 __plugin_meta__ = PluginMetadata(
     name="图片翻译",
     description="利用api翻译图片并返回翻译后的图片",
     usage="""指令：
@@ -70,30 +70,29 @@
     event: Event,
     state: T_State,
     matcher: Matcher,
 ):
     if msg.has(Reply):
         if (reply := await reply_fetch(event, bot)) and reply.msg:
             reply_msg = reply.msg
-            uni_msg_with_reply = UniMessage.generate_without_reply(message=reply_msg)
+            uni_msg_with_reply = UniMessage.generate_without_reply(message=reply_msg) # type: ignore
         msg.extend(uni_msg_with_reply)
-
     if img_list := await extract_images(bot=bot, event=event, state=state, msg=msg):
-        matcher.set_arg("img_list", img_list)
+        state["img_list"]=img_list
 
 
 @pictrans.got("img_list", prompt="请发送要翻译的图片")
 async def handle_event(
     bot: Bot,
     msg: UniMsg,
     event: Event,
     state: T_State,
-    img_list: list = Arg(),
 ):
     try:
+        img_list = state["img_list"]
         img_url_list = await extract_images(bot=bot, event=event, state=state, msg=msg)
         if not img_url_list:
             img_url_list = img_list
         result = await manga_trans.call_api(img_url_list[0])
         await pictrans.send(message=f"翻译完成,当前api:{result[1]}")
         await UniMessage.image(raw=result[0]).send()
     except MatcherException:
@@ -108,20 +107,20 @@
     bot: Bot,
     msg: UniMsg,
     event: Event,
     state: T_State,
     matcher: Matcher,
 ):
     if img_list := await extract_images(bot=bot, event=event, state=state, msg=msg):
-        matcher.set_arg("img_list", img_list)
+        state["img_list"] = img_list
 
 
 @mul_pictrans.got("img_list", prompt="请发送要翻译的图片，发送/退出以退出多图片模式")
 async def _(
-    bot: Bot, msg: UniMsg, event: Event, state: T_State, img_list: list = Arg()
+    bot: Bot, msg: UniMsg, event: Event, state: T_State
 ):
 
     if new_list := await extract_images(bot=bot, event=event, state=state, msg=msg):
         manga_trans.img_url.extend(new_list)
         await mul_pictrans.reject("请继续发送图片，若想退出请发送/退出")
     else:
         await mul_pictrans.send("图片接收完毕，处理中")
@@ -129,37 +128,37 @@
     for img_url in manga_trans.img_url:
         result = await manga_trans.call_api(img_url)
         imgs.append(result[0])
 
     try:
         await send_forward_msg(bot, event, imgs)
     except Exception as e:
-        logger.warning("无法发送合并消息")
+        logger.warning(f"无法发送合并消息：{e}")
         for img in imgs:
             await UniMessage.image(raw=img).send()
     manga_trans.img_url.clear()
 
 
 async def extract_images(
     bot: Bot, event: Event, state: T_State, msg: UniMsg
-) -> List[BytesIO]:
+) -> List[bytes]:
     imgs = []
     for msg_seg in msg:
         if isinstance(msg_seg, Image):
             imgs.append(
                 await image_fetch(bot=bot, event=event, state=state, img=msg_seg)
             )
 
     return imgs
 
 
 async def send_forward_msg(
     bot: Bot,
     event: Event,
-    images: List[BytesIO],
+    images: List[bytes],
 ):
     try:
         from nonebot.adapters.onebot.v11 import Bot as V11Bot
         from nonebot.adapters.onebot.v11 import Event as V11Event
         from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
         from nonebot.adapters.onebot.v11 import Message as V11Msg
         from nonebot.adapters.onebot.v11 import MessageSegment as V11MsgSeg
@@ -198,15 +197,13 @@
 
     except ImportError:
         pass
 
     uid = bot.self_id
     name = "翻译姬"
     time = datetime.now()
-    await UniMessage(
-        Reference(
-            content=[
-                CustomNode(uid, name, time, await UniMessage.image(raw=img).export())
-                for img in images
-            ]
-        )
-    ).send()
+    forward_msg = Reference()
+    forward_msg._children = [
+        CustomNode(uid, name, time, await UniMessage.image(raw=img).export())
+        for img in images
+    ]
+    await UniMessage(forward_msg).send()
```

### Comparing `nonebot_plugin_manga_translator-0.2.1/nonebot_plugin_manga_translator/utils.py` & `nonebot_plugin_manga_translator-0.2.2/nonebot_plugin_manga_translator/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import asyncio
 import time
 import json
 import datetime
 import hashlib
 import hmac
 from urllib.parse import quote
-
-
+from typing import Tuple, Union
+from .config import Config
 class MangaTranslator:
 
-    def __init__(self, Config) -> None:
+    def __init__(self, Config:Config) -> None:
         self.config = Config
         self.img_url = []
         self.api = []
         if self.config.youdao_app_key:
             self.api.append(self.youdao)
             logger.info("检测到有道API")
         if self.config.baidu_app_id:
@@ -30,24 +30,24 @@
         if self.config.offline_url:
             self.api.append(self.offline)
             logger.info("检测到离线模型")
         if self.config.huoshan_access_key_id:
             self.api.append(self.huoshan)
             logger.info("检测到火山API")
 
-    async def call_api(self, image_bytes):
+    async def call_api(self, image_bytes:bytes)->Tuple[Union[None,bytes],str]:
         for api in self.api:
             try:
                 result = await api(image_bytes)
                 return result
             except httpx.HTTPError as e:
                 logger.warning(f"API[{api.__name__}]不可用：{e}尝试切换下一个")
         return None, "无可用API"
 
-    async def youdao(self, image_bytes):
+    async def youdao(self, image_bytes) -> Tuple[bytes, str]:
         """有道翻译"""
         salt = str(uuid.uuid1())
         data = {
             "from": "auto",
             "to": "zh-CHS",
             "type": "1",
             "appKey": self.config.youdao_app_key,
@@ -68,15 +68,15 @@
             youdao_res = await client.post(
                 url="https://openapi.youdao.com/ocrtransapi", data=data, headers=headers
             )
             img_base64 = youdao_res.json()["render_image"]
             pic = base64.b64decode(img_base64)
         return pic, "有道"
 
-    async def baidu(self, image_bytes):
+    async def baidu(self, image_bytes:bytes)->Tuple[bytes,str]:
         """百度翻译"""
         async with httpx.AsyncClient() as client:
             salt = random.randint(32768, 65536)
             image_data = image_bytes
             image_size = len(image_data)
             if image_size >= 4 * 1024 * 1024:
                 logger.info("图片过大，进行压缩")
@@ -108,52 +108,55 @@
                 params=payload,
                 files=image,
             )
             img_base64 = baidu_res.json()["data"]["pasteImg"]
             pic = base64.b64decode(img_base64)
         return pic, "百度"
 
-    async def offline(self, image_bytes, timeout=60):
+    async def offline(self, image_bytes:bytes, timeout=60)->Tuple[Union[None,bytes],str]:
         """离线翻译,这里写的有点烂，求pr"""
         async with httpx.AsyncClient() as client:
             img_content = image_bytes
             form = {"file": ("image.png", img_content, "image/png")}
             response = await client.post(
                 self.config.offline_url + "/submit",
                 files=form,
                 data={"translator": "offline"},
             )  # 改为本地翻译器
             # 这里的填写请参考文档，根据自己情况填写，例如data={"translator":"youdao","tgt_lang":"CHS"},如果是有道、百度、gpt等，请确保填写了key
             response.raise_for_status()  # 检查响应状态
             task_id = response.json()["task_id"]
             req = {"taskid": task_id}
             # 轮询获取翻译结果，超时时间为60s
-            start_time = time.monotonic()
-            while True:
-                response = await client.get(
-                    self.config.offline_url + "/task-state", params=req
+            async def check_translation_result() -> Tuple[Union[None, bytes], str]:
+                start_time = time.monotonic()
+                while True:
+                    response = await client.get(
+                        self.config.offline_url + "/task-state", params=req
+                    )
+                    response.raise_for_status()
+                    state = response.json()["state"]
+                    finished = response.json()["finished"]
+                    if state == "finished" or finished:
+                        break
+                    if time.monotonic() - start_time > timeout:
+                        return None, "超时"
+                    await asyncio.sleep(1)
+
+                img_data = await client.get(
+                    url=self.config.offline_url + "/result/" + task_id
                 )
-                logger.debug(response.content)
-                response.raise_for_status()
-                state = response.json()["state"]
-                finished = response.json()["finished"]
-                if state == "finished" or finished:
-                    break
-                if time.monotonic() - start_time > timeout:
-                    return None, "超时"
-                await asyncio.sleep(1)
-            img_data = await client.get(
-                url=self.config.offline_url + "/result/" + task_id
-            )
-            if img_data.status_code == 200 and img_data.content:
-                return img_data.content, "离线"
-            else:
-                return None, "离线"
+                if img_data.status_code == 200 and img_data.content:
+                    return img_data.content, "离线"
+                else:
+                    return None, "离线"
 
-    async def huoshan(self, image_bytes):
+            return await check_translation_result()
+
+    async def huoshan(self, image_bytes:bytes)->Tuple[bytes,str]:
         """火山引擎翻译，构建签名"""
         async with httpx.AsyncClient() as client:
             data = json.dumps(
                 {
                     "Image": str(base64.b64encode(image_bytes), encoding="utf-8"),
                     "TargetLanguage": "zh",
                 }
@@ -223,30 +226,28 @@
                 ),
             }
             params = {"Action": "TranslateImage", "Version": "2020-07-01"}
             huoshan_res = await client.post(
                 url="https://open.volcengineapi.com/",
                 headers=sign_result,
                 params=params,
-                data=data,
+                data=data, # type: ignore
             )
             img_base64 = huoshan_res.json()["Image"]
             pic = base64.b64decode(img_base64)
         return pic, "火山"
 
     @staticmethod
-    def compress_image(image_data):
-        with BytesIO(image_data) as input:
-            image = Image.open(input)
-            image = image.convert("RGB")
-            image = image.resize(
-                (int(image.width * 0.5), int(image.height * 0.5)), Image.ANTIALIAS
-            )
-            image.save(input, format="JPEG", quality=80)
-            return input.getvalue()
+    def compress_image(image_data: bytes) -> bytes:
+        with BytesIO(image_data) as input_buffer:
+            with Image.open(input_buffer) as image:
+                # image = image.resize((int(image.width * 0.5), int(image.height * 0.5)))
+                output_buffer = BytesIO()
+                image.save(output_buffer, format="JPEG", optimize=True, quality=80)
+                return output_buffer.getvalue()
 
     @staticmethod
     def encrypt(signStr):
         hash_algorithm = md5()
         hash_algorithm.update(signStr.encode("utf-8"))
         return hash_algorithm.hexdigest()
 
@@ -277,7 +278,23 @@
                 )
         query = query[:-1]
         return query.replace("+", "%20")
 
     @staticmethod
     def hmac_sha256(key: bytes, content: str):
         return hmac.new(key, content.encode("utf-8"), hashlib.sha256).digest()
+
+
+if __name__=="__main__":
+    def generate_large_white_image():
+        width = 4000
+        height = 4000
+        image = Image.new("RGB", (width, height), (255, 255, 255))
+        output_buffer = BytesIO()
+        image.save(output_buffer, format="JPEG")
+        return output_buffer.getvalue()
+
+    image_data = generate_large_white_image()
+    print("原始图像大小:", len(image_data))
+
+    compressed_data = MangaTranslator.compress_image(image_data)
+    print("压缩后图像大小:", len(compressed_data))
```

### Comparing `nonebot_plugin_manga_translator-0.2.1/pyproject.toml` & `nonebot_plugin_manga_translator-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-manga-translator"
-version = "0.2.1"
+version = "0.2.2"
 description = "基于nonebot2的适配多种api的图片/漫画翻译插件"
 authors = ["xenophon <674550338@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_manga_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_manga_translator-0.2.1/PKG-INFO` & `nonebot_plugin_manga_translator-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-manga-translator
-Version: 0.2.1
+Version: 0.2.2
 Summary: 基于nonebot2的适配多种api的图片/漫画翻译插件
 License: MIT
 Author: xenophon
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -127,20 +127,20 @@
 (该方案对设备配置要求较高，建议在有足够的硬盘空间、内存、显存，或有一台能为bot处理请求的服务器时考虑使用该方案)
 
    1. 参考[manga-image-translator](https://github.com/zyddnys/manga-image-translator)的说明，克隆仓库，并安装相关依赖(可能需要额外安装`pydensecrf`)
    2. 安装好依赖后，在仓库目录下运行
 
       ```python
       python -m manga_translator -v --mode web --use-cuda
-      # the demo will be serving on http://127.0.0.1:5003
+      # the demo will be serving on http://127.0.0.1:5003，此时会提供一个网页，可以点击打开
       ```
 
    3. 如果你的设备没有成功安装cuda(要求pytorch的版本和cuda对应，不对应请重装)，请去掉参数`--use-cuda`，如果图片处理过程中爆显存，请改成`--use-cuda-limited`
 
-   4. 你可以访问控制台给出的网址，尝试先本地翻译一张图片，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
+   4. 你可以访问控制台给出的网址，**尝试先本地翻译一张图片**，此时会根据选项下载需要的模型(为防止下载失败，也可以提前手动下载)
    5. 如果bot和翻译器在同一台设备，那么.env填写`offline_url="http://127.0.0.1:5003"`即可，如果不在同一台设备，你**可能**还需要放行防火墙、端口转发等，并且填写内容也会有所变化
    6. 最后你**可能**还需要修改一下本插件的代码，找到本插件`utils.py`的`offline`函数，根据注释和[文档](https://github.com/zyddnys/manga-image-translator/blob/main/README.md),修改字典`data`，从而指定你想要的OCR模型和翻译模型(目前是用了offline模型,你可以改成别的)
 
 </details>
 
 ## 🎉命令
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.2.1
+Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.2.2
 Summary: åºäºnonebot2çééå¤ç§apiçå¾ç/æ¼«ç»ç¿»è¯æä»¶ License:
 MIT Author: xenophon Author-email: 674550338@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: Pillow
@@ -64,19 +64,20 @@
 åå«æ ¹æ®ä¸é¢çéç½®è¯´æå¡«å¥.env.*æä»¶ ç¦»çº¿ç¿»è¯
 (è¯¥æ¹æ¡å¯¹è®¾å¤éç½®è¦æ±è¾é«ï¼å»ºè®®å¨æè¶³å¤çç¡¬çç©ºé´ãåå­ãæ¾å­ï¼ææä¸å°è½ä¸ºbotå¤çè¯·æ±çæå¡å¨æ¶èèä½¿ç¨è¯¥æ¹æ¡)
 1. åè[manga-image-translator](https://github.com/zyddnys/manga-image-
 translator)çè¯´æï¼åéä»åºï¼å¹¶å®è£ç¸å³ä¾èµ
 (å¯è½éè¦é¢å¤å®è£`pydensecrf`) 2.
 å®è£å¥½ä¾èµåï¼å¨ä»åºç®å½ä¸è¿è¡ ```python python -
 m manga_translator -v --mode web --use-cuda # the demo will be serving on http:
-//127.0.0.1:5003 ``` 3. å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
+//127.0.0.1:5003ï¼æ­¤æ¶ä¼æä¾ä¸ä¸ªç½é¡µï¼å¯ä»¥ç¹å»æå¼ ``` 3.
+å¦æä½ çè®¾å¤æ²¡ææåå®è£cuda
 (è¦æ±pytorchççæ¬åcudaå¯¹åºï¼ä¸å¯¹åºè¯·éè£)ï¼è¯·å»æåæ°`--
 use-cuda`ï¼å¦æå¾çå¤çè¿ç¨ä¸­çæ¾å­ï¼è¯·æ¹æ`--use-cuda-
 limited` 4.
-ä½ å¯ä»¥è®¿é®æ§å¶å°ç»åºçç½åï¼å°è¯åæ¬å°ç¿»è¯ä¸å¼ å¾çï¼æ­¤æ¶ä¼æ ¹æ®éé¡¹ä¸è½½éè¦çæ¨¡å
+ä½ å¯ä»¥è®¿é®æ§å¶å°ç»åºçç½åï¼**å°è¯åæ¬å°ç¿»è¯ä¸å¼ å¾ç**ï¼æ­¤æ¶ä¼æ ¹æ®éé¡¹ä¸è½½éè¦çæ¨¡å
 (ä¸ºé²æ­¢ä¸è½½å¤±è´¥ï¼ä¹å¯ä»¥æåæå¨ä¸è½½) 5.
 å¦æbotåç¿»è¯å¨å¨åä¸å°è®¾å¤ï¼é£ä¹.envå¡«å`offline_url="http://
 127.0.0.1:
 5003"`å³å¯ï¼å¦æä¸å¨åä¸å°è®¾å¤ï¼ä½ **å¯è½**è¿éè¦æ¾è¡é²ç«å¢ãç«¯å£è½¬åç­ï¼å¹¶ä¸å¡«ååå®¹ä¹ä¼ææåå
 6.
 æåä½ **å¯è½**è¿éè¦ä¿®æ¹ä¸ä¸æ¬æä»¶çä»£ç ï¼æ¾å°æ¬æä»¶`utils.py`ç`offline`å½æ°ï¼æ ¹æ®æ³¨éå
 [ææ¡£](https://github.com/zyddnys/manga-image-translator/blob/main/
```

