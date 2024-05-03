# Comparing `tmp/python-snap7-1.3.tar.gz` & `tmp/python_snap7-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-snap7-1.3.tar", last modified: Tue Jan 17 07:13:11 2023, max compression
+gzip compressed data, was "python_snap7-1.4.tar", last modified: Fri May  3 10:38:25 2024, max compression
```

## Comparing `python-snap7-1.3.tar` & `python_snap7-1.4.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2023-01-17 07:13:11.918081 python-snap7-1.3/
--rw-r--r--   0 gijsm      (501) staff       (20)     1097 2023-01-17 07:13:01.000000 python-snap7-1.3/LICENSE
--rw-r--r--   0 gijsm      (501) staff       (20)       20 2023-01-17 07:13:01.000000 python-snap7-1.3/MANIFEST.in
--rw-r--r--   0 gijsm      (501) staff       (20)     2209 2023-01-17 07:13:11.918208 python-snap7-1.3/PKG-INFO
--rw-r--r--   0 gijsm      (501) staff       (20)     1319 2023-01-17 07:13:01.000000 python-snap7-1.3/README.rst
-drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2023-01-17 07:13:11.904513 python-snap7-1.3/python_snap7.egg-info/
--rw-r--r--   0 gijsm      (501) staff       (20)     2209 2023-01-17 07:13:11.000000 python-snap7-1.3/python_snap7.egg-info/PKG-INFO
--rw-r--r--   0 gijsm      (501) staff       (20)      632 2023-01-17 07:13:11.000000 python-snap7-1.3/python_snap7.egg-info/SOURCES.txt
--rw-r--r--   0 gijsm      (501) staff       (20)        1 2023-01-17 07:13:11.000000 python-snap7-1.3/python_snap7.egg-info/dependency_links.txt
--rw-r--r--   0 gijsm      (501) staff       (20)       60 2023-01-17 07:13:11.000000 python-snap7-1.3/python_snap7.egg-info/entry_points.txt
--rw-r--r--   0 gijsm      (501) staff       (20)      108 2023-01-17 07:13:11.000000 python-snap7-1.3/python_snap7.egg-info/requires.txt
--rw-r--r--   0 gijsm      (501) staff       (20)        6 2023-01-17 07:13:11.000000 python-snap7-1.3/python_snap7.egg-info/top_level.txt
--rw-r--r--   0 gijsm      (501) staff       (20)      160 2023-01-17 07:13:11.919477 python-snap7-1.3/setup.cfg
--rw-r--r--   0 gijsm      (501) staff       (20)     1872 2023-01-17 07:13:01.000000 python-snap7-1.3/setup.py
-drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2023-01-17 07:13:11.911425 python-snap7-1.3/snap7/
--rw-r--r--   0 gijsm      (501) staff       (20)      416 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/__init__.py
-drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2023-01-17 07:13:11.912136 python-snap7-1.3/snap7/client/
--rw-r--r--   0 gijsm      (501) staff       (20)    52588 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/client/__init__.py
--rw-r--r--   0 gijsm      (501) staff       (20)     4496 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/common.py
--rw-r--r--   0 gijsm      (501) staff       (20)     3591 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/error.py
--rw-r--r--   0 gijsm      (501) staff       (20)       90 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/exceptions.py
--rw-r--r--   0 gijsm      (501) staff       (20)    12056 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/logo.py
--rw-r--r--   0 gijsm      (501) staff       (20)     7926 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/partner.py
--rw-r--r--   0 gijsm      (501) staff       (20)        0 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/py.typed
-drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2023-01-17 07:13:11.913265 python-snap7-1.3/snap7/server/
--rw-r--r--   0 gijsm      (501) staff       (20)    16807 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/server/__init__.py
--rw-r--r--   0 gijsm      (501) staff       (20)     1695 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/server/__main__.py
--rwxr-xr-x   0 gijsm      (501) staff       (20)     8010 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/types.py
--rw-r--r--   0 gijsm      (501) staff       (20)    62580 2023-01-17 07:13:01.000000 python-snap7-1.3/snap7/util.py
-drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2023-01-17 07:13:11.917625 python-snap7-1.3/test/
--rwxr-xr-x   0 gijsm      (501) staff       (20)    39350 2023-01-17 07:13:01.000000 python-snap7-1.3/test/test_client.py
--rw-r--r--   0 gijsm      (501) staff       (20)      721 2023-01-17 07:13:01.000000 python-snap7-1.3/test/test_common.py
--rw-r--r--   0 gijsm      (501) staff       (20)     3421 2023-01-17 07:13:01.000000 python-snap7-1.3/test/test_logo_client.py
--rw-r--r--   0 gijsm      (501) staff       (20)     5019 2023-01-17 07:13:01.000000 python-snap7-1.3/test/test_mainloop.py
--rw-r--r--   0 gijsm      (501) staff       (20)     4301 2023-01-17 07:13:01.000000 python-snap7-1.3/test/test_partner.py
--rw-r--r--   0 gijsm      (501) staff       (20)     5340 2023-01-17 07:13:01.000000 python-snap7-1.3/test/test_server.py
--rw-r--r--   0 gijsm      (501) staff       (20)    20611 2023-01-17 07:13:01.000000 python-snap7-1.3/test/test_util.py
+drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.133252 python_snap7-1.4/
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     1097 2024-05-02 10:39:46.000000 python_snap7-1.4/LICENSE
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)       19 2024-05-02 10:39:46.000000 python_snap7-1.4/MANIFEST.in
+-rw-r--r--   0 gijs      (1000) gijs      (1000)     1298 2024-05-03 10:38:25.133252 python_snap7-1.4/PKG-INFO
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)      699 2024-05-03 09:44:07.000000 python_snap7-1.4/README.rst
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     1695 2024-05-03 09:44:07.000000 python_snap7-1.4/pyproject.toml
+drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.132252 python_snap7-1.4/python_snap7.egg-info/
+-rw-r--r--   0 gijs      (1000) gijs      (1000)     1298 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/PKG-INFO
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)      705 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/SOURCES.txt
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)        1 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/dependency_links.txt
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)       60 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/entry_points.txt
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)       91 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/requires.txt
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)        6 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/top_level.txt
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)       38 2024-05-03 10:38:25.133252 python_snap7-1.4/setup.cfg
+drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.131252 python_snap7-1.4/snap7/
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)      418 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/__init__.py
+drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.131252 python_snap7-1.4/snap7/client/
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)    52714 2024-05-03 10:38:12.000000 python_snap7-1.4/snap7/client/__init__.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     4812 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/common.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     3591 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/error.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)       81 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/exceptions.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)    11808 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/logo.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     7643 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/partner.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)        0 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/py.typed
+drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.131252 python_snap7-1.4/snap7/server/
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)    16440 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/server/__init__.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     1676 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/server/__main__.py
+-rwxrwxr-x   0 gijs      (1000) gijs      (1000)     8007 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/types.py
+drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.132252 python_snap7-1.4/snap7/util/
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     5809 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/util/__init__.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)    21098 2024-05-03 09:44:07.000000 python_snap7-1.4/snap7/util/db.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)    22786 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/util/getters.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)    16703 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/util/setters.py
+drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.132252 python_snap7-1.4/tests/
+-rwxrwxr-x   0 gijs      (1000) gijs      (1000)    39525 2024-05-03 10:38:12.000000 python_snap7-1.4/tests/test_client.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)      755 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_common.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     3495 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_logo_client.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     5290 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_mainloop.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     4275 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_partner.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)     5314 2024-05-03 09:44:07.000000 python_snap7-1.4/tests/test_server.py
+-rw-rw-r--   0 gijs      (1000) gijs      (1000)    19902 2024-05-03 09:44:07.000000 python_snap7-1.4/tests/test_util.py
```

### Comparing `python-snap7-1.3/LICENSE` & `python_snap7-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-snap7-1.3/python_snap7.egg-info/SOURCES.txt` & `python_snap7-1.4/python_snap7.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
-setup.py
+pyproject.toml
 python_snap7.egg-info/PKG-INFO
 python_snap7.egg-info/SOURCES.txt
 python_snap7.egg-info/dependency_links.txt
 python_snap7.egg-info/entry_points.txt
 python_snap7.egg-info/requires.txt
 python_snap7.egg-info/top_level.txt
 snap7/__init__.py
 snap7/common.py
 snap7/error.py
 snap7/exceptions.py
 snap7/logo.py
 snap7/partner.py
 snap7/py.typed
 snap7/types.py
-snap7/util.py
 snap7/client/__init__.py
 snap7/server/__init__.py
 snap7/server/__main__.py
-test/test_client.py
-test/test_common.py
-test/test_logo_client.py
-test/test_mainloop.py
-test/test_partner.py
-test/test_server.py
-test/test_util.py
+snap7/util/__init__.py
+snap7/util/db.py
+snap7/util/getters.py
+snap7/util/setters.py
+tests/test_client.py
+tests/test_common.py
+tests/test_logo_client.py
+tests/test_mainloop.py
+tests/test_partner.py
+tests/test_server.py
+tests/test_util.py
```

### Comparing `python-snap7-1.3/snap7/client/__init__.py` & `python_snap7-1.4/snap7/client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Snap7 client used for connection to a siemens 7 server.
 """
+
 import re
 import logging
-from ctypes import byref, create_string_buffer, sizeof
+from ctypes import CFUNCTYPE, byref, create_string_buffer, sizeof
 from ctypes import Array, c_byte, c_char_p, c_int, c_int32, c_uint16, c_ulong, c_void_p
 from datetime import datetime
-from typing import List, Optional, Tuple, Union
+from typing import Any, Callable, List, Optional, Tuple, Union
 
 from ..common import check_error, ipv4, load_library
 from ..types import S7SZL, Areas, BlocksList, S7CpInfo, S7CpuInfo, S7DataItem
 from ..types import S7OrderCode, S7Protection, S7SZLList, TS7BlockInfo, WordLen
 from ..types import S7Object, buffer_size, buffer_type, cpu_statuses, param_types
-from ..types import S7CpuInfo, RemotePort, wordlen_to_ctypes, block_types
+from ..types import RemotePort, wordlen_to_ctypes, block_types
+
 logger = logging.getLogger(__name__)
 
 
 def error_wrap(func):
     """Parses a s7 error code returned the decorated function."""
 
     def f(*args, **kw):
@@ -64,16 +66,15 @@
         self._library = load_library(lib_location)
         self.create()
 
     def __del__(self):
         self.destroy()
 
     def create(self):
-        """Creates a SNAP7 client.
-        """
+        """Creates a SNAP7 client."""
         logger.info("creating snap7 client")
         self._library.Cli_Create.restype = c_void_p
         self._pointer = S7Object(self._library.Cli_Create())
 
     def destroy(self) -> Optional[int]:
         """Destroys the Client object.
 
@@ -186,17 +187,15 @@
             >>> import snap7
             >>> client = snap7.client.Client()
             >>> client.connect("192.168.0.1", 0, 0)  # port is implicit = 102.
         """
         logger.info(f"connecting to {address}:{tcpport} rack {rack} slot {slot}")
 
         self.set_param(RemotePort, tcpport)
-        return self._library.Cli_ConnectTo(
-            self._pointer, c_char_p(address.encode()),
-            c_int(rack), c_int(slot))
+        return self._library.Cli_ConnectTo(self._pointer, c_char_p(address.encode()), c_int(rack), c_int(slot))
 
     def db_read(self, db_number: int, start: int, size: int) -> bytearray:
         """Reads a part of a DB from a PLC
 
         Note:
             Use it only for reading DBs, not Marks, Inputs, Outputs.
 
@@ -216,17 +215,15 @@
             >>> buffer
             bytearray(b'\\x00\\x00')
         """
         logger.debug(f"db_read, db_number:{db_number}, start:{start}, size:{size}")
 
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         data = (type_ * size)()
-        result = (self._library.Cli_DBRead(
-            self._pointer, db_number, start, size,
-            byref(data)))
+        result = self._library.Cli_DBRead(self._pointer, db_number, start, size, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     @error_wrap
     def db_write(self, db_number: int, start: int, data: bytearray) -> int:
         """Writes a part of a DB into a PLC.
 
@@ -246,16 +243,15 @@
             >>> client.db_write(1, 10, buffer)  # writes the bit number 0 from the byte 10 to TRUE.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         size = len(data)
         cdata = (type_ * size).from_buffer_copy(data)
         logger.debug(f"db_write db_number:{db_number} start:{start} size:{size} data:{data}")
-        return self._library.Cli_DBWrite(self._pointer, db_number, start, size,
-                                         byref(cdata))
+        return self._library.Cli_DBWrite(self._pointer, db_number, start, size, byref(cdata))
 
     def delete(self, block_type: str, block_num: int) -> int:
         """Delete a block into AG.
 
         Args:
             block_type: type of block.
             block_num: block number.
@@ -279,42 +275,39 @@
 
         Returns:
             Tuple of the buffer and size.
         """
         _buffer = buffer_type()
         size = c_int(sizeof(_buffer))
         block_type = block_types[_type]
-        result = self._library.Cli_FullUpload(self._pointer, block_type,
-                                              block_num, byref(_buffer),
-                                              byref(size))
+        result = self._library.Cli_FullUpload(self._pointer, block_type, block_num, byref(_buffer), byref(size))
         check_error(result, context="client")
-        return bytearray(_buffer)[:size.value], size.value
+        return bytearray(_buffer)[: size.value], size.value
 
     def upload(self, block_num: int) -> bytearray:
         """Uploads a block from AG.
 
         Note:
             Upload means from the PLC to the PC.
 
         Args:
             block_num: block to be upload.
 
         Returns:
             Buffer with the uploaded block.
         """
         logger.debug(f"db_upload block_num: {block_num}")
-        block_type = block_types['DB']
+        block_type = block_types["DB"]
         _buffer = buffer_type()
         size = c_int(sizeof(_buffer))
 
-        result = self._library.Cli_Upload(self._pointer, block_type, block_num,
-                                          byref(_buffer), byref(size))
+        result = self._library.Cli_Upload(self._pointer, block_type, block_num, byref(_buffer), byref(size))
 
         check_error(result, context="client")
-        logger.info(f'received {size} bytes')
+        logger.info(f"received {size} bytes")
         return bytearray(_buffer)
 
     @error_wrap
     def download(self, data: bytearray, block_num: int = -1) -> int:
         """Download a block into AG.
         A whole block (including header and footer) must be available into the
         user buffer.
@@ -328,16 +321,15 @@
 
         Returns:
             Error code from snap7 library.
         """
         type_ = c_byte
         size = len(data)
         cdata = (type_ * len(data)).from_buffer_copy(data)
-        return self._library.Cli_Download(self._pointer, block_num,
-                                          byref(cdata), size)
+        return self._library.Cli_Download(self._pointer, block_num, byref(cdata), size)
 
     def db_get(self, db_number: int) -> bytearray:
         """Uploads a DB from AG using DBRead.
 
         Note:
             This method can't be use for 1200/1500 PLCs.
 
@@ -353,57 +345,57 @@
             >>> client.connect("192.168.0.1", 0, 0)
             >>> buffer = client.db_get(1)  # reads the db number 1.
             >>> buffer
             bytearray(b"\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00...<truncated>\\x00\\x00")
         """
         logger.debug(f"db_get db_number: {db_number}")
         _buffer = buffer_type()
-        result = self._library.Cli_DBGet(
-            self._pointer, db_number, byref(_buffer),
-            byref(c_int(buffer_size)))
+        result = self._library.Cli_DBGet(self._pointer, db_number, byref(_buffer), byref(c_int(buffer_size)))
         check_error(result, context="client")
         return bytearray(_buffer)
 
     def read_area(self, area: Areas, dbnumber: int, start: int, size: int) -> bytearray:
         """Reads a data area from a PLC
-        With it you can read DB, Inputs, Outputs, Merkers, Timers and Counters.
+                With it you can read DB, Inputs, Outputs, Merkers, Timers and Counters.
 
-        Args:
-            area: area to be read from.
-            dbnumber: number of the db to be read from. In case of Inputs, Marks or Outputs, this should be equal to 0.
-            start: byte index to start reading.
-            size: number of bytes to read.
-
-        Returns:
-            Buffer with the data read.
-
-        Raises:
-            :obj:`ValueError`: if the area is not defined in the `Areas`
-
-        Example:
-            >>> import snap7
-            >>> client = snap7.client.Client()
-            >>> client.connect("192.168.0.1", 0, 0)
-            >>> buffer = client.read_area(Areas.DB, 1, 10, 4)  # Reads the DB number 1 from the byte 10 to the byte 14.
-            >>> buffer
-            bytearray(b'\\x00\\x00')
+                Args:
+                    area: area to be read from.
+                    dbnumber: number of the db to be read from. In case of Inputs, Marks or Outputs, this should be equal to 0.
+                    start: byte index to start reading.
+                    size: number of bytes to read.
+
+                Returns:
+                    Buffer with the data read.
+
+                Raises:
+                    :obj:`ValueError`: if the area is not defined in the `Areas`
+
+                Example:
+        import snap7.util.db            >>> import snap7
+                    >>> client = snap7.client.Client()
+                    >>> client.connect("192.168.0.1", 0, 0)
+                    >>> buffer = client.read_area(snap7.util.db.DB, 1, 10, 4)  # Reads the DB number 1 from the byte 10 to the byte 14.
+                    >>> buffer
+                    bytearray(b'\\x00\\x00')
         """
         if area not in Areas:
             raise ValueError(f"{area} is not implemented in types")
         elif area == Areas.TM:
             wordlen = WordLen.Timer
         elif area == Areas.CT:
             wordlen = WordLen.Counter
         else:
             wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
-        logger.debug(f"reading area: {area.name} dbnumber: {dbnumber} start: {start}: amount {size}: wordlen: {wordlen.name}={wordlen.value}")
+        logger.debug(
+            f"reading area: {area.name} dbnumber: {dbnumber} start: {start} amount: {size} "
+            f"wordlen: {wordlen.name}={wordlen.value}"
+        )
         data = (type_ * size)()
-        result = self._library.Cli_ReadArea(self._pointer, area.value, dbnumber, start,
-                                            size, wordlen.value, byref(data))
+        result = self._library.Cli_ReadArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     @error_wrap
     def write_area(self, area: Areas, dbnumber: int, start: int, data: bytearray) -> int:
         """Writes a data area into a PLC.
 
@@ -413,45 +405,47 @@
             start: byte index to start writting.
             data: buffer to be write.
 
         Returns:
             Snap7 error code.
 
         Exmaple:
+            >>> import snap7.util.db
             >>> import snap7
             >>> client = snap7.client.Client()
             >>> client.connect("192.168.0.1", 0, 0)
             >>> buffer = bytearray([0b00000001])
-            >>> client.write_area(Areas.DB, 1, 10, buffer)  # Writes the bit 0 of the byte 10 from the DB number 1 to TRUE.
+            # Writes the bit 0 of the byte 10 from the DB number 1 to TRUE.
+            >>> client.write_area(snap7.util.DB, 1, 10, buffer)
         """
         if area == Areas.TM:
             wordlen = WordLen.Timer
         elif area == Areas.CT:
             wordlen = WordLen.Counter
         else:
             wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         size = len(data)
-        logger.debug(f"writing area: {area.name} dbnumber: {dbnumber} start: {start}: size {size}: "
-                     f"wordlen {wordlen.name}={wordlen.value} type: {type_}")
+        logger.debug(
+            f"writing area: {area.name} dbnumber: {dbnumber} start: {start}: size {size}: "
+            f"wordlen {wordlen.name}={wordlen.value} type: {type_}"
+        )
         cdata = (type_ * len(data)).from_buffer_copy(data)
-        return self._library.Cli_WriteArea(self._pointer, area.value, dbnumber, start,
-                                           size, wordlen.value, byref(cdata))
+        return self._library.Cli_WriteArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, byref(cdata))
 
     def read_multi_vars(self, items) -> Tuple[int, S7DataItem]:
         """Reads different kind of variables from a PLC simultaneously.
 
         Args:
             items: list of items to be read.
 
         Returns:
             Tuple with the return code from the snap7 library and the list of items.
         """
-        result = self._library.Cli_ReadMultiVars(self._pointer, byref(items),
-                                                 c_int32(len(items)))
+        result = self._library.Cli_ReadMultiVars(self._pointer, byref(items), c_int32(len(items)))
         check_error(result, context="client")
         return result, items
 
     def list_blocks(self) -> BlocksList:
         """Returns the AG blocks amount divided by type.
 
         Returns:
@@ -490,18 +484,15 @@
         logger.debug(f"listing blocks of type: {_blocktype} size: {size}")
 
         if size == 0:
             return 0
 
         data = (c_uint16 * size)()
         count = c_int(size)
-        result = self._library.Cli_ListBlocksOfType(
-            self._pointer, _blocktype,
-            byref(data),
-            byref(count))
+        result = self._library.Cli_ListBlocksOfType(self._pointer, _blocktype, byref(data), byref(count))
 
         logger.debug(f"number of items found: {count}")
 
         check_error(result, context="client")
         return data
 
     def get_block_info(self, blocktype: str, db_number: int) -> TS7BlockInfo:
@@ -559,16 +550,15 @@
             Snap7 code.
 
         Raises:
             :obj:`ValueError`: if the length of the `password` is more than 8 characters.
         """
         if len(password) > 8:
             raise ValueError("Maximum password length is 8")
-        return self._library.Cli_SetSessionPassword(self._pointer,
-                                                    c_char_p(password.encode()))
+        return self._library.Cli_SetSessionPassword(self._pointer, c_char_p(password.encode()))
 
     @error_wrap
     def clear_session_password(self) -> int:
         """Clears the password set for the current session (logout).
 
         Returns:
             Snap7 code.
@@ -589,32 +579,29 @@
         Raises:
             :obj:`ValueError`: if the `address` is not a valid IPV4.
             :obj:`ValueError`: if the result of setting the connection params is
                 different than 0.
         """
         if not re.match(ipv4, address):
             raise ValueError(f"{address} is invalid ipv4")
-        result = self._library.Cli_SetConnectionParams(self._pointer, address,
-                                                       c_uint16(local_tsap),
-                                                       c_uint16(remote_tsap))
+        result = self._library.Cli_SetConnectionParams(self._pointer, address, c_uint16(local_tsap), c_uint16(remote_tsap))
         if result != 0:
             raise ValueError("The parameter was invalid")
 
     def set_connection_type(self, connection_type: int):
-        """ Sets the connection resource type, i.e the way in which the Clients connects to a PLC.
+        """Sets the connection resource type, i.e the way in which the Clients connects to a PLC.
 
         Args:
             connection_type: 1 for PG, 2 for OP, 3 to 10 for S7 Basic
 
         Raises:
             :obj:`ValueError`: if the result of setting the connection type is
                 different than 0.
         """
-        result = self._library.Cli_SetConnectionType(self._pointer,
-                                                     c_uint16(connection_type))
+        result = self._library.Cli_SetConnectionType(self._pointer, c_uint16(connection_type))
         if result != 0:
             raise ValueError("The parameter was invalid")
 
     def get_connected(self) -> bool:
         """Returns the connection status
 
         Note:
@@ -638,16 +625,15 @@
         Returns:
             Buffer with the data read.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         data = (type_ * size)()
         logger.debug(f"ab_read: start: {start}: size {size}: ")
-        result = self._library.Cli_ABRead(self._pointer, start, size,
-                                          byref(data))
+        result = self._library.Cli_ABRead(self._pointer, start, size, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     def ab_write(self, start: int, data: bytearray) -> int:
         """Writes a part of IPU area into a PLC.
 
         Args:
@@ -658,31 +644,29 @@
             Snap7 code.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         size = len(data)
         cdata = (type_ * size).from_buffer_copy(data)
         logger.debug(f"ab write: start: {start}: size: {size}: ")
-        return self._library.Cli_ABWrite(
-            self._pointer, start, size, byref(cdata))
+        return self._library.Cli_ABWrite(self._pointer, start, size, byref(cdata))
 
     def as_ab_read(self, start: int, size: int, data) -> int:
         """Reads a part of IPU area from a PLC asynchronously.
 
         Args:
             start: byte index from where start to read.
             size: amount of bytes to read.
             data: buffer where the data will be place.
 
         Returns:
             Snap7 code.
         """
         logger.debug(f"ab_read: start: {start}: size {size}: ")
-        result = self._library.Cli_AsABRead(self._pointer, start, size,
-                                            byref(data))
+        result = self._library.Cli_AsABRead(self._pointer, start, size, byref(data))
         check_error(result, context="client")
         return result
 
     def as_ab_write(self, start: int, data: bytearray) -> int:
         """Writes a part of IPU area into a PLC asynchronously.
 
         Args:
@@ -693,21 +677,20 @@
             Snap7 code.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         size = len(data)
         cdata = (type_ * size).from_buffer_copy(data)
         logger.debug(f"ab write: start: {start}: size: {size}: ")
-        result = self._library.Cli_AsABWrite(
-            self._pointer, start, size, byref(cdata))
+        result = self._library.Cli_AsABWrite(self._pointer, start, size, byref(cdata))
         check_error(result, context="client")
         return result
 
     def as_compress(self, time: int) -> int:
-        """	Performs the Compress action asynchronously.
+        """Performs the Compress action asynchronously.
 
         Args:
             time: timeout.
 
         Returns:
             Snap7 code.
         """
@@ -923,20 +906,15 @@
         """
         type_ = c_int32
         buffer = (type_ * 9)()
         result = self._library.Cli_GetPlcDateTime(self._pointer, byref(buffer))
         check_error(result, context="client")
 
         return datetime(
-            year=buffer[5] + 1900,
-            month=buffer[4] + 1,
-            day=buffer[3],
-            hour=buffer[2],
-            minute=buffer[1],
-            second=buffer[0]
+            year=buffer[5] + 1900, month=buffer[4] + 1, day=buffer[3], hour=buffer[2], minute=buffer[1], second=buffer[0]
         )
 
     @error_wrap
     def set_plc_datetime(self, dt: datetime) -> int:
         """Sets the PLC date/time with a given value.
 
         Args:
@@ -965,18 +943,38 @@
         Returns:
             Snap7 code. If 0 - Job is done successfully. If 1 - Job is either pending or contains s7errors
         """
         result = self._library.Cli_CheckAsCompletion(self._pointer, p_value)
         check_error(result, context="client")
         return result
 
-    def set_as_callback(self, pfn_clicompletion, p_usr):
-        # Cli_SetAsCallback
-        result = self._library.Cli_SetAsCallback(self._pointer, pfn_clicompletion, p_usr)
-        check_error(result, context='client')
+    def set_as_callback(self, call_back: Callable[..., Any]) -> int:
+        logger.info("setting event callback")
+        callback_wrap: Callable[..., Any] = CFUNCTYPE(None, c_void_p, c_int, c_int)
+
+        def wrapper(usrptr: Optional[c_void_p], op_code: int, op_result: int) -> int:
+            """Wraps python function into a ctypes function
+
+            Args:
+                usrptr: not used
+                op_code:
+                op_result:
+
+            Returns:
+                Should return an int
+            """
+            logger.info(f"callback event: op_code: {op_code} op_result: {op_result}")
+            call_back(op_code, op_result)
+            return 0
+
+        self._callback = callback_wrap(wrapper)
+        usrPtr = c_void_p()
+
+        result = self._library.Cli_SetAsCallback(self._pointer, self._callback, usrPtr)
+        check_error(result, context="client")
         return result
 
     def wait_as_completion(self, timeout: int) -> int:
         """Snap7 Cli_WaitAsCompletion representative.
 
         Args:
             timeout: ms to wait for async job
@@ -1013,15 +1011,18 @@
             size: number of units to read
             pusrdata: buffer where the data will be place.
             wordlen: length of the word to be read.
 
         Returns:
             Snap7 code.
         """
-        logger.debug(f"reading area: {area.name} dbnumber: {dbnumber} start: {start}: amount {size}: wordlen: {wordlen.name}={wordlen.value}")
+        logger.debug(
+            f"reading area: {area.name} dbnumber: {dbnumber} start: {start} amount: {size} "
+            f"wordlen: {wordlen.name}={wordlen.value}"
+        )
         result = self._library.Cli_AsReadArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, pusrdata)
         check_error(result, context="client")
         return result
 
     def _prepare_as_write_area(self, area: Areas, data: bytearray) -> Tuple[WordLen, Array]:
         if area not in Areas:
             raise ValueError(f"{area} is not implemented in types")
@@ -1046,16 +1047,17 @@
             wordlen: length of the word to be written.
             pusrdata: buffer to be written.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
-        logger.debug(f"writing area: {area.name} dbnumber: {dbnumber} start: {start}: size {size}: "
-                     f"wordlen {wordlen} type: {type_}")
+        logger.debug(
+            f"writing area: {area.name} dbnumber: {dbnumber} start: {start}: size {size}: " f"wordlen {wordlen} type: {type_}"
+        )
         cdata = (type_ * len(pusrdata)).from_buffer_copy(pusrdata)
         res = self._library.Cli_AsWriteArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, byref(cdata))
         check_error(res, context="client")
         return res
 
     def as_eb_read(self, start: int, size: int, data) -> int:
         """Reads a part of IPI area from a PLC asynchronously.
@@ -1234,15 +1236,15 @@
             block_num: block number to upload.
             _buffer: buffer where the data will be place.
             size: amount of bytes to uplaod.
 
         Returns:
             Snap7 code.
         """
-        block_type = block_types['DB']
+        block_type = block_types["DB"]
         result = self._library.Cli_AsUpload(self._pointer, block_type, block_num, byref(_buffer), byref(size))
         check_error(result, context="client")
         return result
 
     def copy_ram_to_rom(self, timeout: int = 1) -> int:
         """Performs the Copy Ram to Rom action.
 
@@ -1346,15 +1348,15 @@
             Text error.
         """
         text_length = c_int(256)
         error_code = c_int32(error)
         text = create_string_buffer(buffer_size)
         response = self._library.Cli_ErrorText(error_code, byref(text), text_length)
         check_error(response)
-        result = bytearray(text)[:text_length.value].decode().strip('\x00')
+        result = bytearray(text)[: text_length.value].decode().strip("\x00")
         return result
 
     def get_cp_info(self) -> S7CpInfo:
         """Returns some information about the CP (communication processor).
 
         Returns:
             Structure object containing the CP information.
@@ -1433,15 +1435,15 @@
         Returns:
             Snap7 code.
         """
         size = c_int(len(data))
         cdata = (c_byte * len(data)).from_buffer_copy(data)
         response = self._library.Cli_IsoExchangeBuffer(self._pointer, byref(cdata), byref(size))
         check_error(response)
-        result = bytearray(cdata)[:size.value]
+        result = bytearray(cdata)[: size.value]
         return result
 
     def mb_read(self, start: int, size: int) -> bytearray:
         """Reads a part of Merkers area from a PLC.
 
         Args:
             start: byte index to be read from.
@@ -1495,15 +1497,15 @@
         Returns:
             Buffer read.
         """
         szl_list = S7SZLList()
         items_count = c_int(sizeof(szl_list))
         response = self._library.Cli_ReadSZLList(self._pointer, byref(szl_list), byref(items_count))
         check_error(response, context="client")
-        result = bytearray(szl_list.List)[:items_count.value]
+        result = bytearray(szl_list.List)[: items_count.value]
         return result
 
     def set_plc_system_datetime(self) -> int:
         """Sets the PLC date/time with the host (PC) date/time.
 
         Returns:
             Snap7 code.
```

### Comparing `python-snap7-1.3/snap7/common.py` & `python_snap7-1.4/snap7/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,75 @@
-import os
 import sys
 import logging
 import pathlib
 import platform
+from pathlib import Path
 from ctypes import c_char
 from typing import Optional
 from ctypes.util import find_library
 
-if platform.system() == 'Windows':
+if platform.system() == "Windows":
     from ctypes import windll as cdll  # type: ignore
 else:
     from ctypes import cdll
 
 logger = logging.getLogger(__name__)
 
 # regexp for checking if an ipv4 address is valid.
 ipv4 = r"^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\.){3}([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])$"
 
 
-class ADict(dict):
-    """
-    Accessing dict keys like an attribute.
-    """
-    __getattr__ = dict.__getitem__
-    __setattr__ = dict.__setitem__  # type: ignore
-
-
 class Snap7Library:
     """Snap7 loader and encapsulator. We make this a singleton to make
         sure the library is loaded only once.
 
     Attributes:
         lib_location: full path to the `snap7.dll` file. Optional.
     """
+
     _instance = None
     lib_location: Optional[str]
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = object.__new__(cls)
             cls._instance.lib_location = None
             cls._instance.cdll = None
         return cls._instance
 
     def __init__(self, lib_location: Optional[str] = None):
-        """ Loads the snap7 library using ctypes cdll.
+        """Loads the snap7 library using ctypes cdll.
 
         Args:
             lib_location: full path to the `snap7.dll` file. Optional.
 
         Raises:
             RuntimeError: if `lib_location` is not found.
         """
         if self.cdll:  # type: ignore
             return
-        self.lib_location = (lib_location
-                             or self.lib_location
-                             or find_in_package()
-                             or find_library('snap7')
-                             or find_locally('snap7'))
+        self.lib_location = (
+            lib_location or self.lib_location or find_in_package() or find_library("snap7") or find_locally("snap7")
+        )
         if not self.lib_location:
-            raise RuntimeError("can't find snap7 library. If installed, try running ldconfig")
+            error = f"""can't find snap7 shared library.
+
+This probably means you are installing python-snap7 from source. When no binary wheel is found for you architecture, pip
+install falls back on a source install. For this to work, you need to manually install the snap7 library, which python-snap7
+uses under the hood.
+
+The shortest path to success is to try to get a binary wheel working. Probably you are running on an unsupported
+platform or python version. You are running:
+
+machine: {platform.machine()}
+system: {platform.system()}
+python version: {platform.python_version()}
+"""
+            logger.error(error)
+            raise RuntimeError(error)
         self.cdll = cdll.LoadLibrary(self.lib_location)
 
 
 def load_library(lib_location: Optional[str] = None):
     """Loads the `snap7.dll` library.
     Returns:
         cdll: a ctypes cdll object with the snap7 shared library loaded.
@@ -137,16 +142,16 @@
     """Find the `snap7.dll` file according to the os used.
 
     Returns:
         Full path to the `snap7.dll` file.
     """
     basedir = pathlib.Path(__file__).parent.absolute()
     if sys.platform == "darwin":
-        lib = 'libsnap7.dylib'
+        lib = "libsnap7.dylib"
     elif sys.platform == "win32":
-        lib = 'snap7.dll'
+        lib = "snap7.dll"
     else:
-        lib = 'libsnap7.so'
-    full_path = basedir.joinpath('lib', lib)
-    if os.path.exists(full_path) and os.path.isfile(full_path):
+        lib = "libsnap7.so"
+    full_path = basedir.joinpath("lib", lib)
+    if Path.exists(full_path) and Path.is_file(full_path):
         return str(full_path)
     return None
```

### Comparing `python-snap7-1.3/snap7/error.py` & `python_snap7-1.4/snap7/error.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,100 +3,100 @@
 
 we define all error codes here, but we don't use them (yet/anymore).
 The error code formatting of the snap7 library as already quite good,
 so we are using that now. But maybe we will use this in the future again.
 """
 
 s7_client_errors = {
-    0x00100000: 'errNegotiatingPDU',
-    0x00200000: 'errCliInvalidParams',
-    0x00300000: 'errCliJobPending',
-    0x00400000: 'errCliTooManyItems',
-    0x00500000: 'errCliInvalidWordLen',
-    0x00600000: 'errCliPartialDataWritten',
-    0x00700000: 'errCliSizeOverPDU',
-    0x00800000: 'errCliInvalidPlcAnswer',
-    0x00900000: 'errCliAddressOutOfRange',
-    0x00A00000: 'errCliInvalidTransportSize',
-    0x00B00000: 'errCliWriteDataSizeMismatch',
-    0x00C00000: 'errCliItemNotAvailable',
-    0x00D00000: 'errCliInvalidValue',
-    0x00E00000: 'errCliCannotStartPLC',
-    0x00F00000: 'errCliAlreadyRun',
-    0x01000000: 'errCliCannotStopPLC',
-    0x01100000: 'errCliCannotCopyRamToRom',
-    0x01200000: 'errCliCannotCompress',
-    0x01300000: 'errCliAlreadyStop',
-    0x01400000: 'errCliFunNotAvailable',
-    0x01500000: 'errCliUploadSequenceFailed',
-    0x01600000: 'errCliInvalidDataSizeRecvd',
-    0x01700000: 'errCliInvalidBlockType',
-    0x01800000: 'errCliInvalidBlockNumber',
-    0x01900000: 'errCliInvalidBlockSize',
-    0x01A00000: 'errCliDownloadSequenceFailed',
-    0x01B00000: 'errCliInsertRefused',
-    0x01C00000: 'errCliDeleteRefused',
-    0x01D00000: 'errCliNeedPassword',
-    0x01E00000: 'errCliInvalidPassword',
-    0x01F00000: 'errCliNoPasswordToSetOrClear',
-    0x02000000: 'errCliJobTimeout',
-    0x02100000: 'errCliPartialDataRead',
-    0x02200000: 'errCliBufferTooSmall',
-    0x02300000: 'errCliFunctionRefused',
-    0x02400000: 'errCliDestroying',
-    0x02500000: 'errCliInvalidParamNumber',
-    0x02600000: 'errCliCannotChangeParam',
+    0x00100000: "errNegotiatingPDU",
+    0x00200000: "errCliInvalidParams",
+    0x00300000: "errCliJobPending",
+    0x00400000: "errCliTooManyItems",
+    0x00500000: "errCliInvalidWordLen",
+    0x00600000: "errCliPartialDataWritten",
+    0x00700000: "errCliSizeOverPDU",
+    0x00800000: "errCliInvalidPlcAnswer",
+    0x00900000: "errCliAddressOutOfRange",
+    0x00A00000: "errCliInvalidTransportSize",
+    0x00B00000: "errCliWriteDataSizeMismatch",
+    0x00C00000: "errCliItemNotAvailable",
+    0x00D00000: "errCliInvalidValue",
+    0x00E00000: "errCliCannotStartPLC",
+    0x00F00000: "errCliAlreadyRun",
+    0x01000000: "errCliCannotStopPLC",
+    0x01100000: "errCliCannotCopyRamToRom",
+    0x01200000: "errCliCannotCompress",
+    0x01300000: "errCliAlreadyStop",
+    0x01400000: "errCliFunNotAvailable",
+    0x01500000: "errCliUploadSequenceFailed",
+    0x01600000: "errCliInvalidDataSizeRecvd",
+    0x01700000: "errCliInvalidBlockType",
+    0x01800000: "errCliInvalidBlockNumber",
+    0x01900000: "errCliInvalidBlockSize",
+    0x01A00000: "errCliDownloadSequenceFailed",
+    0x01B00000: "errCliInsertRefused",
+    0x01C00000: "errCliDeleteRefused",
+    0x01D00000: "errCliNeedPassword",
+    0x01E00000: "errCliInvalidPassword",
+    0x01F00000: "errCliNoPasswordToSetOrClear",
+    0x02000000: "errCliJobTimeout",
+    0x02100000: "errCliPartialDataRead",
+    0x02200000: "errCliBufferTooSmall",
+    0x02300000: "errCliFunctionRefused",
+    0x02400000: "errCliDestroying",
+    0x02500000: "errCliInvalidParamNumber",
+    0x02600000: "errCliCannotChangeParam",
 }
 
 isotcp_errors = {
-    0x00010000: 'errIsoConnect',
-    0x00020000: 'errIsoDisconnect',
-    0x00030000: 'errIsoInvalidPDU',
-    0x00040000: 'errIsoInvalidDataSize',
-    0x00050000: 'errIsoNullPointer',
-    0x00060000: 'errIsoShortPacket',
-    0x00070000: 'errIsoTooManyFragments',
-    0x00080000: 'errIsoPduOverflow',
-    0x00090000: 'errIsoSendPacket',
-    0x000A0000: 'errIsoRecvPacket',
-    0x000B0000: 'errIsoInvalidParams',
-    0x000C0000: 'errIsoResvd_1',
-    0x000D0000: 'errIsoResvd_2',
-    0x000E0000: 'errIsoResvd_3',
-    0x000F0000: 'errIsoResvd_4',
+    0x00010000: "errIsoConnect",
+    0x00020000: "errIsoDisconnect",
+    0x00030000: "errIsoInvalidPDU",
+    0x00040000: "errIsoInvalidDataSize",
+    0x00050000: "errIsoNullPointer",
+    0x00060000: "errIsoShortPacket",
+    0x00070000: "errIsoTooManyFragments",
+    0x00080000: "errIsoPduOverflow",
+    0x00090000: "errIsoSendPacket",
+    0x000A0000: "errIsoRecvPacket",
+    0x000B0000: "errIsoInvalidParams",
+    0x000C0000: "errIsoResvd_1",
+    0x000D0000: "errIsoResvd_2",
+    0x000E0000: "errIsoResvd_3",
+    0x000F0000: "errIsoResvd_4",
 }
 
 tcp_errors = {
-    0x00000001: 'evcServerStarted',
-    0x00000002: 'evcServerStopped',
-    0x00000004: 'evcListenerCannotStart',
-    0x00000008: 'evcClientAdded',
-    0x00000010: 'evcClientRejected',
-    0x00000020: 'evcClientNoRoom',
-    0x00000040: 'evcClientException',
-    0x00000080: 'evcClientDisconnected',
-    0x00000100: 'evcClientTerminated',
-    0x00000200: 'evcClientsDropped',
-    0x00000400: 'evcReserved_00000400',
-    0x00000800: 'evcReserved_00000800',
-    0x00001000: 'evcReserved_00001000',
-    0x00002000: 'evcReserved_00002000',
-    0x00004000: 'evcReserved_00004000',
-    0x00008000: 'evcReserved_00008000',
+    0x00000001: "evcServerStarted",
+    0x00000002: "evcServerStopped",
+    0x00000004: "evcListenerCannotStart",
+    0x00000008: "evcClientAdded",
+    0x00000010: "evcClientRejected",
+    0x00000020: "evcClientNoRoom",
+    0x00000040: "evcClientException",
+    0x00000080: "evcClientDisconnected",
+    0x00000100: "evcClientTerminated",
+    0x00000200: "evcClientsDropped",
+    0x00000400: "evcReserved_00000400",
+    0x00000800: "evcReserved_00000800",
+    0x00001000: "evcReserved_00001000",
+    0x00002000: "evcReserved_00002000",
+    0x00004000: "evcReserved_00004000",
+    0x00008000: "evcReserved_00008000",
 }
 
 s7_server_errors = {
-    0x00100000: 'errSrvCannotStart',
-    0x00200000: 'errSrvDBNullPointer',
-    0x00300000: 'errSrvAreaAlreadyExists',
-    0x00400000: 'errSrvUnknownArea',
-    0x00500000: 'verrSrvInvalidParams',
-    0x00600000: 'errSrvTooManyDB',
-    0x00700000: 'errSrvInvalidParamNumber',
-    0x00800000: 'errSrvCannotChangeParam',
+    0x00100000: "errSrvCannotStart",
+    0x00200000: "errSrvDBNullPointer",
+    0x00300000: "errSrvAreaAlreadyExists",
+    0x00400000: "errSrvUnknownArea",
+    0x00500000: "verrSrvInvalidParams",
+    0x00600000: "errSrvTooManyDB",
+    0x00700000: "errSrvInvalidParamNumber",
+    0x00800000: "errSrvCannotChangeParam",
 }
 
 client_errors = s7_client_errors.copy()
 client_errors.update(isotcp_errors)
 client_errors.update(tcp_errors)
 
 server_errors = s7_server_errors.copy()
```

### Comparing `python-snap7-1.3/snap7/logo.py` & `python_snap7-1.4/snap7/logo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Snap7 client used for connection to a siemens LOGO 7/8 server.
 """
+
 import re
 import struct
 import logging
 from ctypes import byref, c_int, c_int32, c_uint16, c_void_p
 
 from .types import WordLen, S7Object, param_types
 from .types import RemotePort, Areas, wordlen_to_ctypes
@@ -130,16 +131,15 @@
             return 0
 
         type_ = wordlen_to_ctypes[wordlen.value]
         data = (type_ * size)()
 
         logger.debug(f"start:{start}, wordlen:{wordlen.name}={wordlen.value}, data-length:{len(data)}")
 
-        result = self.library.Cli_ReadArea(self.pointer, area.value, db_number, start,
-                                           size, wordlen.value, byref(data))
+        result = self.library.Cli_ReadArea(self.pointer, area.value, db_number, start, size, wordlen.value, byref(data))
         check_error(result, context="client")
         # transform result to int value
         if wordlen == WordLen.Bit:
             return data[0]
         if wordlen == WordLen.Byte:
             return struct.unpack_from(">B", data)[0]
         if wordlen == WordLen.Word:
@@ -223,17 +223,15 @@
         Returns:
             Array of bytes
         """
         logger.debug(f"db_read, db_number:{db_number}, start:{start}, size:{size}")
 
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         data = (type_ * size)()
-        result = (self.library.Cli_DBRead(
-            self.pointer, db_number, start, size,
-            byref(data)))
+        result = self.library.Cli_DBRead(self.pointer, db_number, start, size, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     def db_write(self, db_number: int, start: int, data: bytearray) -> int:
         """Writes to a DB object.
 
         Args:
@@ -266,32 +264,31 @@
 
         Raises:
             :obj:`ValueError`: if the `ip_address` is not an IPV4.
             :obj:`ValueError`: if the snap7 error code is diferent from 0.
         """
         if not re.match(ipv4, ip_address):
             raise ValueError(f"{ip_address} is invalid ipv4")
-        result = self.library.Cli_SetConnectionParams(self.pointer, ip_address.encode(),
-                                                      c_uint16(tsap_snap7),
-                                                      c_uint16(tsap_logo))
+        result = self.library.Cli_SetConnectionParams(
+            self.pointer, ip_address.encode(), c_uint16(tsap_snap7), c_uint16(tsap_logo)
+        )
         if result != 0:
             raise ValueError("The parameter was invalid")
 
     def set_connection_type(self, connection_type: int):
         """Sets the connection resource type, i.e the way in which the Clients
             connects to a PLC.
 
         Args:
             connection_type: 1 for PG, 2 for OP, 3 to 10 for S7 Basic
 
         Raises:
             :obj:`ValueError`: if the snap7 error code is diferent from 0.
         """
-        result = self.library.Cli_SetConnectionType(self.pointer,
-                                                    c_uint16(connection_type))
+        result = self.library.Cli_SetConnectionType(self.pointer, c_uint16(connection_type))
         if result != 0:
             raise ValueError("The parameter was invalid")
 
     def get_connected(self) -> bool:
         """Returns the connection status
 
         Notes:
@@ -330,11 +327,10 @@
 
         Returns:
             Parameter value
         """
         logger.debug(f"retreiving param number {number}")
         type_ = param_types[number]
         value = type_()
-        code = self.library.Cli_GetParam(self.pointer, c_int(number),
-                                         byref(value))
+        code = self.library.Cli_GetParam(self.pointer, c_int(number), byref(value))
         check_error(code)
         return value.value
```

### Comparing `python-snap7-1.3/snap7/partner.py` & `python_snap7-1.4/snap7/partner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This allows you to create a S7 peer to peer communication. Unlike the
 client-server model, where the client makes a request and the server replies to
 it, the peer to peer model sees two components with same rights, each of them
 can send data asynchronously. The only difference between them is the one who
 is requesting the connection.
 """
+
 import re
 import logging
 from ctypes import byref, c_int, c_int32, c_uint32, c_void_p
 from typing import Tuple, Optional
 
 from .common import ipv4, check_error, load_library
 from .types import S7Object, param_types, word
@@ -28,14 +29,15 @@
     return f
 
 
 class Partner:
     """
     A snap7 partner.
     """
+
     _pointer: Optional[c_void_p]
 
     def __init__(self, active: bool = False):
         self._library = load_library()
         self._pointer = None
         self.create(active)
 
@@ -122,33 +124,29 @@
     def get_param(self, number) -> int:
         """
         Reads an internal Partner object parameter.
         """
         logger.debug(f"retreiving param number {number}")
         type_ = param_types[number]
         value = type_()
-        code = self._library.Par_GetParam(self._pointer, c_int(number),
-                                          byref(value))
+        code = self._library.Par_GetParam(self._pointer, c_int(number), byref(value))
         check_error(code)
         return value.value
 
     def get_stats(self) -> Tuple[c_uint32, c_uint32, c_uint32, c_uint32]:
         """
         Returns some statistics.
 
         :returns: a tuple containing bytes send, received, send errors, recv errors
         """
         sent = c_uint32()
         recv = c_uint32()
         send_errors = c_uint32()
         recv_errors = c_uint32()
-        result = self._library.Par_GetStats(self._pointer, byref(sent),
-                                            byref(recv),
-                                            byref(send_errors),
-                                            byref(recv_errors))
+        result = self._library.Par_GetStats(self._pointer, byref(sent), byref(recv), byref(send_errors), byref(recv_errors))
         check_error(result, "partner")
         return sent, recv, send_errors, recv_errors
 
     def get_status(self) -> c_int32:
         """
         Returns the Partner status.
         """
@@ -165,19 +163,17 @@
         recv_time = c_int32()
         result = self._library.Par_GetTimes(self._pointer, byref(send_time), byref(recv_time))
         check_error(result, "partner")
         return send_time, recv_time
 
     @error_wrap
     def set_param(self, number: int, value) -> int:
-        """Sets an internal Partner object parameter.
-        """
+        """Sets an internal Partner object parameter."""
         logger.debug(f"setting param number {number} to {value}")
-        return self._library.Par_SetParam(self._pointer, number,
-                                          byref(c_int(value)))
+        return self._library.Par_SetParam(self._pointer, number, byref(c_int(value)))
 
     def set_recv_callback(self) -> int:
         """
         Sets the user callback that the Partner object has to call when a data
         packet is incoming.
         """
         return self._library.Par_SetRecvCallback(self._pointer)
@@ -210,17 +206,17 @@
         """
 
         if not re.match(ipv4, local_ip):
             raise ValueError(f"{local_ip} is invalid ipv4")
         if not re.match(ipv4, remote_ip):
             raise ValueError(f"{remote_ip} is invalid ipv4")
         logger.info(f"starting partnering from {local_ip} to {remote_ip}")
-        return self._library.Par_StartTo(self._pointer, local_ip.encode(), remote_ip.encode(),
-                                         word(local_tsap),
-                                         word(remote_tsap))
+        return self._library.Par_StartTo(
+            self._pointer, local_ip.encode(), remote_ip.encode(), word(local_tsap), word(remote_tsap)
+        )
 
     def stop(self) -> int:
         """
         Stops the Partner, disconnects gracefully the remote partner.
         """
         return self._library.Par_Stop(self._pointer)
```

### Comparing `python-snap7-1.3/snap7/server/__init__.py` & `python_snap7-1.4/snap7/server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Snap7 server used for mimicking a siemens 7 server.
 """
+
 import re
 import time
 import ctypes
 import struct
 import logging
 from typing import Any, Tuple, Callable, Optional
 
@@ -14,14 +15,15 @@
 from ..types import srvAreaDB, srvAreaPA, srvAreaTM, srvAreaCT
 
 logger = logging.getLogger(__name__)
 
 
 def error_wrap(func):
     """Parses a s7 error code returned the decorated function."""
+
     def f(*args, **kw):
         code = func(*args, **kw)
         check_error(code, context="server")
 
     return f
 
 
@@ -57,28 +59,26 @@
         Returns:
             The error string
         """
         logger.debug(f"error text for {hex(event.EvtCode)}")
         len_ = 1024
         text_type = ctypes.c_char * len_
         text = text_type()
-        error = self.library.Srv_EventText(ctypes.byref(event),
-                                           ctypes.byref(text), len_)
+        error = self.library.Srv_EventText(ctypes.byref(event), ctypes.byref(text), len_)
         check_error(error)
-        return text.value.decode('ascii')
+        return text.value.decode("ascii")
 
     def create(self):
-        """Create the server.
-        """
+        """Create the server."""
         logger.info("creating server")
         self.library.Srv_Create.restype = S7Object
         self.pointer = S7Object(self.library.Srv_Create())
 
     @error_wrap
-    def register_area(self, area_code: int, index: int, userdata):
+    def register_area(self, area_code: int, index: int, userdata: ctypes.Array[ctypes.c_int8]):
         """Shares a memory area with the server. That memory block will be
             visible by the clients.
 
         Args:
             area_code: memory area to register.
             index: number of area to write.
             userdata: buffer with the data to write.
@@ -89,15 +89,15 @@
         size = ctypes.sizeof(userdata)
         logger.info(f"registering area {area_code}, index {index}, size {size}")
         return self.library.Srv_RegisterArea(self.pointer, area_code, index, ctypes.byref(userdata), size)
 
     @error_wrap
     def set_events_callback(self, call_back: Callable[..., Any]) -> int:
         """Sets the user callback that the Server object has to call when an
-            event is created.
+        event is created.
         """
         logger.info("setting event callback")
         callback_wrap: Callable[..., Any] = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.POINTER(SrvEvent), ctypes.c_int)
 
         def wrapper(usrptr: Optional[ctypes.c_void_p], pevent: SrvEvent, size: int) -> int:
             """Wraps python function into a ctypes function
 
@@ -122,17 +122,15 @@
         """Sets the user callback that the Server object has to call when a Read
             event is created.
 
         Args:
             call_back: a callback function that accepts a pevent argument.
         """
         logger.info("setting read event callback")
-        callback_wrapper: Callable[..., Any] = ctypes.CFUNCTYPE(None, ctypes.c_void_p,
-                                                                ctypes.POINTER(SrvEvent),
-                                                                ctypes.c_int)
+        callback_wrapper: Callable[..., Any] = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.POINTER(SrvEvent), ctypes.c_int)
 
         def wrapper(usrptr: Optional[ctypes.c_void_p], pevent: SrvEvent, size: int) -> int:
             """Wraps python function into a ctypes function
 
             Args:
                 usrptr: not used
                 pevent: pointer to snap7 event struct
@@ -142,16 +140,15 @@
                 Should return an int
             """
             logger.info(f"callback event: {self.event_text(pevent.contents)}")
             call_back(pevent.contents)
             return 0
 
         self._read_callback = callback_wrapper(wrapper)
-        return self.library.Srv_SetReadEventsCallback(self.pointer,
-                                                      self._read_callback)
+        return self.library.Srv_SetReadEventsCallback(self.pointer, self._read_callback)
 
     def _set_log_callback(self):
         """Sets a callback that logs the events"""
         logger.debug("setting up event logger")
 
         def log_callback(event):
             logger.info(f"callback event: {self.event_text(event)}")
@@ -176,38 +173,34 @@
         """Stop the server."""
         logger.info("stopping server")
         return self.library.Srv_Stop(self.pointer)
 
     def destroy(self):
         """Destroy the server."""
         logger.info("destroying server")
-        if self.library:
+        if hasattr(self, "library") and self.library:
             self.library.Srv_Destroy(ctypes.byref(self.pointer))
 
     def get_status(self) -> Tuple[str, str, int]:
         """Reads the server status, the Virtual CPU status and the number of
             the clients connected.
 
         Returns:
             Server status, cpu status, client count
         """
         logger.debug("get server status")
         server_status = ctypes.c_int()
         cpu_status = ctypes.c_int()
         clients_count = ctypes.c_int()
-        error = self.library.Srv_GetStatus(self.pointer, ctypes.byref(server_status),
-                                           ctypes.byref(cpu_status),
-                                           ctypes.byref(clients_count))
+        error = self.library.Srv_GetStatus(
+            self.pointer, ctypes.byref(server_status), ctypes.byref(cpu_status), ctypes.byref(clients_count)
+        )
         check_error(error)
         logger.debug(f"status server {server_status.value} cpu {cpu_status.value} clients {clients_count.value}")
-        return (
-            server_statuses[server_status.value],
-            cpu_statuses[cpu_status.value],
-            clients_count.value
-        )
+        return (server_statuses[server_status.value], cpu_statuses[cpu_status.value], clients_count.value)
 
     @error_wrap
     def unregister_area(self, area_code: int, index: int):
         """'Unshares' a memory area previously shared with Srv_RegisterArea().
 
         Notes:
             That memory block will be no longer visible by the clients.
@@ -276,16 +269,15 @@
             number: number of the parameter.
             value: value to be set.
 
         Returns:
             Error code from snap7 library.
         """
         logger.debug(f"setting param number {number} to {value}")
-        return self.library.Srv_SetParam(self.pointer, number,
-                                         ctypes.byref(ctypes.c_int(value)))
+        return self.library.Srv_SetParam(self.pointer, number, ctypes.byref(ctypes.c_int(value)))
 
     @error_wrap
     def set_mask(self, kind: int, mask: int):
         """Writes the specified filter mask.
 
         Args:
             kind:
@@ -320,16 +312,15 @@
 
         Returns:
             Server event.
         """
         logger.debug("checking event queue")
         event = SrvEvent()
         ready = ctypes.c_int32()
-        code = self.library.Srv_PickEvent(self.pointer, ctypes.byref(event),
-                                          ctypes.byref(ready))
+        code = self.library.Srv_PickEvent(self.pointer, ctypes.byref(event), ctypes.byref(ready))
         check_error(code)
         if ready:
             logger.debug(f"one event ready: {event}")
             return event
         logger.debug("no events ready")
         return None
 
@@ -340,16 +331,15 @@
             number: number of the parameter to be set.
 
         Returns:
             Value of the parameter.
         """
         logger.debug(f"retreiving param number {number}")
         value = ctypes.c_int()
-        code = self.library.Srv_GetParam(self.pointer, number,
-                                         ctypes.byref(value))
+        code = self.library.Srv_GetParam(self.pointer, number, ctypes.byref(value))
         check_error(code)
         return value.value
 
     def get_mask(self, kind: int) -> ctypes.c_uint32:
         """Reads the specified filter mask.
 
         Args:
@@ -392,31 +382,30 @@
     server.register_area(srvAreaDB, 1, DBdata)
     server.register_area(srvAreaPA, 1, PAdata)
     server.register_area(srvAreaTM, 1, TMdata)
     server.register_area(srvAreaCT, 1, CTdata)
 
     if init_standard_values:
         ba = _init_standard_values()
-        DBdata = wordlen_to_ctypes[WordLen.Byte.value] * len(ba)
-        DBdata = DBdata.from_buffer(ba)
-        server.register_area(srvAreaDB, 0, DBdata)
+        userdata = wordlen_to_ctypes[WordLen.Byte.value] * len(ba)
+        server.register_area(srvAreaDB, 0, userdata.from_buffer(ba))
 
     server.start(tcpport=tcpport)
     while True:
         while True:
             event = server.pick_event()
             if event:
                 logger.info(server.event_text(event))
             else:
                 break
         time.sleep(1)
 
 
 def _init_standard_values() -> bytearray:
-    ''' Standard values
+    """Standard values
     * Boolean
     BYTE    BIT     VALUE
     0       0       True
     0       1       False
     0       2       True
     0       3       False
     0       4       True
@@ -468,77 +457,77 @@
     BYTE    VALUE
     100     254|37|the brown fox jumps over the lazy dog
 
     * Word
     BYTE    VALUE
     400     \x00\x00
     404     \x12\x34
-    408     \xAB\xCD
-    412     \xFF\xFF
+    408     \xab\xcd
+    412     \xff\xff
 
     * Double Word
     BYTE    VALUE
     500     \x00\x00\x00\x00
     508     \x12\x34\x56\x78
-    516     \x12\x34\xAB\xCD
-    524     \xFF\xFF\xFF\xFF
-    '''
+    516     \x12\x34\xab\xcd
+    524     \xff\xff\xff\xff
+    """
 
     ba = bytearray(1000)
     # 1. Bool 1 byte
     ba[0] = 0b10101010
 
     # 2. Small int 1 byte
-    ba[10:10 + 1] = struct.pack(">b", -128)
-    ba[11:11 + 1] = struct.pack(">b", 0)
-    ba[12:12 + 1] = struct.pack(">b", 100)
-    ba[13:13 + 1] = struct.pack(">b", 127)
+    ba[10 : 10 + 1] = struct.pack(">b", -128)
+    ba[11 : 11 + 1] = struct.pack(">b", 0)
+    ba[12 : 12 + 1] = struct.pack(">b", 100)
+    ba[13 : 13 + 1] = struct.pack(">b", 127)
 
     # 3. Unsigned small int 1 byte
-    ba[20:20 + 1] = struct.pack("B", 0)
-    ba[21:21 + 1] = struct.pack("B", 255)
+    ba[20 : 20 + 1] = struct.pack("B", 0)
+    ba[21 : 21 + 1] = struct.pack("B", 255)
 
     # 4. Int 2 bytes
-    ba[30:30 + 2] = struct.pack(">h", -32768)
-    ba[32:32 + 2] = struct.pack(">h", -1234)
-    ba[34:34 + 2] = struct.pack(">h", 0)
-    ba[36:36 + 2] = struct.pack(">h", 1234)
-    ba[38:38 + 2] = struct.pack(">h", 32767)
+    ba[30 : 30 + 2] = struct.pack(">h", -32768)
+    ba[32 : 32 + 2] = struct.pack(">h", -1234)
+    ba[34 : 34 + 2] = struct.pack(">h", 0)
+    ba[36 : 36 + 2] = struct.pack(">h", 1234)
+    ba[38 : 38 + 2] = struct.pack(">h", 32767)
 
     # 5. DInt 4 bytes
-    ba[40:40 + 4] = struct.pack(">i", -2147483648)
-    ba[44:44 + 4] = struct.pack(">i", -32768)
-    ba[48:48 + 4] = struct.pack(">i", 0)
-    ba[52:52 + 4] = struct.pack(">i", 32767)
-    ba[56:56 + 4] = struct.pack(">i", 2147483647)
+    ba[40 : 40 + 4] = struct.pack(">i", -2147483648)
+    ba[44 : 44 + 4] = struct.pack(">i", -32768)
+    ba[48 : 48 + 4] = struct.pack(">i", 0)
+    ba[52 : 52 + 4] = struct.pack(">i", 32767)
+    ba[56 : 56 + 4] = struct.pack(">i", 2147483647)
 
     # 6. Real 4 bytes
-    ba[60:60 + 4] = struct.pack(">f", -3.402823e38)
-    ba[64:64 + 4] = struct.pack(">f", -3.402823e12)
-    ba[68:68 + 4] = struct.pack(">f", -175494351e-38)
-    ba[72:72 + 4] = struct.pack(">f", -1.175494351e-12)
-    ba[76:76 + 4] = struct.pack(">f", 0.0)
-    ba[80:80 + 4] = struct.pack(">f", 1.175494351e-38)
-    ba[84:84 + 4] = struct.pack(">f", 1.175494351e-12)
-    ba[88:88 + 4] = struct.pack(">f", 3.402823466e12)
-    ba[92:92 + 4] = struct.pack(">f", 3.402823466e38)
+    ba[60 : 60 + 4] = struct.pack(">f", -3.402823e38)
+    ba[64 : 64 + 4] = struct.pack(">f", -3.402823e12)
+    ba[68 : 68 + 4] = struct.pack(">f", -175494351e-38)
+    ba[72 : 72 + 4] = struct.pack(">f", -1.175494351e-12)
+    ba[76 : 76 + 4] = struct.pack(">f", 0.0)
+    ba[80 : 80 + 4] = struct.pack(">f", 1.175494351e-38)
+    ba[84 : 84 + 4] = struct.pack(">f", 1.175494351e-12)
+    ba[88 : 88 + 4] = struct.pack(">f", 3.402823466e12)
+    ba[92 : 92 + 4] = struct.pack(">f", 3.402823466e38)
 
     # 7. String 1 byte per char
     string = "the brown fox jumps over the lazy dog"  # len = 37
     ba[100] = 254
     ba[101] = len(string)
     for letter, i in zip(string, range(102, 102 + len(string) + 1)):
         ba[i] = ord(letter)
 
     # 8. WORD 4 bytes
-    ba[400:400 + 4] = b"\x00\x00"
-    ba[404:404 + 4] = b"\x12\x34"
-    ba[408:408 + 4] = b"\xAB\xCD"
-    ba[412:412 + 4] = b"\xFF\xFF"
+    ba[400 : 400 + 4] = b"\x00\x00"
+    ba[404 : 404 + 4] = b"\x12\x34"
+    ba[408 : 408 + 4] = b"\xab\xcd"
+    ba[412 : 412 + 4] = b"\xff\xff"
 
     # # 9 DWORD 8 bytes
-    ba[500:500 + 8] = b"\x00\x00\x00\x00"
-    ba[508:508 + 8] = b"\x12\x34\x56\x78"
-    ba[516:516 + 8] = b"\x12\x34\xAB\xCD"
-    ba[524:524 + 8] = b"\xFF\xFF\xFF\xFF"
+    ba[500 : 500 + 8] = b"\x00\x00\x00\x00"
+    ba[508 : 508 + 8] = b"\x12\x34\x56\x78"
+    ba[516 : 516 + 8] = b"\x12\x34\xab\xcd"
+    ba[524 : 524 + 8] = b"\xff\xff\xff\xff"
 
     return ba
```

### Comparing `python-snap7-1.3/snap7/server/__main__.py` & `python_snap7-1.4/snap7/server/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 Its :code:`main()` function is also exported as an consol-entrypoint.
 """
 
 import logging
 
 try:
     import click
-except ImportError as e:
-    print(e)
+except ImportError:
     print("Try using 'pip install python-snap7[cli]'")
-    exit()
+    raise
 
 from snap7 import __version__
 from snap7.common import load_library
 from snap7.server import mainloop
 
 logger = logging.getLogger("Snap7.Server")
```

### Comparing `python-snap7-1.3/snap7/types.py` & `python_snap7-1.4/snap7/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Python equivalent for snap7 specific types.
 """
+
 import ctypes
 from enum import Enum
 
-from .common import ADict
-
 S7Object = ctypes.c_void_p
 buffer_size = 65536
 buffer_type = ctypes.c_ubyte * buffer_size
 time_t = ctypes.c_uint64  # TODO: check if this is valid for all platforms
 word = ctypes.c_uint16
 longword = ctypes.c_uint32
 
@@ -26,15 +25,15 @@
 PDURequest = 10
 MaxClients = 11
 BSendTimeout = 12
 BRecvTimeout = 13
 RecoveryTime = 14
 KeepAliveTime = 15
 
-param_types = ADict({
+param_types = {
     LocalPort: ctypes.c_uint16,
     RemotePort: ctypes.c_uint16,
     PingTimeout: ctypes.c_int32,
     SendTimeout: ctypes.c_int32,
     RecvTimeout: ctypes.c_int32,
     WorkInterval: ctypes.c_int32,
     SrcRef: ctypes.c_uint16,
@@ -42,15 +41,15 @@
     SrcTSap: ctypes.c_uint16,
     PDURequest: ctypes.c_int32,
     MaxClients: ctypes.c_int32,
     BSendTimeout: ctypes.c_int32,
     BRecvTimeout: ctypes.c_int32,
     RecoveryTime: ctypes.c_uint32,
     KeepAliveTime: ctypes.c_uint32,
-})
+}
 
 # mask types
 mkEvent = 0
 mkLog = 1
 
 
 # Area ID
@@ -67,23 +66,22 @@
 S7AreaPE = 0x81
 S7AreaPA = 0x82
 S7AreaMK = 0x83
 S7AreaDB = 0x84
 S7AreaCT = 0x1C
 S7AreaTM = 0x1D
 
-
-areas = ADict({
-    'PE': 0x81,
-    'PA': 0x82,
-    'MK': 0x83,
-    'DB': 0x84,
-    'CT': 0x1C,
-    'TM': 0x1D,
-})
+areas = {
+    "PE": S7AreaPE,
+    "PA": S7AreaPA,
+    "MK": S7AreaMK,
+    "DB": S7AreaDB,
+    "CT": S7AreaCT,
+    "TM": S7AreaTM,
+}
 
 
 # Word Length
 class WordLen(Enum):
     Bit = 0x01
     Byte = 0x02
     Char = 0x03
@@ -113,107 +111,111 @@
 srvAreaPE = 0
 srvAreaPA = 1
 srvAreaMK = 2
 srvAreaCT = 3
 srvAreaTM = 4
 srvAreaDB = 5
 
-server_areas = ADict({
-    'PE': 0,
-    'PA': 1,
-    'MK': 2,
-    'CT': 3,
-    'TM': 4,
-    'DB': 5,
-})
+server_areas = {
+    "PE": srvAreaPE,
+    "PA": srvAreaPA,
+    "MK": srvAreaMK,
+    "CT": srvAreaCT,
+    "TM": srvAreaTM,
+    "DB": srvAreaDB,
+}
 
-wordlen_to_ctypes = ADict({
+wordlen_to_ctypes = {
     S7WLBit: ctypes.c_int16,
     S7WLByte: ctypes.c_int8,
     S7WLWord: ctypes.c_int16,
     S7WLDWord: ctypes.c_int32,
     S7WLReal: ctypes.c_int32,
     S7WLCounter: ctypes.c_int16,
     S7WLTimer: ctypes.c_int16,
-})
+}
 
-block_types = ADict({
-    'OB': ctypes.c_int(0x38),
-    'DB': ctypes.c_int(0x41),
-    'SDB': ctypes.c_int(0x42),
-    'FC': ctypes.c_int(0x43),
-    'SFC': ctypes.c_int(0x44),
-    'FB': ctypes.c_int(0x45),
-    'SFB': ctypes.c_int(0x46),
-})
+block_types = {
+    "OB": ctypes.c_int(0x38),
+    "DB": ctypes.c_int(0x41),
+    "SDB": ctypes.c_int(0x42),
+    "FC": ctypes.c_int(0x43),
+    "SFC": ctypes.c_int(0x44),
+    "FB": ctypes.c_int(0x45),
+    "SFB": ctypes.c_int(0x46),
+}
 
 server_statuses = {
-    0: 'SrvStopped',
-    1: 'SrvRunning',
-    2: 'SrvError',
+    0: "SrvStopped",
+    1: "SrvRunning",
+    2: "SrvError",
 }
 
 cpu_statuses = {
-    0: 'S7CpuStatusUnknown',
-    4: 'S7CpuStatusStop',
-    8: 'S7CpuStatusRun',
+    0: "S7CpuStatusUnknown",
+    4: "S7CpuStatusStop",
+    8: "S7CpuStatusRun",
 }
 
 
 class SrvEvent(ctypes.Structure):
     _fields_ = [
-        ('EvtTime', time_t),
-        ('EvtSender', ctypes.c_int),
-        ('EvtCode', longword),
-        ('EvtRetCode', word),
-        ('EvtParam1', word),
-        ('EvtParam2', word),
-        ('EvtParam3', word),
-        ('EvtParam4', word),
+        ("EvtTime", time_t),
+        ("EvtSender", ctypes.c_int),
+        ("EvtCode", longword),
+        ("EvtRetCode", word),
+        ("EvtParam1", word),
+        ("EvtParam2", word),
+        ("EvtParam3", word),
+        ("EvtParam4", word),
     ]
 
     def __str__(self) -> str:
-        return f"<event time: {self.EvtTime} sender: {self.EvtSender} code: {self.EvtCode} " \
-               f"retcode: {self.EvtRetCode} param1: {self.EvtParam1} param2:{self.EvtParam2} " \
-               f"param3: {self.EvtParam3} param4: {self.EvtParam4}>"
+        return (
+            f"<event time: {self.EvtTime} sender: {self.EvtSender} code: {self.EvtCode} "
+            f"retcode: {self.EvtRetCode} param1: {self.EvtParam1} param2:{self.EvtParam2} "
+            f"param3: {self.EvtParam3} param4: {self.EvtParam4}>"
+        )
 
 
 class BlocksList(ctypes.Structure):
     _fields_ = [
-        ('OBCount', ctypes.c_int32),
-        ('FBCount', ctypes.c_int32),
-        ('FCCount', ctypes.c_int32),
-        ('SFBCount', ctypes.c_int32),
-        ('SFCCount', ctypes.c_int32),
-        ('DBCount', ctypes.c_int32),
-        ('SDBCount', ctypes.c_int32),
+        ("OBCount", ctypes.c_int32),
+        ("FBCount", ctypes.c_int32),
+        ("FCCount", ctypes.c_int32),
+        ("SFBCount", ctypes.c_int32),
+        ("SFCCount", ctypes.c_int32),
+        ("DBCount", ctypes.c_int32),
+        ("SDBCount", ctypes.c_int32),
     ]
 
     def __str__(self) -> str:
-        return f"<block list count OB: {self.OBCount} FB: {self.FBCount} FC: {self.FCCount} SFB: {self.SFBCount} " \
-               f"SFC: {hex(self.SFCCount)} DB: {self.DBCount} SDB: {self.SDBCount}>"
+        return (
+            f"<block list count OB: {self.OBCount} FB: {self.FBCount} FC: {self.FCCount} SFB: {self.SFBCount} "
+            f"SFC: {hex(self.SFCCount)} DB: {self.DBCount} SDB: {self.SDBCount}>"
+        )
 
 
 class TS7BlockInfo(ctypes.Structure):
     _fields_ = [
-        ('BlkType', ctypes.c_int32),
-        ('BlkNumber', ctypes.c_int32),
-        ('BlkLang', ctypes.c_int32),
-        ('BlkFlags', ctypes.c_int32),
-        ('MC7Size', ctypes.c_int32),
-        ('LoadSize', ctypes.c_int32),
-        ('LocalData', ctypes.c_int32),
-        ('SBBLength', ctypes.c_int32),
-        ('CheckSum', ctypes.c_int32),
-        ('Version', ctypes.c_int32),
-        ('CodeDate', ctypes.c_char * 11),
-        ('IntfDate', ctypes.c_char * 11),
-        ('Author', ctypes.c_char * 9),
-        ('Family', ctypes.c_char * 9),
-        ('Header', ctypes.c_char * 9),
+        ("BlkType", ctypes.c_int32),
+        ("BlkNumber", ctypes.c_int32),
+        ("BlkLang", ctypes.c_int32),
+        ("BlkFlags", ctypes.c_int32),
+        ("MC7Size", ctypes.c_int32),
+        ("LoadSize", ctypes.c_int32),
+        ("LocalData", ctypes.c_int32),
+        ("SBBLength", ctypes.c_int32),
+        ("CheckSum", ctypes.c_int32),
+        ("Version", ctypes.c_int32),
+        ("CodeDate", ctypes.c_char * 11),
+        ("IntfDate", ctypes.c_char * 11),
+        ("Author", ctypes.c_char * 9),
+        ("Family", ctypes.c_char * 9),
+        ("Header", ctypes.c_char * 9),
     ]
 
     def __str__(self) -> str:
         return f"""\
     Block type: {self.BlkType}
     Block number: {self.BlkNumber}
     Block language: {self.BlkLang}
@@ -230,98 +232,93 @@
     Family: {self.Family}
     Header: {self.Header}"""
 
 
 class S7DataItem(ctypes.Structure):
     _pack_ = 1
     _fields_ = [
-        ('Area', ctypes.c_int32),
-        ('WordLen', ctypes.c_int32),
-        ('Result', ctypes.c_int32),
-        ('DBNumber', ctypes.c_int32),
-        ('Start', ctypes.c_int32),
-        ('Amount', ctypes.c_int32),
-        ('pData', ctypes.POINTER(ctypes.c_uint8))
+        ("Area", ctypes.c_int32),
+        ("WordLen", ctypes.c_int32),
+        ("Result", ctypes.c_int32),
+        ("DBNumber", ctypes.c_int32),
+        ("Start", ctypes.c_int32),
+        ("Amount", ctypes.c_int32),
+        ("pData", ctypes.POINTER(ctypes.c_uint8)),
     ]
 
     def __str__(self) -> str:
-        return f"<S7DataItem Area: {self.Area} WordLen: {self.WordLen} Result: {self.Result} "\
-               f"DBNumber: {self.DBNumber} Start: {self.Start} Amount: {self.Amount} pData: {self.pData}>"
+        return (
+            f"<S7DataItem Area: {self.Area} WordLen: {self.WordLen} Result: {self.Result} "
+            f"DBNumber: {self.DBNumber} Start: {self.Start} Amount: {self.Amount} pData: {self.pData}>"
+        )
 
 
 class S7CpuInfo(ctypes.Structure):
     _fields_ = [
-        ('ModuleTypeName', ctypes.c_char * 33),
-        ('SerialNumber', ctypes.c_char * 25),
-        ('ASName', ctypes.c_char * 25),
-        ('Copyright', ctypes.c_char * 27),
-        ('ModuleName', ctypes.c_char * 25)
+        ("ModuleTypeName", ctypes.c_char * 33),
+        ("SerialNumber", ctypes.c_char * 25),
+        ("ASName", ctypes.c_char * 25),
+        ("Copyright", ctypes.c_char * 27),
+        ("ModuleName", ctypes.c_char * 25),
     ]
 
     def __str__(self):
-        return f"<S7CpuInfo ModuleTypeName: {self.ModuleTypeName} SerialNumber: {self.SerialNumber} "\
-               f"ASName: {self.ASName} Copyright: {self.Copyright} ModuleName: {self.ModuleName}>"
+        return (
+            f"<S7CpuInfo ModuleTypeName: {self.ModuleTypeName} SerialNumber: {self.SerialNumber} "
+            f"ASName: {self.ASName} Copyright: {self.Copyright} ModuleName: {self.ModuleName}>"
+        )
 
 
 class S7SZLHeader(ctypes.Structure):
     """
-        LengthDR: Length of a data record of the partial list in bytes
-        NDR: Number of data records contained in the partial list
+    LengthDR: Length of a data record of the partial list in bytes
+    NDR: Number of data records contained in the partial list
     """
-    _fields_ = [
-        ('LengthDR', ctypes.c_uint16),
-        ('NDR', ctypes.c_uint16)
-    ]
+
+    _fields_ = [("LengthDR", ctypes.c_uint16), ("NDR", ctypes.c_uint16)]
 
     def __str__(self) -> str:
         return f"<S7SZLHeader LengthDR: {self.LengthDR}, NDR: {self.NDR}>"
 
 
 class S7SZL(ctypes.Structure):
     """See §33.1 of System Software for S7-300/400 System and Standard Functions"""
-    _fields_ = [
-        ('Header', S7SZLHeader),
-        ('Data', ctypes.c_byte * (0x4000 - 4))
-    ]
+
+    _fields_ = [("Header", S7SZLHeader), ("Data", ctypes.c_byte * (0x4000 - 4))]
 
     def __str__(self) -> str:
         return f"<S7SZL Header: {self.S7SZHeader}, Data: {self.Data}>"
 
 
 class S7SZLList(ctypes.Structure):
-    _fields_ = [
-        ('Header', S7SZLHeader),
-        ('List', word * (0x4000 - 2))
-    ]
+    _fields_ = [("Header", S7SZLHeader), ("List", word * (0x4000 - 2))]
 
 
 class S7OrderCode(ctypes.Structure):
-    _fields_ = [
-        ('OrderCode', ctypes.c_char * 21),
-        ('V1', ctypes.c_byte),
-        ('V2', ctypes.c_byte),
-        ('V3', ctypes.c_byte)
-    ]
+    _fields_ = [("OrderCode", ctypes.c_char * 21), ("V1", ctypes.c_byte), ("V2", ctypes.c_byte), ("V3", ctypes.c_byte)]
 
 
 class S7CpInfo(ctypes.Structure):
     _fields_ = [
-        ('MaxPduLength', ctypes.c_uint16),
-        ('MaxConnections', ctypes.c_uint16),
-        ('MaxMpiRate', ctypes.c_uint16),
-        ('MaxBusRate', ctypes.c_uint16)
+        ("MaxPduLength", ctypes.c_uint16),
+        ("MaxConnections", ctypes.c_uint16),
+        ("MaxMpiRate", ctypes.c_uint16),
+        ("MaxBusRate", ctypes.c_uint16),
     ]
 
     def __str__(self) -> str:
-        return f"<S7CpInfo MaxPduLength: {self.MaxPduLength} MaxConnections: {self.MaxConnections} "\
-               f"MaxMpiRate: {self.MaxMpiRate} MaxBusRate: {self.MaxBusRate}>"
+        return (
+            f"<S7CpInfo MaxPduLength: {self.MaxPduLength} MaxConnections: {self.MaxConnections} "
+            f"MaxMpiRate: {self.MaxMpiRate} MaxBusRate: {self.MaxBusRate}>"
+        )
 
 
 class S7Protection(ctypes.Structure):
     """See §33.19 of System Software for S7-300/400 System and Standard Functions"""
+
     _fields_ = [
-        ('sch_schal', word),
-        ('sch_par', word),
-        ('sch_rel', word),
-        ('bart_sch', word),
-        ('anl_sch', word),
+        ("sch_schal", word),
+        ("sch_par", word),
+        ("sch_rel", word),
+        ("bart_sch", word),
+        ("anl_sch", word),
     ]
```

### Comparing `python-snap7-1.3/test/test_client.py` & `python_snap7-1.4/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import ctypes
 import gc
 import logging
 import struct
 import time
+import pytest
 import unittest
-import platform
 from datetime import datetime, timedelta, date
 from multiprocessing import Process
 from unittest import mock
 
 
 import snap7
+import snap7.util.getters
+import snap7.util.setters
 from snap7 import util
 from snap7.common import check_error
 from snap7.server import mainloop
-from snap7.types import S7AreaDB, S7DataItem, S7SZL, S7SZLList, buffer_type, buffer_size, S7Object, Areas, WordLen
+from snap7.types import S7AreaDB, S7DataItem, S7SZL, S7SZLList, buffer_type, buffer_size, Areas, WordLen
 
 
 logging.basicConfig(level=logging.WARNING)
 
-ip = '127.0.0.1'
+ip = "127.0.0.1"
 tcpport = 1102
 db_number = 1
 rack = 1
 slot = 1
 
 
+@pytest.mark.client
 class TestClient(unittest.TestCase):
-
     process = None
 
     @classmethod
     def setUpClass(cls):
         cls.process = Process(target=mainloop)
         cls.process.start()
         time.sleep(2)  # wait for server to start
@@ -81,24 +83,24 @@
         self.client.db_get(db_number=db_number)
 
     def test_read_multi_vars(self):
         db = 1
 
         # build and write test values
         test_value_1 = 129.5
-        test_bytes_1 = bytearray(struct.pack('>f', test_value_1))
+        test_bytes_1 = bytearray(struct.pack(">f", test_value_1))
         self.client.db_write(db, 0, test_bytes_1)
 
         test_value_2 = -129.5
-        test_bytes_2 = bytearray(struct.pack('>f', test_value_2))
+        test_bytes_2 = bytearray(struct.pack(">f", test_value_2))
         self.client.db_write(db, 4, test_bytes_2)
 
         test_value_3 = 123
         test_bytes_3 = bytearray([0, 0])
-        util.set_int(test_bytes_3, 0, test_value_3)
+        snap7.util.setters.set_int(test_bytes_3, 0, test_value_3)
         self.client.db_write(db, 8, test_bytes_3)
 
         test_values = [test_value_1, test_value_2, test_value_3]
 
         # build up our requests
         data_items = (S7DataItem * 3)()
 
@@ -125,23 +127,22 @@
 
         # create buffers to receive the data
         # use the Amount attribute on each item to size the buffer
         for di in data_items:
             # create the buffer
             dataBuffer = ctypes.create_string_buffer(di.Amount)
             # get a pointer to the buffer
-            pBuffer = ctypes.cast(ctypes.pointer(dataBuffer),
-                                  ctypes.POINTER(ctypes.c_uint8))
+            pBuffer = ctypes.cast(ctypes.pointer(dataBuffer), ctypes.POINTER(ctypes.c_uint8))
             di.pData = pBuffer
 
         result, data_items = self.client.read_multi_vars(data_items)
 
         result_values = []
         # function to cast bytes to match data_types[] above
-        byte_to_value = [util.get_real, util.get_real, util.get_int]
+        byte_to_value = [snap7.util.getters.get_real, snap7.util.getters.get_real, snap7.util.getters.get_int]
 
         # unpack and test the result of each read
         for i in range(len(data_items)):
             btv = byte_to_value[i]
             di = data_items[i]
             value = btv(di.pData, 0)
             result_values.append(value)
@@ -171,83 +172,82 @@
     def test_read_area(self):
         amount = 1
         start = 1
 
         # Test read_area with a DB
         area = Areas.DB
         dbnumber = 1
-        data = bytearray(b'\x11')
+        data = bytearray(b"\x11")
         self.client.write_area(area, dbnumber, start, data)
         res = self.client.read_area(area, dbnumber, start, amount)
         self.assertEqual(data, bytearray(res))
 
         # Test read_area with a TM
         area = Areas.TM
         dbnumber = 0
-        data = bytearray(b'\x12\x34')
+        data = bytearray(b"\x12\x34")
         self.client.write_area(area, dbnumber, start, data)
         res = self.client.read_area(area, dbnumber, start, amount)
         self.assertEqual(data, bytearray(res))
 
         # Test read_area with a CT
         area = Areas.CT
         dbnumber = 0
-        data = bytearray(b'\x13\x35')
+        data = bytearray(b"\x13\x35")
         self.client.write_area(area, dbnumber, start, data)
         res = self.client.read_area(area, dbnumber, start, amount)
         self.assertEqual(data, bytearray(res))
 
     def test_write_area(self):
         # Test write area with a DB
         area = Areas.DB
         dbnumber = 1
         start = 1
-        data = bytearray(b'\x11')
+        data = bytearray(b"\x11")
         self.client.write_area(area, dbnumber, start, data)
         res = self.client.read_area(area, dbnumber, start, 1)
         self.assertEqual(data, bytearray(res))
 
         # Test write area with a TM
         area = Areas.TM
         dbnumber = 0
-        timer = bytearray(b'\x12\x00')
+        timer = bytearray(b"\x12\x00")
         res = self.client.write_area(area, dbnumber, start, timer)
         res = self.client.read_area(area, dbnumber, start, 1)
         self.assertEqual(timer, bytearray(res))
 
         # Test write area with a CT
         area = Areas.CT
         dbnumber = 0
-        timer = bytearray(b'\x13\x00')
+        timer = bytearray(b"\x13\x00")
         res = self.client.write_area(area, dbnumber, start, timer)
         res = self.client.read_area(area, dbnumber, start, 1)
         self.assertEqual(timer, bytearray(res))
 
     def test_list_blocks(self):
         self.client.list_blocks()
 
     def test_list_blocks_of_type(self):
-        self.client.list_blocks_of_type('DB', 10)
+        self.client.list_blocks_of_type("DB", 10)
 
-        self.assertRaises(ValueError, self.client.list_blocks_of_type, 'NOblocktype', 10)
+        self.assertRaises(ValueError, self.client.list_blocks_of_type, "NOblocktype", 10)
 
     def test_get_block_info(self):
         """test Cli_GetAgBlockInfo"""
-        self.client.get_block_info('DB', 1)
+        self.client.get_block_info("DB", 1)
 
-        self.assertRaises(Exception, self.client.get_block_info,
-                          'NOblocktype', 10)
-        self.assertRaises(Exception, self.client.get_block_info, 'DB', 10)
+        self.assertRaises(Exception, self.client.get_block_info, "NOblocktype", 10)
+        self.assertRaises(Exception, self.client.get_block_info, "DB", 10)
 
     def test_get_cpu_state(self):
         """this tests the get_cpu_state function"""
         self.client.get_cpu_state()
 
     def test_set_session_password(self):
-        password = 'abcdefgh'
+        password = "abcdefgh"  # noqa: S105
         self.client.set_session_password(password)
 
     def test_clear_session_password(self):
         self.client.clear_session_password()
 
     def test_set_connection_params(self):
         self.client.set_connection_params("10.0.0.2", 10, 10)
@@ -272,27 +272,27 @@
         start = 1
         size = 10
         data = bytearray(size)
         result = self.client.ab_write(start=start, data=data)
         self.assertEqual(0, result)
 
     def test_as_ab_read(self):
-        expected = b'\x10\x01'
+        expected = b"\x10\x01"
         self.client.ab_write(0, bytearray(expected))
 
         wordlen = WordLen.Byte
         type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
         buffer = (type_ * 2)()
         self.client.as_ab_read(0, 2, buffer)
         result = self.client.wait_as_completion(500)
         self.assertEqual(0, result)
         self.assertEqual(expected, bytearray(buffer))
 
     def test_as_ab_write(self):
-        data = b'\x01\x11'
+        data = b"\x01\x11"
         response = self.client.as_ab_write(0, bytearray(data))
         result = self.client.wait_as_completion(500)
         self.assertEqual(0, response)
         self.assertEqual(0, result)
         self.assertEqual(data, self.client.ab_read(0, 2))
 
     def test_compress(self):
@@ -315,16 +315,15 @@
             (snap7.types.DstRef, 128),
             (snap7.types.SrcTSap, 128),
             (snap7.types.PDURequest, 470),
         )
         for param, value in values:
             self.client.set_param(param, value)
 
-        self.assertRaises(Exception, self.client.set_param,
-                          snap7.types.RemotePort, 1)
+        self.assertRaises(Exception, self.client.set_param, snap7.types.RemotePort, 1)
 
     def test_get_param(self):
         expected = (
             (snap7.types.RemotePort, tcpport),
             (snap7.types.PingTimeout, 750),
             (snap7.types.SendTimeout, 10),
             (snap7.types.RecvTimeout, 3000),
@@ -332,59 +331,65 @@
             (snap7.types.DstRef, 0),
             (snap7.types.SrcTSap, 256),
             (snap7.types.PDURequest, 480),
         )
         for param, value in expected:
             self.assertEqual(self.client.get_param(param), value)
 
-        non_client = (snap7.types.LocalPort, snap7.types.WorkInterval, snap7.types.MaxClients,
-                      snap7.types.BSendTimeout, snap7.types.BRecvTimeout, snap7.types.RecoveryTime,
-                      snap7.types.KeepAliveTime)
+        non_client = (
+            snap7.types.LocalPort,
+            snap7.types.WorkInterval,
+            snap7.types.MaxClients,
+            snap7.types.BSendTimeout,
+            snap7.types.BRecvTimeout,
+            snap7.types.RecoveryTime,
+            snap7.types.KeepAliveTime,
+        )
 
         # invalid param for client
         for param in non_client:
             self.assertRaises(Exception, self.client.get_param, non_client)
 
     def test_as_copy_ram_to_rom(self):
         response = self.client.as_copy_ram_to_rom(timeout=1)
         self.client.wait_as_completion(1100)
         self.assertEqual(0, response)
 
     def test_as_ct_read(self):
         # Cli_AsCTRead
-        expected = b'\x10\x01'
+        expected = b"\x10\x01"
         self.client.ct_write(0, 1, bytearray(expected))
         type_ = snap7.types.wordlen_to_ctypes[WordLen.Counter.value]
         buffer = (type_ * 1)()
         self.client.as_ct_read(0, 1, buffer)
         self.client.wait_as_completion(500)
         self.assertEqual(expected, bytearray(buffer))
 
     def test_as_ct_write(self):
         # Cli_CTWrite
-        data = b'\x01\x11'
+        data = b"\x01\x11"
         response = self.client.as_ct_write(0, 1, bytearray(data))
         result = self.client.wait_as_completion(500)
         self.assertEqual(0, response)
         self.assertEqual(0, result)
         self.assertEqual(data, self.client.ct_read(0, 1))
 
     def test_as_db_fill(self):
         filler = 31
-        expected = bytearray(filler.to_bytes(1, byteorder='big') * 100)
+        expected = bytearray(filler.to_bytes(1, byteorder="big") * 100)
         self.client.db_fill(1, filler)
         self.client.wait_as_completion(500)
         self.assertEqual(expected, self.client.db_read(1, 0, 100))
 
     def test_as_db_get(self):
         _buffer = buffer_type()
         size = ctypes.c_int(buffer_size)
         self.client.as_db_get(db_number, _buffer, size)
         self.client.wait_as_completion(500)
-        result = bytearray(_buffer)[:size.value]
+        result = bytearray(_buffer)[: size.value]
         self.assertEqual(100, len(result))
 
     def test_as_db_read(self):
         size = 40
         start = 0
         db = 1
         expected = bytearray(40)
@@ -425,44 +430,44 @@
     def test_get_pdu_length(self):
         pduRequested = self.client.get_param(10)
         pduSize = self.client.get_pdu_length()
         self.assertEqual(pduSize, pduRequested)
 
     def test_get_cpu_info(self):
         expected = (
-            ('ModuleTypeName', 'CPU 315-2 PN/DP'),
-            ('SerialNumber', 'S C-C2UR28922012'),
-            ('ASName', 'SNAP7-SERVER'),
-            ('Copyright', 'Original Siemens Equipment'),
-            ('ModuleName', 'CPU 315-2 PN/DP')
+            ("ModuleTypeName", "CPU 315-2 PN/DP"),
+            ("SerialNumber", "S C-C2UR28922012"),
+            ("ASName", "SNAP7-SERVER"),
+            ("Copyright", "Original Siemens Equipment"),
+            ("ModuleName", "CPU 315-2 PN/DP"),
         )
         cpuInfo = self.client.get_cpu_info()
         for param, value in expected:
-            self.assertEqual(getattr(cpuInfo, param).decode('utf-8'), value)
+            self.assertEqual(getattr(cpuInfo, param).decode("utf-8"), value)
 
     def test_db_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
         original = self.client._library.Cli_DBWrite
         self.client._library.Cli_DBWrite = mock_write
-        data = b'\xDE\xAD\xBE\xEF'
+        data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.db_write(db_number=1, start=0, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
             self.client._library.Cli_DBWrite = original
 
     def test_download_with_byte_literal_does_not_throw(self):
         mock_download = mock.MagicMock()
         mock_download.return_value = None
         original = self.client._library.Cli_Download
         self.client._library.Cli_Download = mock_download
-        data = b'\xDE\xAD\xBE\xEF'
+        data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.download(block_num=db_number, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
             self.client._library.Cli_Download = original
@@ -472,15 +477,15 @@
         mock_writearea.return_value = None
         original = self.client._library.Cli_WriteArea
         self.client._library.Cli_WriteArea = mock_writearea
 
         area = Areas.DB
         dbnumber = 1
         start = 1
-        data = b'\xDE\xAD\xBE\xEF'
+        data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.write_area(area, dbnumber, start, bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
             self.client._library.Cli_WriteArea = original
@@ -488,15 +493,15 @@
     def test_ab_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
         original = self.client._library.Cli_ABWrite
         self.client._library.Cli_ABWrite = mock_write
 
         start = 1
-        data = b'\xDE\xAD\xBE\xEF'
+        data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.ab_write(start=start, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
             self.client._library.Cli_ABWrite = original
@@ -505,45 +510,45 @@
     def test_as_ab_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
         original = self.client._library.Cli_AsABWrite
         self.client._library.Cli_AsABWrite = mock_write
 
         start = 1
-        data = b'\xDE\xAD\xBE\xEF'
+        data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.as_ab_write(start=start, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
             self.client._library.Cli_AsABWrite = original
 
     @unittest.skip("TODO: not yet fully implemented")
     def test_as_db_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
         original = self.client._library.Cli_AsDBWrite
         self.client._library.Cli_AsDBWrite = mock_write
-        data = b'\xDE\xAD\xBE\xEF'
+        data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.db_write(db_number=1, start=0, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
             self.client._library.Cli_AsDBWrite = original
 
     @unittest.skip("TODO: not yet fully implemented")
     def test_as_download_with_byte_literal_does_not_throw(self):
         mock_download = mock.MagicMock()
         mock_download.return_value = None
         original = self.client._library.Cli_AsDownload
         self.client._library.Cli_AsDownload = mock_download
-        data = b'\xDE\xAD\xBE\xEF'
+        data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.as_download(block_num=db_number, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
             self.client._library.Cli_AsDownload = original
@@ -588,31 +593,33 @@
         for i in range(tries):
             self.client.as_read_area(area, dbnumber, start, size, wordlen, pdata)
             res = None
             try:
                 res = self.client.wait_as_completion(timeout)
                 check_error(res)
             except RuntimeError as s7_err:
-                if not s7_err.args[0] == b'CLI : Job Timeout':
+                if not s7_err.args[0] == b"CLI : Job Timeout":
                     self.fail(f"While waiting another error appeared: {s7_err}")
                 # Wait for a thread to finish
                 time.sleep(0.1)
                 return
             except BaseException:
                 self.fail(f"While waiting another error appeared:>>>>>>>> {res}")
 
-        self.fail(f"After {tries} tries, no timout could be envoked by snap7. Either tests are passing to fast or"
-                  f"a problem is existing in the method. Fail test.")
+        self.fail(
+            f"After {tries} tries, no timout could be envoked by snap7. Either tests are passing to fast or"
+            f"a problem is existing in the method. Fail test."
+        )
 
     def test_check_as_completion(self, timeout=5):
         # Cli_CheckAsCompletion
         check_status = ctypes.c_int(-1)
         pending_checked = False
         # preparing Server values
-        data = bytearray(b'\x01\xFF')
+        data = bytearray(b"\x01\xff")
         size = len(data)
         area = Areas.DB
         db = 1
         start = 1
         self.client.write_area(area, db, start, data)
 
         # start as_request and test
@@ -625,83 +632,82 @@
                 self.assertEqual(data, bytearray(cdata))
                 break
             pending_checked = True
             time.sleep(1)
         else:
             self.fail(f"TimeoutError - Process pends for more than {timeout} seconds")
         if pending_checked is False:
-            logging.warning("Pending was never reached, because Server was to fast,"
-                            " but request to server was successfull.")
+            logging.warning("Pending was never reached, because Server was to fast," " but request to server was successfull.")
 
     def test_as_read_area(self):
         amount = 1
         start = 1
 
         # Test read_area with a DB
         area = Areas.DB
         dbnumber = 1
-        data = bytearray(b'\x11')
+        data = bytearray(b"\x11")
         self.client.write_area(area, dbnumber, start, data)
         wordlen, usrdata = self.client._prepare_as_read_area(area, amount)
         pusrdata = ctypes.byref(usrdata)
         self.client.as_read_area(area, dbnumber, start, amount, wordlen, pusrdata)
         self.client.wait_as_completion(1000)
         self.assertEqual(bytearray(usrdata), data)
 
         # Test read_area with a TM
         area = Areas.TM
         dbnumber = 0
-        data = bytearray(b'\x12\x34')
+        data = bytearray(b"\x12\x34")
         self.client.write_area(area, dbnumber, start, data)
         wordlen, usrdata = self.client._prepare_as_read_area(area, amount)
         pusrdata = ctypes.byref(usrdata)
         self.client.as_read_area(area, dbnumber, start, amount, wordlen, pusrdata)
         self.client.wait_as_completion(1000)
         self.assertEqual(bytearray(usrdata), data)
 
         # Test read_area with a CT
         area = Areas.CT
         dbnumber = 0
-        data = bytearray(b'\x13\x35')
+        data = bytearray(b"\x13\x35")
         self.client.write_area(area, dbnumber, start, data)
         wordlen, usrdata = self.client._prepare_as_read_area(area, amount)
         pusrdata = ctypes.byref(usrdata)
         self.client.as_read_area(area, dbnumber, start, amount, wordlen, pusrdata)
         self.client.wait_as_completion(1000)
         self.assertEqual(bytearray(usrdata), data)
 
     def test_as_write_area(self):
         # Test write area with a DB
         area = Areas.DB
         dbnumber = 1
         size = 1
         start = 1
-        data = bytearray(b'\x11')
+        data = bytearray(b"\x11")
         wordlen, cdata = self.client._prepare_as_write_area(area, data)
         res = self.client.as_write_area(area, dbnumber, start, size, wordlen, cdata)
         self.client.wait_as_completion(1000)
         res = self.client.read_area(area, dbnumber, start, 1)
         self.assertEqual(data, bytearray(res))
 
         # Test write area with a TM
         area = Areas.TM
         dbnumber = 0
         size = 2
-        timer = bytearray(b'\x12\x00')
+        timer = bytearray(b"\x12\x00")
         wordlen, cdata = self.client._prepare_as_write_area(area, timer)
         res = self.client.as_write_area(area, dbnumber, start, size, wordlen, cdata)
         self.client.wait_as_completion(1000)
         res = self.client.read_area(area, dbnumber, start, 1)
         self.assertEqual(timer, bytearray(res))
 
         # Test write area with a CT
         area = Areas.CT
         dbnumber = 0
         size = 2
-        timer = bytearray(b'\x13\x00')
+        timer = bytearray(b"\x13\x00")
         wordlen, cdata = self.client._prepare_as_write_area(area, timer)
         res = self.client.as_write_area(area, dbnumber, start, size, wordlen, cdata)
         self.client.wait_as_completion(1000)
         res = self.client.read_area(area, dbnumber, start, 1)
         self.assertEqual(timer, bytearray(res))
 
     def test_as_eb_read(self):
@@ -711,131 +717,131 @@
         buffer = (type_ * 1)()
         response = self.client.as_eb_read(0, 1, buffer)
         self.assertEqual(0, response)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_eb_write(self):
         # Cli_AsEBWrite
-        response = self.client.as_eb_write(0, 1, bytearray(b'\x00'))
+        response = self.client.as_eb_write(0, 1, bytearray(b"\x00"))
         self.assertEqual(0, response)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_full_upload(self):
         # Cli_AsFullUpload
-        self.client.as_full_upload('DB', 1)
+        self.client.as_full_upload("DB", 1)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_list_blocks_of_type(self):
         data = (ctypes.c_uint16 * 10)()
         count = ctypes.c_int()
-        self.client.as_list_blocks_of_type('DB', data, count)
+        self.client.as_list_blocks_of_type("DB", data, count)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_mb_read(self):
         # Cli_AsMBRead
         wordlen = WordLen.Byte
         type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
         data = (type_ * 1)()
         self.client.as_mb_read(0, 1, data)
         bytearray(data)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_mb_write(self):
         # Cli_AsMBWrite
-        response = self.client.as_mb_write(0, 1, bytearray(b'\x00'))
+        response = self.client.as_mb_write(0, 1, bytearray(b"\x00"))
         self.assertEqual(0, response)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_read_szl(self):
         # Cli_AsReadSZL
-        expected = b'S C-C2UR28922012\x00\x00\x00\x00\x00\x00\x00\x00'
-        ssl_id = 0x011c
+        expected = b"S C-C2UR28922012\x00\x00\x00\x00\x00\x00\x00\x00"
+        ssl_id = 0x011C
         index = 0x0005
         s7_szl = S7SZL()
         size = ctypes.c_int(ctypes.sizeof(s7_szl))
         self.client.as_read_szl(ssl_id, index, s7_szl, size)
         self.client.wait_as_completion(100)
         result = bytes(s7_szl.Data)[2:26]
         self.assertEqual(expected, result)
 
     def test_as_read_szl_list(self):
         # Cli_AsReadSZLList
-        expected = b'\x00\x00\x00\x0f\x02\x00\x11\x00\x11\x01\x11\x0f\x12\x00\x12\x01'
+        expected = b"\x00\x00\x00\x0f\x02\x00\x11\x00\x11\x01\x11\x0f\x12\x00\x12\x01"
         szl_list = S7SZLList()
         items_count = ctypes.c_int(ctypes.sizeof(szl_list))
         self.client.as_read_szl_list(szl_list, items_count)
         self.client.wait_as_completion(500)
         result = bytearray(szl_list.List)[:16]
         self.assertEqual(expected, result)
 
     def test_as_tm_read(self):
         # Cli_AsMBRead
-        expected = b'\x10\x01'
+        expected = b"\x10\x01"
         wordlen = WordLen.Timer
         self.client.tm_write(0, 1, bytearray(expected))
         type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
         buffer = (type_ * 1)()
         self.client.as_tm_read(0, 1, buffer)
         self.client.wait_as_completion(500)
         self.assertEqual(expected, bytearray(buffer))
 
     def test_as_tm_write(self):
         # Cli_AsMBWrite
-        data = b'\x10\x01'
+        data = b"\x10\x01"
         response = self.client.as_tm_write(0, 1, bytearray(data))
         result = self.client.wait_as_completion(500)
         self.assertEqual(0, response)
         self.assertEqual(0, result)
         self.assertEqual(data, self.client.tm_read(0, 1))
 
     def test_copy_ram_to_rom(self):
         # Cli_CopyRamToRom
         self.assertEqual(0, self.client.copy_ram_to_rom(timeout=1))
 
     def test_ct_read(self):
         # Cli_CTRead
-        data = b'\x10\x01'
+        data = b"\x10\x01"
         self.client.ct_write(0, 1, bytearray(data))
         result = self.client.ct_read(0, 1)
         self.assertEqual(data, result)
 
     def test_ct_write(self):
         # Cli_CTWrite
-        data = b'\x01\x11'
+        data = b"\x01\x11"
         self.assertEqual(0, self.client.ct_write(0, 1, bytearray(data)))
         self.assertRaises(ValueError, self.client.ct_write, 0, 2, bytes(1))
 
     def test_db_fill(self):
         # Cli_DBFill
         filler = 31
-        expected = bytearray(filler.to_bytes(1, byteorder='big') * 100)
+        expected = bytearray(filler.to_bytes(1, byteorder="big") * 100)
         self.client.db_fill(1, filler)
         self.assertEqual(expected, self.client.db_read(1, 0, 100))
 
     def test_eb_read(self):
         # Cli_EBRead
         self.client._library.Cli_EBRead = mock.Mock(return_value=0)
         response = self.client.eb_read(0, 1)
         self.assertTrue(isinstance(response, bytearray))
         self.assertEqual(1, len(response))
 
     def test_eb_write(self):
         # Cli_EBWrite
         self.client._library.Cli_EBWrite = mock.Mock(return_value=0)
-        response = self.client.eb_write(0, 1, bytearray(b'\x00'))
+        response = self.client.eb_write(0, 1, bytearray(b"\x00"))
         self.assertEqual(0, response)
 
     def test_error_text(self):
         # Cli_ErrorText
         CPU_INVALID_PASSWORD = 0x01E00000
         CPU_INVLID_VALUE = 0x00D00000
         CANNOT_CHANGE_PARAM = 0x02600000
-        self.assertEqual('CPU : Invalid password', self.client.error_text(CPU_INVALID_PASSWORD))
-        self.assertEqual('CPU : Invalid value supplied', self.client.error_text(CPU_INVLID_VALUE))
-        self.assertEqual('CLI : Cannot change this param now', self.client.error_text(CANNOT_CHANGE_PARAM))
+        self.assertEqual("CPU : Invalid password", self.client.error_text(CPU_INVALID_PASSWORD))
+        self.assertEqual("CPU : Invalid value supplied", self.client.error_text(CPU_INVLID_VALUE))
+        self.assertEqual("CLI : Cannot change this param now", self.client.error_text(CANNOT_CHANGE_PARAM))
 
     def test_get_cp_info(self):
         # Cli_GetCpInfo
         result = self.client.get_cp_info()
         self.assertEqual(2048, result.MaxPduLength)
         self.assertEqual(0, result.MaxConnections)
         self.assertEqual(1024, result.MaxMpiRate)
@@ -848,161 +854,169 @@
 
     def test_get_last_error(self):
         # Cli_GetLastError
         self.assertEqual(0, self.client.get_last_error())
 
     def test_get_order_code(self):
         # Cli_GetOrderCode
-        expected = b'6ES7 315-2EH14-0AB0 '
+        expected = b"6ES7 315-2EH14-0AB0 "
         result = self.client.get_order_code()
         self.assertEqual(expected, result.OrderCode)
 
     def test_get_protection(self):
         # Cli_GetProtection
         result = self.client.get_protection()
         self.assertEqual(1, result.sch_schal)
         self.assertEqual(0, result.sch_par)
         self.assertEqual(1, result.sch_rel)
         self.assertEqual(2, result.bart_sch)
         self.assertEqual(0, result.anl_sch)
 
     def test_get_pg_block_info(self):
-        valid_db_block = b'pp\x01\x01\x05\n\x00c\x00\x00\x00t\x00\x00\x00\x00\x01\x8d\xbe)2\xa1\x01' \
-                         b'\x85V\x1f2\xa1\x00*\x00\x00\x00\x00\x00\x02\x01\x0f\x05c\x00#\x00\x00\x00' \
-                         b'\x11\x04\x10\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01' \
-                         b'\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x00' \
-                         b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00' \
-                         b'\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+        valid_db_block = (
+            b"pp\x01\x01\x05\n\x00c\x00\x00\x00t\x00\x00\x00\x00\x01\x8d\xbe)2\xa1\x01"
+            b"\x85V\x1f2\xa1\x00*\x00\x00\x00\x00\x00\x02\x01\x0f\x05c\x00#\x00\x00\x00"
+            b"\x11\x04\x10\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01"
+            b"\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x01\x04\x00"
+            b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+            b"\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        )
         block_info = self.client.get_pg_block_info(bytearray(valid_db_block))
         self.assertEqual(10, block_info.BlkType)
         self.assertEqual(99, block_info.BlkNumber)
         self.assertEqual(2752512, block_info.SBBLength)
         self.assertEqual(bytes((util.utc2local(date(2019, 6, 27)).strftime("%Y/%m/%d")), encoding="utf-8"), block_info.CodeDate)
         self.assertEqual(bytes((util.utc2local(date(2019, 6, 27)).strftime("%Y/%m/%d")), encoding="utf-8"), block_info.IntfDate)
 
     def test_iso_exchange_buffer(self):
         # Cli_IsoExchangeBuffer
-        self.client.db_write(1, 0, bytearray(b'\x11'))
+        self.client.db_write(1, 0, bytearray(b"\x11"))
         # PDU read DB1 1.0 BYTE
-        data = b'\x32\x01\x00\x00\x01\x00\x00\x0e\x00\x00\x04\x01\x12\x0a\x10\x02\x00\x01\x00\x01\x84\x00\x00\x00'
+        data = b"\x32\x01\x00\x00\x01\x00\x00\x0e\x00\x00\x04\x01\x12\x0a\x10\x02\x00\x01\x00\x01\x84\x00\x00\x00"
         # PDU response
-        expected = bytearray(b'2\x03\x00\x00\x01\x00\x00\x02\x00\x05\x00\x00\x04\x01\xff\x04\x00\x08\x11')
+        expected = bytearray(b"2\x03\x00\x00\x01\x00\x00\x02\x00\x05\x00\x00\x04\x01\xff\x04\x00\x08\x11")
         self.assertEqual(expected, self.client.iso_exchange_buffer(bytearray(data)))
 
     def test_mb_read(self):
         # Cli_MBRead
         self.client._library.Cli_MBRead = mock.Mock(return_value=0)
         response = self.client.mb_read(0, 10)
         self.assertTrue(isinstance(response, bytearray))
         self.assertEqual(10, len(response))
 
     def test_mb_write(self):
         # Cli_MBWrite
         self.client._library.Cli_MBWrite = mock.Mock(return_value=0)
-        response = self.client.mb_write(0, 1, bytearray(b'\x00'))
+        response = self.client.mb_write(0, 1, bytearray(b"\x00"))
         self.assertEqual(0, response)
 
     def test_read_szl(self):
         # read_szl_partial_list
         expected_number_of_records = 10
         expected_length_of_record = 34
-        ssl_id = 0x001c
+        ssl_id = 0x001C
         response = self.client.read_szl(ssl_id)
         self.assertEqual(expected_number_of_records, response.Header.NDR)
         self.assertEqual(expected_length_of_record, response.Header.LengthDR)
         # read_szl_single_data_record
-        expected = b'S C-C2UR28922012\x00\x00\x00\x00\x00\x00\x00\x00'
-        ssl_id = 0x011c
+        expected = b"S C-C2UR28922012\x00\x00\x00\x00\x00\x00\x00\x00"
+        ssl_id = 0x011C
         index = 0x0005
         response = self.client.read_szl(ssl_id, index)
         result = bytes(response.Data)[2:26]
         self.assertEqual(expected, result)
         # read_szl_order_number
-        expected = b'6ES7 315-2EH14-0AB0 '
+        expected = b"6ES7 315-2EH14-0AB0 "
         ssl_id = 0x0111
         index = 0x0001
         response = self.client.read_szl(ssl_id, index)
         result = bytes(response.Data[2:22])
         self.assertEqual(expected, result)
         # read_szl_invalid_id
-        ssl_id = 0xffff
-        index = 0xffff
+        ssl_id = 0xFFFF
+        index = 0xFFFF
         self.assertRaises(RuntimeError, self.client.read_szl, ssl_id)
         self.assertRaises(RuntimeError, self.client.read_szl, ssl_id, index)
 
     def test_read_szl_list(self):
         # Cli_ReadSZLList
-        expected = b'\x00\x00\x00\x0f\x02\x00\x11\x00\x11\x01\x11\x0f\x12\x00\x12\x01'
+        expected = b"\x00\x00\x00\x0f\x02\x00\x11\x00\x11\x01\x11\x0f\x12\x00\x12\x01"
         result = self.client.read_szl_list()
         self.assertEqual(expected, result[:16])
 
     def test_set_plc_system_datetime(self):
         # Cli_SetPlcSystemDateTime
         self.assertEqual(0, self.client.set_plc_system_datetime())
 
     def test_tm_read(self):
         # Cli_TMRead
-        data = b'\x10\x01'
+        data = b"\x10\x01"
         self.client.tm_write(0, 1, bytearray(data))
         result = self.client.tm_read(0, 1)
         self.assertEqual(data, result)
 
     def test_tm_write(self):
         # Cli_TMWrite
-        data = b'\x10\x01'
+        data = b"\x10\x01"
         self.assertEqual(0, self.client.tm_write(0, 1, bytearray(data)))
         self.assertEqual(data, self.client.tm_read(0, 1))
         self.assertRaises(RuntimeError, self.client.tm_write, 0, 100, bytes(200))
         self.assertRaises(ValueError, self.client.tm_write, 0, 2, bytes(2))
 
     def test_write_multi_vars(self):
         # Cli_WriteMultiVars
         items_count = 3
         items = []
         areas = [Areas.DB, Areas.CT, Areas.TM]
         expected_list = []
-        for i in range(0, items_count):
+        for i in range(items_count):
             item = S7DataItem()
             item.Area = ctypes.c_int32(areas[i].value)
             wordlen = WordLen.Byte
             item.WordLen = ctypes.c_int32(wordlen.value)
             item.DBNumber = ctypes.c_int32(1)
             item.Start = ctypes.c_int32(0)
             item.Amount = ctypes.c_int32(4)
-            data = (i + 1).to_bytes(1, byteorder='big') * 4
+            data = (i + 1).to_bytes(1, byteorder="big") * 4
             array_class = ctypes.c_uint8 * len(data)
             cdata = array_class.from_buffer_copy(data)
             item.pData = ctypes.cast(cdata, ctypes.POINTER(array_class)).contents
             items.append(item)
             expected_list.append(data)
         result = self.client.write_multi_vars(items)
         self.assertEqual(0, result)
         self.assertEqual(expected_list[0], self.client.db_read(db_number=1, start=0, size=4))
         self.assertEqual(expected_list[1], self.client.ct_read(0, 2))
         self.assertEqual(expected_list[2], self.client.tm_read(0, 2))
 
-    @unittest.skipIf(platform.system() in ['Windows', 'Darwin'], 'Access Violation error')
     def test_set_as_callback(self):
-        expected = b"\x11\x11"
-        self.callback_counter = 0
-        cObj = ctypes.cast(ctypes.pointer(ctypes.py_object(self)), S7Object)
-
-        def callback(FUsrPtr, JobOp, response):
-            self = ctypes.cast(FUsrPtr, ctypes.POINTER(ctypes.py_object)).contents.value
-            self.callback_counter += 1
-
-        cfunc_type = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.POINTER(S7Object), ctypes.c_int, ctypes.c_int)
-        self.client.set_as_callback(cfunc_type(callback), cObj)
-        self.client.as_ct_write(0, 1, bytearray(expected))
-
-        self._as_check_loop()
-        self.assertEqual(expected, self.client.ct_read(0, 1))
-        self.assertEqual(1, self.callback_counter)
+        def event_call_back(op_code, op_result):
+            logging.info(f"callback event: {op_code} op_result: {op_result}")
+
+        self.client.set_as_callback(event_call_back)
+
+
+#        expected = b"\x11\x11"
+#        self.callback_counter = 0
+#        cObj = ctypes.cast(ctypes.pointer(ctypes.py_object(self)), S7Object)
+
+#        def callback(FUsrPtr, JobOp, response):
+#            self = ctypes.cast(FUsrPtr, ctypes.POINTER(ctypes.py_object)).contents.value
+#            self.callback_counter += 1
+#
+#        cfunc_type = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.POINTER(S7Object), ctypes.c_int, ctypes.c_int)
+#        self.client.set_as_callback(cfunc_type(callback), cObj)
+#        self.client.as_ct_write(0, 1, bytearray(expected))
+
+#        self._as_check_loop()
+#        self.assertEqual(expected, self.client.ct_read(0, 1))
+#        self.assertEqual(1, self.callback_counter)
 
 
+@pytest.mark.client
 class TestClientBeforeConnect(unittest.TestCase):
     """
     Test suite of items that should run without an open connection.
     """
 
     def setUp(self):
         self.client = snap7.client.Client()
@@ -1018,18 +1032,19 @@
             (snap7.types.SrcTSap, 128),
             (snap7.types.PDURequest, 470),
         )
         for param, value in values:
             self.client.set_param(param, value)
 
 
+@pytest.mark.client
 class TestLibraryIntegration(unittest.TestCase):
     def setUp(self):
         # replace the function load_library with a mock
-        self.loadlib_patch = mock.patch('snap7.client.load_library')
+        self.loadlib_patch = mock.patch("snap7.client.load_library")
         self.loadlib_func = self.loadlib_patch.start()
 
         # have load_library return another mock
         self.mocklib = mock.MagicMock()
         self.loadlib_func.return_value = self.mocklib
 
         # have the Cli_Create of the mock return None
@@ -1039,18 +1054,18 @@
         # restore load_library
         self.loadlib_patch.stop()
 
     def test_create(self):
         snap7.client.Client()
         self.mocklib.Cli_Create.assert_called_once()
 
-    @mock.patch('snap7.client.byref')
+    @mock.patch("snap7.client.byref")
     def test_gc(self, byref_mock):
         client = snap7.client.Client()
         client._pointer = 10
         del client
         gc.collect()
         self.mocklib.Cli_Destroy.assert_called_once()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `python-snap7-1.3/test/test_common.py` & `python_snap7-1.4/tests/test_common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
+import pytest
 import unittest
 import pathlib
 
 from snap7.common import find_locally
 
 
 logging.basicConfig(level=logging.WARNING)
 
 file_name_test = "test.dll"
 
 
+@pytest.mark.common
 class TestCommon(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls):
         pass
 
     @classmethod
     def tearDownClass(cls):
         pass
@@ -29,9 +30,9 @@
         self.file.unlink()
 
     def test_find_locally(self):
         file = find_locally(file_name_test.replace(".dll", ""))
         self.assertEqual(file, str(self.BASE_DIR / file_name_test))
 
 
-if __name__ == '__main__':
-    unittest.main()
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `python-snap7-1.3/test/test_logo_client.py` & `python_snap7-1.4/tests/test_logo_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 import time
+import pytest
 import unittest
 from multiprocessing import Process
 
 import snap7
 from snap7.server import mainloop
 
 logging.basicConfig(level=logging.WARNING)
 
-ip = '127.0.0.1'
+ip = "127.0.0.1"
 tcpport = 1102
 db_number = 1
 rack = 0x1000
 slot = 0x2000
 
 
+@pytest.mark.logo
 class TestLogoClient(unittest.TestCase):
-
     process = None
 
     @classmethod
     def setUpClass(cls):
         cls.process = Process(target=mainloop)
         cls.process.start()
         time.sleep(2)  # wait for server to start
@@ -64,16 +65,15 @@
             (snap7.types.DstRef, 128),
             (snap7.types.SrcTSap, 128),
             (snap7.types.PDURequest, 470),
         )
         for param, value in values:
             self.client.set_param(param, value)
 
-        self.assertRaises(Exception, self.client.set_param,
-                          snap7.types.RemotePort, 1)
+        self.assertRaises(Exception, self.client.set_param, snap7.types.RemotePort, 1)
 
     def test_get_param(self):
         expected = (
             (snap7.types.RemotePort, tcpport),
             (snap7.types.PingTimeout, 750),
             (snap7.types.SendTimeout, 10),
             (snap7.types.RecvTimeout, 3000),
@@ -81,23 +81,30 @@
             (snap7.types.DstRef, 0),
             (snap7.types.SrcTSap, 4096),
             (snap7.types.PDURequest, 480),
         )
         for param, value in expected:
             self.assertEqual(self.client.get_param(param), value)
 
-        non_client = (snap7.types.LocalPort, snap7.types.WorkInterval, snap7.types.MaxClients,
-                      snap7.types.BSendTimeout, snap7.types.BRecvTimeout, snap7.types.RecoveryTime,
-                      snap7.types.KeepAliveTime)
+        non_client = (
+            snap7.types.LocalPort,
+            snap7.types.WorkInterval,
+            snap7.types.MaxClients,
+            snap7.types.BSendTimeout,
+            snap7.types.BRecvTimeout,
+            snap7.types.RecoveryTime,
+            snap7.types.KeepAliveTime,
+        )
 
         # invalid param for client
         for param in non_client:
             self.assertRaises(Exception, self.client.get_param, non_client)
 
 
+@pytest.mark.logo
 class TestClientBeforeConnect(unittest.TestCase):
     """
     Test suite of items that should run without an open connection.
     """
 
     def setUp(self):
         self.client = snap7.client.Client()
@@ -113,9 +120,9 @@
             (snap7.types.SrcTSap, 128),
             (snap7.types.PDURequest, 470),
         )
         for param, value in values:
             self.client.set_param(param, value)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `python-snap7-1.3/test/test_mainloop.py` & `python_snap7-1.4/tests/test_mainloop.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 import logging
 from multiprocessing.context import Process
 import time
+import pytest
 import unittest
+from typing import Optional
 
 import snap7.error
 import snap7.server
 import snap7.util
+import snap7.util.getters
 from snap7.util import get_bool, get_dint, get_dword, get_int, get_real, get_sint, get_string, get_usint, get_word
 from snap7.client import Client
 import snap7.types
 
 logging.basicConfig(level=logging.WARNING)
 
-ip = '127.0.0.1'
+ip = "127.0.0.1"
 tcpport = 1102
 db_number = 1
 rack = 1
 slot = 1
 
 
+@pytest.mark.mainloop
 class TestServer(unittest.TestCase):
-
-    process = None
+    process: Optional[Process] = None
+    client: Client
 
     @classmethod
     def setUpClass(cls):
         cls.process = Process(target=snap7.server.mainloop, args=[tcpport, True])
         cls.process.start()
         time.sleep(2)  # wait for server to start
 
     @classmethod
-    def tearDownClass(cls):
-        cls.process.terminate()
-        cls.process.join(1)
-        if cls.process.is_alive():
-            cls.process.kill()
+    def tearDownClass(cls) -> None:
+        if cls.process:
+            cls.process.terminate()
+            cls.process.join(1)
+            if cls.process.is_alive():
+                cls.process.kill()
 
-    def setUp(self):
+    def setUp(self) -> None:
         self.client: Client = snap7.client.Client()
         self.client.connect(ip, rack, slot, tcpport)
 
-    def tearDown(self):
-        self.client.disconnect()
-        self.client.destroy()
+    def tearDown(self) -> None:
+        if self.client:
+            self.client.disconnect()
+            self.client.destroy()
 
     @unittest.skip("TODO: only first test used")
-    def test_read_prefill_db(self):
+    def test_read_prefill_db(self) -> None:
         data = self.client.db_read(0, 0, 7)
-        boolean = snap7.util.get_bool(data, 0, 0)
+        boolean = snap7.util.getters.get_bool(data, 0, 0)
         self.assertEqual(boolean, True)
-        integer = snap7.util.get_int(data, 1)
+        integer = snap7.util.getters.get_int(data, 1)
         self.assertEqual(integer, 128)
-        real = snap7.util.get_real(data, 3)
+        real = snap7.util.getters.get_real(data, 3)
         self.assertEqual(real, -128)
 
-    def test_read_booleans(self):
+    def test_read_booleans(self) -> None:
         data = self.client.db_read(0, 0, 1)
         self.assertEqual(False, get_bool(data, 0, 0))
         self.assertEqual(True, get_bool(data, 0, 1))
         self.assertEqual(False, get_bool(data, 0, 2))
         self.assertEqual(True, get_bool(data, 0, 3))
         self.assertEqual(False, get_bool(data, 0, 4))
         self.assertEqual(True, get_bool(data, 0, 5))
         self.assertEqual(False, get_bool(data, 0, 6))
         self.assertEqual(True, get_bool(data, 0, 7))
 
-    def test_read_small_int(self):
+    def test_read_small_int(self) -> None:
         data = self.client.db_read(0, 10, 4)
         value_1 = get_sint(data, 0)
         value_2 = get_sint(data, 1)
         value_3 = get_sint(data, 2)
         value_4 = get_sint(data, 3)
         self.assertEqual(value_1, -128)
         self.assertEqual(value_2, 0)
@@ -124,12 +130,12 @@
         data = self.client.db_read(0, 500, 8 * 4)
         self.assertEqual(get_dword(data, 0), 0x00000000)
         self.assertEqual(get_dword(data, 8), 0x12345678)
         self.assertEqual(get_dword(data, 16), 0x1234ABCD)
         self.assertEqual(get_dword(data, 24), 0xFFFFFFFF)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import logging
 
     logging.basicConfig()
     unittest.main()
```

### Comparing `python-snap7-1.3/test/test_partner.py` & `python_snap7-1.4/tests/test_partner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
+import pytest
 import unittest as unittest
 from unittest import mock
 
 import snap7.partner
-from snap7.exceptions import Snap7Exception
 
 logging.basicConfig(level=logging.WARNING)
 
 
+@pytest.mark.partner
 class TestPartner(unittest.TestCase):
     def setUp(self):
         self.partner = snap7.partner.Partner()
         self.partner.start()
 
     def tearDown(self):
         self.partner.stop()
@@ -60,16 +61,15 @@
             (snap7.types.BRecvTimeout, 3000),
             (snap7.types.RecoveryTime, 500),
             (snap7.types.KeepAliveTime, 5000),
         )
         for param, value in expected:
             self.assertEqual(self.partner.get_param(param), value)
 
-        self.assertRaises(Exception, self.partner.get_param,
-                          snap7.types.MaxClients)
+        self.assertRaises(Exception, self.partner.get_param, snap7.types.MaxClients)
 
     def test_get_stats(self):
         self.partner.get_stats()
 
     def test_get_status(self):
         self.partner.get_status()
 
@@ -90,40 +90,40 @@
             (snap7.types.BRecvTimeout, 2000),
             (snap7.types.RecoveryTime, 400),
             (snap7.types.KeepAliveTime, 4000),
         )
         for param, value in values:
             self.partner.set_param(param, value)
 
-        self.assertRaises(Exception, self.partner.set_param,
-                          snap7.types.RemotePort, 1)
+        self.assertRaises(Exception, self.partner.set_param, snap7.types.RemotePort, 1)
 
     def test_set_recv_callback(self):
         self.partner.set_recv_callback()
 
     def test_set_send_callback(self):
         self.partner.set_send_callback()
 
     def test_start(self):
         self.partner.start()
 
     def test_start_to(self):
-        self.partner.start_to('0.0.0.0', '0.0.0.0', 0, 0)
+        self.partner.start_to("0.0.0.0", "0.0.0.0", 0, 0)  # noqa: S104
 
     def test_stop(self):
         self.partner.stop()
 
     def test_wait_as_b_send_completion(self):
         self.assertRaises(RuntimeError, self.partner.wait_as_b_send_completion)
 
 
+@pytest.mark.partner
 class TestLibraryIntegration(unittest.TestCase):
     def setUp(self):
         # replace the function load_library with a mock
-        self.loadlib_patch = mock.patch('snap7.partner.load_library')
+        self.loadlib_patch = mock.patch("snap7.partner.load_library")
         self.loadlib_func = self.loadlib_patch.start()
 
         # have load_library return another mock
         self.mocklib = mock.MagicMock()
         self.loadlib_func.return_value = self.mocklib
 
         # have the Par_Create of the mock return None
@@ -139,9 +139,9 @@
 
     def test_gc(self):
         partner = snap7.partner.Partner()
         del partner
         self.mocklib.Par_Destroy.assert_called_once()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `python-snap7-1.3/test/test_server.py` & `python_snap7-1.4/tests/test_server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 import ctypes
 import logging
+import pytest
 import unittest
 from unittest import mock
 
-import snap7.error
-import snap7.server
-import snap7.types
+from snap7.common import error_text
+from snap7.error import server_errors
+from snap7.server import Server
+from snap7.types import SrvEvent, mkEvent, mkLog, srvAreaDB, LocalPort, WorkInterval, MaxClients, RemotePort
 
 logging.basicConfig(level=logging.WARNING)
 
 
+@pytest.mark.server
 class TestServer(unittest.TestCase):
-
     def setUp(self):
-        self.server = snap7.server.Server()
+        self.server = Server()
         self.server.start(tcpport=1102)
 
     def tearDown(self):
         self.server.stop()
         self.server.destroy()
 
     def test_register_area(self):
         db1_type = ctypes.c_char * 1024
-        self.server.register_area(snap7.types.srvAreaDB, 3, db1_type())
+        self.server.register_area(srvAreaDB, 3, db1_type())
 
     def test_error(self):
-        for error in snap7.error.server_errors:
-            snap7.common.error_text(error, context="client")
+        for error in server_errors:
+            error_text(error, context="client")
 
     def test_event(self):
-        event = snap7.types.SrvEvent()
+        event = SrvEvent()
         self.server.event_text(event)
 
     def test_get_status(self):
         server, cpu, num_clients = self.server.get_status()
 
     def test_get_mask(self):
-        self.server.get_mask(snap7.types.mkEvent)
-        self.server.get_mask(snap7.types.mkLog)
+        self.server.get_mask(mkEvent)
+        self.server.get_mask(mkLog)
         # invalid kind
         self.assertRaises(Exception, self.server.get_mask, 3)
 
     def test_lock_area(self):
         from threading import Thread
-        area_code = snap7.types.srvAreaDB
+
+        area_code = srvAreaDB
         index = 1
         db1_type = ctypes.c_char * 1024
         # we need to register first
         self.server.register_area(area_code, index, db1_type())
         self.server.lock_area(code=area_code, index=index)
 
         def second_locker():
@@ -66,30 +69,30 @@
     def test_set_cpu_status(self):
         self.server.set_cpu_status(0)
         self.server.set_cpu_status(4)
         self.server.set_cpu_status(8)
         self.assertRaises(ValueError, self.server.set_cpu_status, -1)
 
     def test_set_mask(self):
-        self.server.set_mask(kind=snap7.types.mkEvent, mask=10)
+        self.server.set_mask(kind=mkEvent, mask=10)
 
     def test_unlock_area(self):
-        area_code = snap7.types.srvAreaDB
+        area_code = srvAreaDB
         index = 1
         db1_type = ctypes.c_char * 1024
 
         # we need to register first
         self.assertRaises(Exception, self.server.lock_area, area_code, index)
 
         self.server.register_area(area_code, index, db1_type())
         self.server.lock_area(area_code, index)
         self.server.unlock_area(area_code, index)
 
     def test_unregister_area(self):
-        area_code = snap7.types.srvAreaDB
+        area_code = srvAreaDB
         index = 1
         db1_type = ctypes.c_char * 1024
         self.server.register_area(area_code, index, db1_type())
         self.server.unregister_area(area_code, index)
 
     def test_events_callback(self):
         def event_call_back(event):
@@ -101,74 +104,75 @@
         def read_events_call_back(event):
             logging.debug(event)
 
         self.server.set_read_events_callback(read_events_call_back)
 
     def test_pick_event(self):
         event = self.server.pick_event()
-        self.assertEqual(type(event), snap7.types.SrvEvent)
+        self.assertEqual(type(event), SrvEvent)
         event = self.server.pick_event()
         self.assertFalse(event)
 
     def test_clear_events(self):
         self.server.clear_events()
         self.assertFalse(self.server.clear_events())
 
     def test_start_to(self):
-        self.server.start_to('0.0.0.0')
-        self.assertRaises(ValueError, self.server.start_to, 'bogus')
+        self.server.start_to("0.0.0.0")  # noqa: S104
+        self.assertRaises(ValueError, self.server.start_to, "bogus")
 
     def test_get_param(self):
         # check the defaults
-        self.assertEqual(self.server.get_param(snap7.types.LocalPort), 1102)
-        self.assertEqual(self.server.get_param(snap7.types.WorkInterval), 100)
-        self.assertEqual(self.server.get_param(snap7.types.MaxClients), 1024)
+        self.assertEqual(self.server.get_param(LocalPort), 1102)
+        self.assertEqual(self.server.get_param(WorkInterval), 100)
+        self.assertEqual(self.server.get_param(MaxClients), 1024)
 
         # invalid param for server
-        self.assertRaises(Exception, self.server.get_param,
-                          snap7.types.RemotePort)
+        self.assertRaises(Exception, self.server.get_param, RemotePort)
 
 
+@pytest.mark.server
 class TestServerBeforeStart(unittest.TestCase):
     """
     Tests for server before it is started
     """
 
     def setUp(self):
-        self.server = snap7.server.Server()
+        self.server = Server()
 
     def test_set_param(self):
-        self.server.set_param(snap7.types.LocalPort, 1102)
+        self.server.set_param(LocalPort, 1102)
 
 
+@pytest.mark.server
 class TestLibraryIntegration(unittest.TestCase):
     def setUp(self):
         # replace the function load_library with a mock
-        self.loadlib_patch = mock.patch('snap7.server.load_library')
+        self.loadlib_patch = mock.patch("snap7.server.load_library")
         self.loadlib_func = self.loadlib_patch.start()
 
         # have load_library return another mock
         self.mocklib = mock.MagicMock()
         self.loadlib_func.return_value = self.mocklib
 
         # have the Srv_Create of the mock return None
         self.mocklib.Srv_Create.return_value = None
 
     def tearDown(self):
         # restore load_library
         self.loadlib_patch.stop()
 
     def test_create(self):
-        snap7.server.Server(log=False)
+        Server(log=False)
         self.mocklib.Srv_Create.assert_called_once()
 
     def test_gc(self):
-        server = snap7.server.Server(log=False)
+        server = Server(log=False)
         del server
         self.mocklib.Srv_Destroy.assert_called_once()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import logging
 
     logging.basicConfig()
     unittest.main()
```

### Comparing `python-snap7-1.3/test/test_util.py` & `python_snap7-1.4/tests/test_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import datetime
-import re
+import pytest
 import unittest
 import struct
 
-from snap7 import util, types
+from snap7.util.db import DB_Row, DB
+from snap7.util.getters import get_byte, get_time, get_fstring, get_int
+from snap7.util.setters import set_byte, set_time, set_fstring, set_int
+from snap7 import types
 
 test_spec = """
 
 4	    ID	         INT
 6	    NAME	 STRING[4]
 
 12.0	testbool1    BOOL
@@ -73,495 +76,533 @@
     80      testDate    DATE
 82      testTod     TOD
     86      testDtl     DTL
             98      testFstring FSTRING[8]
 """
 
 
-_bytearray = bytearray([
-    0, 0,  # test int
-    4, 4, ord('t'), ord('e'), ord('s'), ord('t'),  # test string
-    128 * 0 + 64 * 0 + 32 * 0 + 16 * 0
-    + 8 * 1 + 4 * 1 + 2 * 1 + 1 * 1,                 # test bools
-    68, 78, 211, 51,                               # test real
-    255, 255, 255, 255,                            # test dword
-    0, 0,                                          # test int 2
-    128, 0, 0, 0,                                  # test dint
-    255, 255,                                      # test word
-    0, 16,                                         # test s5time, 0 is the time base,
-                                                   # 16 is value, those two integers should be declared together
-    32, 7, 18, 23, 50, 2, 133, 65,                 # these 8 values build the date and time 12 byte total
-                                                   # data typ together, for details under this link
-                                                   # https://support.industry.siemens.com/cs/document/36479/date_and_time-format-bei-s7-?dti=0&lc=de-DE
-    254, 254, 254, 254, 254, 127,                  # test small int
-    128,                                           # test set byte
-    143, 255, 255, 255,                            # test time
-    254,                                           # test byte              0xFE
-    48, 57,                                        # test uint              12345
-    7, 91, 205, 21,                                # test udint             123456789
-    65, 157, 111, 52, 84, 126, 107, 117,           # test lreal             123456789.123456789
-    65,                                            # test char              A
-    3, 169,                                        # test wchar             Ω
-    0, 4, 0, 4, 3, 169, 0, ord('s'), 0, ord('t'), 0, 196,  # test wstring   Ω s t Ä
-    45, 235,                                       # test date              09.03.2022
-    2, 179, 41, 128,                               # test tod               12:34:56
-    7, 230, 3, 9, 4, 12, 34, 45, 0, 0, 0, 0,       # test dtl               09.03.2022 12:34:56
-    116, 101, 115, 116, 32, 32, 32, 32             # test fstring           'test    '
-])
+_bytearray = bytearray(
+    [
+        0,
+        0,  # test int
+        4,
+        4,
+        ord("t"),
+        ord("e"),
+        ord("s"),
+        ord("t"),  # test string
+        128 * 0 + 64 * 0 + 32 * 0 + 16 * 0 + 8 * 1 + 4 * 1 + 2 * 1 + 1 * 1,  # test bools
+        68,
+        78,
+        211,
+        51,  # test real
+        255,
+        255,
+        255,
+        255,  # test dword
+        0,
+        0,  # test int 2
+        128,
+        0,
+        0,
+        0,  # test dint
+        255,
+        255,  # test word
+        0,
+        16,  # test s5time, 0 is the time base,
+        # 16 is value, those two integers should be declared together
+        32,
+        7,
+        18,
+        23,
+        50,
+        2,
+        133,
+        65,  # these 8 values build the date and time 12 byte total
+        # data typ together, for details under this link
+        # https://support.industry.siemens.com/cs/document/36479/date_and_time-format-bei-s7-?dti=0&lc=de-DE
+        254,
+        254,
+        254,
+        254,
+        254,
+        127,  # test small int
+        128,  # test set byte
+        143,
+        255,
+        255,
+        255,  # test time
+        254,  # test byte              0xFE
+        48,
+        57,  # test uint              12345
+        7,
+        91,
+        205,
+        21,  # test udint             123456789
+        65,
+        157,
+        111,
+        52,
+        84,
+        126,
+        107,
+        117,  # test lreal             123456789.123456789
+        65,  # test char              A
+        3,
+        169,  # test wchar             Ω
+        0,
+        4,
+        0,
+        4,
+        3,
+        169,
+        0,
+        ord("s"),
+        0,
+        ord("t"),
+        0,
+        196,  # test wstring   Ω s t Ä
+        45,
+        235,  # test date              09.03.2022
+        2,
+        179,
+        41,
+        128,  # test tod               12:34:56
+        7,
+        230,
+        3,
+        9,
+        4,
+        12,
+        34,
+        45,
+        0,
+        0,
+        0,
+        0,  # test dtl               09.03.2022 12:34:56
+        116,
+        101,
+        115,
+        116,
+        32,
+        32,
+        32,
+        32,  # test fstring           'test    '
+    ]
+)
 
 _new_bytearray = bytearray(100)
-_new_bytearray[41:41 + 1] = struct.pack("B", 128)       # byte_index=41, value=128, bytes=1
-_new_bytearray[42:42 + 1] = struct.pack("B", 255)       # byte_index=41, value=255, bytes=1
-_new_bytearray[43:43 + 4] = struct.pack("I", 286331153)  # byte_index=43, value=286331153(T#3D_7H_32M_11S_153MS), bytes=4
+_new_bytearray[41 : 41 + 1] = struct.pack("B", 128)  # byte_index=41, value=128, bytes=1
+_new_bytearray[42 : 42 + 1] = struct.pack("B", 255)  # byte_index=41, value=255, bytes=1
+_new_bytearray[43 : 43 + 4] = struct.pack("I", 286331153)  # byte_index=43, value=286331153(T#3D_7H_32M_11S_153MS), bytes=4
 
 
+@pytest.mark.util
 class TestS7util(unittest.TestCase):
-
     def test_get_byte_new(self):
         test_array = bytearray(_new_bytearray)
-        byte_ = util.get_byte(test_array, 41)
+        byte_ = get_byte(test_array, 41)
         self.assertEqual(byte_, 128)
-        byte_ = util.get_byte(test_array, 42)
+        byte_ = get_byte(test_array, 42)
         self.assertEqual(byte_, 255)
 
     def test_set_byte_new(self):
         test_array = bytearray(_new_bytearray)
-        util.set_byte(test_array, 41, 127)
-        byte_ = util.get_byte(test_array, 41)
+        set_byte(test_array, 41, 127)
+        byte_ = get_byte(test_array, 41)
         self.assertEqual(byte_, 127)
 
     def test_get_byte(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        value = row.get_value(50, 'BYTE')  # get value
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        value = row.get_value(50, "BYTE")  # get value
         self.assertEqual(value, 254)
 
     def test_set_byte(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['testByte'] = 255
-        self.assertEqual(row['testByte'], 255)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["testByte"] = 255
+        self.assertEqual(row["testByte"], 255)
+
+    def test_set_lreal(self):
+        test_array = bytearray(_bytearray)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["testLreal"] = 123.123
+        self.assertEqual(row["testLreal"], 123.123)
 
     def test_get_s5time(self):
         """
         S5TIME extraction from bytearray
         """
         test_array = bytearray(_bytearray)
 
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
 
-        self.assertEqual(row['testS5time'], '0:00:00.100000')
+        self.assertEqual(row["testS5time"], "0:00:00.100000")
 
     def test_get_dt(self):
         """
         DATE_AND_TIME extraction from bytearray
         """
         test_array = bytearray(_bytearray)
 
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
 
-        self.assertEqual(row['testdateandtime'], '2020-07-12T17:32:02.854000')
+        self.assertEqual(row["testdateandtime"], "2020-07-12T17:32:02.854000")
 
     def test_get_time(self):
         test_values = [
-            (0, '0:0:0:0.0'),
-            (1, '0:0:0:0.1'),  # T#1MS
-            (1000, '0:0:0:1.0'),  # T#1S
-            (60000, '0:0:1:0.0'),  # T#1M
-            (3600000, '0:1:0:0.0'),  # T#1H
-            (86400000, '1:0:0:0.0'),  # T#1D
-            (2147483647, '24:20:31:23.647'),  # max range
-            (-0, '0:0:0:0.0'),
-            (-1, '-0:0:0:0.1'),  # T#-1MS
-            (-1000, '-0:0:0:1.0'),  # T#-1S
-            (-60000, '-0:0:1:0.0'),  # T#-1M
-            (-3600000, '-0:1:0:0.0'),  # T#-1H
-            (-86400000, '-1:0:0:0.0'),  # T#-1D
-            (-2147483647, '-24:20:31:23.647'),  # min range
+            (0, "0:0:0:0.0"),
+            (1, "0:0:0:0.1"),  # T#1MS
+            (1000, "0:0:0:1.0"),  # T#1S
+            (60000, "0:0:1:0.0"),  # T#1M
+            (3600000, "0:1:0:0.0"),  # T#1H
+            (86400000, "1:0:0:0.0"),  # T#1D
+            (2147483647, "24:20:31:23.647"),  # max range
+            (-0, "0:0:0:0.0"),
+            (-1, "-0:0:0:0.1"),  # T#-1MS
+            (-1000, "-0:0:0:1.0"),  # T#-1S
+            (-60000, "-0:0:1:0.0"),  # T#-1M
+            (-3600000, "-0:1:0:0.0"),  # T#-1H
+            (-86400000, "-1:0:0:0.0"),  # T#-1D
+            (-2147483647, "-24:20:31:23.647"),  # min range
         ]
 
         data = bytearray(4)
         for value_to_test, expected_value in test_values:
             data[:] = struct.pack(">i", value_to_test)
-            self.assertEqual(util.get_time(data, 0), expected_value)
+            self.assertEqual(get_time(data, 0), expected_value)
 
     def test_set_time(self):
         test_array = bytearray(_new_bytearray)
 
         with self.assertRaises(ValueError):
-            util.set_time(test_array, 43, '-24:25:30:23:193')
+            set_time(test_array, 43, "-24:25:30:23:193")
         with self.assertRaises(ValueError):
-            util.set_time(test_array, 43, '-24:24:32:11.648')
+            set_time(test_array, 43, "-24:24:32:11.648")
         with self.assertRaises(ValueError):
-            util.set_time(test_array, 43, '-25:23:32:11.648')
+            set_time(test_array, 43, "-25:23:32:11.648")
         with self.assertRaises(ValueError):
-            util.set_time(test_array, 43, '24:24:30:23.620')
+            set_time(test_array, 43, "24:24:30:23.620")
 
-        util.set_time(test_array, 43, '24:20:31:23.647')
-        byte_ = util.get_time(test_array, 43)
-        self.assertEqual(byte_, '24:20:31:23.647')
-
-        util.set_time(test_array, 43, '-24:20:31:23.648')
-        byte_ = util.get_time(test_array, 43)
-        self.assertEqual(byte_, '-24:20:31:23.648')
-
-        util.set_time(test_array, 43, '3:7:32:11.153')
-        byte_ = util.get_time(test_array, 43)
-        self.assertEqual(byte_, '3:7:32:11.153')
+        set_time(test_array, 43, "24:20:31:23.647")
+        byte_ = get_time(test_array, 43)
+        self.assertEqual(byte_, "24:20:31:23.647")
+
+        set_time(test_array, 43, "-24:20:31:23.648")
+        byte_ = get_time(test_array, 43)
+        self.assertEqual(byte_, "-24:20:31:23.648")
+
+        set_time(test_array, 43, "3:7:32:11.153")
+        byte_ = get_time(test_array, 43)
+        self.assertEqual(byte_, "3:7:32:11.153")
 
     def test_get_string(self):
         """
         Text extraction from string from bytearray
         """
         test_array = bytearray(_bytearray)
 
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        self.assertEqual(row['NAME'], 'test')
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        self.assertEqual(row["NAME"], "test")
 
     def test_write_string(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['NAME'] = 'abc'
-        self.assertEqual(row['NAME'], 'abc')
-        row['NAME'] = ''
-        self.assertEqual(row['NAME'], '')
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["NAME"] = "abc"
+        self.assertEqual(row["NAME"], "abc")
+        row["NAME"] = ""
+        self.assertEqual(row["NAME"], "")
         try:
-            row['NAME'] = 'waaaaytoobig'
+            row["NAME"] = "waaaaytoobig"
         except ValueError:
             pass
         # value should still be empty
-        self.assertEqual(row['NAME'], '')
+        self.assertEqual(row["NAME"], "")
         try:
-            row['NAME'] = 'TrÖt'
+            row["NAME"] = "TrÖt"
         except ValueError:
             pass
 
     def test_get_fstring(self):
         data = [ord(letter) for letter in "hello world    "]
-        self.assertEqual(util.get_fstring(data, 0, 15), 'hello world')
-        self.assertEqual(util.get_fstring(data, 0, 15, remove_padding=False), 'hello world    ')
+        self.assertEqual(get_fstring(data, 0, 15), "hello world")
+        self.assertEqual(get_fstring(data, 0, 15, remove_padding=False), "hello world    ")
 
     def test_get_fstring_name(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        value = row['testFstring']
-        self.assertEqual(value, 'test')
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        value = row["testFstring"]
+        self.assertEqual(value, "test")
 
     def test_get_fstring_index(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        value = row.get_value(98, 'FSTRING[8]')  # get value
-        self.assertEqual(value, 'test')
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        value = row.get_value(98, "FSTRING[8]")  # get value
+        self.assertEqual(value, "test")
 
     def test_set_fstring(self):
         data = bytearray(20)
-        util.set_fstring(data, 0, "hello world", 15)
-        self.assertEqual(data, bytearray(b'hello world    \x00\x00\x00\x00\x00'))
+        set_fstring(data, 0, "hello world", 15)
+        self.assertEqual(data, bytearray(b"hello world    \x00\x00\x00\x00\x00"))
 
     def test_set_fstring_name(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['testFstring'] = 'TSET'
-        self.assertEqual(row['testFstring'], 'TSET')
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["testFstring"] = "TSET"
+        self.assertEqual(row["testFstring"], "TSET")
 
     def test_set_fstring_index(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row.set_value(98, 'FSTRING[8]', 'TSET')
-        self.assertEqual(row['testFstring'], 'TSET')
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row.set_value(98, "FSTRING[8]", "TSET")
+        self.assertEqual(row["testFstring"], "TSET")
 
     def test_get_int(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        x = row['ID']
-        y = row['testint2']
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        x = row["ID"]
+        y = row["testint2"]
         self.assertEqual(x, 0)
         self.assertEqual(y, 0)
 
     def test_set_int(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['ID'] = 259
-        self.assertEqual(row['ID'], 259)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["ID"] = 259
+        self.assertEqual(row["ID"], 259)
 
     def test_get_usint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        value = row.get_value(43, 'USINT')  # get value
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        value = row.get_value(43, "USINT")  # get value
         self.assertEqual(value, 254)
 
     def test_set_usint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['testusint0'] = 255
-        self.assertEqual(row['testusint0'], 255)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["testusint0"] = 255
+        self.assertEqual(row["testusint0"], 255)
 
     def test_get_sint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        value = row.get_value(44, 'SINT')  # get value
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        value = row.get_value(44, "SINT")  # get value
         self.assertEqual(value, 127)
 
     def test_set_sint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['testsint0'] = 127
-        self.assertEqual(row['testsint0'], 127)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["testsint0"] = 127
+        self.assertEqual(row["testsint0"], 127)
 
     def test_set_int_roundtrip(self):
         DB1 = (types.wordlen_to_ctypes[types.S7WLByte] * 4)()
 
-        for i in range(-(2 ** 15) + 1, (2 ** 15) - 1):
-            util.set_int(DB1, 0, i)
-            result = util.get_int(DB1, 0)
+        for i in range(-(2**15) + 1, (2**15) - 1):
+            set_int(DB1, 0, i)
+            result = get_int(DB1, 0)
             self.assertEqual(i, result)
 
     def test_get_int_values(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        for value in (
-                -32768,
-                -16385,
-                -256,
-                -128,
-                -127,
-                0,
-                127,
-                128,
-                255,
-                256,
-                16384,
-                32767):
-            row['ID'] = value
-            self.assertEqual(row['ID'], value)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        for value in (-32768, -16385, -256, -128, -127, 0, 127, 128, 255, 256, 16384, 32767):
+            row["ID"] = value
+            self.assertEqual(row["ID"], value)
 
     def test_get_bool(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        self.assertEqual(row['testbool1'], 1)
-        self.assertEqual(row['testbool8'], 0)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        self.assertEqual(row["testbool1"], 1)
+        self.assertEqual(row["testbool8"], 0)
 
     def test_set_bool(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['testbool8'] = True
-        row['testbool1'] = False
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["testbool8"] = True
+        row["testbool1"] = False
 
-        self.assertEqual(row['testbool8'], True)
-        self.assertEqual(row['testbool1'], False)
+        self.assertEqual(row["testbool8"], True)
+        self.assertEqual(row["testbool1"], False)
 
     def test_db_creation(self):
         test_array = bytearray(_bytearray * 10)
 
-        test_db = util.DB(1, test_array, test_spec,
-                          row_size=len(_bytearray),
-                          size=10,
-                          layout_offset=4,
-                          db_offset=0)
+        test_db = DB(1, test_array, test_spec, row_size=len(_bytearray), size=10, layout_offset=4, db_offset=0)
 
         self.assertEqual(len(test_db.index), 10)
 
         for i, row in test_db:
             # print row
-            self.assertEqual(row['testbool1'], 1)
-            self.assertEqual(row['testbool2'], 1)
-            self.assertEqual(row['testbool3'], 1)
-            self.assertEqual(row['testbool4'], 1)
-
-            self.assertEqual(row['testbool5'], 0)
-            self.assertEqual(row['testbool6'], 0)
-            self.assertEqual(row['testbool7'], 0)
-            self.assertEqual(row['testbool8'], 0)
-            self.assertEqual(row['NAME'], 'test')
+            self.assertEqual(row["testbool1"], 1)
+            self.assertEqual(row["testbool2"], 1)
+            self.assertEqual(row["testbool3"], 1)
+            self.assertEqual(row["testbool4"], 1)
+
+            self.assertEqual(row["testbool5"], 0)
+            self.assertEqual(row["testbool6"], 0)
+            self.assertEqual(row["testbool7"], 0)
+            self.assertEqual(row["testbool8"], 0)
+            self.assertEqual(row["NAME"], "test")
 
     def test_db_export(self):
         test_array = bytearray(_bytearray * 10)
-        test_db = util.DB(1, test_array, test_spec,
-                          row_size=len(_bytearray),
-                          size=10,
-                          layout_offset=4,
-                          db_offset=0)
+        test_db = DB(1, test_array, test_spec, row_size=len(_bytearray), size=10, layout_offset=4, db_offset=0)
 
         db_export = test_db.export()
         for i in db_export:
-            self.assertEqual(db_export[i]['testbool1'], 1)
-            self.assertEqual(db_export[i]['testbool2'], 1)
-            self.assertEqual(db_export[i]['testbool3'], 1)
-            self.assertEqual(db_export[i]['testbool4'], 1)
-
-            self.assertEqual(db_export[i]['testbool5'], 0)
-            self.assertEqual(db_export[i]['testbool6'], 0)
-            self.assertEqual(db_export[i]['testbool7'], 0)
-            self.assertEqual(db_export[i]['testbool8'], 0)
-            self.assertEqual(db_export[i]['NAME'], 'test')
+            self.assertEqual(db_export[i]["testbool1"], 1)
+            self.assertEqual(db_export[i]["testbool2"], 1)
+            self.assertEqual(db_export[i]["testbool3"], 1)
+            self.assertEqual(db_export[i]["testbool4"], 1)
+
+            self.assertEqual(db_export[i]["testbool5"], 0)
+            self.assertEqual(db_export[i]["testbool6"], 0)
+            self.assertEqual(db_export[i]["testbool7"], 0)
+            self.assertEqual(db_export[i]["testbool8"], 0)
+            self.assertEqual(db_export[i]["NAME"], "test")
 
     def test_get_real(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        self.assertTrue(0.01 > (row['testReal'] - 827.3) > -0.1)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        self.assertTrue(0.01 > (row["testReal"] - 827.3) > -0.1)
 
     def test_set_real(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        row['testReal'] = 1337.1337
-        self.assertTrue(0.01 > (row['testReal'] - 1337.1337) > -0.01)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        row["testReal"] = 1337.1337
+        self.assertTrue(0.01 > (row["testReal"] - 1337.1337) > -0.01)
 
     def test_set_dword(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
         # The range of numbers is 0 to 4294967295.
-        row['testDword'] = 9999999
-        self.assertEqual(row['testDword'], 9999999)
+        row["testDword"] = 9999999
+        self.assertEqual(row["testDword"], 9999999)
 
     def test_get_dword(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        self.assertEqual(row['testDword'], 4294967295)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        self.assertEqual(row["testDword"], 4294967295)
 
     def test_set_dint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
         # The range of numbers is -2147483648 to 2147483647 +
-        row.set_value(23, 'DINT', 2147483647)  # set value
-        self.assertEqual(row['testDint'], 2147483647)
+        row.set_value(23, "DINT", 2147483647)  # set value
+        self.assertEqual(row["testDint"], 2147483647)
 
     def test_get_dint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        value = row.get_value(23, 'DINT')  # get value
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        value = row.get_value(23, "DINT")  # get value
         self.assertEqual(value, -2147483648)
 
     def test_set_word(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
         # The range of numbers is 0 to 65535
-        row.set_value(27, 'WORD', 0)  # set value
-        self.assertEqual(row['testWord'], 0)
+        row.set_value(27, "WORD", 0)  # set value
+        self.assertEqual(row["testWord"], 0)
 
     def test_get_word(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
-        value = row.get_value(27, 'WORD')  # get value
+        row = DB_Row(test_array, test_spec, layout_offset=4)
+        value = row.get_value(27, "WORD")  # get value
         self.assertEqual(value, 65535)
 
     def test_export(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec, layout_offset=4)
+        row = DB_Row(test_array, test_spec, layout_offset=4)
         data = row.export()
-        self.assertIn('testDword', data)
-        self.assertIn('testbool1', data)
-        self.assertEqual(data['testbool5'], 0)
+        self.assertIn("testDword", data)
+        self.assertIn("testbool1", data)
+        self.assertEqual(data["testbool5"], 0)
 
     def test_indented_layout(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        x = row['ID']
-        y_single_space = row['testbool1']
-        y_multi_space = row['testbool2']
-        y_single_indent = row['testint2']
-        y_multi_indent = row['testbool8']
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        x = row["ID"]
+        y_single_space = row["testbool1"]
+        y_multi_space = row["testbool2"]
+        y_single_indent = row["testint2"]
+        y_multi_indent = row["testbool8"]
 
         with self.assertRaises(KeyError):
-            fail_single_space = row['testbool4']
+            fail_single_space = row["testbool4"]  # noqa: F841
         with self.assertRaises(KeyError):
-            fail_multiple_spaces = row['testbool5']
+            fail_multiple_spaces = row["testbool5"]  # noqa: F841
         with self.assertRaises(KeyError):
-            fail_single_indent = row['testbool6']
+            fail_single_indent = row["testbool6"]  # noqa: F841
         with self.assertRaises(KeyError):
-            fail_multiple_indent = row['testbool7']
+            fail_multiple_indent = row["testbool7"]  # noqa: F841
 
         self.assertEqual(x, 0)
         self.assertEqual(y_single_space, True)
         self.assertEqual(y_multi_space, True)
         self.assertEqual(y_single_indent, 0)
         self.assertEqual(y_multi_indent, 0)
 
     def test_get_uint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testUint']
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testUint"]
         self.assertEqual(val, 12345)
 
     def test_get_udint(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testUdint']
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testUdint"]
         self.assertEqual(val, 123456789)
 
     def test_get_lreal(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testLreal']
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testLreal"]
         self.assertEqual(val, 123456789.123456789)
 
     def test_get_char(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testChar']
-        self.assertEqual(val, 'A')
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testChar"]
+        self.assertEqual(val, "A")
 
     def test_get_wchar(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testWchar']
-        self.assertEqual(val, 'Ω')
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testWchar"]
+        self.assertEqual(val, "Ω")
 
     def test_get_wstring(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testWstring']
-        self.assertEqual(val, 'ΩstÄ')
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testWstring"]
+        self.assertEqual(val, "ΩstÄ")
 
     def test_get_date(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testDate']
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testDate"]
         self.assertEqual(val, datetime.date(day=9, month=3, year=2022))
 
     def test_get_tod(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testTod']
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testTod"]
         self.assertEqual(val, datetime.timedelta(hours=12, minutes=34, seconds=56))
 
     def test_get_dtl(self):
         test_array = bytearray(_bytearray)
-        row = util.DB_Row(test_array, test_spec_indented, layout_offset=4)
-        val = row['testDtl']
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        val = row["testDtl"]
         self.assertEqual(val, datetime.datetime(year=2022, month=3, day=9, hour=12, minute=34, second=45))
 
-
-def print_row(data):
-    """print a single db row in chr and str
-    """
-    index_line = ""
-    pri_line1 = ""
-    chr_line2 = ""
-    asci = re.compile('[a-zA-Z0-9 ]')
-
-    for i, xi in enumerate(data):
-        # index
-        if not i % 5:
-            diff = len(pri_line1) - len(index_line)
-            i = str(i)
-            index_line += diff * ' '
-            index_line += i
-            # i = i + (ws - len(i)) * ' ' + ','
-
-        # byte array line
-        str_v = str(xi)
-        pri_line1 += str(xi) + ','
-        # char line
-        c = chr(xi)
-        c = c if asci.match(c) else ' '
-        # align white space
-        w = len(str_v)
-        c = c + (w - 1) * ' ' + ','
-        chr_line2 += c
-
-    print(index_line)
-    print(pri_line1)
-    print(chr_line2)
+    def test_set_date(self):
+        test_array = bytearray(_bytearray)
+        row = DB_Row(test_array, test_spec_indented, layout_offset=4)
+        row["testDate"] = datetime.date(day=28, month=3, year=2024)
+        self.assertEqual(row["testDate"], datetime.date(day=28, month=3, year=2024))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

