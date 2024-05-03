# Comparing `tmp/RTS_WebUIBuilder-0.2.tar.gz` & `tmp/RTS-WebUIBuilder-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS_WebUIBuilder-0.2.tar", last modified: Mon Apr 29 17:32:06 2024, max compression
+gzip compressed data, was "RTS-WebUIBuilder-0.3.tar", last modified: Fri May  3 21:35:18 2024, max compression
```

## Comparing `RTS_WebUIBuilder-0.2.tar` & `RTS-WebUIBuilder-0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:32:05.998748 RTS_WebUIBuilder-0.2/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_WebUIBuilder-0.2/LICENCE
--rw-rw-rw-   0        0        0      823 2024-04-29 17:32:05.998242 RTS_WebUIBuilder-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-04-29 16:57:15.000000 RTS_WebUIBuilder-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:32:05.987326 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/
--rw-rw-rw-   0        0        0     1055 2024-04-15 18:28:33.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RAdditions.py
--rw-rw-rw-   0        0        0     2282 2024-04-29 16:01:41.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RBody.py
--rw-rw-rw-   0        0        0     2718 2024-04-28 15:20:36.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RBox.py
--rw-rw-rw-   0        0        0     3233 2024-04-29 15:07:44.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RDocument.py
--rw-rw-rw-   0        0        0     2320 2024-04-13 14:53:29.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RFrame.py
--rw-rw-rw-   0        0        0    10637 2024-04-24 17:48:28.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RGroupStyle.py
--rw-rw-rw-   0        0        0     1261 2024-04-13 14:44:52.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RHead.py
--rw-rw-rw-   0        0        0       92 2024-04-13 18:50:09.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RImage.py
--rw-rw-rw-   0        0        0     2754 2024-04-21 08:51:23.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RInput.py
--rw-rw-rw-   0        0        0      839 2024-04-26 21:26:34.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RLabel.py
--rw-rw-rw-   0        0        0      326 2024-04-27 16:51:27.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RQuickScripts.py
--rw-rw-rw-   0        0        0    10454 2024-04-24 17:44:53.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RStyle.py
--rw-rw-rw-   0        0        0      796 2024-04-28 18:56:26.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RTitle.py
--rw-rw-rw-   0        0        0     5839 2024-04-28 15:21:31.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RWebserver.py
--rw-rw-rw-   0        0        0     3523 2024-04-29 16:16:05.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RpyColorizer.py
--rw-rw-rw-   0        0        0      474 2024-04-29 14:58:45.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-13 17:25:24.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/cache.py
--rw-rw-rw-   0        0        0      888 2024-04-29 15:07:12.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/exeptional.py
--rw-rw-rw-   0        0        0     1015 2024-04-21 15:08:22.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/privatizehead.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:32:05.997233 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/
--rw-rw-rw-   0        0        0      823 2024-04-29 17:32:05.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2024-04-29 17:32:05.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:32:05.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 17:32:05.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 17:32:05.000000 RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 17:32:05.998748 RTS_WebUIBuilder-0.2/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-29 17:31:58.000000 RTS_WebUIBuilder-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:35:18.832833 RTS-WebUIBuilder-0.3/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS-WebUIBuilder-0.3/LICENCE
+-rw-rw-rw-   0        0        0      823 2024-05-03 21:35:18.832327 RTS-WebUIBuilder-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-04-29 16:57:15.000000 RTS-WebUIBuilder-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:35:18.820085 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/
+-rw-rw-rw-   0        0        0     1055 2024-04-15 18:28:33.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RAdditions.py
+-rw-rw-rw-   0        0        0     2282 2024-04-29 16:01:41.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RBody.py
+-rw-rw-rw-   0        0        0     2718 2024-04-28 15:20:36.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RBox.py
+-rw-rw-rw-   0        0        0     3233 2024-04-29 15:07:44.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RDocument.py
+-rw-rw-rw-   0        0        0     2320 2024-04-13 14:53:29.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RFrame.py
+-rw-rw-rw-   0        0        0    10637 2024-04-24 17:48:28.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RGroupStyle.py
+-rw-rw-rw-   0        0        0     1261 2024-04-13 14:44:52.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RHead.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 18:50:09.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RImage.py
+-rw-rw-rw-   0        0        0     2754 2024-04-21 08:51:23.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RInput.py
+-rw-rw-rw-   0        0        0      839 2024-04-26 21:26:34.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RLabel.py
+-rw-rw-rw-   0        0        0      326 2024-04-27 16:51:27.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RQuickScripts.py
+-rw-rw-rw-   0        0        0    10454 2024-04-24 17:44:53.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RStyle.py
+-rw-rw-rw-   0        0        0      796 2024-04-28 18:56:26.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RTitle.py
+-rw-rw-rw-   0        0        0     6181 2024-05-03 21:33:11.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RWebserver.py
+-rw-rw-rw-   0        0        0     3523 2024-04-29 16:16:05.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RpyColorizer.py
+-rw-rw-rw-   0        0        0      474 2024-04-29 14:58:45.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-13 17:25:24.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/cache.py
+-rw-rw-rw-   0        0        0      888 2024-04-29 15:07:12.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/exeptional.py
+-rw-rw-rw-   0        0        0     1015 2024-04-21 15:08:22.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/privatizehead.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:35:18.831320 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-03 21:35:18.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2024-05-03 21:35:18.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:35:18.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 21:35:18.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 21:35:18.000000 RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:35:18.832833 RTS-WebUIBuilder-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-05-03 21:35:17.000000 RTS-WebUIBuilder-0.3/setup.py
```

### Comparing `RTS_WebUIBuilder-0.2/LICENCE` & `RTS-WebUIBuilder-0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/PKG-INFO` & `RTS-WebUIBuilder-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: RTS_WebUIBuilder
-Version: 0.2
+Name: RTS-WebUIBuilder
+Version: 0.3
 Summary: A simple webserver with a simple webui builder.
 Home-page: https://github.com/RandomTimeLP/RTS_Webbuilder
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: WebUIBuilder,Webserver,Work In Progress
 Platform: UNKNOWN
```

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RAdditions.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RAdditions.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RBody.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RBody.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RBox.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RBox.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RDocument.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RDocument.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RFrame.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RFrame.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RGroupStyle.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RGroupStyle.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RHead.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RHead.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RInput.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RInput.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RLabel.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RLabel.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RStyle.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RStyle.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RTitle.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RTitle.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RWebserver.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RWebserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from aiohttp import web
 import os
 import asyncio, threading, time
+from threading import Thread
 
 
 
 class RWebserver:
     def __init__(self, host:str='localhost', port:int=8080) -> None:
         from .cache import rtswuib_cache
         if not rtswuib_cache.MAIN_WEBSERVER is None:
@@ -14,15 +15,15 @@
         self.bannedRoutes:set = set()
         self.loop:asyncio = asyncio.get_event_loop()
         self.app:web.Application = web.Application()
         self.runner:web.AppRunner = web.AppRunner(self.app)
         self.site = None
         self._srcFolders:set = set()
 
-    async def start(self) -> None:
+    async def __start(self) -> None:
         from .cache import rtswuib_cache
         if not rtswuib_cache.MAIN_WEBSERVER is None:
             raise ValueError('It is best practice to only have one webserver running at a time. Please stop the current webserver before starting a new one.')
         rtswuib_cache.MAIN_WEBSERVER = self
        
         
         await self.runner.setup()
@@ -56,20 +57,27 @@
             if os.path.isfile(safe_path):
                 return web.FileResponse(safe_path)
         raise web.HTTPNotFound()
 
     def init_routes(self):
         self.app.router.add_route('GET', '/src/{path:.*}', self.serve_file)
 
+    def __proceed(proceedWithFunction, *args, **kwargs):
+        time.sleep(2)
+        if proceedWithFunction:
+            proceedWithFunction(*args, **kwargs)
+
+
+    def run(self, proceedWithFunction, *args, **kwargs) -> None:
+        Thread(target=proceedWithFunction, args=(proceedWithFunction, *args), kwargs=kwargs).start()
 
-    def run(self) -> None:
         self.init_routes()
         self.automountGet()
         
-        self.loop.run_until_complete(self.start())
+        self.loop.run_until_complete(self.__start())
         try:
             self.loop.run_forever()
         except KeyboardInterrupt:
             self.loop.run_until_complete(self.stop())
 
     def bannDynamicroutesFromAutomount(self, routes:any) -> None:
         if isinstance(routes, list):
```

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/RpyColorizer.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/RpyColorizer.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/exeptional.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/exeptional.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder/privatizehead.py` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder/privatizehead.py`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/PKG-INFO` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-WebUIBuilder
-Version: 0.2
+Version: 0.3
 Summary: A simple webserver with a simple webui builder.
 Home-page: https://github.com/RandomTimeLP/RTS_Webbuilder
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: WebUIBuilder,Webserver,Work In Progress
 Platform: UNKNOWN
```

### Comparing `RTS_WebUIBuilder-0.2/RTS_WebUIBuilder.egg-info/SOURCES.txt` & `RTS-WebUIBuilder-0.3/RTS_WebUIBuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RTS_WebUIBuilder-0.2/setup.py` & `RTS-WebUIBuilder-0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='RTS_WebUIBuilder',
-    version='0.2',
+    name='RTS-WebUIBuilder',
+    version='0.3',
     packages=find_packages(),
     description='A simple webserver with a simple webui builder.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

