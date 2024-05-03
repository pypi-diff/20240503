# Comparing `tmp/linkai-0.0.5.0-py3-none-any.whl.zip` & `tmp/linkai-0.0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4956 bytes, number of entries: 10
+Zip file size: 4962 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      111 b- defN 24-Jan-06 15:46 linkai/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/_common/__init__.py
 -rw-r--r--  2.0 unx      717 b- defN 24-Apr-09 05:45 linkai/_common/log.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/api/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/api/client/__init__.py
--rw-r--r--  2.0 unx     9126 b- defN 24-Apr-09 07:26 linkai/api/client/client.py
--rw-r--r--  2.0 unx      516 b- defN 24-Apr-09 07:29 linkai-0.0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 07:29 linkai-0.0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-09 07:29 linkai-0.0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      774 b- defN 24-Apr-09 07:29 linkai-0.0.5.0.dist-info/RECORD
-10 files, 11343 bytes uncompressed, 3624 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx     9148 b- defN 24-May-03 10:51 linkai/api/client/client.py
+-rw-r--r--  2.0 unx      516 b- defN 24-May-03 10:56 linkai-0.0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 10:56 linkai-0.0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-03 10:56 linkai-0.0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      774 b- defN 24-May-03 10:56 linkai-0.0.6.0.dist-info/RECORD
+10 files, 11365 bytes uncompressed, 3630 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: linkai/api/client/__init__.py
 Comment: 
 
 Filename: linkai/api/client/client.py
 Comment: 
 
-Filename: linkai-0.0.5.0.dist-info/METADATA
+Filename: linkai-0.0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: linkai-0.0.5.0.dist-info/WHEEL
+Filename: linkai-0.0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: linkai-0.0.5.0.dist-info/top_level.txt
+Filename: linkai-0.0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: linkai-0.0.5.0.dist-info/RECORD
+Filename: linkai-0.0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## linkai/api/client/client.py

```diff
@@ -34,15 +34,15 @@
         self.session_id = session_id
         self.msg_content = msg_content
         self.is_group = is_group
 
 
 CLIENT_CONFIG_FILE = 'client_config.json'
 CLIENT_ID_KEY = "client_id"
-DEFAULT_HOST = "link-ai.chat"
+DEFAULT_HOST = "client.link-ai.tech"
 
 
 class LinkAIClient:
     def __init__(self, api_key: str, host: str = "", client_type: str = "", heartbeat_interval=30, reconnect_times=2, reconnect_interval=10):
         self.client_id = self.fetch_client_id()
         self.client_type = client_type
         self.api_key = api_key
@@ -264,10 +264,10 @@
         elif msg.get("type") == ClientMsgType.CONFIG.name:
             data = msg.get("data")
             logger.debug(f"Received config refresh: {msg}")  # 打印接收到的消息
             del data["channelId"]
             self.on_config(data)
 
     def check_host(self):
-        pattern = re.compile(r'^(.*\.)?(link-ai\.tech|link-ai\.chat|link-ai\.pro)$')
+        pattern = re.compile(r'^(.*\.)?(link-ai\.tech|link-ai\.chat|link-ai\.pro|link-ai\.cloud)$')
         if not bool(pattern.match(self.host)):
             raise RuntimeError("Can not connect")
```

## Comparing `linkai-0.0.5.0.dist-info/METADATA` & `linkai-0.0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkai
-Version: 0.0.5.0
+Version: 0.0.6.0
 Summary: LinkAI python sdk
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `linkai-0.0.5.0.dist-info/RECORD` & `linkai-0.0.6.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 linkai/__init__.py,sha256=JSbbcxuUYRUgT4EP-m3WKukCjakcoQJnJtsLlxUTKCY,111
 linkai/_common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 linkai/_common/log.py,sha256=e_mS6HxIuMbtVwC_RbVrOEIbE0tZH6VTMknkQkGMsfo,717
 linkai/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 linkai/api/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-linkai/api/client/client.py,sha256=1wH-CkSCRMfDCT5y3mn0z6fdyXxCDFT0U8b_g4f1esA,9126
-linkai-0.0.5.0.dist-info/METADATA,sha256=LalFGbQoKYdspnkuatN7hGkSfYZAvnhiLn7-o9RqaW0,516
-linkai-0.0.5.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-linkai-0.0.5.0.dist-info/top_level.txt,sha256=6gMseb-hjwjOWwaqKNCqTQzpa7ZQROxu4VUkP2JbT5g,7
-linkai-0.0.5.0.dist-info/RECORD,,
+linkai/api/client/client.py,sha256=nJtivtGwGADaOFR2390-gC1YPcdnWIXDjh_dvfjBmeo,9148
+linkai-0.0.6.0.dist-info/METADATA,sha256=LqEXkp-LOjeH4OIKKa0j6AbOL1CX9zRRAp5JNXSPA2E,516
+linkai-0.0.6.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+linkai-0.0.6.0.dist-info/top_level.txt,sha256=6gMseb-hjwjOWwaqKNCqTQzpa7ZQROxu4VUkP2JbT5g,7
+linkai-0.0.6.0.dist-info/RECORD,,
```

