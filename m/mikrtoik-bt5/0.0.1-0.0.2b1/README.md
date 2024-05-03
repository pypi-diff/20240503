# Comparing `tmp/mikrtoik-bt5-0.0.1.tar.gz` & `tmp/mikrtoik-bt5-0.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mikrtoik-bt5-0.0.1.tar", last modified: Mon Oct 10 14:55:59 2022, max compression
+gzip compressed data, was "mikrtoik-bt5-0.0.2b1.tar", last modified: Fri May  3 08:44:30 2024, max compression
```

## Comparing `mikrtoik-bt5-0.0.1.tar` & `mikrtoik-bt5-0.0.2b1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/
--rw-r--r--   0 pi        (1000) pi        (1000)      700 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/PKG-INFO
--rw-rw-rw-   0 pi        (1000) pi        (1000)      251 2022-10-10 14:50:20.000000 mikrtoik-bt5-0.0.1/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/mikrotik_bt5/
--rw-r--r--   0 pi        (1000) pi        (1000)       67 2022-10-10 08:02:43.000000 mikrtoik-bt5-0.0.1/mikrotik_bt5/__init__.py
--rw-rw-rw-   0 pi        (1000) pi        (1000)     4173 2022-10-10 14:15:45.000000 mikrtoik-bt5-0.0.1/mikrotik_bt5/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/mikrtoik_bt5.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      700 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/mikrtoik_bt5.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      245 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/mikrtoik_bt5.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/mikrtoik_bt5.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/mikrtoik_bt5.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       13 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/mikrtoik_bt5.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-10-10 14:55:59.000000 mikrtoik-bt5-0.0.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      637 2022-10-10 14:55:46.000000 mikrtoik-bt5-0.0.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 08:44:30.520745 mikrtoik-bt5-0.0.2b1/
+-rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-03 08:44:30.516745 mikrtoik-bt5-0.0.2b1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      501 2024-05-03 08:43:20.000000 mikrtoik-bt5-0.0.2b1/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 08:44:30.504745 mikrtoik-bt5-0.0.2b1/mikrotik_bt5/
+-rw-r--r--   0 pi        (1000) pi        (1000)       67 2024-05-03 08:43:20.000000 mikrtoik-bt5-0.0.2b1/mikrotik_bt5/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4278 2024-05-03 08:43:20.000000 mikrtoik-bt5-0.0.2b1/mikrotik_bt5/client.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 08:44:30.516745 mikrtoik-bt5-0.0.2b1/mikrtoik_bt5.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-03 08:44:29.000000 mikrtoik-bt5-0.0.2b1/mikrtoik_bt5.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      245 2024-05-03 08:44:30.000000 mikrtoik-bt5-0.0.2b1/mikrtoik_bt5.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-03 08:44:29.000000 mikrtoik-bt5-0.0.2b1/mikrtoik_bt5.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-03 08:44:29.000000 mikrtoik-bt5-0.0.2b1/mikrtoik_bt5.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2024-05-03 08:44:29.000000 mikrtoik-bt5-0.0.2b1/mikrtoik_bt5.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-03 08:44:30.520745 mikrtoik-bt5-0.0.2b1/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      639 2024-05-03 08:44:24.000000 mikrtoik-bt5-0.0.2b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mikrtoik-bt5-0.0.1/mikrotik_bt5/client.py` & `mikrtoik-bt5-0.0.2b1/mikrotik_bt5/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,17 +44,32 @@
     salt: int = 0
     acceleration = Acceleration()
     temperature: float = -1
     uptime: int = -1
     flags: int = -1
     battery: int = -1
 
-    def __init__(self):
+    def __init__(self, device = None, ad_data = None):
         super().__init__(BeaconType.MIKROTIK.value)
 
+        if device and ad_data and MikrotikBT5.MIKROTIK_ID in ad_data.manufacturer_data:
+            raw_bytes = ad_data.manufacturer_data[MikrotikBT5.MIKROTIK_ID]
+
+            version = int(raw_bytes[0])
+            value_fmt = None
+
+            if version == 0:
+                value_fmt = "<BBHhhhbIBB"
+            elif version == 1:
+                value_fmt = "<BBHhhhhIBB"
+
+            if value_fmt:
+                value = struct.unpack(value_fmt, raw_bytes)
+                self.decode(value)
+
     def decode(self, value: tuple):
         self.version = value[0]
         self.udata   = value[1]
         self.salt    = value[2]
 
         self.acceleration.x = value[3] / 256.0
         self.acceleration.y = value[4] / 256.0
@@ -129,30 +144,16 @@
         return dev
 
 
     def _process_advertisement(self, device, ad_data):
         """Processes Mikrotik advertisement data"""
 
         if self.MIKROTIK_ID in ad_data.manufacturer_data:
-            raw_bytes = ad_data.manufacturer_data[self.MIKROTIK_ID]
-
-            version = int(raw_bytes[0])
-            beacon = None
-            value_fmt = None
-
-            if version == 0:
-                value_fmt = "<BBHhhhbIBB"
-            elif version == 1:
-                value_fmt = "<BBHhhhhIBB"
-
-            if value_fmt:
-                value = struct.unpack(value_fmt, raw_bytes)
-                beacon = MikrotikBeacon()
-                beacon.decode(value)
-                beacon.rssi = device.rssi
+            beacon = MikrotikBeacon(device, ad_data)
+            if beacon.version != -1:
                 dev = self._register_beacon(device, beacon)
                 self.on_scan(beacon, dev)
 
     def __init__(self, on_scan):
         self.on_scan = on_scan
 
     async def start_scan(self):
```

### Comparing `mikrtoik-bt5-0.0.1/setup.py` & `mikrtoik-bt5-0.0.2b1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mikrtoik-bt5",
-    version="0.0.1",
+    version="0.0.2b1",
     description="MikroTik BT5 scanner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/MikroTik-BT5-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

