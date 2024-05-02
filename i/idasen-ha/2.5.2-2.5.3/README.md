# Comparing `tmp/idasen-ha-2.5.2.tar.gz` & `tmp/idasen_ha-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idasen-ha-2.5.2.tar", last modified: Thu Apr  4 23:26:20 2024, max compression
+gzip compressed data, was "idasen_ha-2.5.3.tar", last modified: Thu May  2 23:24:54 2024, max compression
```

## Comparing `idasen-ha-2.5.2.tar` & `idasen_ha-2.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.087425 idasen-ha-2.5.2/idasen_ha/
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/idasen_ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/idasen_ha/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/idasen_ha/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/idasen_ha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/tests/test_connection_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/tests/test_desk_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:24:54.075985 idasen_ha-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 23:24:54.075985 idasen_ha-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:24:54.071985 idasen_ha-2.5.3/idasen_ha/
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/idasen_ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/idasen_ha/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/idasen_ha/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:24:54.071985 idasen_ha-2.5.3/idasen_ha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 23:24:54.000000 idasen_ha-2.5.3/idasen_ha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-02 23:24:54.000000 idasen_ha-2.5.3/idasen_ha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:24:54.000000 idasen_ha-2.5.3/idasen_ha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 23:24:54.000000 idasen_ha-2.5.3/idasen_ha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 23:24:54.000000 idasen_ha-2.5.3/idasen_ha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:24:54.075985 idasen_ha-2.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:24:54.071985 idasen_ha-2.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/tests/test_connection_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-02 23:24:45.000000 idasen_ha-2.5.3/tests/test_desk_functions.py
```

### Comparing `idasen-ha-2.5.2/LICENSE` & `idasen_ha-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idasen-ha-2.5.2/PKG-INFO` & `idasen_ha-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idasen-ha
-Version: 2.5.2
+Version: 2.5.3
 Summary: Home Assistant helper lib for the IKEA Idasen Desk integration
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/idasen-ha/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `idasen-ha-2.5.2/idasen_ha/__init__.py` & `idasen_ha-2.5.3/idasen_ha/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import Callable
 
+from bleak import BleakClient
 from bleak.backends.device import BLEDevice
 from idasen import IdasenDesk
 
 from .connection_manager import ConnectionManager
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -20,70 +21,63 @@
     def __init__(
         self,
         update_callback: Callable[[int | None], None] | None,
         monitor_height: bool = True,
     ) -> None:
         """Initialize the wrapper."""
         self._idasen_desk: IdasenDesk | None = None
+        self._ble_device: BLEDevice | None = None
+        self._connection_manager: ConnectionManager | None = None
         self._height: float | None = None
+        self._monitor_height: bool = monitor_height
 
         if update_callback:
             self._update_callback = update_callback
         else:
 
             def empty_update_callback(height: int | None) -> None:
                 pass
 
             self._update_callback = empty_update_callback
 
-        async def connect_callback(idasen_desk: IdasenDesk):
-            _LOGGER.debug("Connect callback called")
-            self._idasen_desk = idasen_desk
-            if monitor_height:
-                self._height = await self._idasen_desk.get_height()
-                await self._start_monitoring()
-            self._update_callback(self.height_percent)
-
-        def disconnect_callback() -> None:
-            """Handle bluetooth disconnection."""
-            _LOGGER.debug("Disconnect callback called")
-            self._update_callback(self.height_percent)
-
-        self._connection_manager: ConnectionManager = ConnectionManager(
-            connect_callback=connect_callback, disconnect_callback=disconnect_callback
-        )
-
-    async def connect(
-        self,
-        ble_device: BLEDevice,
-        auto_reconnect: bool = True,
-    ) -> None:
+    async def connect(self, ble_device: BLEDevice, retry: bool = True) -> None:
         """Perform the bluetooth connection to the desk."""
         _LOGGER.debug("Connecting")
 
-        await self._connection_manager.connect(
-            ble_device, auto_reconnect=auto_reconnect
-        )
+        if (
+            self._connection_manager is None
+            or self._ble_device is None
+            or ble_device.address != self._ble_device.address
+        ):
+            _LOGGER.debug("Initializing idasen desk")
+            await self.disconnect()
+            self._ble_device = ble_device
+            self._idasen_desk = self._create_idasen_desk(self._ble_device)
+            self._connection_manager = self._create_connection_manager(
+                self._idasen_desk
+            )
+
+        await self._connection_manager.connect(retry=retry)
 
     async def disconnect(self) -> None:
         """Disconnect from the desk."""
-        _LOGGER.debug("Disconnecting")
-        await self._connection_manager.disconnect()
-        self._idasen_desk = None
+        if self._connection_manager:
+            _LOGGER.debug("Disconnecting")
+            await self._connection_manager.disconnect()
 
     async def move_to(self, heigh_percent: int) -> None:
         """Move the desk to a specific position."""
         _LOGGER.debug("Moving to %s", heigh_percent)
         if not self.is_connected or self._idasen_desk is None:
             _LOGGER.warning("Not connected")
             return
 
         if self._idasen_desk.is_moving:
             await self._idasen_desk.stop()
-            # Let it settle before requesting new move
+            # Let it settle before requesting a new move
             await asyncio.sleep(0.5)
 
         height = IdasenDesk.MIN_HEIGHT + (
             IdasenDesk.MAX_HEIGHT - IdasenDesk.MIN_HEIGHT
         ) * (heigh_percent / 100)
 
         await self._idasen_desk.move_to_target(height)
@@ -142,7 +136,35 @@
         """True if the bluetooth connection is currently established."""
         if self._idasen_desk is None:
             return False
         # bleak `is_connected` method returns a `_DeprecatedIsConnectedReturn`,
         # so we properly cast it to bool otherwise `is_connected == True`
         # will always be False.
         return bool(self._idasen_desk.is_connected)
+
+    def _create_idasen_desk(self, ble_device: BLEDevice) -> IdasenDesk:
+        def disconnect_callback(client: BleakClient) -> None:
+            """Handle bluetooth disconnection."""
+            _LOGGER.debug("Disconnect callback called")
+            self._update_callback(self.height_percent)
+
+        return IdasenDesk(
+            ble_device, exit_on_fail=False, disconnected_callback=disconnect_callback
+        )
+
+    def _create_connection_manager(self, desk: IdasenDesk) -> ConnectionManager:
+        async def connect_callback() -> None:
+            _LOGGER.debug("Connect callback called")
+            if self._idasen_desk is None:
+                _LOGGER.error("Desk is None after connecting")
+                return
+
+            if self._monitor_height:
+                self._height = await self._idasen_desk.get_height()
+                await self._start_monitoring()
+
+            self._update_callback(self.height_percent)
+
+        return ConnectionManager(
+            desk,
+            connect_callback=connect_callback,
+        )
```

### Comparing `idasen-ha-2.5.2/idasen_ha.egg-info/PKG-INFO` & `idasen_ha-2.5.3/idasen_ha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idasen-ha
-Version: 2.5.2
+Version: 2.5.3
 Summary: Home Assistant helper lib for the IKEA Idasen Desk integration
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/idasen-ha/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `idasen-ha-2.5.2/pyproject.toml` & `idasen_ha-2.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idasen-ha"
-version = "2.5.2"
+version = "2.5.3"
 authors = [{name = "Abílio Costa", email = "amfcalt@gmail.com"}]
 description = "Home Assistant helper lib for the IKEA Idasen Desk integration"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `idasen-ha-2.5.2/tests/test_connection_management.py` & `idasen_ha-2.5.3/tests/test_connection_management.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests for idasen_ha."""
 
 import asyncio
 from unittest import mock
 from unittest.mock import MagicMock, Mock
 
+from bleak.backends.device import BLEDevice
 from bleak.exc import BleakDBusError, BleakError
 import pytest
 
 from idasen_ha import Desk
 from idasen_ha.connection_manager import AuthFailedError
 
 from . import FAKE_BLE_DEVICE
@@ -27,34 +28,60 @@
     await desk.disconnect()
     await desk.disconnect()  # double disconnect should be a no-op
     assert not desk.is_connected
     mock_idasen_desk.disconnect.assert_called()
     assert update_callback.call_count == 2
 
 
-async def test_double_connect_call(mock_idasen_desk: MagicMock):
-    """Test connect being called again, while still connecting."""
+async def test_double_connect_call_with_same_bledevice(mock_idasen_desk: MagicMock):
+    """Test connect being called again with the same BLEDevice, while still connecting."""
     update_callback = Mock()
     desk = Desk(update_callback, False)
 
     default_connect_side_effect = mock_idasen_desk.connect.side_effect
 
     async def connect_side_effect():
+        # call the seccond `connect` while the first is ongoing
         await desk.connect(FAKE_BLE_DEVICE)
         await default_connect_side_effect()
 
     mock_idasen_desk.connect.side_effect = connect_side_effect
 
     await desk.connect(FAKE_BLE_DEVICE)
     assert desk.is_connected
     mock_idasen_desk.connect.assert_awaited()
     mock_idasen_desk.pair.assert_called()
     assert update_callback.call_count == 1
 
 
+async def test_double_connect_call_with_different_bledevice():
+    """Test connect being called again with a new BLEDevice, while still connecting."""
+
+    with mock.patch("idasen_ha.IdasenDesk", autospec=True) as patched_idasen_desk:
+        mock_idasen_desk = patched_idasen_desk.return_value
+
+        async def connect_side_effect():
+            # call the seccond `connect` while the first is ongoing
+            mock_idasen_desk.connect.side_effect = MagicMock()
+            new_ble_device = BLEDevice("AA:BB:CC:DD:EE:AA", None, None, 0)
+            await desk.connect(new_ble_device)
+
+        mock_idasen_desk.is_connected = False
+        mock_idasen_desk.connect.side_effect = connect_side_effect
+
+        update_callback = Mock()
+        desk = Desk(update_callback, False)
+        await desk.connect(FAKE_BLE_DEVICE)
+
+        mock_idasen_desk.connect.assert_awaited()
+        mock_idasen_desk.pair.assert_called()
+        assert update_callback.call_count == 2
+        assert patched_idasen_desk.call_count == 2
+
+
 @mock.patch("idasen_ha.connection_manager.asyncio.sleep")
 async def test_connect_called_while_retry_pending(
     sleep_mock,
     mock_idasen_desk: MagicMock,
 ) -> None:
     """Test connect being called while a retry is pending."""
     retry_maxed_future = asyncio.Future()
@@ -82,15 +109,15 @@
 
 async def test_connect_raises_without_auto_reconnect(mock_idasen_desk: MagicMock):
     """Test that connect raises if auto_reconnect is False."""
     desk = Desk(Mock(), False)
 
     mock_idasen_desk.connect.side_effect = TimeoutError()
     with pytest.raises(TimeoutError):
-        await desk.connect(FAKE_BLE_DEVICE, auto_reconnect=False)
+        await desk.connect(FAKE_BLE_DEVICE, retry=False)
     assert not desk.is_connected
 
 
 @pytest.mark.parametrize(
     ("pair_exception", "raised_exception"),
     [
         (Exception(), Exception),
@@ -102,15 +129,15 @@
 ):
     """Test that disconnect is called if pair fails."""
     update_callback = Mock()
     desk = Desk(update_callback, False)
 
     mock_idasen_desk.pair.side_effect = pair_exception
     with pytest.raises(raised_exception):
-        await desk.connect(FAKE_BLE_DEVICE, auto_reconnect=False)
+        await desk.connect(FAKE_BLE_DEVICE, retry=False)
     assert not desk.is_connected
     mock_idasen_desk.disconnect.assert_called()
     assert update_callback.call_count == 1
 
 
 @mock.patch("idasen_ha.connection_manager.asyncio.sleep")
 @pytest.mark.parametrize("exception", [TimeoutError(), BleakError()])
@@ -124,18 +151,18 @@
     """Test connect retries on connection exception."""
     TEST_RETRIES_MAX = 3
     retry_count = 0
     retry_maxed_future = asyncio.Future()
 
     async def sleep_handler(delay):
         nonlocal retry_count
+        retry_count = retry_count + 1
         if retry_count == TEST_RETRIES_MAX:
-            await desk.disconnect()
+            asyncio.get_event_loop().create_task(desk.disconnect())
             retry_maxed_future.set_result(None)
-        retry_count = retry_count + 1
 
     sleep_mock.side_effect = sleep_handler
 
     desk = Desk(Mock(), False)
 
     getattr(mock_idasen_desk, fail_call_name).side_effect = exception
     await desk.connect(FAKE_BLE_DEVICE)
```

### Comparing `idasen-ha-2.5.2/tests/test_desk_functions.py` & `idasen_ha-2.5.3/tests/test_desk_functions.py`

 * *Files identical despite different names*

