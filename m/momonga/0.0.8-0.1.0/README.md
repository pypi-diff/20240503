# Comparing `tmp/momonga-0.0.8-py3-none-any.whl.zip` & `tmp/momonga-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15429 bytes, number of entries: 11
--rw-r--r--  2.0 unx      136 b- defN 24-Apr-30 02:44 momonga/__init__.py
--rw-r--r--  2.0 unx    15394 b- defN 24-May-01 02:16 momonga/momonga.py
--rw-r--r--  2.0 unx      959 b- defN 24-Apr-30 02:44 momonga/momonga_exception.py
--rw-r--r--  2.0 unx     2698 b- defN 24-Apr-30 02:44 momonga/momonga_response.py
--rw-r--r--  2.0 unx    11915 b- defN 24-Apr-30 02:44 momonga/momonga_session_manager.py
--rw-r--r--  2.0 unx     9392 b- defN 24-Apr-30 02:44 momonga/momonga_sk_wrapper.py
--rw-r--r--  2.0 unx     1061 b- defN 24-May-01 02:20 momonga-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    10353 b- defN 24-May-01 02:20 momonga-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 02:20 momonga-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-01 02:20 momonga-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      883 b- defN 24-May-01 02:20 momonga-0.0.8.dist-info/RECORD
-11 files, 52891 bytes uncompressed, 13943 bytes compressed:  73.6%
+Zip file size: 15761 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      135 b- defN 24-May-03 15:05 momonga/__init__.py
+-rw-r--r--  2.0 unx    15714 b- defN 24-May-03 19:10 momonga/momonga.py
+-rw-r--r--  2.0 unx      973 b- defN 24-May-03 02:36 momonga/momonga_exception.py
+-rw-r--r--  2.0 unx     2712 b- defN 24-May-03 19:01 momonga/momonga_response.py
+-rw-r--r--  2.0 unx    12539 b- defN 24-May-03 19:01 momonga/momonga_session_manager.py
+-rw-r--r--  2.0 unx    10110 b- defN 24-May-03 19:02 momonga/momonga_sk_wrapper.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10439 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      884 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/RECORD
+11 files, 54667 bytes uncompressed, 14275 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: momonga/momonga_session_manager.py
 Comment: 
 
 Filename: momonga/momonga_sk_wrapper.py
 Comment: 
 
-Filename: momonga-0.0.8.dist-info/LICENSE
+Filename: momonga-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: momonga-0.0.8.dist-info/METADATA
+Filename: momonga-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: momonga-0.0.8.dist-info/WHEEL
+Filename: momonga-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: momonga-0.0.8.dist-info/top_level.txt
+Filename: momonga-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: momonga-0.0.8.dist-info/RECORD
+Filename: momonga-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## momonga/__init__.py

```diff
@@ -2,8 +2,7 @@
     Momonga,
     logger,
     session_manager_logger,
     sk_wrapper_logger,
 )
 
 from .momonga_exception import *
-
```

## momonga/momonga.py

```diff
@@ -1,15 +1,16 @@
-
 import datetime
 import time
 import queue
 import logging
 
-from .momonga_exception import *
-from .momonga_response import *
+from .momonga_exception import (MomongaResponseNotExpected,
+                                MomongaResponseNotPossible,
+                                MomongaNeedToReopen)
+from .momonga_response import SkEventRxUdp
 from .momonga_session_manager import MomongaSessionManager
 from .momonga_session_manager import logger as session_manager_logger
 from .momonga_sk_wrapper import logger as sk_wrapper_logger
 
 
 try:
     from typing import Self
@@ -32,29 +33,24 @@
         self.recv_timeout = 12
         self.internal_xmit_interval = 5
         self.transaction_id = 0
         self.energy_coefficient = None
         self.energy_unit = None
 
         # the following value will be set a pyserial object.
-        self.session_manager = MomongaSessionManager(rbid,
-                                                 pwd,
-                                                 dev,
-                                                 baudrate,
-                                                 reset_dev,
-                                                )
+        self.session_manager = MomongaSessionManager(rbid, pwd, dev, baudrate, reset_dev)
 
-#    def __enter__(self) -> Self:
+    # def __enter__(self) -> Self:
     def __enter__(self):
         return self.open()
 
     def __exit__(self, type, value, traceback) -> None:
         self.close()
 
-#    def open(self) -> Self:
+    # def open(self) -> Self:
     def open(self):
         logger.info('Opening Momonga.')
         self.session_manager.open()
         time.sleep(self.internal_xmit_interval)
         logger.info('Momonga is open.')
         return self
 
@@ -66,46 +62,49 @@
         logger.info('Momonga is closed.')
 
     def __build_request_payload(self,
                                 tid: int,
                                 epc: int,
                                 edt: bytes = b'',
                                ) -> bytes:
-        ehd  = b'\x10\x81'     # echonet lite edata format 1
-        tid  = tid.to_bytes(4, 'big')[-2:]
-        seoj = b'\x05\xFF\x01' # controller class
-        deoj = b'\x02\x88\x01' # low-voltage smart electric energy meter class
-        opc  = b'\x01'
+        ehd = b'\x10\x81'  # echonet lite edata format 1
+        tid = tid.to_bytes(4, 'big')[-2:]
+        seoj = b'\x05\xFF\x01'  # controller class
+        deoj = b'\x02\x88\x01'  # low-voltage smart electric energy meter class
+        opc = b'\x01'
         if edt:
-            esv = b'\x61' # setc
+            esv = b'\x61'  # setc
         else:
-            esv = b'\x62' # get
-        epc  = epc.to_bytes(1, 'big')
+            esv = b'\x62'  # get
+        epc = epc.to_bytes(1, 'big')
         pdc = len(edt).to_bytes(1, 'big')
 
         return ehd + tid + seoj + deoj + esv + opc + epc + pdc + edt
 
     def __extract_response_payload(self,
                                    data: bytes,
                                    tid: int,
                                    epc: int,
-                                  ):
+                                  ) -> dict[str: bytes, str: int,
+                                            str: bytes, str: bytes,
+                                            str: int, str: int, str: int,
+                                            str: int, str: bytes | None]:
         ehd = data[0:2]
-        if  ehd != b'\x10\x81': # echonet lite edata format 1
+        if ehd != b'\x10\x81':  # echonet lite edata format 1
             raise MomongaResponseNotExpected('The data format is not ECHONET Lite EDATA format 1')
 
-        if int.from_bytes(data[2:4], 'big') != tid:
+        if data[2:4] != tid.to_bytes(4, 'big')[-2:]:
             raise MomongaResponseNotExpected('The transaction ID does not match.')
 
         seoj = data[4:7]
-        if seoj != b'\x02\x88\x01': # low-voltage smart electric energy meter class
+        if seoj != b'\x02\x88\x01':  # low-voltage smart electric energy meter class
             raise MomongaResponseNotExpected('The source is not a smart meter.')
 
         deoj = data[7:10]
-        if deoj != b'\x05\xFF\x01': # controller class
+        if deoj != b'\x05\xFF\x01':  # controller class
             raise MomongaResponseNotExpected('The destination is not a controller.')
 
         if data[12] != epc:
             raise MomongaResponseNotExpected('The property code does not match. EPC: %X' % epc)
 
         esv = data[10]
         if 0x50 <= esv <= 0x5F:
@@ -116,27 +115,25 @@
 
         pdc = data[13]
         if pdc == 0:
             edt = None
         else:
             edt = data[14:14+pdc]
 
-        return {'ehd': ehd, 'tid': tid, 'seoj': seoj, 'deoj': deoj, 'esv': esv,
-                'opc': opc, 'epc': epc, 'pdc': pdc, 'epc': epc, 'edt': edt}
+        return {'ehd': ehd, 'tid': tid, 'seoj': seoj, 'deoj': deoj,
+                'epc': epc, 'esv': esv, 'opc': opc, 'pdc': pdc, 'edt': edt}
 
     def __request(self,
                   epc: int,
                   edt: bytes = b'',
                  ) -> bytes:
         self.transaction_id += 1
-        tx_payload = self.__build_request_payload(self.transaction_id,
-                                                  epc,
-                                                  edt)
+        tx_payload = self.__build_request_payload(self.transaction_id, epc, edt)
         while not self.session_manager.recv_q.empty():
-            self.session_manager.recv_q.get() # drops stored data
+            self.session_manager.recv_q.get()  # drops stored data
 
         for _ in range(self.xmit_retry):
             self.session_manager.xmitter(tx_payload)
             while True:
                 try:
                     res = self.session_manager.recv_q.get(timeout=self.recv_timeout)
                 except queue.Empty:
@@ -146,15 +143,15 @@
                     param = res.split()[-1]
                     if param == '00':
                         logger.info('Successfully transmitted a packet for "%X" request.' % (epc))
                         continue
                     elif param == '01':
                         logger.warning('Retransmitting the packet for "%X" request.' % (epc))
                         time.sleep(self.internal_xmit_interval)
-                        break # to rexmit
+                        break  # to rexmit
                     elif param == '02':
                         logger.warning('Transmitting neighbor solicitation packets.' % (epc))
                         continue
                 elif res.startswith('EVENT 02'):
                     logger.info('Received a neighbor advertisement packet.' % (epc))
                     continue
                 elif res.startswith('ERXUDP'):
@@ -163,17 +160,15 @@
                         continue
                     elif udp_pkt.side != 0:
                         continue
                     elif udp_pkt.src_addr != self.session_manager.smart_meter_addr:
                         continue
 
                     try:
-                        rx_payload = self.__extract_response_payload(udp_pkt.data,
-                                                                     self.transaction_id,
-                                                                     epc)
+                        rx_payload = self.__extract_response_payload(udp_pkt.data, self.transaction_id, epc)
                     except MomongaResponseNotExpected:
                         continue
 
                     logger.info('Successfully received a packet for "%X" response.' % (epc))
                     return rx_payload
 
         logger.error('Gave up to obtain a response for "%X" request. Close Momonga and open it again.' % (epc))
@@ -186,20 +181,20 @@
                 time.sleep(self.internal_xmit_interval)
             except MomongaResponseNotPossible:
                 self.energy_coefficient = 1
         if self.energy_unit is None:
             self.energy_unit = self.get_unit_for_cumulative_energy()
             time.sleep(self.internal_xmit_interval)
 
-    def get_operation_status(self) -> int:
+    def get_operation_status(self) -> bool | None:
         res = self.__request(0x80)
         status = int.from_bytes(res.get('edt'), 'big')
-        if status == 0x30:   # turned on
+        if status == 0x30:  # turned on
             status = True
-        elif status == 0x31: # turned off
+        elif status == 0x31:  # turned off
             status = False
         else:
             status = None
         return status
 
     def get_coefficient_for_cumulative_energy(self) -> int:
         res = self.__request(0xD3)
@@ -209,125 +204,125 @@
     def get_number_of_effective_digits_for_cumulative_energy(self) -> int:
         res = self.__request(0xD7)
         digits = int.from_bytes(res.get('edt'), 'big')
         return digits
 
     def get_measured_cumulative_energy(self,
                                        reverse: bool = False,
-                                      ) -> int: 
+                                      ) -> int | float:
         self.__prepare_to_get_cumulative_energy()
 
         if reverse is False:
             epc = 0xE0
         else:
             epc = 0xE3
 
         res = self.__request(epc)
         cumulative_energy = int.from_bytes(res.get('edt'), 'big')
         cumulative_energy *= self.energy_coefficient
-        cumulative_energy *= self.energy_unit 
+        cumulative_energy *= self.energy_unit
         return cumulative_energy
 
     def get_unit_for_cumulative_energy(self) -> int | float:
         res = self.__request(0xE1)
         unit_index = int.from_bytes(res.get('edt'), 'big')
-        unit_map = {0x00:1,
-                    0x01:0.1,
-                    0x02:0.01,
-                    0x03:0.001,
-                    0x04:0.0001,
-                    0x0A:10,
-                    0x0B:100,
-                    0x0C:1000,
-                    0x0D:10000,
-                   }
+        unit_map = {0x00: 1,
+                    0x01: 0.1,
+                    0x02: 0.01,
+                    0x03: 0.001,
+                    0x04: 0.0001,
+                    0x0A: 10,
+                    0x0B: 100,
+                    0x0C: 1000,
+                    0x0D: 10000}
         return unit_map.get(unit_index)
 
     def get_historical_cumulative_energy_1(self,
                                            day: int = 0,
                                            reverse: bool = False,
-                                          ) -> list:
+                                           ) -> list[dict[str: datetime.datetime,
+                                                          str: int | float | None]]:
         self.__prepare_to_get_cumulative_energy()
         self.set_day_for_historical_data_1(day)
 
         if reverse is False:
             epc = 0xE2
         else:
             epc = 0xE4
 
         res = self.__request(epc)
         edt = res.get('edt')
         day = int.from_bytes(edt[0:2], 'big')
-        timestamp = datetime.datetime.combine(datetime.date.today(),
-                                              datetime.datetime.min.time())
+        timestamp = datetime.datetime.combine(datetime.date.today(), datetime.datetime.min.time())
         timestamp -= datetime.timedelta(days=day)
 
         energy_data_points = edt[2:]
         historical_cumulative_energy = []
         for i in range(48):
             j = i * 4
             cumulative_energy = int.from_bytes(energy_data_points[j:j+4], 'big')
             if cumulative_energy == 0xFFFFFFFE:
                 cumulative_energy = None
             else:
                 cumulative_energy *= self.energy_coefficient
-                cumulative_energy *= self.energy_unit 
+                cumulative_energy *= self.energy_unit
             historical_cumulative_energy.append({'timestamp': timestamp, 'cumulative energy': cumulative_energy})
             timestamp += datetime.timedelta(minutes=30)
         return historical_cumulative_energy
- 
+
     def set_day_for_historical_data_1(self,
                                       day: int = 0,
                                      ) -> None:
         self.__request(0xE5, day.to_bytes(1, 'big'))
 
     def get_day_for_historical_data_1(self) -> int:
         res = self.__request(0xE5)
         day = int.from_bytes(res.get('edt'), 'big')
         return day
- 
+
     def get_instantaneous_power(self) -> float:
         res = self.__request(0xE7)
         power = int.from_bytes(res.get('edt'), 'big', signed=True)
         return power
 
-    def get_instantaneous_current(self) -> dict:
+    def get_instantaneous_current(self) -> dict[str: float, str: float]:
         res = self.__request(0xE8)
         edt = res.get('edt')
         r_phase_current = int.from_bytes(edt[0:2], 'big', signed=True)
         t_phase_current = int.from_bytes(edt[2:4], 'big', signed=True)
-        r_phase_current *= 0.1 # to Ampere
-        t_phase_current *= 0.1 # to Ampere
-        return {'r phase current': r_phase_current,
-                't phase current': t_phase_current}
+        r_phase_current *= 0.1  # to Ampere
+        t_phase_current *= 0.1  # to Ampere
+        return {'r phase current': r_phase_current, 't phase current': t_phase_current}
 
     def get_cumulative_energy_measured_at_fixed_time(self,
                                                      reverse: bool = False,
-                                                    ) -> dict:
+                                                    ) -> dict[str: datetime.datetime,
+                                                              str: int | float]:
         self.__prepare_to_get_cumulative_energy()
 
         if reverse is False:
             epc = 0xEA
         else:
             epc = 0xEB
 
         res = self.__request(epc)
         edt = res.get('edt')
         timestamp = datetime.datetime(int.from_bytes(edt[0:2], 'big'),
                                       edt[2], edt[3], edt[4], edt[5], edt[6])
         cumulative_energy = int.from_bytes(edt[7:], 'big')
         cumulative_energy *= self.energy_coefficient
-        cumulative_energy *= self.energy_unit 
-        return {'timestamp': timestamp,
-                'cumulative_energy': cumulative_energy}
+        cumulative_energy *= self.energy_unit
+        return {'timestamp': timestamp, 'cumulative_energy': cumulative_energy}
 
     def get_historical_cumulative_energy_2(self,
                                            timestamp: datetime.datetime = None,
                                            num_of_data_points: int = 12,
-                                          ) -> list:
+                                          ) -> list[dict[str: datetime.datetime,
+                                                         str: dict[str: int | float | None,
+                                                                   str: int | float | None]]]:
         if timestamp is None:
             timestamp = datetime.datetime.now()
 
         self.__prepare_to_get_cumulative_energy()
         self.set_time_for_historical_data_2(timestamp, num_of_data_points)
 
         res = self.__request(0xEC)
@@ -341,30 +336,30 @@
         for i in range(num_of_data_points):
             j = i * 8
             normal_direction_energy = int.from_bytes(energy_data_points[j:j+4], 'big')
             if normal_direction_energy == 0xFFFFFFFE:
                 normal_direction_energy = None
             else:
                 normal_direction_energy *= self.energy_coefficient
-                normal_direction_energy *= self.energy_unit 
+                normal_direction_energy *= self.energy_unit
 
             reverse_direction_energy = int.from_bytes(energy_data_points[j+4:j+8], 'big')
             if reverse_direction_energy == 0xFFFFFFFE:
                 reverse_direction_energy = None
             else:
                 reverse_direction_energy *= self.energy_coefficient
-                reverse_direction_energy *= self.energy_unit 
+                reverse_direction_energy *= self.energy_unit
 
             historical_cumulative_energy.append(
                 {'timestamp': timestamp,
                  'cumulative energy': {'normal direction': normal_direction_energy,
                                        'reverse direction': reverse_direction_energy}})
             timestamp -= datetime.timedelta(minutes=30)
         return historical_cumulative_energy
- 
+
     def set_time_for_historical_data_2(self,
                                        timestamp: datetime.datetime,
                                        num_of_data_points: int = 12,
                                       ) -> None:
         year = timestamp.year.to_bytes(2, 'big')
         month = timestamp.month.to_bytes(1, 'big')
         day = timestamp.day.to_bytes(1, 'big')
@@ -375,15 +370,15 @@
         else:
             minute = 30
 
         minute = minute.to_bytes(1, 'big')
         num_of_data_points = num_of_data_points.to_bytes(1, 'big')
         self.__request(0xED, year + month + day + hour + minute + num_of_data_points)
 
-    def get_time_for_historical_data_2(self) -> dict:
+    def get_time_for_historical_data_2(self) -> dict[str: datetime.datetime | None, str: int]:
         res = self.__request(0xED)
         edt = res.get('edt')
         year = int.from_bytes(edt[0:2], 'big')
         if year == 0xFFFF:
             timestamp = None
         else:
             timestamp = datetime.datetime(year, edt[2], edt[3], edt[4], edt[5])
```

## momonga/momonga_exception.py

```diff
@@ -1,44 +1,58 @@
 class MomongaError(Exception):
     pass
 
+
 class MomongaSkCommandExecutionFailure(MomongaError):
     pass
 
+
 class MomongaSkCommandUnknownError(MomongaSkCommandExecutionFailure):
     pass
 
+
 class MomongaSkCommandUnsupported(MomongaSkCommandExecutionFailure):
     pass
 
+
 class MomongaSkCommandInvalidArgument(MomongaSkCommandExecutionFailure):
     pass
 
+
 class MomongaSkCommandInvalidSyntax(MomongaSkCommandExecutionFailure):
     pass
 
+
 class MomongaSkCommandSerialInputError(MomongaSkCommandExecutionFailure):
     pass
 
+
 class MomongaSkCommandFailedToExecute(MomongaSkCommandExecutionFailure):
     pass
 
+
 class MomongaSkScanFailure(MomongaError):
     pass
 
+
 class MomongaSkJoinFailure(MomongaError):
     pass
 
+
 class MomongaTimeoutError(TimeoutError):
     pass
 
+
 class MomongaKeyError(KeyError):
     pass
 
+
 class MomongaNeedToReopen(MomongaError):
     pass
 
+
 class MomongaResponseNotExpected(MomongaError):
     pass
 
+
 class MomongaResponseNotPossible(MomongaError):
     pass
```

## momonga/momonga_response.py

```diff
@@ -1,9 +1,8 @@
-
-from .momonga_exception import *
+from .momonga_exception import MomongaKeyError
 
 
 class MomongaSkResponseBase:
     def __init__(self, res):
         self.raw_response = res
         self.decode()
 
@@ -12,14 +11,15 @@
 
     def extract(self, key):
         for elm in reversed(self.raw_response):
             if key in elm:
                 return elm
         raise MomongaKeyError(key)
 
+
 class SkVerResponse(MomongaSkResponseBase):
     def decode(self):
         res_list = self.extract('EVER').split()
         self.stack_ver = res_list[1]
 
 
 class SkAppVerResponse(MomongaSkResponseBase):
```

## momonga/momonga_session_manager.py

```diff
@@ -1,14 +1,17 @@
-
 import logging
 import threading
 import queue
 import time
 
-from .momonga_exception import *
+from .momonga_exception import (MomongaSkScanFailure,
+                                MomongaSkJoinFailure,
+                                MomongaNeedToReopen,
+                                MomongaSkCommandExecutionFailure,
+)
 from .momonga_sk_wrapper import MomongaSkWrapper
 from .momonga_sk_wrapper import logger as sk_wrapper_logger
 
 
 try:
     from typing import Self
 except ImportError:
@@ -49,22 +52,22 @@
         self.xmit_lock = threading.Lock()
         self.rejoin_lock = threading.Lock()
 
         self.pkt_sbsc_q = queue.Queue()
         self.recv_q = queue.Queue()
         self.xmit_q = queue.Queue()
 
-#    def __enter__(self) -> Self:
+    #def __enter__(self) -> Self:
     def __enter__(self):
         return self.open()
 
     def __exit__(self, type, value, traceback) -> None:
         self.close()
 
-#    def open(self) -> Self:
+    #def open(self) -> Self:
     def open(self):
         logger.info('Opening a Momonga session...')
         try:
             self.skw.open()
 
             if self.reset_dev is True:
                 # to reset the specified wi-sun module.
@@ -82,15 +85,15 @@
             # to set a pasword.
             self.skw.sksetpwd(self.pwd)
             logger.info('The Route-B ID and the password were registered.')
             try:
                 logger.info('Scanning PAN channels...')
                 scan_res = self.skw.skscan()
                 logger.info('A PAN was found.')
-            except MomongaSkScanFailure as e:
+            except MomongaSkScanFailure:
                 logger.error('Gave up to find a PAN. Check the device location and Route-B ID. Then try again.')
                 raise MomongaSkScanFailure('Gave up to find a PAN. Check the device location and Route-B ID. Then try again.')
             self.smart_meter_mac = scan_res.mac_addr
             self.channel = scan_res.channel
             self.pan_id = scan_res.pan_id
             # converting mac addr to ip6 addr.
             self.smart_meter_addr = self.skw.skll64(scan_res.mac_addr).ip6_addr
@@ -146,15 +149,15 @@
             finally:
                 self.rejoin_lock.release()
         else:
             self.rejoin_lock.release()
 
         if self.receiver_th is not None:
             if self.receiver_th.is_alive():
-                self.pkt_sbsc_q.put('__CLOSE__') # to close the receiver thread.
+                self.pkt_sbsc_q.put('__CLOSE__')  # to close the receiver thread.
                 self.receiver_th.join()
             self.receiver_th = None
 
         if self.skw.subscribers.get('pkt_sbsc_q') is not None:
             self.skw.subscribers.pop('pkt_sbsc_q')
 
         self.unrestrict_to_xmit(force=True)
@@ -184,16 +187,16 @@
                     logger.warning('Could not rejoin the PAN.')
                     self.rejoin_lock.acquire()
                     if self.session_established is True:
                         self.session_established = False
                         try:
                             self.skw.skjoin(self.smart_meter_addr)
                         except MomongaSkJoinFailure as e:
-                            logger.error('%s Close Momonga and open it again.' % e)
-                            raise MomongaNeedToReopen('%s Close Momonga and open it again.' % e)
+                            logger.error('%s Close Momonga and open it again.' % (e))
+                            raise MomongaNeedToReopen('%s Close Momonga and open it again.' % (e))
                         finally:
                             self.rejoin_lock.release()
                     else:
                         self.rejoin_lock.release()
                 elif res.startswith('EVENT 25'):
                     logger.debug('Successfully rejoined the PAN.')
                     self.session_established = True
@@ -203,57 +206,59 @@
                     self.restrict_to_xmit()
                 elif res.startswith('EVENT 33'):
                     logger.debug('The transmission rate limit has been released.')
                     self.unrestrict_to_xmit()
                 elif res.startswith('EVENT 27'):
                     self.restrict_to_xmit()
                     logger.debug('The PANA session has been closed successfully.')
-                elif res.startswith('EVENT 28'): # there was no session to close.
+                elif res.startswith('EVENT 28'):  # there was no session to close.
                     self.restrict_to_xmit()
                     logger.warning('There was no PANA session to close.')
-                elif res.startswith('EVENT 21') or res.startswith('EVENT 02'):
-                    self.recv_q.put(res)
-                elif res.startswith('ERXUDP'):
+                elif self.is_restricted_to_xmit() is False and (res.startswith("EVENT 21") or
+                                                                res.startswith("EVENT 02") or
+                                                                res.startswith("ERXUDP")):
                     self.recv_q.put(res)
         except Exception as e:
             logger.error('An exception was raised from the receiver thread. %s: %s' % (type(e).__name__, e))
             self.receiver_exception = e
 
         logger.debug('The packet receiver has been stopped.')
 
     def xmitter(self,
                 data: bytes,
                ) -> None:
+        retry_to_xmit = 3
+        retry_to_acquire_xmit_lock = 60
         xmitted = False
-        for _ in range(3):
+        for _ in range(retry_to_xmit):
             logger.debug('Trying to acquire "xmit_lock".')
-            for _ in range(30):
-                unlocked =  self.xmit_lock.acquire(timeout=120) 
-                if unlocked is False: 
-                    logger.warning('Could not acquire "xmit_lock".')
+            for r in range(retry_to_acquire_xmit_lock):
+                unlocked = self.xmit_lock.acquire(timeout=60)
+                if unlocked is False:
+                    logger.warning('Could not acquire "xmit_lock". (%d/%d)' % (r + 1, retry_to_acquire_xmit_lock))
                     if self.receiver_exception is not None:
                         logger.error('Got an exception from the receiver thread. %s: %s' % (type(self.receiver_exception).__name__, self.receiver_exception))
                         raise MomongaNeedToReopen('Got an exception from the receiver thread. %s: %s' % (type(self.receiver_exception).__name__, self.receiver_exception))
                 else:
                     break
 
-            if unlocked is False: 
+            if unlocked is False:
                 logger.error('Transmission rights could not be acquired. Close Momonga and open it again.')
                 raise MomongaNeedToReopen('Transmission rights could not be acquired. Close Momonga and open it again.')
             else:
                 logger.debug('Acquired "xmit_lock".')
 
             assert self.session_established is not False, 'Tried to transmit a packet, but no PANA session was established.'
 
             try:
                 self.skw.sksendto(self.smart_meter_addr, data)
                 xmitted = True
                 break
             except MomongaSkCommandExecutionFailure as e:
-                logger.warning('Failed to transmit a packet: %s' % e)
+                logger.warning('Failed to transmit a packet: %s' % (e))
             except Exception as e:
                 logger.warning('An error occurred to transmit a packet. %s: %s' % (type(e).__name__, e))
             finally:
                 self.xmit_lock.release()
             time.sleep(3)
         if xmitted is False:
             logger.error('Could not transmit a packet. Close Momonga and open it again.')
@@ -266,24 +271,32 @@
         assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmission is inconsistent: Too big than expected.'
 
         if self.xmit_restriction_cnt == 1:
             logger.debug('Trying to restrict data transmission.')
             self.xmit_lock.acquire()
             logger.debug('Data transmission is being restricted.')
 
-    def unrestrict_to_xmit(self, force=False) -> None:
+    def unrestrict_to_xmit(self,
+                           force=False,
+                          ) -> None:
         if force is True:
             self.xmit_restriction_cnt = 0
             logger.debug('The counter for the restriction was forcibly set to zero.')
         else:
             self.xmit_restriction_cnt -= 1
             logger.debug('The counter for the restriction was decremented: %d' % (self.xmit_restriction_cnt))
 
         assert self.xmit_restriction_cnt >= 0, 'The critical section counter for data transmit is inconsistent: Too small than expected.'
 
         if self.xmit_restriction_cnt == 0:
             try:
                 self.xmit_lock.release()
-            except RuntimeError as e:
-                #logger.warning('Could not release "xmit_lock": %s' % e)
-                pass
+            except RuntimeError:
+                pass  # xmit_lock is likely already unlocked.
+
             logger.debug('Data transmission is being unrestricted.')
+
+    def is_restricted_to_xmit(self) -> bool:
+        if self.xmit_restriction_cnt == 0:
+            return False
+        else:
+            return True
```

## momonga/momonga_sk_wrapper.py

```diff
@@ -1,15 +1,27 @@
-
 import logging
 import threading
 import queue
 import serial
 
-from .momonga_exception import *
-from .momonga_response import *
+from .momonga_exception import (MomongaError,
+                                MomongaTimeoutError,
+                                MomongaSkCommandUnknownError,
+                                MomongaSkCommandUnsupported,
+                                MomongaSkCommandInvalidArgument,
+                                MomongaSkCommandInvalidSyntax,
+                                MomongaSkCommandSerialInputError,
+                                MomongaSkCommandFailedToExecute,
+                                MomongaSkScanFailure,
+                                MomongaSkJoinFailure)
+from .momonga_response import (SkVerResponse,
+                               SkAppVerResponse,
+                               SkInfoResponse,
+                               SkScanResponse,
+                               SkLl64Response)
 
 
 try:
     from typing import Self
 except ImportError:
     Self = object
 
@@ -26,60 +38,60 @@
         self.baudrate = baudrate
 
         # the following value will be set a pyserial object.
         self.ser = None
         self.publisher_th = None
         self.subscribers = {'cmd_exec_q': queue.Queue()}
 
-#    def __enter__(self) -> Self:
+    #def __enter__(self) -> Self:
     def __enter__(self):
         return self.open()
 
     def __exit__(self, type, value, traceback) -> None:
         self.close()
 
-#    def open(self) -> Self:
+    #def open(self) -> Self:
     def open(self):
         self.ser = serial.Serial(self.dev, self.baudrate)
 
         # to drop garbage data in the buffer.
         self.__clear_buf()
 
         # to check to be returned the udp payloads in ascii.
         if self.__exec_ropt() != '01':
             raise MomongaError("Execute 'WOPT 01\\r' yourself before using Momonga to make the wi-sun module return the UDP payloads in ASCII format. Note: The WOPT command can only be executed a limited number of times, so execute it only once!")
 
         for q in self.subscribers.values():
             while not q.empty():
                 q.get()
 
-        self.publisher_th_breaker = False # set True when you want to stop the publisher.
+        self.publisher_th_breaker = False  # set True when you want to stop the publisher.
         self.publisher_th = threading.Thread(target=self.received_packet_publisher, daemon=True)
         self.publisher_th.start()
 
     def close(self) -> None:
         if self.publisher_th is not None:
             self.publisher_th_breaker = True
             self.publisher_th.join()
             self.publisher_th = None
         if self.ser is not None and not self.ser.closed:
             self.ser.close()
 
-    def __clear_buf(self) -> None: # do not call this after open().
+    def __clear_buf(self) -> None:  # do not call this after open().
         self.ser.write(b'\r\n')
         self.ser.flush()
         timeout = self.ser.timeout
-        self.ser.timeout = 2 # will wait the specified seconds.
+        self.ser.timeout = 2  # will wait the specified seconds.
         while self.ser.read():
             # this loop clears garbage data if it exists.
             pass
         # to undo the timeout.
         self.ser.timeout = timeout
 
-    def __exec_ropt(self) -> str: # do not call this after open().
+    def __exec_ropt(self) -> str:  # do not call this after open().
         self.ser.write(b'ROPT\r')
         self.ser.flush()
         res = b''
         ok = b'OK '
         while True:
             res += self.ser.read()
             if ok in res and res.endswith(b'\r'):
@@ -94,31 +106,31 @@
         data_bytes = self.ser.readline()
         self.ser.timeout = org_timeout
         if data_bytes != b'':
             logger.debug('<<< %s' % data_bytes)
         line = data_bytes.decode().split('\r\n')[0]
         return line
 
-    def received_packet_publisher(self):
+    def received_packet_publisher(self) -> None:
         logger.debug('The received packet publisher has been started.')
         while True:
             if self.publisher_th_breaker is True:
                 break
             line = self.__readline(timeout=1)
             if line == '':
                 continue
             for q in self.subscribers.values():
-                q.put(line) # will dispatch the line to each subscriber
+                q.put(line)  # will dispatch the line to each subscriber
         logger.debug('The received packet publisher has been stopped.')
-   
+
     def __writeline(self,
                     line: str,
                     payload: bytes | None = None,
                    ) -> None:
-        if payload is not None: 
+        if payload is not None:
             data_bytes = (line + ' ').encode() + payload
         else:
             data_bytes = (line + '\r\n').encode()
         self.ser.write(data_bytes)
         logger.debug('>>> %s' % data_bytes)
         self.ser.flush()
 
@@ -207,15 +219,15 @@
     def sksetpwd(self,
                  pwd: str,
                 ) -> None:
         self.exec_command(['SKSETPWD', '%X' % len(pwd), pwd])
 
     def skscan(self,
                retry: int = 3,
-               ) -> SkScanResponse:
+              ) -> SkScanResponse:
         duration = 6
         for _ in range(retry):
             logger.debug('Trying to scan a PAN... Duration: %d' % duration)
             res = self.exec_command(['SKSCAN', '2', 'FFFFFFFF', str(duration), '0'], 'EVENT 22')
             # estimated execution time: 0.0096s*(2^(DURATION=6)+1)*28 = 17.5s
             # estimated execution time: 0.0096s*(2^(DURATION=7)+1)*28 = 34.7s
             # estimated execution time: 0.0096s*(2^(DURATION=8)+1)*28 = 69.1s
@@ -253,12 +265,10 @@
                  ip6_addr: str,
                  data: bytes,
                  handle: int = 1,
                  port: int = 0x0E1A,
                  sec: int = 2,
                  side: int = 0,
                 ) -> None:
-        self.exec_command(['SKSENDTO', str(handle),
-                          ip6_addr, '%04X' % port,
-                          str(sec), str(side),
-                          '%04X' % len(data)],
-                          payload=data)
+        self.exec_command(['SKSENDTO', str(handle), ip6_addr, '%04X' % port,
+                           str(sec), str(side), '%04X' % len(data)],
+                          payload = data)
```

## Comparing `momonga-0.0.8.dist-info/LICENSE` & `momonga-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `momonga-0.0.8.dist-info/METADATA` & `momonga-0.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: momonga
-Version: 0.0.8
+Version: 0.1.0
 Summary: Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 Home-page: https://github.com/nbtk/momonga
 Author: nbtk
 License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial ~=3.5
 
+[![Downloads](https://static.pepy.tech/badge/momonga)](https://pepy.tech/project/momonga)
+
 # Momonga
 Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 
 # Description
 MomongaはBルートサービスを利用してスマートメーターと通信するライブラリです。ターゲットデバイスはROHM社製Wi-SUNモジュールBP35C2を搭載したラトックシステムRS-WSUHA-Pです。
 
 # Preparation
```

## Comparing `momonga-0.0.8.dist-info/RECORD` & `momonga-0.1.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-momonga/__init__.py,sha256=iWnaMiIWmYho2GfBZJiZ82rlo4znFfQlqNXkGwNXhLg,136
-momonga/momonga.py,sha256=dVaNo0dxaoOHFh5VPUXJYypnvTfpYdQ_ewS_ukgrjN4,15394
-momonga/momonga_exception.py,sha256=IPcOVNU7mpm-upYTLLo6gIxFHzjCXxs-YwzhIej8PMU,959
-momonga/momonga_response.py,sha256=_t_aaA6z5cpZVGWIkir7J_fgwYabPSNrpBAiS36Ro7c,2698
-momonga/momonga_session_manager.py,sha256=jcOgnpXPdXvzqifyEBDsWMrjyAmuFTPlVaNi1vHbgvY,11915
-momonga/momonga_sk_wrapper.py,sha256=xaffyj3D3Mt84LljroJ07j-GHJTpsXTMp695vztZbz4,9392
-momonga-0.0.8.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
-momonga-0.0.8.dist-info/METADATA,sha256=bN2U4GC2uL5BWfJ6ZHWWwkYoey-lHFSm5ymXRcPbF20,10353
-momonga-0.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-momonga-0.0.8.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
-momonga-0.0.8.dist-info/RECORD,,
+momonga/__init__.py,sha256=DJfFmQ8oRnm69XfkH5TL0n9CXJsiqrgdO7D7D7GyLSk,135
+momonga/momonga.py,sha256=VX4bSPGHDL1-UZb_Gw3VG3THyEHcxn-r50ZX4eBx3Xg,15714
+momonga/momonga_exception.py,sha256=Cc7Jo3rjczP9-LqblFuyUq8jSjR7wjO4AXmDKjIARWw,973
+momonga/momonga_response.py,sha256=vj37u7FZUO-SAQvBSt71OLH5N6-cjLtPSIpKmDehSi8,2712
+momonga/momonga_session_manager.py,sha256=Q1yfcNnSSf7P2o6nNf7nyiNWmK8KcmpsLnaD3Oqr_fo,12539
+momonga/momonga_sk_wrapper.py,sha256=S4T-DsRzEJf9ifzxKxZ86we1DjlYqVunVqGaF0G6GRw,10110
+momonga-0.1.0.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
+momonga-0.1.0.dist-info/METADATA,sha256=oJ4aFZEzdkDnrj2qJ0yorHgk85QsI5fRR8ezcOTjbaw,10439
+momonga-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+momonga-0.1.0.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
+momonga-0.1.0.dist-info/RECORD,,
```

