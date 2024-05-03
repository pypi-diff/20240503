# Comparing `tmp/roktools-6.1.2.tar.gz` & `tmp/roktools-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.1.2.tar", max compression
+gzip compressed data, was "roktools-6.2.0.tar", max compression
```

## Comparing `roktools-6.1.2.tar` & `roktools-6.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-04-30 07:25:56.872515 roktools-6.1.2/LICENSE
--rw-r--r--   0        0        0     1665 2024-04-30 07:25:56.872515 roktools-6.1.2/README.md
--rw-r--r--   0        0        0     1162 2024-04-30 07:25:56.872515 roktools-6.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/decorator.py
--rw-r--r--   0        0        0      933 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/file.py
--rw-r--r--   0        0        0    33628 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-04-30 07:25:56.924515 roktools-6.1.2/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1884 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9505 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-04-30 07:25:56.924515 roktools-6.1.2/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1745 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5905 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-04-30 07:25:56.924515 roktools-6.1.2/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    31199 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/rinex.py
--rwxr-xr-x   0        0        0     1084 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/tensorial.py
--rw-r--r--   0        0        0    11178 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/time.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-03 10:04:56.539736 roktools-6.2.0/LICENSE
+-rw-r--r--   0        0        0     1665 2024-05-03 10:04:56.539736 roktools-6.2.0/README.md
+-rw-r--r--   0        0        0     1162 2024-05-03 10:04:56.539736 roktools-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/decorator.py
+-rw-r--r--   0        0        0      933 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/file.py
+-rw-r--r--   0        0        0    33628 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:04:56.583736 roktools-6.2.0/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9572 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:04:56.583736 roktools-6.2.0/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1745 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5905 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:04:56.583736 roktools-6.2.0/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    48895 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/rinex.py
+-rwxr-xr-x   0        0        0     1084 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/tensorial.py
+-rw-r--r--   0        0        0    11178 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/time.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.2.0/PKG-INFO
```

### Comparing `roktools-6.1.2/LICENSE` & `roktools-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/README.md` & `roktools-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/pyproject.toml` & `roktools-6.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.1.2"
+version = "6.2.0"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.1.2/roktools/cl.py` & `roktools-6.2.0/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/file.py` & `roktools-6.2.0/roktools/file.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/geodetic.py` & `roktools-6.2.0/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/gnss/edit.py` & `roktools-6.2.0/roktools/gnss/edit.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/gnss/observables.py` & `roktools-6.2.0/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/gnss/residuals.py` & `roktools-6.2.0/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/gnss/types.py` & `roktools-6.2.0/roktools/gnss/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,21 @@
     GPS: str = 'G'
     GALILEO: str = 'E'
     GLONASS: str = 'R'
     BEIDOU: str = 'C'
     QZSS: str = 'J'
     IRNSS: str = 'I'
     SBAS: str = 'S'
-    STARLINK: str = 'V'
-    SPIRE: str = 'Z'
     LEO: str = 'L'
+    XONA: str = 'P'
+    GEELY: str = 'Y'
+    STARLINK: str = 'X'
     ONEWEB: str = 'O'
+    SPIRE: str = 'V'
+    CENTISPACE: str = 'Z'
 
     @staticmethod
     def from_string(constellation_char: str) -> 'ConstellationId':
         """
         Returns the corresponding ConstellationId from input character
 
         >>> ConstellationId.from_string('E')
```

### Comparing `roktools-6.1.2/roktools/logger.py` & `roktools-6.2.0/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/orbit/kepler.py` & `roktools-6.2.0/roktools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/orbit/tle.py` & `roktools-6.2.0/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/parsers/rtklib/stats.py` & `roktools-6.2.0/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/rinex.py` & `roktools-6.2.0/roktools/rinex.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from dataclasses import dataclass, fields, asdict
 import datetime
 import enum
 import math
 import pandas as pd
 import re
-from typing import List, Tuple, Union, IO
+from typing import Dict, List, Tuple, Union, IO
 import sys
 
 from . import logger
 from . import time
 from .constants import SPEED_OF_LIGHT
 from .file import process_filename_or_file_handler, skip_lines
 from .gnss.types import ConstellationId, Band, TrackingChannel, Satellite
@@ -61,14 +61,53 @@
     ConstellationId.SBAS: {
         '1': Band.L1,
         '5': Band.L5
     }
 }
 
 
+class EphType(enum.Enum):
+
+    GPS_LNAV = f'{ConstellationId.GPS.value}_LNAV'
+    GPS_CNAV = f'{ConstellationId.GPS.value}_CNAV'
+    GPS_CNV2 = f'{ConstellationId.GPS.value}_CNV2'
+    GAL_INAV = f'{ConstellationId.GALILEO.value}_INAV'
+    GAL_FNAV = f'{ConstellationId.GALILEO.value}_FNAV'
+    GLO_FDMA = f'{ConstellationId.GLONASS.value}_FDMA'
+    QZS_LNAV = f'{ConstellationId.QZSS.value}_LNAV'
+    QZS_CNAV = f'{ConstellationId.QZSS.value}_CNAV'
+    QZS_CNV2 = f'{ConstellationId.QZSS.value}_CNV2'
+    BDS_D1 = f'{ConstellationId.BEIDOU.value}_D1'
+    BDS_F2 = f'{ConstellationId.BEIDOU.value}_D2'
+    BDS_CNV1 = f'{ConstellationId.BEIDOU.value}_CNV1'
+    BDS_CNV2 = f'{ConstellationId.BEIDOU.value}_CNV2'
+    BDS_CNV3 = f'{ConstellationId.BEIDOU.value}_CNV3'
+    SBS = f'{ConstellationId.SBAS.value}_SBAS'
+    IRN_LNAV = f'{ConstellationId.IRNSS.value}_LNAV'
+    LEO = f'{ConstellationId.LEO.value}'
+    SPIRE = f'{ConstellationId.SPIRE.value}'
+    STARLINK = f'{ConstellationId.STARLINK.value}'
+    ONEWEB = f'{ConstellationId.ONEWEB.value}'
+
+    @staticmethod
+    def from_string(value: str) -> 'EphType':
+        """
+        Get the Ephemerides type from an input string (or raise an exception if not found)
+
+        >>> EphType.from_string('G_LNAV')
+        <EphType.GPS_LNAV: 'G_LNAV'>
+        """
+
+        for member in EphType:
+            if member.value == value:
+                return member
+
+        raise ValueError(f"Value [ {value} ] could not be mapped into a Rinex 4 ephemeris type")
+
+
 class RinexSatIdProvider(ABC):
     """
     This abstract class provides an interface to provide the RINEX Satellite ID and constellation
     """
     @abstractmethod
     def get_constellation_letter(self) -> str:
         pass
@@ -342,47 +381,14 @@
         return 15
     elif mod_seconds < 2700:
         return 30
     else:
         return 45
 
 
-def parse_obs_line(line: str, n_obs: int) -> Tuple[Satellite, List[ObservableValue]]:
-    """
-
-    >>> line = "C05  40058862.469 6 208597044.05206  40058858.572 7 161300483.44407  40058861.947 7 169502210.29507"
-    >>> parse_obs_line(line, 6)
-    (C05, [ObservableValue(value=40058862.469, lli=0, snr=6), \
-ObservableValue(value=208597044.052, lli=0, snr=6), \
-ObservableValue(value=40058858.572, lli=0, snr=7), \
-ObservableValue(value=161300483.444, lli=0, snr=7), \
-ObservableValue(value=40058861.947, lli=0, snr=7), \
-ObservableValue(value=169502210.295, lli=0, snr=7)])
-    """
-
-    satellite = Satellite.from_string(line[0:3])
-
-    observable_values = []
-
-    offset = 3
-    for i_obs in range(n_obs):
-        start = offset + i_obs * 16
-        obs_str = line[start:start + 14]
-        lli_str = line[start + 14:start + 14 + 1]
-        snr_str = line[start + 15:start + 15 + 1]
-
-        obs = float(obs_str) if obs_str and obs_str != '              ' and obs_str != '\n' else math.nan
-        lli = int(lli_str) if lli_str and lli_str != ' ' and lli_str != '\n' else 0
-        snr = int(snr_str) if snr_str and snr_str != ' ' and snr_str != '\n' else 0
-
-        observable_values.append(ObservableValue(obs, lli, snr))
-
-    return satellite, observable_values
-
-
 def get_channels(observables: List[ObservableType]) -> List[TrackingChannel]:
     """
     Get the channel list from a list of observables
 
     >>> C1C = ObservableType.from_string("C1C")
     >>> L1C = ObservableType.from_string("L1C")
     >>> C1W = ObservableType.from_string("C1W")
@@ -434,46 +440,14 @@
 
         else:
             values.extend(values_partial)
 
     return {constellation: values}
 
 
-def parse_rnx3_epoch(line):
-    """
-    Parse a measurement epoch from a Rinex3 and return a tuple
-    with the epochm event type and number of lines
-
-    >>> parse_rnx3_epoch("> 2017 08 03 11 22 30.1234000  0 29")
-    (datetime.datetime(2017, 8, 3, 11, 22, 30, 123400), 0, 29)
-
-    >>> parse_rnx3_epoch("> 2021  2  5 15 51 30.2000000 0 22")
-    (datetime.datetime(2021, 2, 5, 15, 51, 30, 200000), 0, 22)
-
-    >>> parse_rnx3_epoch("> 2020 11 18 21 43 30.0000000  0 28       0.000000000000")
-    (datetime.datetime(2020, 11, 18, 21, 43, 30), 0, 28)
-
-    >>> parse_rnx3_epoch("> 2019 07 02 13 25  5.9999995  0 31")
-    (datetime.datetime(2019, 7, 2, 13, 25, 5, 999999), 0, 31)
-    """
-
-    try:
-        _, year, month, day, hour, minute, seconds, epoch_flag, n_lines, *b = line.split()
-    except ValueError as e:
-        raise ValueError(f"Invalid Rinex 3 epoch line [ {line} ]: {e}")
-
-    seconds, microseconds, *b = seconds.split('.')
-
-    t = datetime.datetime(int(year), int(month), int(day),
-                          hour=int(hour), minute=int(minute), second=int(seconds),
-                          microsecond=int(microseconds[0:6]))
-
-    return t, int(epoch_flag), int(n_lines)
-
-
 def to_dataframe(rinex_file: str) -> pd.DataFrame:
 
     with open(rinex_file, 'r') as file:
 
         constellation_observables = {}
         records = []
 
@@ -496,29 +470,29 @@
         # Body parsing
         for line in file:
 
             epoch_flag = EpochFlag.get_from_line(line)
 
             if epoch_flag == EpochFlag.OK:
 
-                epoch, _, n_lines = parse_rnx3_epoch(line)
+                epoch, _, n_lines = _parse_rnx3_epoch(line)
 
                 for _ in range(n_lines):
 
                     line = next(file)
 
                     constellation = line[0]
 
                     observable_types = constellation_observables.get(constellation, None)
                     if observable_types is None:
                         continue
 
                     n_obs = len(observable_types)
                     channels = get_channels(observable_types)
-                    satellite, observable_values = parse_obs_line(line, n_obs)
+                    satellite, observable_values = _parse_obs_line(line, n_obs)
 
                     epoch_records = [
                         Record(epoch, satellite, channel, math.nan, math.nan, math.nan, math.nan, '00000000', 0)
                         for channel in channels]
 
                     # Create a dictionary with channels as keys and records as values
                     epoch_records_dict = {record.channel: record for record in epoch_records}
@@ -579,14 +553,287 @@
 
         grouped_df['cmc_detrended'] = cmc - trend
 
         return grouped_df
 
 
 @dataclass
+class NavBlock(ABC):
+    """
+    Abstract class for RINEX Navigation block
+    """
+    satellite: Satellite
+    epoch: datetime
+
+    @staticmethod
+    def csv_fields() -> str:
+        return None
+
+    def to_csv(self) -> str:
+        # Get all field names from the __dataclass_fields__ attribute
+        field_names = [field.name for field in fields(self)]
+
+        # Get the value of each field from the instance dictionary
+        field_values = [getattr(self, field_name) for field_name in field_names]
+
+        # Convert field values to strings and join them with commas
+        body = ",".join(map(str, field_values))
+
+        return f'{self.get_type().value},{body}'
+
+    # Custom function to convert each NavBlock to a dict with string satellite
+    def to_dict(self):
+        block_dict = asdict(self)
+        block_dict['satellite'] = str(self.satellite)  # Convert satellite to string
+        return block_dict
+
+    @abstractmethod
+    def get_type(self) -> EphType:
+        return None
+
+
+@dataclass
+class GpsLnavNavBlock(NavBlock):
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    iode: int
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    toe_sow: float
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    codesL2: int
+    toe_week: int
+    l2p_flag: int
+
+    accuracy: float
+    health: int
+    tgd: float
+    iodc: int
+
+    tx_time_tow: float
+    fit_interval: int
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_IODE_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_TOE_SOW_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_CODESL2_STR},{_TOE_WEEK_STR},{_L2PFLAG_STR},\
+{_ACCURACY_STR},{_HEALTH_STR},{_TGD_STR},{_IODC_STR},\
+{_TX_TIME_TOW_STR},{_FIT_INTERVAL_STR}"
+
+    def get_type(self) -> EphType:
+        return EphType.GPS_LNAV
+
+
+@dataclass
+class GpsCnavNavBlock(NavBlock):
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    adot: float
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    top: float
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    deltan_dot: float
+    urai_ned0: float
+    urai_ned1: float
+
+    urai_ed: float
+    health: int
+    tgd: float
+    urai_ned2: float
+
+    isc_l1ca: float
+    isc_l2c: float
+    isc_l5i5: float
+    isc_l5q5: float
+
+    tx_time_tow: float
+    wn_op: int
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_ADOT_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_T_OP_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_DELTAN_DOT_STR},{_URAI_NED0_STR},{_URAI_NED1_STR},\
+{_URAI_ED_STR},{_HEALTH_STR},{_TGD_STR},{_URAI_NED2_STR},\
+{_ISC_L1CA_STR},{_ISC_L2C_STR},{_ISC_L5I5_STR},{_ISC_L5Q5_STR},\
+{_TX_TIME_TOW_STR},{_WN_OP_STR}"
+
+    def get_type(self) -> EphType:
+        return EphType.GPS_CNAV
+
+
+@dataclass
+class GpsCnv2NavBlock(NavBlock):
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    adot: float
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    top: float
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    deltan_dot: float
+    urai_ned0: float
+    urai_ned1: float
+
+    urai_ed: float
+    health: int
+    tgd: float
+    urai_ned2: float
+
+    isc_l1ca: float
+    isc_l2c: float
+    isc_l5i5: float
+    isc_l5q5: float
+
+    isc_l1cd: float
+    isc_l1cp: float
+
+    tx_time_tow: float
+    wn_op: int
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_ADOT_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_T_OP_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_DELTAN_DOT_STR},{_URAI_NED0_STR},{_URAI_NED1_STR},\
+{_URAI_ED_STR},{_HEALTH_STR},{_TGD_STR},{_URAI_NED2_STR},\
+{_ISC_L1CA_STR},{_ISC_L2C_STR},{_ISC_L5I5_STR},{_ISC_L5Q5_STR},\
+{_ISC_L1CD_STR},{_ISC_L1CP_STR},\
+{_TX_TIME_TOW_STR},{_WN_OP_STR}"
+
+    def get_type(self) -> EphType:
+        return EphType.GPS_CNV2
+
+
+@dataclass
+class GalNavBlock(NavBlock):
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    iodnav: float
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    toe_gal_tow: int
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    data_source: int
+    toe_gal_week: int
+
+    sisa: float
+    health: int
+    bgd_e5a_e1: float
+    bgd_e5b_e1: float
+
+    tx_time_tow: float
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_IODNAV_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_TOE_GAL_TOW_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_DATA_SOURCES_STR},{_TOE_GAL_WEEK_STR},,\
+{_SISA_STR},{_HEALTH_STR},{_BGD_E5A_STR},{_BGD_E5B_STR},\
+{_TX_TIME_TOW_STR}"
+
+    def get_type(self) -> EphType:
+        INAV_MASK = 0b101
+        FNAV_MASK = 0b10
+
+        if self.data_source & INAV_MASK:
+            return EphType.GAL_INAV
+        elif self.data_source & FNAV_MASK:
+            return EphType.GAL_FNAV
+
+        raise ValueError(f'Cannot extract the Galileo Eph type from the data sources [ {self.data_source} ]')
+
+
+@dataclass
 class RawNavBlock(object):
     satellite: Satellite
     epoch: datetime.datetime
     lines: List[str]
 
     def __repr__(self):
         return '\n'.join(self.lines)
@@ -616,43 +863,161 @@
             out = out + f'{brdc_line[1:]}\n'
         # print extra lines
         out = out + '    0.000000000000e+00 0.000000000000e+00 0.000000000000e+00 0.000000000000e+00\n'
         out = out + f'{self.lines[4][1:23]} 0.000000000000e+00'
 
         return out
 
+    def to_csv(self) -> str:
+        pass
+
+    def to_nav_block(self) -> NavBlock:
+        """
+        Convert to Navigation Block
+        """
+
+        # Get the type of EPH block
+        eph_type = _get_eph_type_from_rinex4_nav_block_header(self.lines[0])
+        if eph_type == EphType.GPS_LNAV:
+            return self._to_GPS_LNAV()
+        elif eph_type == EphType.GPS_CNAV:
+            return self._to_GPS_CNAV()
+        elif eph_type == EphType.GPS_CNV2:
+            return self._to_GPS_CNV2()
+        elif eph_type == EphType.GAL_FNAV or eph_type == EphType.GAL_INAV:
+            return self._to_GAL()
+
+        raise ValueError(f'There is no NavBlock generator for [ {eph_type} ]')
+
+    def _to_GPS_LNAV(self) -> GpsLnavNavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        iode, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        toe_sow, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, codesL2, toe_week, l2p_flag = _parse_nav_orb_line(self.lines[6])
+        accuracy, health, tgd, iodc = _parse_nav_orb_line(self.lines[7])
+        tx_time_tow, fit_interval, _, _ = _parse_nav_orb_line(self.lines[8])
+
+        if fit_interval is None:
+            fit_interval = 0
+
+        return GpsLnavNavBlock(Satellite.from_string(sat_str),
+                               datetime.datetime(year, month, day, hour, min, sec),
+                               clk_bias, clk_drift, clk_drift_rate,
+                               iode, crs, deltan, M0,
+                               cuc, e, cus, sqrtA,
+                               toe_sow, cic, OMEGA0, cis,
+                               i0, crc, omega, OMEGA_DOT,
+                               idot, int(codesL2), int(toe_week), int(l2p_flag),
+                               accuracy, int(health), tgd, int(iodc),
+                               tx_time_tow, int(fit_interval))
+
+    def _to_GPS_CNAV(self) -> GpsCnavNavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        adot, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        top, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, deltan_dot, urai_ned0, urai_ned1 = _parse_nav_orb_line(self.lines[6])
+        urai_ed, health, tgd, urai_ned = _parse_nav_orb_line(self.lines[7])
+        isc_l1ca, isc_l2c, isc_l5i5, isc_l5q5 = _parse_nav_orb_line(self.lines[8])
+        tx_time_tow, wn_op, _, _ = _parse_nav_orb_line(self.lines[9])
+
+        return GpsCnavNavBlock(Satellite.from_string(sat_str),
+                               datetime.datetime(year, month, day, hour, min, sec),
+                               clk_bias, clk_drift, clk_drift_rate,
+                               adot, crs, deltan, M0,
+                               cuc, e, cus, sqrtA,
+                               top, cic, OMEGA0, cis,
+                               i0, crc, omega, OMEGA_DOT,
+                               idot, deltan_dot, urai_ned0, urai_ned1,
+                               urai_ed, health, tgd, urai_ned,
+                               isc_l1ca, isc_l2c, isc_l5i5, isc_l5q5,
+                               tx_time_tow, int(wn_op))
+
+    def _to_GPS_CNV2(self) -> GpsCnv2NavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        adot, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        top, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, deltan_dot, urai_ned0, urai_ned1 = _parse_nav_orb_line(self.lines[6])
+        urai_ed, health, tgd, urai_ned = _parse_nav_orb_line(self.lines[7])
+        isc_l1ca, isc_l2c, isc_l5i5, isc_l5q5 = _parse_nav_orb_line(self.lines[8])
+        isc_l1cd, isc_l1cp, _, _ = _parse_nav_orb_line(self.lines[9])
+        tx_time_tow, wn_op, _, _ = _parse_nav_orb_line(self.lines[10])
+
+        return GpsCnv2NavBlock(Satellite.from_string(sat_str),
+                               datetime.datetime(year, month, day, hour, min, sec),
+                               clk_bias, clk_drift, clk_drift_rate,
+                               adot, crs, deltan, M0,
+                               cuc, e, cus, sqrtA,
+                               top, cic, OMEGA0, cis,
+                               i0, crc, omega, OMEGA_DOT,
+                               idot, deltan_dot, urai_ned0, urai_ned1,
+                               urai_ed, health, tgd, urai_ned,
+                               isc_l1ca, isc_l2c, isc_l5i5, isc_l5q5,
+                               isc_l1cd, isc_l1cp,
+                               tx_time_tow, int(wn_op))
+
+    def _to_GAL(self) -> GalNavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        iodnav, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        toe_tow, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, datasources, toe_week, _ = _parse_nav_orb_line(self.lines[6])
+        sisa, health, bgd_e5a, bgd_e5b = _parse_nav_orb_line(self.lines[7])
+        tx_tm, _, _, _ = _parse_nav_orb_line(self.lines[8])
+
+        return GalNavBlock(Satellite.from_string(sat_str),
+                           datetime.datetime(year, month, day, hour, min, sec),
+                           clk_bias, clk_drift, clk_drift_rate,
+                           int(iodnav), crs, deltan, M0,
+                           cuc, e, cus, sqrtA,
+                           toe_tow, cic, OMEGA0, cis,
+                           i0, crc, omega, OMEGA_DOT,
+                           idot, int(datasources), int(toe_week),
+                           sisa, health, bgd_e5a, bgd_e5b,
+                           tx_tm)
+
 
 class Nav(object):
     """
     Class that holds Rinex Navigation data
     """
 
     RINEX4_EPH_BLOCK_LINES_LEO = 6
 
     RINEX4_EPH_BLOCK_LINES = {
-        f'{ConstellationId.GPS.value} LNAV': 8,
-        f'{ConstellationId.GPS.value} CNAV': 9,
-        f'{ConstellationId.GPS.value} CNV2': 10,
-        f'{ConstellationId.GALILEO.value} INAV': 8,
-        f'{ConstellationId.GALILEO.value} FNAV': 8,
-        f'{ConstellationId.GLONASS.value} FDMA': 5,
-        f'{ConstellationId.QZSS.value} LNAV': 8,
-        f'{ConstellationId.QZSS.value} CNAV': 9,
-        f'{ConstellationId.QZSS.value} CNV2': 10,
-        f'{ConstellationId.BEIDOU.value} D1': 8,
-        f'{ConstellationId.BEIDOU.value} D2': 8,
-        f'{ConstellationId.BEIDOU.value} CNV1': 10,
-        f'{ConstellationId.BEIDOU.value} CNV2': 10,
-        f'{ConstellationId.BEIDOU.value} CNV3': 9,
-        f'{ConstellationId.SBAS.value} SBAS': 4,
-        f'{ConstellationId.IRNSS.value} LNAV': 8,
-        f'{ConstellationId.LEO.value}': RINEX4_EPH_BLOCK_LINES_LEO,
-        f'{ConstellationId.SPIRE.value}': RINEX4_EPH_BLOCK_LINES_LEO,
-        f'{ConstellationId.STARLINK.value}': RINEX4_EPH_BLOCK_LINES_LEO,
-        f'{ConstellationId.ONEWEB.value}': RINEX4_EPH_BLOCK_LINES_LEO,
+        EphType.GPS_LNAV: 8,
+        EphType.GPS_CNAV: 9,
+        EphType.GPS_CNV2: 10,
+        EphType.GAL_INAV: 8,
+        EphType.GAL_FNAV: 8,
+        EphType.GLO_FDMA: 5,
+        EphType.QZS_LNAV: 8,
+        EphType.QZS_CNAV: 9,
+        EphType.QZS_CNV2: 10,
+        EphType.BDS_D1: 8,
+        EphType.BDS_F2: 8,
+        EphType.BDS_CNV1: 10,
+        EphType.BDS_CNV2: 10,
+        EphType.BDS_CNV3: 9,
+        EphType.SBS: 4,
+        EphType.IRN_LNAV: 8,
+        EphType.LEO: RINEX4_EPH_BLOCK_LINES_LEO,
+        EphType.SPIRE: RINEX4_EPH_BLOCK_LINES_LEO,
+        EphType.STARLINK: RINEX4_EPH_BLOCK_LINES_LEO,
+        EphType.ONEWEB: RINEX4_EPH_BLOCK_LINES_LEO,
     }
 
     def __init__(self, file: Union[str, IO]):
         self.blocks = Nav._load(file)
 
     @staticmethod
     @process_filename_or_file_handler('r')
@@ -701,15 +1066,18 @@
 
             if not line.startswith('> EPH'):
                 continue
 
             fields = line.split()
             sat = fields[2]
             satellite = Satellite(sat[0], int(sat[1:]))  # satellite from eph
-            n_lines = Nav._get_block_n_lines(line.rstrip())
+
+            eph_type = _get_eph_type_from_rinex4_nav_block_header(line)
+            n_lines = Nav.RINEX4_EPH_BLOCK_LINES[eph_type]
+
             lines = [fh.readline().rstrip() for _ in range(n_lines)]
 
             epoch_line = lines[0]
             epoch = datetime.datetime.strptime(epoch_line[4:23], "%Y %m %d %H %M %S")
 
             block_lines = [line] + lines
             block = RawNavBlock(satellite, epoch, block_lines)
@@ -717,14 +1085,46 @@
             blocks.append(block)
 
         return blocks
 
     def get(satellite: Satellite):
         pass
 
+    def to_blocks(self) -> Dict[EphType, List[NavBlock]]:
+
+        out = {}
+
+        for block in self.blocks:
+
+            try:
+                nav_block = block.to_nav_block()
+            except ValueError:
+                pass
+
+            eph_type = nav_block.get_type()
+
+            if eph_type not in out:
+                out[eph_type] = []
+
+            out[eph_type].append(nav_block)
+
+        return out
+
+    def to_dataframes(self) -> Dict[EphType, pd.DataFrame]:
+
+        blocks = self.to_blocks()
+
+        dfs = {}
+
+        for eph_type, nav_blocks in blocks.items():
+            data = [block.to_dict() for block in nav_blocks]
+            dfs[eph_type] = pd.DataFrame(data)
+
+        return dfs
+
     def __len__(self):
         """
         Number of blocks of the Rinex Nav file
         """
         return len(self.blocks)
 
     def __iter__(self):
@@ -883,30 +1283,20 @@
                 try:
                     fh.write(block.to_rinex2() if rinex2 else str(block))
                     fh.write('\n')
                 except Exception as e:
                     logger.warning(e)
                     continue
 
-    @staticmethod
-    def _get_block_n_lines(line: str) -> int:
-        """
-        Give the number of lines of a navigation block for a given constellation
-        """
-
-        key = line[6]
-        constellation = ConstellationId(key)
-
-        if constellation is not ConstellationId.ONEWEB and \
-           constellation is not ConstellationId.SPIRE and \
-           constellation is not ConstellationId.LEO and \
-           constellation is not ConstellationId.STARLINK:
-            key = key + " " + line[10:]
-
-        return Nav.RINEX4_EPH_BLOCK_LINES[key]
+#    def to_csv(self, csv_filename:str) -> None:
+#
+#        with open(csv_filename, "w") as fh:
+#
+#            for block in self.blocks:
+#                pass
 
     @staticmethod
     def _write_orbit_line(a: float, b: float, c: float, d: float) -> str:
         return f'    {a:19.12e}{b:19.12e}{c:19.12e}{d:19.12e}'
 
 
 def compute_greenwich_ascending_node_rad(epoch_utc: datetime.datetime) -> float:
@@ -983,7 +1373,204 @@
     if args.celestrak_file:
         tle_list = read_celestrak(args.celestrak_file)
         Nav.write_from_tle(sys.stdout, tle_list, rinex2=args.rinex2)
 
     elif args.csv:
         df = pd.read_csv(args.csv, parse_dates=['epoch'])
         Nav.write_from_dataframe(sys.stdout, df, rinex2=args.rinex2)
+
+
+_ACCURACY_STR = "accuracy"
+_ADOT_STR = "Adot[m/s]"
+_BGD_E5A_STR = "bgd_e5a_e1[s]"
+_BGD_E5B_STR = "bgd_e5b_e1[s]"
+_CIC_STR = "cic[rad]"
+_CIS_STR = "cis[rad]"
+_CLK_BIAS_STR = "clock_bias[s]"
+_CLK_DRIFT_RATE_STR = "clock_drift_rate[s/s2]"
+_CLK_DRIFT_STR = "clock_drift[s/s]"
+_CODESL2_STR = "codesL2"
+_CRC_STR = "crc[m]"
+_CRS_STR = "crs[m]"
+_CUC_STR = "cuc[rad]"
+_CUS_STR = "cus[rad]"
+_DATA_SOURCES_STR = "datasources"
+_DELTAN_DOT_STR = "deltan_dot[r/s^2]"
+_DELTAN_STR = "deltan[rad/s]"
+_EPOCH_STR = "epoch"
+_E_STR = "e"
+_FIT_INTERVAL_STR = "fit_interval"
+_HEALTH_STR = "health"
+_I0_STR = "i0[rad]"
+_IDOT_STR = "idot[rad/s]"
+_IODC_STR = "iodc"
+_IODE_STR = "iode"
+_IODNAV_STR = "iodnav"
+_ISC_L1CA_STR = "isc_L1CA[s]"
+_ISC_L1CD_STR = "isc_L1CD[s]"
+_ISC_L1CP_STR = "isc_L1CP[s]"
+_ISC_L2C_STR = "isc_L2C[s]"
+_ISC_L5I5_STR = "isc_L5I5[s]"
+_ISC_L5Q5_STR = "isc_L5Q5[s]"
+_L2PFLAG_STR = "l2p_flag"
+_M0_STR = "M0[rad]"
+_OMEGA0_STR = "OMEGA0[rad]"
+_OMEGA_DOT_STR = "OMEGA_DOT[rad/s]"
+_OMEGA_STR = "omega[rad]"
+_SAT_STR = "sat"
+_SISA_STR = "sisa[m]"
+_SQRTA_STR = "sqrtA[sqrt(m)]"
+_TGD_STR = "tgd[s]"
+_TOE_GAL_TOW_STR = "toe_gal_tow[s]"
+_TOE_GAL_WEEK_STR = "toe_gal_week[week]"
+_TOE_SOW_STR = "toe[s]"
+_TOE_WEEK_STR = "toe[week]"
+_TX_TIME_TOW_STR = "tx_time[s]"
+_T_OP_STR = "t_op[s]"
+_URAI_ED_STR = "urai_ed"
+_URAI_NED0_STR = "urai_ned0"
+_URAI_NED1_STR = "urai_ned1"
+_URAI_NED2_STR = "urai_ned2"
+_WN_OP_STR = "wn_op[week]"
+
+
+def _parse_nav_epoch_line(line: str) -> tuple:
+    """
+    Parse a Rinex 4 Navigation line
+
+    >>> _parse_nav_epoch_line("G01 2024 02 13 11 22 33 1.693181693554e-04 1.477928890381e-12 1.000000000000e+00")
+    ('G01', 2024, 2, 13, 11, 22, 33, 0.0001693181693554, 1.477928890381e-12, 1.0)
+    """
+
+    return line[0:3], \
+        int(line[4:8]), int(line[9:11]), int(line[12:14]),  \
+        int(line[15:17]),  int(line[17:20]),  int(line[20:23]), \
+        float(line[23:42]), float(line[42:61]), float(line[61:])
+
+
+def _parse_nav_orb_line(line: str) -> tuple:
+    """
+    Parse a Rinex 4 Navigation line (broadcast orbit line)
+
+
+    >>> _parse_nav_orb_line('     1.700595021248e-06')
+    (1.700595021248e-06, None, None, None)
+
+    >>> _parse_nav_orb_line('     1.700595021248e-06 1.270996686071e-02')
+    (1.700595021248e-06, 0.01270996686071, None, None)
+
+    >>> _parse_nav_orb_line('     1.700595021248e-06 1.270996686071e-02 1.259148120880e-05')
+    (1.700595021248e-06, 0.01270996686071, 1.25914812088e-05, None)
+
+    >>> _parse_nav_orb_line('     1.700595021248e-06 1.270996686071e-02 1.259148120880e-05 5.154011671066e+03')
+    (1.700595021248e-06, 0.01270996686071, 1.25914812088e-05, 5154.011671066)
+    """
+
+    try:
+        v1 = float(line[4:23])
+    except ValueError:
+        v1 = None
+
+    try:
+        v2 = float(line[23:42])
+    except ValueError:
+        v2 = None
+
+    try:
+        v3 = float(line[42:61])
+    except ValueError:
+        v3 = None
+
+    try:
+        v4 = float(line[61:])
+    except ValueError:
+        v4 = None
+
+    return v1, v2, v3, v4
+
+
+def _parse_obs_line(line: str, n_obs: int) -> Tuple[Satellite, List[ObservableValue]]:
+    """
+
+    >>> line = "C05  40058862.469 6 208597044.05206  40058858.572 7 161300483.44407  40058861.947 7 169502210.29507"
+    >>> _parse_obs_line(line, 6)
+    (C05, [ObservableValue(value=40058862.469, lli=0, snr=6), \
+ObservableValue(value=208597044.052, lli=0, snr=6), \
+ObservableValue(value=40058858.572, lli=0, snr=7), \
+ObservableValue(value=161300483.444, lli=0, snr=7), \
+ObservableValue(value=40058861.947, lli=0, snr=7), \
+ObservableValue(value=169502210.295, lli=0, snr=7)])
+    """
+
+    satellite = Satellite.from_string(line[0:3])
+
+    observable_values = []
+
+    offset = 3
+    for i_obs in range(n_obs):
+        start = offset + i_obs * 16
+        obs_str = line[start:start + 14]
+        lli_str = line[start + 14:start + 14 + 1]
+        snr_str = line[start + 15:start + 15 + 1]
+
+        obs = float(obs_str) if obs_str and obs_str != '              ' and obs_str != '\n' else math.nan
+        lli = int(lli_str) if lli_str and lli_str != ' ' and lli_str != '\n' else 0
+        snr = int(snr_str) if snr_str and snr_str != ' ' and snr_str != '\n' else 0
+
+        observable_values.append(ObservableValue(obs, lli, snr))
+
+    return satellite, observable_values
+
+
+def _parse_rnx3_epoch(line):
+    """
+    Parse a measurement epoch from a Rinex3 and return a tuple
+    with the epochm event type and number of lines
+
+    >>> _parse_rnx3_epoch("> 2017 08 03 11 22 30.1234000  0 29")
+    (datetime.datetime(2017, 8, 3, 11, 22, 30, 123400), 0, 29)
+
+    >>> _parse_rnx3_epoch("> 2021  2  5 15 51 30.2000000 0 22")
+    (datetime.datetime(2021, 2, 5, 15, 51, 30, 200000), 0, 22)
+
+    >>> _parse_rnx3_epoch("> 2020 11 18 21 43 30.0000000  0 28       0.000000000000")
+    (datetime.datetime(2020, 11, 18, 21, 43, 30), 0, 28)
+
+    >>> _parse_rnx3_epoch("> 2019 07 02 13 25  5.9999995  0 31")
+    (datetime.datetime(2019, 7, 2, 13, 25, 5, 999999), 0, 31)
+    """
+
+    try:
+        _, year, month, day, hour, minute, seconds, epoch_flag, n_lines, *b = line.split()
+    except ValueError as e:
+        raise ValueError(f"Invalid Rinex 3 epoch line [ {line} ]: {e}")
+
+    seconds, microseconds, *b = seconds.split('.')
+
+    t = datetime.datetime(int(year), int(month), int(day),
+                          hour=int(hour), minute=int(minute), second=int(seconds),
+                          microsecond=int(microseconds[0:6]))
+
+    return t, int(epoch_flag), int(n_lines)
+
+
+def _get_eph_type_from_rinex4_nav_block_header(block_header: str) -> EphType:
+    """
+    Get the type of ephemeris based on the header line of the Rinex 4 navigation block
+
+    >>> _get_eph_type_from_rinex4_nav_block_header('> EPH G01 LNAV')
+    <EphType.GPS_LNAV: 'G_LNAV'>
+
+    >>> _get_eph_type_from_rinex4_nav_block_header('> EPH X02434')
+    <EphType.STARLINK: 'X'>
+    """
+
+    fields = block_header.split()
+
+    sat = Satellite.from_string(fields[2])
+
+    sat.constellation.value
+    key = sat.constellation.value
+    if len(fields) == 4:
+        key = f'{key}_{fields[-1]}'
+
+    return EphType.from_string(key)
```

### Comparing `roktools-6.1.2/roktools/stats.py` & `roktools-6.2.0/roktools/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/tensorial.py` & `roktools-6.2.0/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/roktools/time.py` & `roktools-6.2.0/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.2/PKG-INFO` & `roktools-6.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.1.2
+Version: 6.2.0
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

