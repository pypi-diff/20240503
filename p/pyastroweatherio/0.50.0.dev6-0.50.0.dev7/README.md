# Comparing `tmp/pyastroweatherio-0.50.0.dev6.tar.gz` & `tmp/pyastroweatherio-0.50.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.0.dev6.tar", last modified: Wed May  1 08:15:55 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.0.dev7.tar", last modified: Fri May  3 10:37:48 2024, max compression
```

## Comparing `pyastroweatherio-0.50.0.dev6.tar` & `pyastroweatherio-0.50.0.dev7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-01 08:15:55.139840 pyastroweatherio-0.50.0.dev6/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev6/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-01 08:15:55.135840 pyastroweatherio-0.50.0.dev6/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev6/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-01 08:15:55.131840 pyastroweatherio-0.50.0.dev6/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    40772 2024-05-01 08:14:51.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4142 2024-04-29 14:09:59.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20142 2024-04-29 10:03:52.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    42090 2024-04-29 14:59:50.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-01 08:15:55.135840 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-01 08:15:55.139840 pyastroweatherio-0.50.0.dev6/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-05-01 08:15:27.000000 pyastroweatherio-0.50.0.dev6/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-03 10:37:48.478827 pyastroweatherio-0.50.0.dev7/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev7/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-03 10:37:48.478827 pyastroweatherio-0.50.0.dev7/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev7/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-03 10:37:48.474827 pyastroweatherio-0.50.0.dev7/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    41207 2024-05-03 10:37:17.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     5128 2024-05-03 09:44:33.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20007 2024-05-03 09:38:40.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    44912 2024-05-03 09:15:48.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-03 10:37:48.478827 pyastroweatherio-0.50.0.dev7/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-03 10:37:48.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-03 10:37:48.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-03 10:37:48.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-05-03 10:37:48.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-03 10:37:48.000000 pyastroweatherio-0.50.0.dev7/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-03 10:37:48.478827 pyastroweatherio-0.50.0.dev7/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-05-03 09:20:05.000000 pyastroweatherio-0.50.0.dev7/setup.py
```

### Comparing `pyastroweatherio-0.50.0.dev6/LICENSE` & `pyastroweatherio-0.50.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev6/PKG-INFO` & `pyastroweatherio-0.50.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev6
+Version: 0.50.0.dev7
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev6/README.md` & `pyastroweatherio-0.50.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev6/pyastroweatherio/client.py` & `pyastroweatherio-0.50.0.dev7/pyastroweatherio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,16 @@
 
         if self._test_datetime is not None:
             await self._astro_routines.need_update()
         else:
             await self._astro_routines.need_update(forecast_time=now)
 
         forecast_time = now.replace(minute=0, second=0, microsecond=0)
+        if self._test_datetime is not None:
+            forecast_time = self._test_datetime.replace(minute=0, second=0, microsecond=0)
         _LOGGER.debug("Forecast time: %s", str(forecast_time))
 
         # Met.no
         metno_index = 0
         seventimer_index = 0
 
         # Met.no: Search for start index
@@ -177,15 +179,15 @@
             _LOGGER.debug("7Timer start index: %s", str(seventimer_index))
             details_seventimer = self._weather_data_seventimer[seventimer_index]
         else:
             details_seventimer = {"timepoint": 0, "seeing": -1, "transparency": -1, "lifted_index": -1}
 
         seeing = 0
         if details_seventimer["seeing"] == -1:
-            seeing = await self._astro_seeing.calculate_seeing_model6(
+            seeing = await self._astro_seeing.calculate_seeing_model(
                 temperature=details_metno.get("air_temperature", -1),
                 humidity=details_metno.get("relative_humidity", -1),
                 dew_point_temperature=details_metno.get("dew_point_temperature", -1),
                 wind_speed=details_metno.get("wind_speed", -1),
                 cloud_cover=details_metno.get("cloud_area_fraction", -1),
                 altitude=self._elevation,
                 air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
@@ -209,14 +211,15 @@
 
         lifted_index = 0
         if details_seventimer["lifted_index"] == -1 or details_seventimer["lifted_index"] == -9999:
             lifted_index = await self._astro_lifted_index.calculate_lifted_index(
                 temperature=details_metno.get("air_temperature", -1),
                 dew_point_temperature=details_metno.get("dew_point_temperature", -1),
                 altitude=self._elevation,
+                air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
             )
         else:
             lifted_index = LIFTED_INDEX[details_seventimer["lifted_index"] - 1]
      
         item = {
             # seventimer_init is "init" of 7timer astro data
             "seventimer_init": seventimer_init,  # init
@@ -329,14 +332,16 @@
         await self.retrieve_data_seventimer()
         now = datetime.now(timezone.utc).replace(tzinfo=None)
 
         # Create items
         cnt = 0
 
         forecast_time = now.replace(minute=0, second=0, microsecond=0)
+        if self._test_datetime is not None:
+            forecast_time = self._test_datetime.replace(minute=0, second=0, microsecond=0)
         _LOGGER.debug("Forecast time: %s", str(forecast_time))
 
         # Met.no
         # metno_index = 0
         # seventimer_index = 0
 
         # Met.no: Search for start index
@@ -389,15 +394,15 @@
                 "seventimer_timepoint": details_seventimer["timepoint"],
                 "forecast_time": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"),
                 "hour": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ").hour,  # forecast_time.hour % 24,
             }
 
             seeing = 0
             if details_seventimer["seeing"] == -1 or details_seventimer["seeing"] == -9999:
-                seeing = await self._astro_seeing.calculate_seeing_model6(
+                seeing = await self._astro_seeing.calculate_seeing_model(
                     temperature=details_metno.get("air_temperature", -1),
                     humidity=details_metno.get("relative_humidity", -1),
                     dew_point_temperature=details_metno.get("dew_point_temperature", -1),
                     wind_speed=details_metno.get("wind_speed", -1),
                     cloud_cover=details_metno.get("cloud_area_fraction", -1),
                     altitude=self._elevation,
                     air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
@@ -421,19 +426,19 @@
 
             lifted_index = 0
             if details_seventimer["lifted_index"] == -1 or details_seventimer["lifted_index"] == -9999:
                 lifted_index = await self._astro_lifted_index.calculate_lifted_index(
                     temperature=details_metno.get("air_temperature", -1),
                     dew_point_temperature=details_metno.get("dew_point_temperature", -1),
                     altitude=self._elevation,
+                    air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
                 )
             else:
                 lifted_index = LIFTED_INDEX[details_seventimer["lifted_index"] - 1]
-            
-            
+
             item["cloudcover"] = details_metno.get("cloud_area_fraction", -1)
             item["cloud_area_fraction"] = details_metno.get("cloud_area_fraction", -1)
             item["cloud_area_fraction_high"] = details_metno.get("cloud_area_fraction_high", -1)
             item["cloud_area_fraction_medium"] = details_metno.get("cloud_area_fraction_medium", -1)
             item["cloud_area_fraction_low"] = details_metno.get("cloud_area_fraction_low", -1)
             item["fog_area_fraction"] = details_metno.get("fog_area_fraction", -1)
             item["rh2m"] = details_metno.get("relative_humidity", -1)
```

### Comparing `pyastroweatherio-0.50.0.dev6/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.0.dev7/pyastroweatherio/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 import math
 
 from pyastroweatherio.const import (
     # CLOUDCOVER_PLAIN,
     CONDITION,
     CONDITION_PLAIN,
     DEEP_SKY_THRESHOLD,
-    # LIFTED_INDEX_PLAIN,
+    LIFTED_INDEX_VALUE,
+    LIFTED_INDEX_RANGE,
+    LIFTED_INDEX_PLAIN,
     # SEEING_PLAIN,
     # TRANSPARENCY_PLAIN,
-    WIND10M_PLAIN,
-    WIND10M_DIRECTON,
     WIND10M_VALUE,
     WIND10M_RANGE,
+    WIND10M_PLAIN,
+    WIND10M_DIRECTON,
 )
 
 
 class BaseData:
     """A representation of the base class for AstroWeather Data."""
 
     def __init__(self, data):
@@ -122,17 +124,17 @@
 
     @property
     def transparency_percentage(self) -> int:
         """Return Transparency."""
         return int(100 - self._transparency * 100)
 
     @property
-    def lifted_index(self) -> int:
+    def lifted_index(self) -> float:
         """Return Lifted Index."""
-        return int(self._lifted_index)
+        return round(self._lifted_index, 2)
 
     @property
     def rh2m(self) -> int:
         """Return 2m Relative Humidity."""
         return self._rh2m
 
     @property
@@ -247,59 +249,52 @@
     #         return CLOUDCOVER_PLAIN[cover - 1]
     #     return None
 
     @property
     def seeing_plain(self) -> str:
         """Return Seeing."""
         return "Deprecated. Use seeing instead."
-        seeing = self._seeing
-        if seeing >= 1 and seeing <= 8:
-            return SEEING_PLAIN[seeing - 1]
-        return None
+        # seeing = self._seeing
+        # if seeing >= 1 and seeing <= 8:
+        #     return SEEING_PLAIN[seeing - 1]
+        # return None
 
     # @property
     # def transparency_plain(self) -> str:
     #     """Return Transparency."""
     #     transparency = self._transparency
     #     if transparency >= 1 and transparency <= 8:
     #         return TRANSPARENCY_PLAIN[self._transparency - 1]
     #     return None
 
     @property
     def wind10m_speed_plain(self) -> str:
-        """Return Transparency."""
-        wind10m_speed = self._wind_speed
+        """Return wind speed plain."""
 
         wind_speed_value = 0
         for (start, end), derate in zip(WIND10M_RANGE, WIND10M_VALUE):
-            if start <= wind10m_speed <= end:
+            if start <= self._wind_speed <= end:
                 wind_speed_value = derate
 
         if wind_speed_value >= 1 and wind_speed_value <= 8:
             return WIND10M_PLAIN[wind_speed_value - 1]
         return None
 
-    # @property
-    # def lifted_index_plain(self) -> str:
-    #     """Return Lifted Index."""
+    @property
+    def lifted_index_plain(self) -> str:
+        """Return Lifted Index plain."""
 
-    #     trans = {
-    #         -10: LIFTED_INDEX_PLAIN[0],
-    #         -6: LIFTED_INDEX_PLAIN[1],
-    #         -4: LIFTED_INDEX_PLAIN[2],
-    #         -1: LIFTED_INDEX_PLAIN[3],
-    #         2: LIFTED_INDEX_PLAIN[4],
-    #         6: LIFTED_INDEX_PLAIN[5],
-    #         10: LIFTED_INDEX_PLAIN[6],
-    #         15: LIFTED_INDEX_PLAIN[7],
-    #     }
-    #     lifted_index = self._lifted_index
-    #     if lifted_index in trans:
-    #         return trans.get(self._lifted_index, "")
-    #     return None
+        lifted_index_value = 0
+        for (start, end), derate in zip(LIFTED_INDEX_RANGE, LIFTED_INDEX_VALUE):
+            if start <= self._lifted_index <= end:
+                lifted_index_value = derate
+
+        if lifted_index_value >= 1 and lifted_index_value <= 8:
+            return LIFTED_INDEX_PLAIN[lifted_index_value - 1]
+        return None
 
     @property
     def deep_sky_view(self) -> bool:
         """Return True if Deep Sky should be possible."""
         if self.condition_percentage >= DEEP_SKY_THRESHOLD:
             return True
         return False
```

### Comparing `pyastroweatherio-0.50.0.dev6/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.0.dev7/pyastroweatherio/helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Contains Helper functions for AstroWeather."""
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 import logging
 import ephem
 import math
 from decimal import Decimal
 from ephem import degree
 from math import degrees as deg
 import pytz
@@ -46,35 +46,120 @@
         _LOGGER.debug("7timer anchor timestamp: %s", str(datetime.strptime(value, "%Y%m%d%H")))
         return datetime.strptime(value, "%Y%m%d%H")
 
 
 class AstronomicalLiftedIndex:
     """Calculate astronomical lifted index"""
 
-    # Write a python3 program to calculate atmospheric lifted index based on humidity, temperature, clouds, wind, altitude, dew_point_temperature, transparency, and air_pressure_at_sea_level and convert the transparency to magnitude degradation
-
     def __init__(
         self,
     ):
-        _LOGGER.debug("AstronomicalTransparency calculation mode active")
-        # Temperature in Celsius
-        # Altitude in meters
-        # Dew point temperature in Celsius
+        _LOGGER.debug("AstronomicalLiftedIndex calculation mode active")
 
-    async def calculate_lifted_index(self, temperature, altitude, dew_point_temperature):
+    def calculate_vapor_pressure(self, surface_temp):
+        """
+        Calculate the actual vapor pressure at the surface using the Magnus-Tetens formula.
+
+        Args:
+        - surface_temp: Surface temperature in Celsius.
+
+        Returns:
+        - e: Actual vapor pressure at the surface in millibars (mb) or hectopascals (hPa).
+        """
+        # Constants
+        A = 6.112
+        B = 17.67
+        C = 243.5
+
+        # Calculate actual vapor pressure using Magnus-Tetens formula
+        e = A * math.exp((B * surface_temp) / (surface_temp + C))
+
+        return e
+
+    def calculate_mixing_ratio(self, e, air_pressure_at_sea_level):
+        """
+        Calculate the mixing ratio.
+
+        Args:
+        - e: Vapor pressure
+        - air_pressure_at_sea_level: Air pressure at sea level
+
+        Returns:
+        - w: mixing ratio at surface in grams per kilogram
+        """
         # Constants
-        lapse_rate = 0.0098  # Standard lapse rate (temperature decrease with altitude)
+        A = 621.97
 
-        # Calculate temperature at lifting condensation level (LCL)
-        temperature_LCL = dew_point_temperature - ((altitude / 1000) * lapse_rate)
+        # Calculate actual vapor pressure using Magnus-Tetens formula
+        w = A * (e / (air_pressure_at_sea_level - e))
 
-        # Calculate lifted index
-        lifted_index = temperature - temperature_LCL
+        return w
+
+    def calculate_lifting_condensation_level(self, w, air_pressure_at_sea_level):
+        """
+        The Lifting Condensation Level is the level at which a parcel becomes saturated. It can be used as
+        a reasonable estimate of cloud base height when parcels experience forced ascent.
+        Here, we calculate it using the Clausius-Clapeyron equation. This equation relates the saturation vapor
+        pressure (e) to the temperature and pressure.
+        https://en.wikipedia.org/wiki/Lifted_condensation_level
+
+        Args:
+        - w: Mixing ratio
+        - air_pressure_at_sea_level: Air pressure at sea level
+
+        Returns:
+        - lcl: LCL in meters
+        """
+        # Constants
+        A = 2440
+        B = 0.00029
+
+        # Calculate actual vapor pressure using Magnus-Tetens formula
+        lcl = (A * w) / ((air_pressure_at_sea_level - w) * (1 - B * air_pressure_at_sea_level))
+
+        return lcl
+        
+    async def calculate_lifted_index(self, temperature, altitude, dew_point_temperature, air_pressure_at_sea_level):
+        # https://en.wikipedia.org/wiki/Lifted_index
+        
+        # Constants
+        env_temp_500mb = -20  # Celsius (environmental temperature at 500 mb level)
+
+        # Calculate saturation vapor pressure at surface temperature
+        # Checked with https://www.weather.gov/epz/wxcalc_vaporpressure
+        es = self.calculate_vapor_pressure(temperature)
+
+        # Calculate actual vapor pressure at surface
+        # Checked with https://www.weather.gov/epz/wxcalc_vaporpressure
+        e = self.calculate_vapor_pressure(dew_point_temperature)  #6.112 * (10 ** (7.5 * (Td - Tn) / (Td - 35.85)))
+
+        # Calculate mixing ratio at surface in grams per kilogram
+        # Checked with https://www.weather.gov/epz/wxcalc_mixingratio
+        w = self.calculate_mixing_ratio(e, air_pressure_at_sea_level)
+
+        # Calculate Lifting Condensation Level
+        lcl = self.calculate_lifting_condensation_level(w, air_pressure_at_sea_level)
+        
+        _LOGGER.debug("Air pressure at sea level (AP): {} mbar".format(air_pressure_at_sea_level))
+        _LOGGER.debug("Dew point(DP): {} °C".format(dew_point_temperature))
+        _LOGGER.debug("Temperature (T): {} °C".format(temperature))
+        _LOGGER.debug("Saturation vapor pressure at surface (ES): {} mbar".format(es))
+        _LOGGER.debug("Actual vapor pressure at surface (E): {} mbar".format(e))
+        _LOGGER.debug("Mixing ratio at surface (W): {} grams per kg".format(w))
+        _LOGGER.debug("Lifting Condensation Level (LCL): {} meters".format(lcl))
+        
+        # Calculate temperature of lifted parcel at 500 mb level
+        lifted_temp_500mb = env_temp_500mb + (temperature - lcl) * 0.5  # Assumption: 500 mb is halfway through the troposphere
+
+        # Calculate Lifted Index
+        lifted_index = env_temp_500mb - lifted_temp_500mb
+    
+        _LOGGER.debug("Temperature of the lifted parcel (T Parcel): {} °C".format(lifted_temp_500mb))
+        _LOGGER.debug("Lifted Index (LI): {} °C".format(lifted_index))
 
-        # print("Estimated Atmospheric Lifted Index: {:.2f}".format(lifted_index))
         return lifted_index
 
 
 class AstronomicalTransparency:
     """Calculate astronomical transparency"""
 
     # Write a python3 program to calculate atmospheric transparence based on humidity, temperature, clouds, wind, altitude, dew_point_temperature, and air_pressure_at_sea_level and convert the transparency to magnitude degradation
@@ -122,15 +207,14 @@
         #     return float(2.5)  #float('inf')
         # else:
         #     magnitude_degradation = -2.5 * math.log10(transparency)
         #     magnitude_degradation = max(0, min(2.5, magnitude_degradation))
 
         #     return magnitude_degradation
 
-        # 7Timer
         if transparency == 0:
             return float(MAG_DEGRATION_MAX)  #float('inf')
         else:
             magnitude_degradation = -2.5 * math.log10(transparency)
             magnitude_degradation = max(0, min(MAG_DEGRATION_MAX, magnitude_degradation))
 
             return magnitude_degradation
@@ -164,47 +248,49 @@
 
     # Modell 4:
     # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
     # and altitude above sea level. The seeing factor is then used to calculate the astronomical
     # seeing in arcseconds. The empirical relationship used here states that the seeing in arcseconds
     # is approximately equal to the reciprocal of the seeing factor multiplied by a conversion
     # factor of 0.98.
-    # def calculate_dew_point(self, temperature, humidity):
-    #     alpha = math.log(humidity / 100) + (MAGNUS_COEFFICIENT_A * temperature) / (MAGNUS_COEFFICIENT_B + temperature)
-    #     dew_point = (MAGNUS_COEFFICIENT_B * alpha) / (MAGNUS_COEFFICIENT_A - alpha)
-
-    #     return dew_point
-
     def calculate_saturation_vapor_pressure(self, dew_point):
-        es = 6.11 * (10 ** (7.5 * dew_point / (237.7 + dew_point)))
+        """
+        Calculate the actual vapor pressure at the surface using the Magnus-Tetens formula.
 
-        return es
+        Args:
+        - dew_point: Dew point temperature in Celsius.
 
-    # def calculate_water_vapor_pressure(self, temperature, humidity):
-    #     dew_point = self.calculate_dew_point(temperature, humidity)
-    #     es = self.calculate_saturation_vapor_pressure(dew_point)
-    #     water_vapor_pressure = (humidity / 100) * es
+        Returns:
+        - e: Saturation vapor pressure at the surface in millibars (mb) or hectopascals (hPa).
+        """
+        # Constants
+        A = 6.112
+        B = 17.67
+        C = 243.5
 
-    #     return water_vapor_pressure
+        # Calculate actual vapor pressure using Magnus-Tetens formula
+        es = A * math.exp((B * dew_point) / (dew_point + C))
 
-    def calculate_water_vapor_pressure6(self, dew_point_temperature, humidity):
+        return es
+    
+    def calculate_water_vapor_pressure(self, dew_point_temperature, humidity):
         dew_point = dew_point_temperature
         es = self.calculate_saturation_vapor_pressure(dew_point)
         water_vapor_pressure = (humidity / 100) * es
 
         return water_vapor_pressure
 
     # Modell 6:
     # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
     # and altitude above sea level. It is similar to Model 4 and 5 but uses the air pressure at sea level
     # and dew point provided by Met.no.
-    async def calculate_seeing_model6(
+    async def calculate_seeing_model(
         self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level
     ):
-        water_vapor_pressure = self.calculate_water_vapor_pressure6(dew_point_temperature, humidity)
+        water_vapor_pressure = self.calculate_water_vapor_pressure(dew_point_temperature, humidity)
 
         adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
         relative_pressure = adjusted_pressure / air_pressure_at_sea_level
 
         seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.35 * (wind_speed / 10) ** 0.65 * relative_pressure
         seeing = 0.98 / seeing_factor
 
@@ -222,29 +308,22 @@
         )
 
         if seeing > 2.5:
             seeing = 2.5  # max out seeing
 
         return seeing
 
-    def calculate_water_vapor_pressure7(self, dew_point_temperature, humidity):
-        dew_point = dew_point_temperature
-        es = self.calculate_saturation_vapor_pressure(dew_point)
-        water_vapor_pressure = (humidity / 100) * es
-
-        return water_vapor_pressure
-
     # Modell 7:
     # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
     # and altitude above sea level. It is similar to Model 6 but takes the cloud coverage into account.
     # This somehow doesn't seem to be correct, since seeing can be good even with clouds.
     async def calculate_seeing_model7(
         self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level
     ):
-        water_vapor_pressure = self.calculate_water_vapor_pressure7(dew_point_temperature, humidity)
+        water_vapor_pressure = self.calculate_water_vapor_pressure(dew_point_temperature, humidity)
 
         adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
         relative_pressure = adjusted_pressure / air_pressure_at_sea_level
 
         # Take care on the clouds
         cloud_factor = 1 - (cloud_cover / 100)
 
@@ -294,15 +373,15 @@
         self._elevation = elevation
         self._timezone_info = timezone_info
         # tz_find = TimezoneFinder()
         # self._timezone_info = tz_find.timezone_at(lng=longitude, lat=latitude)
         self._test_mode = False
         _LOGGER.debug("Timezone: %s", self._timezone_info)
         if forecast_time is None:
-            self._forecast_time = datetime.utcnow().replace(tzinfo=pytz.utc)
+            self._forecast_time = datetime.now(timezone.utc).replace(tzinfo=pytz.utc)
         else:
             self._forecast_time = forecast_time.replace(tzinfo=pytz.utc)
             self._test_mode = True
         _LOGGER.debug("Forecast Time: %s", self._forecast_time)
 
         self._sun_observer = None
         self._sun_observer_nautical = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.0.dev7/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev6
+Version: 0.50.0.dev7
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev6/setup.py` & `pyastroweatherio-0.50.0.dev7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.0.dev6",
+    version="0.50.0.dev7",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

