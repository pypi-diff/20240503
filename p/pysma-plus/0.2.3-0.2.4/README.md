# Comparing `tmp/pysma_plus-0.2.3.tar.gz` & `tmp/pysma_plus-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.2.3.tar", last modified: Wed May  1 14:30:33 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.4.tar", last modified: Fri May  3 14:13:35 2024, max compression
```

## Comparing `pysma_plus-0.2.3.tar` & `pysma_plus-0.2.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 14:30:33.569361 pysma_plus-0.2.3/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-01 14:30:33.569361 pysma_plus-0.2.3/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-05-01 14:30:29.000000 pysma_plus-0.2.3/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 14:30:33.569361 pysma_plus-0.2.3/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-01 14:30:33.000000 pysma_plus-0.2.3/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1046 2024-05-01 14:30:33.000000 pysma_plus-0.2.3/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 14:30:33.000000 pysma_plus-0.2.3/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-01 14:30:33.000000 pysma_plus-0.2.3/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-01 14:30:33.000000 pysma_plus-0.2.3/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.3/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 14:30:33.568360 pysma_plus-0.2.3/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1439 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    18648 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/const_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9266 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/definitions_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21918 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/definitions_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/definitions_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      576 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/device_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    11597 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/device_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    20012 2024-05-01 14:28:11.000000 pysma_plus-0.2.3/pysmaplus/device_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    16414 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/device_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.3/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.3/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-01 14:30:33.570361 pysma_plus-0.2.3/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-01 14:30:29.000000 pysma_plus-0.2.3/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 14:30:33.569361 pysma_plus-0.2.3/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.3/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.3/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 14:30:33.569361 pysma_plus-0.2.3/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.3/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-05-03 14:13:28.000000 pysma_plus-0.2.4/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1046 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-03 14:13:35.000000 pysma_plus-0.2.4/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.4/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.420245 pysma_plus-0.2.4/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2409 2024-05-03 13:42:28.000000 pysma_plus-0.2.4/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    18929 2024-05-03 13:42:53.000000 pysma_plus-0.2.4/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9346 2024-05-03 13:35:20.000000 pysma_plus-0.2.4/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21600 2024-05-03 13:41:20.000000 pysma_plus-0.2.4/pysmaplus/definitions_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-05-03 11:25:27.000000 pysma_plus-0.2.4/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      825 2024-05-02 14:56:18.000000 pysma_plus-0.2.4/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    12557 2024-05-03 13:41:56.000000 pysma_plus-0.2.4/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21090 2024-05-03 13:41:03.000000 pysma_plus-0.2.4/pysmaplus/device_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17213 2024-05-02 14:59:07.000000 pysma_plus-0.2.4/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-03 14:13:28.000000 pysma_plus-0.2.4/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.421245 pysma_plus-0.2.4/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.4/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.4/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-03 14:13:35.422245 pysma_plus-0.2.4/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.4/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.3/LICENSE` & `pysma_plus-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/PKG-INFO` & `pysma_plus-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.3
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.4
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.3/README.md` & `pysma_plus-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/pyproject.toml` & `pysma_plus-0.2.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.2.3"
+version = "0.2.4"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma_plus-0.2.3/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.4/pysma_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.3
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.4
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.3/pysma_plus.egg-info/SOURCES.txt` & `pysma_plus-0.2.4/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/pysmaplus/__init__.py` & `pysma_plus-0.2.4/pysmaplus/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 See: http://www.sma.de/en/products/monitoring-control/webconnect.html
 
 Source: http://www.github.com/kellerza/pysma
 """
 import logging
 from typing import Optional
-
+import asyncio
 from aiohttp import ClientSession
 from .device_webconnect import SMAwebconnect
 from .device_ennexos import SMAennexos
 from .device_speedwire import SMAspeedwireINV
 from .device_em import SMAspeedwireEM
 from .device import Device
 _LOGGER = logging.getLogger(__name__)
@@ -34,7 +34,35 @@
             return SMAennexos(session, url, password=password, group=groupuser)
         elif (accessmethod == "speedwire") or (accessmethod == "speedwireem"):
               return SMAspeedwireEM()
         elif (accessmethod == "speedwireinv"):
               return SMAspeedwireINV(host = url, password= password, group=groupuser)
         else:
              return None
+
+async def _runDetect(accessmethod: str, session: ClientSession, ip):
+        sma = None
+        if (accessmethod == "webconnect"):
+            sma = SMAwebconnect(session, ip, password="", group="user")
+        elif (accessmethod == "ennexos"):
+            sma = SMAennexos(session, ip, password=None, group=None)
+        elif (accessmethod == "speedwireinv"):
+            sma = SMAspeedwireINV(host=ip, password="", group="user")
+        ret = await sma.detect(ip)
+        for i in ret:
+            i["access"] = accessmethod
+        try:
+             await sma.close_session()
+        except Exception:
+             pass
+        return ret
+
+async def autoDetect(session: ClientSession, ip:str):
+    ret = await asyncio.gather(
+        _runDetect("ennexos", session, ip),
+        _runDetect("speedwireinv", session, ip),
+        _runDetect("webconnect", session, ip)
+    )
+    results = []
+    for r in ret:
+         results.extend(r)
+    return results
```

### Comparing `pysma_plus-0.2.3/pysmaplus/const.py` & `pysma_plus-0.2.4/pysmaplus/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
     381: "Stop",
     402: "Phases L1 and L2 (phsAB)",
     403: "Phases L1 and L3 (phsAC)",
     404: "Phases L2 and L3 (phsBC)",
     433: "Contant voltage",
     455: "Warning",
     461: "SMA",
+    569: "activated",
     887: "No recommended action",
     1041: "leading / overexcited",
     1042: "lagging / underexcited",
     1069: "Reactive power / voltage characteristic curve Q(V)",
     1070: "Reactive power Q, direct setpoint",
     1071: "Reactive power const. Q (kVAr)",
     1072: "Q specified by PV system control",
@@ -165,14 +166,15 @@
     1077: "Active power limitation P (W)",
     1078: "Active power limitation P (%) of PMAX",
     1079: "Active power limitation P via system control",
     1129: "Yes",
     1130: "No",
     1264: "Full dynamic grid support",
     1265: "Limited dynamic grid support",
+#    1295:
     1387: "Reactive power Q, setpoint via analog input",
     1388: "cos φ, setpoint via analog input",
     1389: "Reactive power / voltage characteristic curve Q(U) with hysteresis and deadband",
     1390: "Active power limitation P via analog input",
     1391: "Active power limitation P via digital inputs",
     1392: "Errors",
     1393: "Wait for PV voltage",
@@ -193,14 +195,18 @@
     1475: "Error e-mail OK",
     1476: "Error e-mail not OK",
     1477: "Warning e-mail OK",
     1478: "Warning e-mail not OK",
     1479: "Wait after grid interruption",
     1480: "Wait for electric utility company",
     1749: "Full Stop",
+    1779: "disconnected",
+    1780: "public grid",
+    1781: "off-Grid",
+    1795: "locked",
     # 2055: "Status digital inlet: DI1",
     # 2056: "Status digital inlet: DI1, DI2",
     # 2057: "Status digital inlet: DI1, DI2, DI3",
     # 2058: "Status digital inlet: DI1, DI2, DI3, DI4",
     # 2059: "Status digital inlet: DI1, DI2, DI4",
     # 2060: "Status digital inlet: DI1, DI3",
     # 2061: "Status digital inlet: DI1, DI3, DI4",
@@ -229,18 +235,23 @@
     4718: "Boost Charging", # EV-Charger
     4950: "Smart Chargig", # EV-Charger
     5169: "Station locked", # EV-Charger
     5249: "Potential power with characteristic curve break",
 
 
 
-    # DevClass
-    8001: "Solar Inveters",
-    8008: "SMAEVCharger",
+    # Device Classes
+    8000: "All Devices",
+    8001: "Solar Inverters",
+    8002: "Wind Turbine Inverter",
+    8007: "Batterie Inverters",
+    8008: "EV Chargers",
+    8009: "Hybrid Inverters",
 
+    # Inverter Classes
     9000: "SWR 700",
     9001: "SWR 850",
     9002: "SWR 850E",
     9003: "SWR 1100",
     9004: "SWR 1100E",
     9005: "SWR 1100LV",
     9006: "SWR 1500",
@@ -537,10 +548,10 @@
     9492: "STP-12-50",
     9484: "EVC22-3AC-10",
 
 
     200111: "Not connected", # EV-Charger
     200112: "Sleep Mode", # EV-Charger
     200113: "Active Mode", # EV-Charger
-
+    
     16777213: "Information not available",
 }
```

### Comparing `pysma_plus-0.2.3/pysmaplus/const_webconnect.py` & `pysma_plus-0.2.4/pysmaplus/const_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/pysmaplus/definitions_ennexos.py` & `pysma_plus-0.2.4/pysmaplus/definitions_ennexos.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,20 +62,20 @@
         Sensor("Operation.DrtStt", None, factor=1, unit=None),
         Sensor("Operation.Evt.Dsc", None, factor=1, unit=None),
         Sensor("Operation.Evt.EvtNo", None, factor=1, unit=None),
         Sensor("Operation.Evt.Msg", None, factor=1, unit=None),
         Sensor("Operation.EvtCntIstl", None, factor=1, unit=None),
         Sensor("Operation.EvtCntUsr", None, factor=1, unit=None),
         Sensor("Operation.GriSwCnt", None, factor=1, unit=None),
-        Sensor("Operation.GriSwStt", None, factor=1, unit=None),
+        Sensor("Operation.GriSwStt", Identifier.grid_relay_status, unit=None,  mapper=SMATagList), 
         Sensor("Operation.Health", Identifier.status, factor=1, unit=None, mapper=SMATagList),
         Sensor("Operation.HealthStt.Alm", None, factor=1, unit=None),
         Sensor("Operation.HealthStt.Ok", None, factor=1, unit=None),
         Sensor("Operation.HealthStt.Wrn", None, factor=1, unit=None),
-        Sensor("Operation.OpStt", None, factor=1, unit=None),
+        Sensor("Operation.OpStt", Identifier.operating_status_genereal, unit=None, mapper=SMATagList),
         Sensor("Operation.PvGriConn", None, factor=1, unit=None),
         Sensor("Operation.RstrLokStt", None, factor=1, unit=None),
         Sensor("Operation.RunStt", None, factor=1, unit=None),
         Sensor("Operation.StandbyStt", None, factor=1, unit=None),
         Sensor("Operation.VArCtl.VArModAct", None, factor=1, unit=None),
         Sensor("Operation.VArCtl.VArModStt", None, factor=1, unit=None),
         Sensor("Operation.WMaxLimSrc", None, factor=1, unit=None),
@@ -105,15 +105,15 @@
         Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
         Sensor("GridMs.TotPF", None, factor=1, unit=None),
         Sensor("GridMs.TotVA", Identifier.grid_apparent_power, factor=1, unit="VA"),
         Sensor("GridMs.TotVAr", Identifier.grid_reactive_power, factor=1, unit="var"),
         Sensor("InOut.GI1", None, factor=1, unit=None),
         Sensor("Metering.GridMs.TotWIn", Identifier.metering_power_absorbed, factor=1, unit="W"), #
         Sensor("Metering.GridMs.TotWIn.ChaSta", None, factor=1, unit=None), # same as Metering.GridMs.TotWIn
-        Sensor("Metering.GridMs.TotWhIn", Identifier.metering_total_absorbed, factor=1, unit="Wh"), # charging_station_meter_reading
+        Sensor("Metering.GridMs.TotWhIn", Identifier.metering_total_absorbed, factor=1000, unit="kWh"), # charging_station_meter_reading
         Sensor("Metering.GridMs.TotWhIn.ChaSta", None, factor=1, unit=None), # same as Metering.GridMs.TotWhIn 
         Sensor("Operation.EVeh.ChaStt", Identifier.operating_status, factor=1, unit=None, mapper=SMATagList), # charging_session_status
         Sensor("Operation.EVeh.Health", Identifier.status, factor=1, unit=None, mapper=SMATagList), 
         Sensor("Operation.Evt.Msg", None, factor=1, unit=None),
         Sensor("Operation.Health", None, factor=1, unit=None), # same as EVeh.Health?
         Sensor("Operation.WMaxLimNom", None, factor=1, unit=None),
         Sensor("Operation.WMaxLimSrc", None, factor=1, unit=None),
```

### Comparing `pysma_plus-0.2.3/pysmaplus/definitions_speedwire.py` & `pysma_plus-0.2.4/pysmaplus/definitions_speedwire.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 # based on https://github.com/Wired-Square/sma-query/blob/main/src/sma_query_sw/commands.py
+# improved with https://github.com/mhop/fhem-mirror/blob/master/fhem/FHEM/76_SMAInverter.pm  
+
 from .const import Identifier
 from .sensor import Sensor
 from .const import SMATagList
 
 commands = {
     "login": {"command": 0xFFFD040C, 
               "response": 0xFFFD040D,
               "first": 0x0030CB00,
               "last": 0x0030CB00,
-
-                "registers": [
+              "registers": [
                     {"name": "susyid", "format": "H", "offset": 20},
                     {"name": "serial", "format": "uint","offset": 22},
                     {"name": "pkt_ID", "format": "H","offset": 40},
                     {"name": "cmdid", "format": "H","offset": 42},
                     {"name": "error", "format": "uint","offset": 36},
                 ]   
-              
-        #               my $r_susyid = unpack("v*", substr $data, 20, 2);
-        # my $r_serial = unpack("V*", substr $data, 22, 4);
-        # my $r_pkt_ID = unpack("v*", substr $data, 40, 2);
-        # my $r_cmd_ID = unpack("V*", substr $data, 42, 4);
-        # my $r_error  = unpack("V*", substr $data, 36, 4);
-
               },
     "logoff": {"command": 0xFFFD010E, "response": 0xFFFD010F},
     "TypeLabel": {
         "command": 0x58000200,
         "response": 0x00821E00,
         "first": 0x00821E00,
         "last": 0x008220FF,
         "registers": [
             {"name": "inverter_class", "offset": 102, "mask": 0x00FFFFFF},
             {"name": "inverter_type", "format": "list", "offset": 142},
-            #$temp = unpack("V*", substr $data, $i, 4);
-
         ],
     },
     "EnergyProduction": {
         "command": 0x54000200,
         "response": 0x00260100,
         "first": 0x00260100,
         "last": 0x002622FF,
@@ -366,27 +358,24 @@
         "first": 0x00411E00,
         "last": 0x004120FF,
         "registers": [
             {
                 "name": "MaxACPower1",
                 "offset": 62,
                 "invalid": 0x80000000,
-                #     "sensor": Sensor("battery_current_a", Identifier.battery_current_a, unit="A", factor=1000)
             },
             {
                 "name": "MaxACPower2",
                 "offset": 90,
                 "invalid": 0x80000000,
-                # "sensor": Sensor("battery_current_b", Identifier.battery_current_b, unit="A", factor=1000)
             },
             {
                 "name": "MaxACPower3",
                 "offset": 118,
                 "invalid": 0x80000000,
-                # "sensor": Sensor("battery_current_b", Identifier.battery_current_b, unit="A", factor=1000)
             },
         ],
     },
     "MaxACPower2": {
         "command": 0x51000200,
         "response": 0x00832A00,
         "first": 0x00832A00,
@@ -394,46 +383,51 @@
     },
     "GridRelayStatus": {
         "command": 0x51800200,
         "response": 0x00416400,
         "first": 0x00416400,
         "last": 0x004164FF,
         "registers": [
-            {"name": "grid_relay_status", "offset": 62, "invalid": 0x80000000}
+            {"name": "grid_relay_status", "format": "list", "offset": 62, "invalid": 0x80000000,
+             "sensor":  Sensor("GridRelayStatus", Identifier.grid_relay_status, unit=None, mapper = SMATagList)}
         ],
     },
     "BackupRelayStatus": {
         "command": 0x51800200,
         "response": 0x08412500,
         "first": 0x08412500,
         "last": 0x084125FF,
     },
     "GridConection": {
         "command": 0x51800200,
-        "response": 0x0846A600,
-        "first": 0x0846A600,
-        "last": 0x0846A6FF,
-        # "registers": [
-        #     {"name": "GridConection", "format": "list", "offset": 62},
-        # ],
+        "response": 0x0046A600,
+        "first": 0x0046A600,
+        "last": 0x0046A6FF,
+         "registers": [
+             {"name": "GridConection", "format": "list", "offset": 62},
+         ],
     },
     "OperatingStatus": {
         "command": 0x51800200,
         "response": 0x08412B00,
         "first": 0x08412B00,
         "last": 0x08412BFF,
     },
     "GeneralOperatingStatus": {
         "command": 0x51800200,
-        "response": 0x08412800,
-        "first": 0x08412800,
-        "last": 0x084128FF,
-        #"registers": [
-        #    {"name": "GeneralOperatingStatus", "format": "list", "offset": 142},
-        #],
+        "response": 0x00412800,
+        "first": 0x00412800,
+        "last": 0x004128FF,
+        "registers": [
+            {
+                "name": "GeneralOperatingStatus", "format": "list", "offset": 62,
+                "sensor":  Sensor(
+                    "GeneralOperatingStatus", Identifier.operating_status_genereal, factor=1, unit=None, mapper = SMATagList
+                )},
+        ],
     },
     "WaitingTimeUntilFeedIn": {
         "command": 0x51000200,
         "response": 0x00416600,
         "first": 0x00416600,
         "last": 0x004166FF,
         "registers": [
@@ -443,16 +437,16 @@
     "DeviceStatus": {
         "command": 0x51800200,
         "response": 0x00214800,
         "first": 0x00214800,
         "last": 0x002148FF,
         "registers": [
             {   
-                # TODO Schleife
                 "name": "inverter_status",
+                "format": "list",
                 "offset": 62,
                 "invalid": 0x80000000,
                 "sensor": Sensor(
                     "inverter_status", Identifier.status, factor=1, unit=None, mapper = SMATagList
                 ),
             }
         ],
@@ -614,15 +608,15 @@
                 ),
             },
             {
                 "name": "today",
                 "offset": 78,
                 "invalid": 0x8000000000000000,
                 "sensor": Sensor(
-                    "today", Identifier.daily_yield, factor=1000, unit="kWh"
+                    "today", Identifier.daily_yield, unit="Wh"
                 ),
             },
         ],
         # $inv_SPOT_ETODAY,$inv_SPOT_ETOTAL
     },
     "spot_ac_power": {
         "command": 0x51000200,
```

### Comparing `pysma_plus-0.2.3/pysmaplus/definitions_webconnect.py` & `pysma_plus-0.2.4/pysmaplus/definitions_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/pysmaplus/device_em.py` & `pysma_plus-0.2.4/pysmaplus/device_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/pysmaplus/device_ennexos.py` & `pysma_plus-0.2.4/pysmaplus/device_ennexos.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     SmaConnectionException,
     SmaReadException,
 )
 from .sensor import Sensors
 from .device import Device
 from .const import Identifier
 from .definitions_ennexos import ennexosSensorProfiles
+from .const import SMATagList
+
 
 _LOGGER = logging.getLogger(__name__)
 class SMAennexos(Device):
     """Class to connect to the ennexos based SMA inverters. (e.g. Tripower X Devices)"""
 
     # pylint: disable=too-many-instance-attributes
     _aio_session: ClientSession
@@ -348,7 +350,29 @@
         return {
             "device": self._last_device,
             "measurements": self._last_measurements,
             "parameters": self._last_parameters,
             "device_info": self._device_info
         }
 
+    async def detect(self, ip):
+        rets = []
+        for prefix in ["https", "http"]:
+            url = f"{prefix}://{ip}/api/v1/system/info"
+            ret = (await super().detect(ip))[0]
+            rets.append(ret)
+            ret["testedEndpoints"] = url
+            ret["remark"] = prefix
+            try:
+                dev = await self._jsonrequest(url,{}, hdrs.METH_GET)
+                if ("productFriendlyNameTagId" in dev):
+                    fallback = "Unkown: "+ str(dev["productFriendlyNameTagId"])
+                    ret["device"] = SMATagList.get(dev["productFriendlyNameTagId"], fallback)
+                    ret["status"] = "found"
+                    break
+                else:
+                    ret["status"] = "failed"
+                    ret["exception"] = dev
+            except Exception as e:
+                ret["status"] = "failed"
+                ret["exception"] = e
+        return rets
```

### Comparing `pysma_plus-0.2.3/pysmaplus/device_speedwire.py` & `pysma_plus-0.2.4/pysmaplus/device_speedwire.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#based on https://github.com/Wired-Square/sma-query/blob/main/src/sma_query_sw/protocol.py
+# based on https://github.com/Wired-Square/sma-query/blob/main/src/sma_query_sw/protocol.py
 import logging
 import time
 import ctypes
 import binascii
 import copy
 import collections
 import struct
@@ -531,7 +531,31 @@
         return {
             "msg": list(self._protocol.debug["msg"]),
             "data": self._protocol.debug["data"],
             "device_info": self._deviceinfo,
             "unfinished": list(self._protocol.debug["unfinished"])
        }
 
+
+    async def detect(self, ip) -> bool:
+        ret = await super().detect(ip)
+        try:
+            ret[0]["testedEndpoints"] = str(ip) + ":9522"
+            await self.new_session()
+            fut = asyncio.get_running_loop().create_future()
+            self._protocol.start_query(["TypeLabel"], fut, self._group)
+            try:
+                await asyncio.wait_for(fut, timeout=5)
+            except TimeoutError:
+                _LOGGER.warning("Timeout in device_info")
+            if "error" in self._protocol.inverter["data"] and self._protocol.inverter["data"]["error"] == 0:
+                raise SmaReadException("Reply for request not received")
+            else:
+                raise SmaConnectionException("No connection to device")
+        except SmaAuthenticationException as e:
+            ret[0]["status"] = "maybe"
+            ret[0]["exception"] = e
+            ret[0]["remark"] = "only unencrypted Speedwire is supported"
+        except Exception as e:
+            ret[0]["status"] = "failed"
+            ret[0]["exception"] = e
+        return ret
```

### Comparing `pysma_plus-0.2.3/pysmaplus/device_webconnect.py` & `pysma_plus-0.2.4/pysmaplus/device_webconnect.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,7 +472,30 @@
                         new_sensor.name = f"{sensor_definition.name}_{idx}"
                         device_sensors.add(new_sensor)
 
         return device_sensors
 
     async def get_debug(self) -> Dict:
         return {}
+
+
+    async def detect(self, ip) -> bool:
+        results = []
+        for urls in ["https://" + ip, "http://" + ip]:
+            self._url = urls
+            ret = await super().detect(ip)
+            ret[0]["remark"] = urls
+            try:
+                ret[0]["testedEndpoints"] = self._url
+                await self.new_session()
+            except SmaAuthenticationException as e:
+                if self._sid:
+                    ret[0]["status"] = "found"
+                    ret[0]["exception"] = e
+                else:
+                    ret[0]["status"] = "failed"
+                    ret[0]["exception"] = e
+            except Exception as e:
+                ret[0]["status"] = "failed"
+                ret[0]["exception"] = e
+            results.extend(ret)
+        return results
```

### Comparing `pysma_plus-0.2.3/pysmaplus/helpers.py` & `pysma_plus-0.2.4/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/pysmaplus/sensor.py` & `pysma_plus-0.2.4/pysmaplus/sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/setup.py` & `pysma_plus-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.2.3"
+VERSION = "0.2.4"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.2.3/tests/__init__.py` & `pysma_plus-0.2.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/test_em.py` & `pysma_plus-0.2.4/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/test_ennexos.py` & `pysma_plus-0.2.4/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/test_sensor.py` & `pysma_plus-0.2.4/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/test_webconnect.py` & `pysma_plus-0.2.4/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.4/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.4/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.4/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.4/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.3/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.4/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*

