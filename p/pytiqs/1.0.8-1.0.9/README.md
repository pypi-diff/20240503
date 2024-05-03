# Comparing `tmp/pytiqs-1.0.8.tar.gz` & `tmp/pytiqs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiqs-1.0.8.tar", last modified: Fri Apr 12 10:11:03 2024, max compression
+gzip compressed data, was "pytiqs-1.0.9.tar", last modified: Mon Apr 15 07:16:49 2024, max compression
```

## Comparing `pytiqs-1.0.8.tar` & `pytiqs-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 10:11:03.744402 pytiqs-1.0.8/
--rw-r--r--   0 nitin      (501) staff       (20)     3288 2024-04-12 10:11:03.744336 pytiqs-1.0.8/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)     2785 2024-04-12 08:43:46.000000 pytiqs-1.0.8/README.md
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 10:11:03.741768 pytiqs-1.0.8/pytiqs/
--rw-r--r--   0 nitin      (501) staff       (20)      172 2024-04-10 04:14:30.000000 pytiqs-1.0.8/pytiqs/__init__.py
--rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-12 10:10:52.000000 pytiqs-1.0.8/pytiqs/__version__.py
--rw-r--r--   0 nitin      (501) staff       (20)    16952 2024-04-12 04:46:16.000000 pytiqs-1.0.8/pytiqs/connect.py
--rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-10 04:14:30.000000 pytiqs-1.0.8/pytiqs/constants.py
--rw-r--r--   0 nitin      (501) staff       (20)      555 2024-04-10 04:14:30.000000 pytiqs-1.0.8/pytiqs/exceptions.py
--rw-r--r--   0 nitin      (501) staff       (20)    19068 2024-04-12 09:39:16.000000 pytiqs-1.0.8/pytiqs/sockets.py
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 10:11:03.744066 pytiqs-1.0.8/pytiqs.egg-info/
--rw-r--r--   0 nitin      (501) staff       (20)     3288 2024-04-12 10:11:03.000000 pytiqs-1.0.8/pytiqs.egg-info/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)      295 2024-04-12 10:11:03.000000 pytiqs-1.0.8/pytiqs.egg-info/SOURCES.txt
--rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-12 10:11:03.000000 pytiqs-1.0.8/pytiqs.egg-info/dependency_links.txt
--rw-r--r--   0 nitin      (501) staff       (20)      145 2024-04-12 10:11:03.000000 pytiqs-1.0.8/pytiqs.egg-info/requires.txt
--rw-r--r--   0 nitin      (501) staff       (20)        7 2024-04-12 10:11:03.000000 pytiqs-1.0.8/pytiqs.egg-info/top_level.txt
--rw-r--r--   0 nitin      (501) staff       (20)      290 2024-04-12 10:11:03.744645 pytiqs-1.0.8/setup.cfg
--rw-r--r--   0 nitin      (501) staff       (20)     1192 2024-04-10 04:19:46.000000 pytiqs-1.0.8/setup.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-15 07:16:49.830314 pytiqs-1.0.9/
+-rw-r--r--   0 nitin      (501) staff       (20)     4673 2024-04-15 07:16:49.830219 pytiqs-1.0.9/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)     4170 2024-04-15 07:15:45.000000 pytiqs-1.0.9/README.md
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-15 07:16:49.828023 pytiqs-1.0.9/pytiqs/
+-rw-r--r--   0 nitin      (501) staff       (20)      172 2024-04-10 04:14:30.000000 pytiqs-1.0.9/pytiqs/__init__.py
+-rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-15 07:08:37.000000 pytiqs-1.0.9/pytiqs/__version__.py
+-rw-r--r--   0 nitin      (501) staff       (20)    16952 2024-04-12 04:46:16.000000 pytiqs-1.0.9/pytiqs/connect.py
+-rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-10 04:14:30.000000 pytiqs-1.0.9/pytiqs/constants.py
+-rw-r--r--   0 nitin      (501) staff       (20)      555 2024-04-10 04:14:30.000000 pytiqs-1.0.9/pytiqs/exceptions.py
+-rw-r--r--   0 nitin      (501) staff       (20)    18931 2024-04-15 07:07:57.000000 pytiqs-1.0.9/pytiqs/sockets.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-15 07:16:49.829825 pytiqs-1.0.9/pytiqs.egg-info/
+-rw-r--r--   0 nitin      (501) staff       (20)     4673 2024-04-15 07:16:49.000000 pytiqs-1.0.9/pytiqs.egg-info/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)      295 2024-04-15 07:16:49.000000 pytiqs-1.0.9/pytiqs.egg-info/SOURCES.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-15 07:16:49.000000 pytiqs-1.0.9/pytiqs.egg-info/dependency_links.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      145 2024-04-15 07:16:49.000000 pytiqs-1.0.9/pytiqs.egg-info/requires.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        7 2024-04-15 07:16:49.000000 pytiqs-1.0.9/pytiqs.egg-info/top_level.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      290 2024-04-15 07:16:49.830779 pytiqs-1.0.9/setup.cfg
+-rw-r--r--   0 nitin      (501) staff       (20)     1192 2024-04-10 04:19:46.000000 pytiqs-1.0.9/setup.py
```

### Comparing `pytiqs-1.0.8/pytiqs/connect.py` & `pytiqs-1.0.9/pytiqs/connect.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.8/pytiqs/constants.py` & `pytiqs-1.0.9/pytiqs/constants.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.8/pytiqs/exceptions.py` & `pytiqs-1.0.9/pytiqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.8/pytiqs/sockets.py` & `pytiqs-1.0.9/pytiqs/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         # If the message is binary, parse it and send it to the callback.
         if self.on_ticks and is_binary and len(payload) > 4:
             self.on_ticks(self, self._parse_binary(payload))
 
         # Parse text messages
         if not is_binary:
-            self._parse_text_message(ws, payload)
+            self._parse_message(ws, payload)
 
     def _on_open(self, ws) -> None:
         if not self._is_first_connect:
             self.resubscribe()
         self._is_first_connect = False
 
         if self.on_open:
@@ -393,25 +393,23 @@
         if self.on_reconnect:
             return self.on_reconnect(self, attempts_count)
 
     def _on_noreconnect(self) -> None:
         if self.on_noreconnect:
             return self.on_noreconnect(self)
 
-    def _parse_text_message(self, ws, payload: Union[str, bytes]) -> None:
+    def _parse_message(self, ws, payload: Union[str, bytes]) -> None:
         if type(payload) == bytes:
             payload = payload.decode("utf-8")
         try:
             data = json.loads(payload)
         except ValueError:
             return
-        if self.on_order_update and data.get("type") == "order" and data.get("data"):
-            self.on_order_update(self, data["data"])
-        if data.get("type") == "error":
-            self._on_error(ws, code=0, reason=data.get("data"))
+        if self.on_order_update and data.get("type") == "orderUpdate":
+            self.on_order_update(self, data)
 
     def _parse_binary(self, data: bytes) -> Dict[str, Any]:
         tick = {}  # type: Dict[str, Any]
         if self.debug:
             log.debug("Parsing binary, len: {}".format(len(data)))
         if len(data) >= 13:
             tick['token'] = int.from_bytes(data[0:4])
```

### Comparing `pytiqs-1.0.8/setup.py` & `pytiqs-1.0.9/setup.py`

 * *Files identical despite different names*

