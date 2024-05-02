# Comparing `tmp/habluetooth-2.8.1.tar.gz` & `tmp/habluetooth-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habluetooth-2.8.1.tar", max compression
+gzip compressed data, was "habluetooth-3.0.0.tar", max compression
```

## Comparing `habluetooth-2.8.1.tar` & `habluetooth-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11345 2024-05-02 22:30:35.614340 habluetooth-2.8.1/LICENSE
--rw-r--r--   0        0        0     3805 2024-05-02 22:30:35.614340 habluetooth-2.8.1/README.md
--rw-r--r--   0        0        0     1496 2024-05-02 22:30:35.614340 habluetooth-2.8.1/build_ext.py
--rw-r--r--   0        0        0     3819 2024-05-02 22:30:36.310341 habluetooth-2.8.1/pyproject.toml
--rw-r--r--   0        0        0     1457 2024-05-02 22:30:36.310341 habluetooth-2.8.1/src/habluetooth/__init__.py
--rw-r--r--   0        0        0      395 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/advertisement_tracker.pxd
--rw-r--r--   0        0        0     2809 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/advertisement_tracker.py
--rw-r--r--   0        0        0     1917 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/base_scanner.pxd
--rw-r--r--   0        0        0    16704 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/base_scanner.py
--rw-r--r--   0        0        0      650 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/central_manager.py
--rw-r--r--   0        0        0     1752 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/const.py
--rw-r--r--   0        0        0     2252 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/manager.pxd
--rw-r--r--   0        0        0    29213 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/manager.py
--rw-r--r--   0        0        0      726 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/models.pxd
--rw-r--r--   0        0        0     7310 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/models.py
--rw-r--r--   0        0        0        0 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/py.typed
--rw-r--r--   0        0        0      625 2024-05-02 22:30:35.614340 habluetooth-2.8.1/src/habluetooth/scanner.pxd
--rw-r--r--   0        0        0    19962 2024-05-02 22:30:35.618340 habluetooth-2.8.1/src/habluetooth/scanner.py
--rw-r--r--   0        0        0      530 2024-05-02 22:30:35.618340 habluetooth-2.8.1/src/habluetooth/scanner_device.py
--rw-r--r--   0        0        0     1733 2024-05-02 22:30:35.618340 habluetooth-2.8.1/src/habluetooth/usage.py
--rw-r--r--   0        0        0      544 2024-05-02 22:30:35.618340 habluetooth-2.8.1/src/habluetooth/util.py
--rw-r--r--   0        0        0    15031 2024-05-02 22:30:35.618340 habluetooth-2.8.1/src/habluetooth/wrappers.py
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 habluetooth-2.8.1/setup.py
--rw-r--r--   0        0        0     5133 1970-01-01 00:00:00.000000 habluetooth-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-02 22:58:48.099389 habluetooth-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3805 2024-05-02 22:58:48.099389 habluetooth-3.0.0/README.md
+-rw-r--r--   0        0        0     1496 2024-05-02 22:58:48.099389 habluetooth-3.0.0/build_ext.py
+-rw-r--r--   0        0        0     3819 2024-05-02 22:58:48.835394 habluetooth-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1457 2024-05-02 22:58:48.835394 habluetooth-3.0.0/src/habluetooth/__init__.py
+-rw-r--r--   0        0        0      395 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/advertisement_tracker.pxd
+-rw-r--r--   0        0        0     2809 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/advertisement_tracker.py
+-rw-r--r--   0        0        0     1917 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/base_scanner.pxd
+-rw-r--r--   0        0        0    16403 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/base_scanner.py
+-rw-r--r--   0        0        0      650 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/central_manager.py
+-rw-r--r--   0        0        0     1752 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/const.py
+-rw-r--r--   0        0        0     2252 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/manager.pxd
+-rw-r--r--   0        0        0    29252 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/manager.py
+-rw-r--r--   0        0        0      759 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/models.pxd
+-rw-r--r--   0        0        0     8102 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/models.py
+-rw-r--r--   0        0        0        0 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/py.typed
+-rw-r--r--   0        0        0      625 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/scanner.pxd
+-rw-r--r--   0        0        0    20135 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/scanner.py
+-rw-r--r--   0        0        0      530 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/scanner_device.py
+-rw-r--r--   0        0        0     1733 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/usage.py
+-rw-r--r--   0        0        0      544 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/util.py
+-rw-r--r--   0        0        0    15031 2024-05-02 22:58:48.103389 habluetooth-3.0.0/src/habluetooth/wrappers.py
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 habluetooth-3.0.0/setup.py
+-rw-r--r--   0        0        0     5133 1970-01-01 00:00:00.000000 habluetooth-3.0.0/PKG-INFO
```

### Comparing `habluetooth-2.8.1/LICENSE` & `habluetooth-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/README.md` & `habluetooth-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/build_ext.py` & `habluetooth-3.0.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/pyproject.toml` & `habluetooth-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "habluetooth"
-version = "2.8.1"
+version = "3.0.0"
 description = "High availability Bluetooth"
 authors = ["J. Nick Koston <bluetooth@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/habluetooth"
 documentation = "https://habluetooth.readthedocs.io"
 classifiers = [
```

### Comparing `habluetooth-2.8.1/src/habluetooth/__init__.py` & `habluetooth-3.0.0/src/habluetooth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.8.1"
+__version__ = "3.0.0"
 
 from .advertisement_tracker import (
     TRACKER_BUFFERING_WOBBLE_SECONDS,
     AdvertisementTracker,
 )
 from .base_scanner import BaseHaRemoteScanner, BaseHaScanner
 from .central_manager import get_manager, set_manager
```

### Comparing `habluetooth-2.8.1/src/habluetooth/advertisement_tracker.py` & `habluetooth-3.0.0/src/habluetooth/advertisement_tracker.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/base_scanner.pxd` & `habluetooth-3.0.0/src/habluetooth/base_scanner.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/base_scanner.py` & `habluetooth-3.0.0/src/habluetooth/base_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import logging
 from collections.abc import Generator
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Final, Iterable, final
 
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
-from bleak_retry_connector import NO_RSSI_VALUE
 from bluetooth_adapters import DiscoveredDeviceAdvertisementData, adapter_human_name
 from bluetooth_data_tools import monotonic_time_coarse
 
 from .central_manager import get_manager
 from .const import (
     CALLBACK_TYPE,
     CONNECTABLE_FALLBACK_MAXIMUM_STALE_ADVERTISEMENT_SECONDS,
@@ -234,14 +233,15 @@
                 adv.service_data,
                 adv.service_uuids,
                 self.source,
                 device,
                 adv,
                 self.connectable,
                 discovered_device_timestamps[address],
+                adv.tx_power,
             )
             for address, (
                 device,
                 adv,
             ) in history.discovered_device_advertisement_datas.items()
         }
         # Expire anything that is too old
@@ -418,35 +418,27 @@
             #
             device = prev_device
             device.name = local_name
             prev_details.update(details)
             # pylint: disable-next=protected-access
             device._rssi = rssi  # deprecated, will be removed in newer bleak
 
-        advertisement_data = AdvertisementData(
-            None if local_name == "" else local_name,
-            manufacturer_data,
-            service_data,
-            service_uuids,
-            NO_RSSI_VALUE if tx_power is None else tx_power,
-            rssi,
-            (),
-        )
         service_info = BluetoothServiceInfoBleak(
             local_name or address,
             address,
             rssi,
             manufacturer_data,
             service_data,
             service_uuids,
             self.source,
             device,
-            advertisement_data,
+            None,
             self.connectable,
             advertisement_monotonic_time,
+            tx_power,
         )
         self._previous_service_info[address] = service_info
         self._manager.scanner_adv_received(service_info)
 
     async def async_diagnostics(self) -> dict[str, Any]:
         """Return diagnostic information about the scanner."""
         now = monotonic_time_coarse()
```

### Comparing `habluetooth-2.8.1/src/habluetooth/central_manager.py` & `habluetooth-3.0.0/src/habluetooth/central_manager.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/const.py` & `habluetooth-3.0.0/src/habluetooth/const.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/manager.pxd` & `habluetooth-3.0.0/src/habluetooth/manager.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/manager.py` & `habluetooth-3.0.0/src/habluetooth/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,14 +563,15 @@
                 service_info.service_data,
                 service_info.service_uuids,
                 source,
                 service_info.device,
                 service_info.advertisement,
                 True,
                 service_info.time,
+                service_info.tx_power,
             )
 
         if (connectable or old_connectable_service_info is not None) and (
             bleak_callbacks := self._bleak_callbacks
         ) is not None:
             # Bleak callbacks must get a connectable device
             device = service_info.device
```

### Comparing `habluetooth-2.8.1/src/habluetooth/models.pxd` & `habluetooth-3.0.0/src/habluetooth/models.pxd`

 * *Files 8% similar despite different names*

```diff
@@ -21,10 +21,11 @@
     cdef public str source
 
 
 cdef class BluetoothServiceInfoBleak(BluetoothServiceInfo):
     """BluetoothServiceInfo with bleak data."""
 
     cdef public object device
-    cdef public object advertisement
     cdef public bint connectable
+    cdef public object _advertisement
     cdef public double time
+    cdef public object tx_power
```

### Comparing `habluetooth-2.8.1/src/habluetooth/models.py` & `habluetooth-3.0.0/src/habluetooth/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Final, TypeVar
 
 from bleak import BaseBleakClient
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
+from bleak_retry_connector import NO_RSSI_VALUE
 
 if TYPE_CHECKING:
     from .manager import BluetoothManager
 
 _BluetoothServiceInfoSelfT = TypeVar(
     "_BluetoothServiceInfoSelfT", bound="BluetoothServiceInfo"
 )
@@ -138,41 +139,58 @@
 
     Integrations may need BLEDevice and AdvertisementData
     to connect to the device without having bleak trigger
     another scan to translate the address to the system's
     internal details.
     """
 
-    __slots__ = ("device", "advertisement", "connectable", "time")
+    __slots__ = ("device", "_advertisement", "connectable", "time", "tx_power")
 
     def __init__(
         self,
         name: _str,  # may be a pyobjc object
         address: _str,  # may be a pyobjc object
         rssi: _int,  # may be a pyobjc object
         manufacturer_data: dict[_int, bytes],
         service_data: dict[_str, bytes],
         service_uuids: list[_str],
         source: _str,
         device: BLEDevice,
-        advertisement: AdvertisementData,
+        advertisement: AdvertisementData | None,
         connectable: bool,
         time: _float,
+        tx_power: _int | None,
     ) -> None:
         self.name = name
         self.address = address
         self.rssi = rssi
         self.manufacturer_data = manufacturer_data
         self.service_data = service_data
         self.service_uuids = service_uuids
         self.source = source
         self.device = device
-        self.advertisement = advertisement
+        self._advertisement = advertisement
         self.connectable = connectable
         self.time = time
+        self.tx_power = tx_power
+
+    @property
+    def advertisement(self) -> AdvertisementData:
+        """Get the advertisement data."""
+        if self._advertisement is None:
+            self._advertisement = AdvertisementData(
+                None if self.name == "" else self.name,
+                self.manufacturer_data,
+                self.service_data,
+                self.service_uuids,
+                NO_RSSI_VALUE if self.tx_power is None else self.tx_power,
+                self.rssi,
+                (),
+            )
+        return self._advertisement
 
     def as_dict(self) -> dict[str, Any]:
         """
         Return as dict.
 
         The dataclass asdict method is not used because
         it will try to deepcopy pyobjc data which will fail.
@@ -185,14 +203,15 @@
             "service_data": self.service_data,
             "service_uuids": self.service_uuids,
             "source": self.source,
             "advertisement": self.advertisement,
             "device": self.device,
             "connectable": self.connectable,
             "time": self.time,
+            "tx_power": self.tx_power,
         }
 
     @classmethod
     def from_scan(
         cls: type[_BluetoothServiceInfoBleakSelfT],
         source: str,
         device: BLEDevice,
@@ -209,14 +228,15 @@
             advertisement_data.service_data,
             advertisement_data.service_uuids,
             source,
             device,
             advertisement_data,
             connectable,
             monotonic_time,
+            advertisement_data.tx_power,
         )
 
     @classmethod
     def from_device_and_advertisement_data(
         cls: type[_BluetoothServiceInfoBleakSelfT],
         device: BLEDevice,
         advertisement_data: AdvertisementData,
@@ -233,8 +253,9 @@
             advertisement_data.service_data,
             advertisement_data.service_uuids,
             source,
             device,
             advertisement_data,
             connectable,
             time,
+            advertisement_data.tx_power,
         )
```

### Comparing `habluetooth-2.8.1/src/habluetooth/scanner.pxd` & `habluetooth-3.0.0/src/habluetooth/scanner.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/scanner.py` & `habluetooth-3.0.0/src/habluetooth/scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -232,27 +232,31 @@
             # Don't count empty advertisements
             # as the adapter is in a failure
             # state if all the data is empty.
             self._last_detection = callback_time
         name = advertisement_data.local_name or device.name or device.address
         if name is not None and type(name) is not str:
             name = str(name)
+        tx_power = advertisement_data.tx_power
+        if tx_power is not None and type(tx_power) is not int:
+            tx_power = int(tx_power)
         self._manager.scanner_adv_received(
             BluetoothServiceInfoBleak(
                 name,
                 device.address,
                 advertisement_data.rssi,
                 advertisement_data.manufacturer_data,
                 advertisement_data.service_data,
                 advertisement_data.service_uuids,
                 self.source,
                 device,
                 advertisement_data,
                 True,
                 callback_time,
+                tx_power,
             )
         )
 
     async def async_start(self) -> None:
         """Start bluetooth scanner."""
         async with self._start_stop_lock:
             await self._async_start()
```

### Comparing `habluetooth-2.8.1/src/habluetooth/scanner_device.py` & `habluetooth-3.0.0/src/habluetooth/scanner_device.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/usage.py` & `habluetooth-3.0.0/src/habluetooth/usage.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/util.py` & `habluetooth-3.0.0/src/habluetooth/util.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/src/habluetooth/wrappers.py` & `habluetooth-3.0.0/src/habluetooth/wrappers.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.8.1/setup.py` & `habluetooth-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'bleak>=0.21.1',
  'bluetooth-adapters>=0.16.1',
  'bluetooth-auto-recovery>=1.2.3',
  'bluetooth-data-tools>=1.16.0']
 
 setup_kwargs = {
     'name': 'habluetooth',
-    'version': '2.8.1',
+    'version': '3.0.0',
     'description': 'High availability Bluetooth',
     'long_description': '# habluetooth\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/habluetooth/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bluetooth-devices/habluetooth/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://habluetooth.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/habluetooth.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/habluetooth">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/habluetooth.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/habluetooth/">\n    <img src="https://img.shields.io/pypi/v/habluetooth.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/habluetooth.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/habluetooth.svg?style=flat-square" alt="License">\n</p>\n\n---\n\n**Documentation**: <a href="https://habluetooth.readthedocs.io" target="_blank">https://habluetooth.readthedocs.io </a>\n\n**Source Code**: <a href="https://github.com/bluetooth-devices/habluetooth" target="_blank">https://github.com/bluetooth-devices/habluetooth </a>\n\n---\n\nHigh availability Bluetooth\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install habluetooth`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'bluetooth@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/habluetooth',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['habluetooth'] package_data = \ {'': ['*']}
 install_requires = \ ['async-interrupt>=1.1.1', 'bleak-retry-connector>=3.3.0',
 'bleak>=0.21.1', 'bluetooth-adapters>=0.16.1', 'bluetooth-auto-
 recovery>=1.2.3', 'bluetooth-data-tools>=1.16.0'] setup_kwargs = { 'name':
-'habluetooth', 'version': '2.8.1', 'description': 'High availability
+'habluetooth', 'version': '3.0.0', 'description': 'High availability
 Bluetooth', 'long_description': '# habluetooth\n\n
     \n _\_n_ _[_C_I_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_T_e_s_t_ _c_o_v_e_r_a_g_e
                                _p_e_r_c_e_n_t_a_g_e_]_\_n_ \n
 \n
            \n _\_n_ _[_P_o_e_t_r_y_]_\_n_ \n _\_n_ _[_b_l_a_c_k_]_\_n_ \n _\_n_ _[_p_r_e_-_c_o_m_m_i_t_]_\_n_ \n
 \n
       \n _\_n_ _[_P_y_P_I_ _V_e_r_s_i_o_n_]_\_n_ \n [Supported Python versions]\n [License]\n
```

### Comparing `habluetooth-2.8.1/PKG-INFO` & `habluetooth-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habluetooth
-Version: 2.8.1
+Version: 3.0.0
 Summary: High availability Bluetooth
 Home-page: https://github.com/bluetooth-devices/habluetooth
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: bluetooth@koston.org
 Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: habluetooth Version: 2.8.1 Summary: High
+Metadata-Version: 2.1 Name: habluetooth Version: 3.0.0 Summary: High
 availability Bluetooth Home-page: https://github.com/bluetooth-devices/
 habluetooth License: Apache Software License 2.0 Author: J. Nick Koston Author-
 email: bluetooth@koston.org Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

