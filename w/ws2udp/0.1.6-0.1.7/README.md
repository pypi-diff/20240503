# Comparing `tmp/ws2udp-0.1.6.tar.gz` & `tmp/ws2udp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws2udp-0.1.6.tar", last modified: Tue Jan  4 15:10:06 2022, max compression
+gzip compressed data, was "ws2udp-0.1.7.tar", last modified: Fri May  3 06:23:36 2024, max compression
```

## Comparing `ws2udp-0.1.6.tar` & `ws2udp-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 bgola     (1000) bgola     (1000)        0 2022-01-04 15:10:06.218808 ws2udp-0.1.6/
--rw-rw-r--   0 bgola     (1000) bgola     (1000)    35149 2020-11-22 10:34:36.000000 ws2udp-0.1.6/LICENSE
--rw-rw-r--   0 bgola     (1000) bgola     (1000)     2132 2022-01-04 15:10:06.218808 ws2udp-0.1.6/PKG-INFO
--rw-rw-r--   0 bgola     (1000) bgola     (1000)     1578 2020-11-23 14:53:22.000000 ws2udp-0.1.6/README.md
--rw-rw-r--   0 bgola     (1000) bgola     (1000)       38 2022-01-04 15:10:06.218808 ws2udp-0.1.6/setup.cfg
--rw-rw-r--   0 bgola     (1000) bgola     (1000)      959 2022-01-04 15:01:55.000000 ws2udp-0.1.6/setup.py
-drwxrwxr-x   0 bgola     (1000) bgola     (1000)        0 2022-01-04 15:10:06.218808 ws2udp-0.1.6/ws2udp/
--rw-rw-r--   0 bgola     (1000) bgola     (1000)        0 2020-11-23 14:10:22.000000 ws2udp-0.1.6/ws2udp/__init__.py
--rw-rw-r--   0 bgola     (1000) bgola     (1000)     1351 2022-01-04 15:01:39.000000 ws2udp-0.1.6/ws2udp/__main__.py
--rwxrwxr-x   0 bgola     (1000) bgola     (1000)     7227 2022-01-04 15:03:07.000000 ws2udp-0.1.6/ws2udp/ws2udp.py
-drwxrwxr-x   0 bgola     (1000) bgola     (1000)        0 2022-01-04 15:10:06.218808 ws2udp-0.1.6/ws2udp.egg-info/
--rw-rw-r--   0 bgola     (1000) bgola     (1000)     2132 2022-01-04 15:10:06.000000 ws2udp-0.1.6/ws2udp.egg-info/PKG-INFO
--rw-rw-r--   0 bgola     (1000) bgola     (1000)      263 2022-01-04 15:10:06.000000 ws2udp-0.1.6/ws2udp.egg-info/SOURCES.txt
--rw-rw-r--   0 bgola     (1000) bgola     (1000)        1 2022-01-04 15:10:06.000000 ws2udp-0.1.6/ws2udp.egg-info/dependency_links.txt
--rw-rw-r--   0 bgola     (1000) bgola     (1000)       49 2022-01-04 15:10:06.000000 ws2udp-0.1.6/ws2udp.egg-info/entry_points.txt
--rw-rw-r--   0 bgola     (1000) bgola     (1000)       11 2022-01-04 15:10:06.000000 ws2udp-0.1.6/ws2udp.egg-info/requires.txt
--rw-rw-r--   0 bgola     (1000) bgola     (1000)        7 2022-01-04 15:10:06.000000 ws2udp-0.1.6/ws2udp.egg-info/top_level.txt
+drwxr-xr-x   0 bgola     (1000) bgola     (1000)        0 2024-05-03 06:23:36.322122 ws2udp-0.1.7/
+-rw-r--r--   0 bgola     (1000) bgola     (1000)    35149 2023-12-06 17:10:26.000000 ws2udp-0.1.7/LICENSE
+-rw-r--r--   0 bgola     (1000) bgola     (1000)     2610 2024-05-03 06:23:36.322122 ws2udp-0.1.7/PKG-INFO
+-rwxr-xr-x   0 bgola     (1000) bgola     (1000)     2026 2024-05-03 06:21:50.000000 ws2udp-0.1.7/README.md
+-rw-r--r--   0 bgola     (1000) bgola     (1000)       38 2024-05-03 06:23:36.322122 ws2udp-0.1.7/setup.cfg
+-rwxr-xr-x   0 bgola     (1000) bgola     (1000)     1000 2024-05-03 06:21:50.000000 ws2udp-0.1.7/setup.py
+drwxr-xr-x   0 bgola     (1000) bgola     (1000)        0 2024-05-03 06:23:36.322122 ws2udp-0.1.7/ws2udp/
+-rw-r--r--   0 bgola     (1000) bgola     (1000)        0 2023-12-06 17:10:26.000000 ws2udp-0.1.7/ws2udp/__init__.py
+-rwxr-xr-x   0 bgola     (1000) bgola     (1000)     2051 2024-05-03 06:21:50.000000 ws2udp-0.1.7/ws2udp/__main__.py
+-rwxr-xr-x   0 bgola     (1000) bgola     (1000)     8185 2024-05-03 06:21:50.000000 ws2udp-0.1.7/ws2udp/ws2udp.py
+drwxr-xr-x   0 bgola     (1000) bgola     (1000)        0 2024-05-03 06:23:36.322122 ws2udp-0.1.7/ws2udp.egg-info/
+-rw-r--r--   0 bgola     (1000) bgola     (1000)     2610 2024-05-03 06:23:36.000000 ws2udp-0.1.7/ws2udp.egg-info/PKG-INFO
+-rw-r--r--   0 bgola     (1000) bgola     (1000)      263 2024-05-03 06:23:36.000000 ws2udp-0.1.7/ws2udp.egg-info/SOURCES.txt
+-rw-r--r--   0 bgola     (1000) bgola     (1000)        1 2024-05-03 06:23:36.000000 ws2udp-0.1.7/ws2udp.egg-info/dependency_links.txt
+-rw-r--r--   0 bgola     (1000) bgola     (1000)       48 2024-05-03 06:23:36.000000 ws2udp-0.1.7/ws2udp.egg-info/entry_points.txt
+-rw-r--r--   0 bgola     (1000) bgola     (1000)       11 2024-05-03 06:23:36.000000 ws2udp-0.1.7/ws2udp.egg-info/requires.txt
+-rw-r--r--   0 bgola     (1000) bgola     (1000)        7 2024-05-03 06:23:36.000000 ws2udp-0.1.7/ws2udp.egg-info/top_level.txt
```

### Comparing `ws2udp-0.1.6/LICENSE` & `ws2udp-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ws2udp-0.1.6/README.md` & `ws2udp-0.1.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,25 +20,34 @@
 $ ws2udp
 WebSocket to UDP proxy
 
 optional arguments:
   -h, --help           show this help message and exit
   --udp-addr UDP_ADDR  Address of the UDP receiver for broadcasting messages (default=localhost)
   --udp-port UDP_PORT  Port of the UDP receiver (default=57142)
+  --fwd-fixed          Forward UDP to fixed target address/port
+  --fwd-addr FWD_ADDR  Address of the UDP target for messages (default=localhost)
+  --fwd-port FWD_PORT  Port of the UDP target (default=57143)
   --addr ADDR          WebSocket address to listen (default=0.0.0.0)
   --port PORT          WebSocket port to listen (default=8765)
+  --broadcast          Enable UDP broadcasting
+  --quiet              No verbose output
 ```
 
-The server expects binary messages following the format:
+If the `fwd-fixed` option is not given (default behavior),
+the server expects binary messages following the format:
 
 **address_length**(uint32)**address**(string)**port**(uint32)**data**
 
 * _address_length_ is an integer representing the total length of the address
 * _address_ the address where to forward the data as a string (example: localhost)
 * _port_ as an integer
 * _data_ the original message data
 
 For example, to send the message `hello world` to `localhost:57120`, one would send:
 
 `b'\x09\x00\x00\x00localhost\x20\xdf\x00\x00hello, world'`
 
 The first 4 bytes `b'\x09\x00\x00\x00` represents 9, then comes `b'localhost'` and lastly `b'\x20\xdf\x00\x00'` for 57120. Whatever comes after this is forwarded.
+
+
+If the `fwd-fixed` option is given, the original message data will be forwarded unaltered.
```

### Comparing `ws2udp-0.1.6/setup.py` & `ws2udp-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='ws2udp',
-      version='0.1.6',
-      author='Bruno Gola',
-      author_email='me@bgo.la',
+      version='0.1.7',
+      author='Bruno Gola, additions by Thomas Grill',
+      author_email='me@bgo.la, gr@grrrr.org',
       description='A WebSocket to UDP proxy',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/bgola/ws2udp",
       packages=find_namespace_packages(include=['ws2udp']),
 	  classifiers=[
           "Programming Language :: Python :: 3",
```

### Comparing `ws2udp-0.1.6/ws2udp/ws2udp.py` & `ws2udp-0.1.7/ws2udp/ws2udp.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 clients = []
 
 class UDPSock:
     """
     Class forked / modified from 
     https://github.com/bashkirtsevich-llc/aioudp
     """
-    def __init__(self, addr='', port=0, loop=None, datagram_received=None):
+    def __init__(self, addr='', port=0, loop=None, datagram_received=None, enable_broadcast=False):
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, 0)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        if enable_broadcast:
+            self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
         self._sock.setblocking(False)
 
         self._send_event = asyncio.Event()
         self._send_queue = deque()
 
         if loop is None:
             loop = asyncio.get_running_loop()
@@ -128,19 +130,19 @@
 
 class Client:
     """
     Simple representation of a websocket client.
     Keeps a map of ports used for proxying UDP messages and uses a queue
     for sending UDP messages back to the websocket.
     """
-    def __init__(self, websocket):
+    def __init__(self, websocket, enable_broadcast=False):
         logging.info(f"New WebSocket client from {websocket.remote_address}")
         self.websocket = websocket
         
-        self._sock = UDPSock(datagram_received=self._got_udp_message)
+        self._sock = UDPSock(datagram_received=self._got_udp_message, enable_broadcast=enable_broadcast)
         logging.info(f"{self} listening to UDP messages on {self._sock.getsockname()}")
 
         self.queue = asyncio.Queue()
 
     def __repr__(self):
         return f"Client{self.websocket.remote_address}"
 
@@ -163,81 +165,92 @@
         self._sock.bind(('', 0))
         asyncio.ensure_future(self._recv(), loop=asyncio.get_running_loop())
 
     def _got_udp_message(self, message, addr):
         self.send_ws(message)
 
 
-async def ws2udp_sender(client):
-    """
-    Sends UDP message received to WebSocket
-    """
-    while True:
-        message = await client.queue.get()
-        await client.websocket.send(message)
+class Handler:
+    def __init__(self, fwd_address=None, enable_broadcast=False):
+        self.fwd_address = fwd_address
+        self.enable_broadcast = enable_broadcast
 
 
-async def ws2udp_receiver(client):
-    """
-    Receives UDP message via WebSocket and forwards to UDP.
-    """
-    async for message in client.websocket:
-        # Parse addres and port where to send
-        # Format is [addr_string_length:uint32][addr:string][port:uint32][message]
-        original_message = message[:]
-        try:
-            addr_size = struct.unpack("I", message[:4])[0]
-            message = message[4:]
-            addr = message[:addr_size]
-            message = message[addr_size:]
-            port = struct.unpack("I", message[:4])[0]
-            message = message[4:]
-        except TypeError:
-            logging.error(f"Got a bad message, can't parse address to forward: {original_message}")
-        else:
-            client.send_udp(message, (addr, port))
+    async def ws2udp_sender(self, client):
+        """
+        Sends UDP message received to WebSocket
+        """
+        while True:
+            message = await client.queue.get()
+            await client.websocket.send(message)
 
 
-async def ws2udp_handler(websocket, path):
-    """
-    Wrapper handler for both way communication.
-    """
-    client = Client(websocket)
-    clients.append(client)
+    async def ws2udp_receiver(self, client):
+        """
+        Receives UDP message via WebSocket and forwards to UDP.
+        """
+        async for message in client.websocket:
+            if self.fwd_address is None:
+                # Parse addres and port where to send
+                # Format is [addr_string_length:uint32][addr:string][port:uint32][message]
+                original_message = message[:]
+                try:
+                    addr_size = struct.unpack("I", message[:4])[0]
+                    message = message[4:]
+                    addr = message[:addr_size]
+                    message = message[addr_size:]
+                    port = struct.unpack("I", message[:4])[0]
+                    message = message[4:]
+                except TypeError:
+                    logging.error(f"Got a bad message, can't parse address to forward: {original_message}")
+                else:
+                    client.send_udp(message, (addr, port))
+            else:
+                # No parsing - directly forwarding original message
+                client.send_udp(message, self.fwd_address)
+
+
+    async def ws2udp_handler(self, websocket, path):
+        """
+        Wrapper handler for both way communication.
+        """
+        client = Client(websocket, self.enable_broadcast)
+        clients.append(client)
+
+        receiver = asyncio.ensure_future(
+            self.ws2udp_receiver(client))
+        sender = asyncio.ensure_future(
+            self.ws2udp_sender(client))
+
+        try:
+            done, pending = await asyncio.wait(
+                [receiver, sender],
+                return_when=asyncio.FIRST_COMPLETED,
+            )
+
+            for task in pending:
+                task.cancel()
+            for task in done:
+                # trigger exceptions, if any
+                task.result()
+        except (
+                websockets.exceptions.ConnectionClosedError,
+                websockets.exceptions.ConnectionClosedOK,
+                asyncio.exceptions.CancelledError):
+            # Connection ended
+            pass
 
-    receiver = asyncio.ensure_future(
-        ws2udp_receiver(client))
-    sender = asyncio.ensure_future(
-        ws2udp_sender(client))
-    
-    try:
-        done, pending = await asyncio.wait(
-            [receiver, sender],
-            return_when=asyncio.FIRST_COMPLETED,
-        )
-        
-        for task in pending:
-            task.cancel()
-        for task in done:
-            # trigger exceptions, if any
-            task.result()
-    except (
-            websockets.exceptions.ConnectionClosedError,
-            websockets.exceptions.ConnectionClosedOK,
-            asyncio.exceptions.CancelledError):
-        # Connection ended
-        pass
-
-    await client.leave()
-    clients.remove(client)
-    logging.info(f"Client{client.websocket.remote_address} left")
+        await client.leave()
+        clients.remove(client)
+        logging.info(f"Client{client.websocket.remote_address} left")
 
 
-async def run(udp_addr, websocket_addr, websocket_port):
-    ws_server = await websockets.serve(ws2udp_handler, websocket_addr, websocket_port)
+async def run(udp_addr, websocket_addr, websocket_port, fwd_addr=None, enable_broadcast=False):
+    handler = Handler(fwd_addr, enable_broadcast)
+    ws_server = await websockets.serve(handler.ws2udp_handler, websocket_addr, websocket_port)
 
     def send_broadcast(message, addr):
         for client in clients:
             client.send_ws(message)
 
     udp_server = UDPSock(*udp_addr, datagram_received=send_broadcast)  
     await ws_server.server.serve_forever()
```

