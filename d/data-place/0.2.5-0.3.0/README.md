# Comparing `tmp/data-place-0.2.5.tar.gz` & `tmp/data-place-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-place-0.2.5.tar", last modified: Fri May  3 10:26:37 2024, max compression
+gzip compressed data, was "data-place-0.3.0.tar", last modified: Fri May  3 15:20:26 2024, max compression
```

## Comparing `data-place-0.2.5.tar` & `data-place-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 10:26:37.410180 data-place-0.2.5/
--rw-rw-rw-   0        0        0       44 2024-05-03 10:26:37.000000 data-place-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6073 2024-05-03 10:26:37.409179 data-place-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.5/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.5/build.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:26:37.408180 data-place-0.2.5/data_place.egg-info/
--rw-rw-rw-   0        0        0     6073 2024-05-03 10:26:37.000000 data-place-0.2.5/data_place.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-05-03 10:26:37.000000 data-place-0.2.5/data_place.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 10:26:37.000000 data-place-0.2.5/data_place.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-03 10:26:37.000000 data-place-0.2.5/data_place.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 10:26:37.000000 data-place-0.2.5/data_place.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 10:26:37.407180 data-place-0.2.5/dataplace/
--rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.5/dataplace/__init__.py
--rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.5/dataplace/base.py
--rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.5/dataplace/callback.py
--rw-rw-rw-   0        0        0     3178 2024-05-03 10:26:32.000000 data-place-0.2.5/dataplace/control.py
--rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.5/dataplace/handler.py
--rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.5/dataplace/io.py
--rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.5/dataplace/receive.py
--rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.5/dataplace/send.py
--rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.2.5/dataplace/store.py
--rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 10:26:37.410180 data-place-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-05-03 10:26:32.000000 data-place-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:26.633219 data-place-0.3.0/
+-rw-rw-rw-   0        0        0       44 2024-05-03 15:20:26.000000 data-place-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6073 2024-05-03 15:20:26.631885 data-place-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.3.0/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.3.0/build.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:26.631885 data-place-0.3.0/data_place.egg-info/
+-rw-rw-rw-   0        0        0     6073 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:26.630886 data-place-0.3.0/dataplace/
+-rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.3.0/dataplace/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-05-03 15:13:02.000000 data-place-0.3.0/dataplace/base.py
+-rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.3.0/dataplace/callback.py
+-rw-rw-rw-   0        0        0     3178 2024-05-03 10:26:32.000000 data-place-0.3.0/dataplace/control.py
+-rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.3.0/dataplace/handler.py
+-rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.3.0/dataplace/io.py
+-rw-rw-rw-   0        0        0     8742 2024-05-03 15:20:22.000000 data-place-0.3.0/dataplace/receive.py
+-rw-rw-rw-   0        0        0    11010 2024-05-03 15:20:22.000000 data-place-0.3.0/dataplace/send.py
+-rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.3.0/dataplace/store.py
+-rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:20:26.633219 data-place-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-05-03 15:20:22.000000 data-place-0.3.0/setup.py
```

### Comparing `data-place-0.2.5/PKG-INFO` & `data-place-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.5
+Version: 0.3.0
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.5/README.md` & `data-place-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `data-place-0.2.5/build.py` & `data-place-0.3.0/build.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.5/data_place.egg-info/PKG-INFO` & `data-place-0.3.0/data_place.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.5
+Version: 0.3.0
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.5/dataplace/base.py` & `data-place-0.3.0/dataplace/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,14 +59,19 @@
         pass
 
     @abstractmethod
     async def connect(self) -> None:
 
         pass
 
+    @abstractmethod
+    async def close(self) -> None:
+
+        pass
+
     async def _connect(self) -> None:
 
         await self.connect()
 
         self._connected = True
 
     async def start(self) -> None:
```

### Comparing `data-place-0.2.5/dataplace/callback.py` & `data-place-0.3.0/dataplace/callback.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.5/dataplace/control.py` & `data-place-0.3.0/dataplace/control.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.5/dataplace/handler.py` & `data-place-0.3.0/dataplace/handler.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.5/dataplace/io.py` & `data-place-0.3.0/dataplace/io.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.5/dataplace/receive.py` & `data-place-0.3.0/dataplace/receive.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,24 +235,36 @@
 
         self.running = True
 
         await self._handling_loop(
             reader=self.reader, writer=self.writer
         )
 
+    async def close(self) -> None:
+
+        self.writer.close()
+
+        await self.writer.wait_closed()
+
 class ReceiverSocketServer(ReceiverSocket, ReceiverServer):
 
     server: asyncio.Server | None = None
 
     async def connect(self) -> None:
 
         self.server = await asyncio.start_server(
             self._handling_loop, self.host, self.port
         )
 
+    async def close(self) -> None:
+
+        self.server.close()
+
+        await self.server.wait_closed()
+
     async def start(self) -> None:
 
         await super().start()
 
         async with self.server:
             await self.server.serve_forever()
 
@@ -260,14 +272,18 @@
 
     client: Connect | None = None
 
     async def connect(self) -> None:
 
         self.client = connect(self.url)
 
+    async def close(self) -> None:
+
+        await self.client.protocol.close()
+
     async def start(self) -> None:
 
         await super().start()
 
         async with self.client as websocket:
             await self._handling_loop(websocket=websocket)
 
@@ -304,14 +320,20 @@
             data=data
         )
 
     async def connect(self) -> None:
 
         self.server = serve(self._handling_loop, self.host, self.port)
 
+    async def close(self) -> None:
+
+        self.server.ws_server.close()
+
+        await self.server.ws_server.wait_closed()
+
     async def start(self) -> None:
 
         await super().start()
 
         async with self.server:
             await asyncio.Future()
```

### Comparing `data-place-0.2.5/dataplace/send.py` & `data-place-0.3.0/dataplace/send.py`

 * *Files 5% similar despite different names*

```diff
@@ -244,14 +244,20 @@
 
     async def connect(self) -> None:
 
         self.reader, self.writer = await asyncio.open_connection(
             host=self.host, port=self.port
         )
 
+    async def close(self) -> None:
+
+        self.writer.close()
+
+        await self.writer.wait_closed()
+
 class SenderSocketServer(SenderServer, SenderSocket):
 
     server: asyncio.Server | None = None
 
     def __init__(
             self,
             host: str,
@@ -307,14 +313,20 @@
 
     async def connect(self) -> None:
 
         self.server = await asyncio.start_server(
             self._handling_loop, self.host, self.port
         )
 
+    async def close(self) -> None:
+
+        self.server.close()
+
+        await self.server.wait_closed()
+
     async def start(self) -> None:
 
         await super().start()
 
         async with self.server:
             await self.server.serve_forever()
 
@@ -344,14 +356,18 @@
 
         await self.handle(data, self.client)
 
     async def connect(self) -> None:
 
         self.client = connect(self.url)
 
+    async def close(self) -> None:
+
+        self.client.close()
+
 class SenderWebSocketServer(SenderServer, SenderWebSocket):
 
     server: Serve | None = None
 
     def __init__(
             self,
             host: str,
@@ -384,14 +400,20 @@
 
         await super()._handling_loop(websocket=websocket)
 
     async def connect(self) -> None:
 
         self.server = serve(self._handling_loop, self.host, self.port)
 
+    async def close(self) -> None:
+
+        self.server.ws_server.close()
+
+        await self.server.ws_server.wait_closed()
+
     async def start(self) -> None:
 
         await super().start()
 
         async with self.server:
             await asyncio.Future()
```

### Comparing `data-place-0.2.5/dataplace/store.py` & `data-place-0.3.0/dataplace/store.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.5/setup.py` & `data-place-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='data-place',
-        version='0.2.5',
+        version='0.3.0',
         description=(
             "A powerfull and flexible framework for designing async "
             "socket based data streaming and distribution systems, "
             "with automated parsing, dynamic data store and "
             "high-level control hooks."
         ),
         license='MIT',
```

