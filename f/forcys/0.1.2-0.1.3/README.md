# Comparing `tmp/forcys-0.1.2.tar.gz` & `tmp/forcys-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forcys-0.1.2.tar", max compression
+gzip compressed data, was "forcys-0.1.3.tar", max compression
```

## Comparing `forcys-0.1.2.tar` & `forcys-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1084 2024-03-08 13:59:43.119628 forcys-0.1.2/LICENSE
--rw-r--r--   0        0        0      607 2024-03-31 12:04:08.812534 forcys-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-06 19:05:54.690190 forcys-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-06 20:07:50.660956 forcys-0.1.2/src/forcys/__init__.py
--rw-r--r--   0        0        0      130 2024-03-07 13:32:00.288910 forcys-0.1.2/src/forcys/time_funcs.py
--rw-r--r--   0        0        0     3964 2024-03-31 12:03:18.222055 forcys-0.1.2/src/forcys/wavedata.py
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 forcys-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-03-08 13:59:43.119628 forcys-0.1.3/LICENSE
+-rw-r--r--   0        0        0      683 2024-05-03 12:37:39.338418 forcys-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-06 19:05:54.690190 forcys-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-06 20:07:50.660956 forcys-0.1.3/src/forcys/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-07 21:46:34.267046 forcys-0.1.3/src/forcys/nc/__init__.py
+-rw-r--r--   0        0        0     2960 2024-04-13 14:34:33.992161 forcys-0.1.3/src/forcys/nc/nc_datafile.py
+-rw-r--r--   0        0        0     4212 2024-04-13 12:18:02.262895 forcys-0.1.3/src/forcys/nc/nc_variable.py
+-rw-r--r--   0        0        0      130 2024-03-07 13:32:00.288910 forcys-0.1.3/src/forcys/time_funcs.py
+-rw-r--r--   0        0        0     5280 2024-04-06 16:30:50.743155 forcys-0.1.3/src/forcys/wavedata.py
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 forcys-0.1.3/PKG-INFO
```

### Comparing `forcys-0.1.2/LICENSE` & `forcys-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `forcys-0.1.2/pyproject.toml` & `forcys-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forcys"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["panagop <gpanagop@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "forcys", from = "src" }
 ]
 
@@ -19,12 +19,15 @@
 jupyter = "^1.0.0"
 lab = "^8.1"
 seaborn = "^0.13.2"
 copernicusmarine = "^1.0.4"
 twine = "^5.0.0"
 virocon = "^2.3.0"
 cdsapi = "^0.6.1"
+streamlit-authenticator = "^0.3.2"
+eqsig = "^1.2.11"
+openpyxl = "^3.1.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `forcys-0.1.2/src/forcys/wavedata.py` & `forcys-0.1.3/src/forcys/wavedata.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ﻿from dataclasses import dataclass
 from functools import cached_property
 import netCDF4
 import numpy as np
-from datetime import datetime, timedelta
+from datetime import datetime  # , timedelta
+from scipy.interpolate import griddata
 
 
 @dataclass
 class WaveDataFile:
     """WaveDataFile class"""
     dataset: netCDF4.Dataset
 
@@ -81,18 +82,52 @@
     def min_value(self) -> float:
         return self.values.min()
 
     @cached_property
     def max_value(self) -> float:
         return self.values.max()
 
+    def get_point_interpolation_at_time_index(
+            self, lat: float, lon: float,
+            time_index: int) -> float:
+        # Create meshgrid of longitude and latitude
+        lon_grid, lat_grid = np.meshgrid(self.wdf.lon, self.wdf.lat)
+
+        data_values_at_time = self.values[time_index]
+        # Flatten the arrays
+        lon_flat = lon_grid.flatten()
+        lat_flat = lat_grid.flatten()
+        data_flat = data_values_at_time.flatten()
+
+        # Interpolate the data to the new location
+        interpolated_value = griddata(
+            (lon_flat, lat_flat), data_flat, (lon, lat), method='linear')
+
+        return interpolated_value
+
+    def get_interpolations(self, lat: float, lon: float) -> np.ma.masked_array:
+        """
+        Get values from a masked array at specified coordinates across all arrays.
+
+        Parameters:
+            lat (float): Latitude.
+            lon (float): Longitude.
+
+        Returns:
+            np.ma.masked_array: Array of values at the specified coords
+                                for each time step.
+        """
+        lat_index = np.where(self.wdf.lat == lat)[0][0]
+        lon_index = np.where(self.wdf.lon == lon)[0][0]
+        return self.values[:, lat_index, lon_index]
+
     def get_time_history_at_indices(
             self, lat_index: int, lon_index: int) -> np.ma.masked_array:
-            # start_date_index: int = 0,
-            # end_date_index: int = -1) -> np.ma.masked_array:
+        # start_date_index: int = 0,
+        # end_date_index: int = -1) -> np.ma.masked_array:
         """
         Get values from a masked array at specified indices across all arrays.
 
         Parameters:
             lat_index (int): Index along the lat dimension.
             lon_index (int): Index along the lon dimension.
```

