# Comparing `tmp/molecularprofiles-0.5.6.tar.gz` & `tmp/molecularprofiles-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularprofiles-0.5.6.tar", last modified: Wed Nov 15 08:20:28 2023, max compression
+gzip compressed data, was "molecularprofiles-0.5.7.tar", last modified: Fri May  3 15:14:01 2024, max compression
```

## Comparing `molecularprofiles-0.5.6.tar` & `molecularprofiles-0.5.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mexanick   (501) staff       (20)        0 2023-11-15 08:20:28.577272 molecularprofiles-0.5.6/
--rw-r--r--   0 mexanick   (501) staff       (20)     1474 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/LICENSE
--rw-r--r--   0 mexanick   (501) staff       (20)     3269 2023-11-15 08:20:28.576413 molecularprofiles-0.5.6/PKG-INFO
--rw-r--r--   0 mexanick   (501) staff       (20)      450 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/README.md
--rw-r--r--   0 mexanick   (501) staff       (20)     1638 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/pyproject.toml
--rw-r--r--   0 mexanick   (501) staff       (20)       38 2023-11-15 08:20:28.577409 molecularprofiles-0.5.6/setup.cfg
-drwxr-xr-x   0 mexanick   (501) staff       (20)        0 2023-11-15 08:20:28.529371 molecularprofiles-0.5.6/src/
-drwxr-xr-x   0 mexanick   (501) staff       (20)        0 2023-11-15 08:20:28.543972 molecularprofiles-0.5.6/src/molecularprofiles/
--rwxr-xr-x   0 mexanick   (501) staff       (20)      195 2023-11-15 08:19:58.000000 molecularprofiles-0.5.6/src/molecularprofiles/__init__.py
--rwxr-xr-x   0 mexanick   (501) staff       (20)    21225 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/src/molecularprofiles/molecularprofiles.py
-drwxr-xr-x   0 mexanick   (501) staff       (20)        0 2023-11-15 08:20:28.572939 molecularprofiles-0.5.6/src/molecularprofiles/utils/
--rw-r--r--   0 mexanick   (501) staff       (20)       27 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/src/molecularprofiles/utils/__init__.py
--rwxr-xr-x   0 mexanick   (501) staff       (20)     2169 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/src/molecularprofiles/utils/constants.py
--rwxr-xr-x   0 mexanick   (501) staff       (20)     9086 2023-11-15 08:19:58.000000 molecularprofiles-0.5.6/src/molecularprofiles/utils/grib_utils.py
--rwxr-xr-x   0 mexanick   (501) staff       (20)    10490 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/src/molecularprofiles/utils/humidity.py
--rw-r--r--   0 mexanick   (501) staff       (20)      327 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/src/molecularprofiles/utils/mdps_log.conf
--rw-r--r--   0 mexanick   (501) staff       (20)    14694 2023-11-15 07:59:14.000000 molecularprofiles-0.5.6/src/molecularprofiles/utils/rayleigh.py
-drwxr-xr-x   0 mexanick   (501) staff       (20)        0 2023-11-15 08:20:28.549564 molecularprofiles-0.5.6/src/molecularprofiles.egg-info/
--rw-r--r--   0 mexanick   (501) staff       (20)     3269 2023-11-15 08:20:28.000000 molecularprofiles-0.5.6/src/molecularprofiles.egg-info/PKG-INFO
--rw-r--r--   0 mexanick   (501) staff       (20)      578 2023-11-15 08:20:28.000000 molecularprofiles-0.5.6/src/molecularprofiles.egg-info/SOURCES.txt
--rw-r--r--   0 mexanick   (501) staff       (20)        1 2023-11-15 08:20:28.000000 molecularprofiles-0.5.6/src/molecularprofiles.egg-info/dependency_links.txt
--rw-r--r--   0 mexanick   (501) staff       (20)      193 2023-11-15 08:20:28.000000 molecularprofiles-0.5.6/src/molecularprofiles.egg-info/requires.txt
--rw-r--r--   0 mexanick   (501) staff       (20)       18 2023-11-15 08:20:28.000000 molecularprofiles-0.5.6/src/molecularprofiles.egg-info/top_level.txt
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.289250 molecularprofiles-0.5.7/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     1474 2022-11-22 15:24:35.000000 molecularprofiles-0.5.7/LICENSE
+-rw-r--r--   0 mdalchen   (501) staff       (20)     3269 2024-05-03 15:14:01.288790 molecularprofiles-0.5.7/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)      450 2023-02-01 16:41:16.000000 molecularprofiles-0.5.7/README.md
+-rw-r--r--   0 mdalchen   (501) staff       (20)     1638 2023-07-21 08:41:06.000000 molecularprofiles-0.5.7/pyproject.toml
+-rw-r--r--   0 mdalchen   (501) staff       (20)       38 2024-05-03 15:14:01.289323 molecularprofiles-0.5.7/setup.cfg
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.279369 molecularprofiles-0.5.7/src/
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.281453 molecularprofiles-0.5.7/src/molecularprofiles/
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)      195 2024-05-03 15:10:02.000000 molecularprofiles-0.5.7/src/molecularprofiles/__init__.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    24137 2024-05-03 15:07:02.000000 molecularprofiles-0.5.7/src/molecularprofiles/molecularprofiles.py
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.286605 molecularprofiles-0.5.7/src/molecularprofiles/utils/
+-rw-r--r--   0 mdalchen   (501) staff       (20)       27 2023-02-03 15:27:32.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/__init__.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)     2168 2024-05-03 15:07:02.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/constants.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)     8758 2024-05-03 15:09:25.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/grib_utils.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    10490 2023-07-21 08:41:06.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/humidity.py
+-rw-r--r--   0 mdalchen   (501) staff       (20)      327 2023-02-03 15:27:32.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/mdps_log.conf
+-rw-r--r--   0 mdalchen   (501) staff       (20)    14694 2023-07-21 08:41:06.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/rayleigh.py
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.287265 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     3269 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)      578 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)        1 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)      193 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/requires.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)       18 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/top_level.txt
```

### Comparing `molecularprofiles-0.5.6/LICENSE` & `molecularprofiles-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularprofiles-0.5.6/PKG-INFO` & `molecularprofiles-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.5.6
+Version: 0.5.7
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `molecularprofiles-0.5.6/pyproject.toml` & `molecularprofiles-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molecularprofiles-0.5.6/src/molecularprofiles/molecularprofiles.py` & `molecularprofiles-0.5.7/src/molecularprofiles/molecularprofiles.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 Mykhailo Dalchenko (mykhailo.dalchenko@unige.ch) and
 Georgios Voutsinas (georgios.voutsinas@unige.ch)
 """
 
 import os
 import sys
 import logging
-import json
-import itertools
 
 import astropy.units as u
 from astropy.table import Table, QTable, vstack, Column
 import numpy as np
 from scipy.interpolate import interp1d
 from bisect import bisect_left
 
@@ -159,34 +157,100 @@
         }
 
     def _refractive_index(self, P, T, RH, wavelength, C):
         """Wrapper for Rayleigh.calculate_n()."""
         rayleigh = Rayleigh(wavelength, C, P, T, RH)
         return rayleigh.refractive_index
 
-    def _take_closest(self, myList, myNumber):
+    def _take_closest(self, my_list, my_number):
         """
-        Returns closest value to myNumber.
+        Returns closest value to my_number.
         If two numbers are equally close, return the smallest number.
         This function comes from the answer of user:
         https://stackoverflow.com/users/566644/lauritz-v-thaulow
         found in stack overflow post:
         https://stackoverflow.com/questions/12141150/from-list-of-integers-get-number-closest-to-a-given-value/12141511#12141511
         """
-        pos = bisect_left(myList, myNumber)
+        pos = bisect_left(my_list, my_number)
         if pos == 0:
-            return myList[0]
-        if pos == len(myList):
-            return myList[-1]
-        before = myList[pos - 1]
-        after = myList[pos]
-        if after - myNumber < myNumber - before:
+            return my_list[0]
+        if pos == len(my_list):
+            return my_list[-1]
+        before = my_list[pos - 1]
+        after = my_list[pos]
+        if after - my_number < my_number - before:
             return after
-        else:
-            return before
+        return before
+
+    def _get_data_altitude_range(self, altitude_profile):
+        """
+        Calculates the floor and ceiling of the available DAS data.
+
+        Parameters:
+        -----------
+        altitude_profile : Quantity
+            Tuple with the altitudes that the atmospheric parameters will be calculated. Units of length.
+        Returns:
+        --------
+            floor, ceiling : Quantities that define the highest and lowest altitude that DAS data are available.
+        """
+
+        floor = self._take_closest(
+            altitude_profile,
+            (
+                (self.stat_description["avg"]["Altitude"][-1])
+                * (self.stat_description["avg"]["Altitude"].unit)
+            ).to(altitude_profile.unit),
+        )
+        ceiling = self._take_closest(
+            altitude_profile,
+            (
+                (self.stat_description["avg"]["Altitude"][0])
+                * (self.stat_description["avg"]["Altitude"].unit)
+            ).to(altitude_profile.unit),
+        )
+        return floor, ceiling
+
+    def _create_profile(self, interpolation_centers):
+        """Interpolates atmospheric parameters in the requested interpolation centers"""
+
+        temperature = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"].to(u.km),
+                self.stat_description["avg"]["Temperature"],
+                interpolation_centers.to(u.km),
+            )
+            * self.stat_description["avg"]["Temperature"].unit
+        )
+        relative_humidity = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"].to(u.km),
+                self.stat_description["avg"]["Relative humidity"],
+                interpolation_centers.to(u.km),
+            )
+            * self.stat_description["avg"]["Relative humidity"].unit
+        )
+        pressure = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"].to(u.km),
+                self.stat_description["avg"]["Pressure"],
+                interpolation_centers.to(u.km),
+            )
+            * self.stat_description["avg"]["Pressure"].unit
+        )
+        density = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"].to(u.km),
+                self.stat_description["avg"]["Density"],
+                interpolation_centers.to(u.km),
+            )
+            * self.stat_description["avg"]["Density"].unit
+            / N0_AIR
+        )
+        return temperature, relative_humidity, pressure, density
 
     def _pick_up_reference_atmosphere(self, ceiling, floor, reference_atmosphere):
         """
         Picks up the reference atmosphere corresponding to the season and
         the geographical location. It selects all rows above the given ceiling.
 
         Parameters:
@@ -210,15 +274,15 @@
             sys.exit(1)
         try:
             mask = (
                 reference_atmosphere_table["altitude"]
                 >= ceiling.to(reference_atmosphere_table["altitude"].unit)
             ) | (
                 reference_atmosphere_table["altitude"]
-                < floor.to(reference_atmosphere_table["altitude"].unit)
+                <= floor.to(reference_atmosphere_table["altitude"].unit)
             )
             return reference_atmosphere_table[mask]
         except Exception as ex:
             template = "An exception of type {0} occurred. Arguments:\n{1!r}"
             message = template.format(type(ex).__name__, ex.args)
             logger.error(message)
             sys.exit(1)
@@ -253,62 +317,24 @@
             Tuple with the altitudes that the atmospheric parameters will be calculated. Units of length.
 
         Returns:
         --------
             Ecsv file in the style of a CORSIKA atmospheric configuration file.
         """
 
-        if floor is None:
-            floor = (self.stat_description["avg"]["Altitude"][-1]) * self.stat_description["avg"][
-                "Altitude"
-            ].unit
-        ceiling = self._take_closest(
-            altitude_list.to(self.stat_description["avg"]["Altitude"].unit),
-            (self.stat_description["avg"]["Altitude"][0])
-            * self.stat_description["avg"]["Altitude"].unit,
+        floor, ceiling = self._get_data_altitude_range(
+            altitude_list.to(self.stat_description["avg"]["Altitude"].unit)
         )
         altitude = altitude_list[
-            (altitude_list.to_value() >= floor.to_value(altitude_list.unit))
+            (altitude_list.to_value() > floor.to_value(altitude_list.unit))
             & (altitude_list.to_value() < ceiling.to_value(altitude_list.unit))
         ]
         altitude = altitude.to(self.stat_description["avg"]["Altitude"].unit)
-        temperature = (
-            self._interpolate_cubic(
-                self.stat_description["avg"]["Altitude"],
-                self.stat_description["avg"]["Temperature"],
-                altitude,
-            )
-            * self.stat_description["avg"]["Temperature"].unit
-        )
-        relative_humidity = (
-            self._interpolate_cubic(
-                self.stat_description["avg"]["Altitude"],
-                self.stat_description["avg"]["Relative humidity"],
-                altitude,
-            )
-            * self.stat_description["avg"]["Relative humidity"].unit
-        )
-        pressure = (
-            self._interpolate_cubic(
-                self.stat_description["avg"]["Altitude"],
-                self.stat_description["avg"]["Pressure"],
-                altitude,
-            )
-            * self.stat_description["avg"]["Pressure"].unit
-        )
+        temperature, relative_humidity, pressure, density = self._create_profile(altitude)
         thickness = pressure / STD_GRAVITATIONAL_ACCELERATION
-        density = (
-            self._interpolate_cubic(
-                self.stat_description["avg"]["Altitude"],
-                self.stat_description["avg"]["Density"],
-                altitude,
-            )
-            * self.stat_description["avg"]["Density"].unit
-            / N0_AIR
-        )
         rel_water_vapor_pressure = (
             partial_pressure_water_vapor(temperature, relative_humidity) / pressure
         ).decompose()
         rel_refractive_index = (
             self._refractive_index(
                 pressure, temperature, relative_humidity, 350.0 * u.nm, co2_concentration
             )
@@ -368,17 +394,16 @@
             sys.exit(1)
 
     def rayleigh_extinction(
         self,
         rayleigh_extinction_file,
         co2_concentration,
         wavelength_min=200 * u.nm,
-        wavelength_max=1000 * u.nm,
+        wavelength_max=700 * u.nm,
         reference_atmosphere=None,
-        altitude_list=STD_CORSIKA_ALTITUDE_PROFILE,
         rayleigh_scattering_altitude_bins=RAYLEIGH_SCATTERING_ALTITUDE_BINS,
     ):
         """
         Calculates the absolute integral optical depth due to Rayleigh scattering
         per altitude bins as a function of wavelength.
         The optical depth (AOD) for an altitude h over the observatory will be given by
         the integral of the monochromatic volume coefficient beta, with integration limits
@@ -387,67 +412,36 @@
         Parameters:
         -----------
         rayleigh_extinction_file : string
             Name of the returned file with the extinction profile.
         co2_concentration : float
             12MACOBAC value
         wavelength_min : Quantity
-
         wavelength_max : Quantity
-
         reference_atmosphere : path
             The path where the file with the reference atmosphere model is located.
-        altitude_list : Quantity
-            Tuple with the altitudes that the atmospheric parameters will be calculated. Units of length.
         rayleigh_scattering_altitude_bins : Quantity
             Tuple with the altitudes that the AOD will be calculated. Units of length.
 
         Returns:
         --------
             Ecsv file with absolute optical depth per altitude bin per wavelength bin. The data model is the same with MODTRAN files.
         """
 
-        floor = rayleigh_scattering_altitude_bins[0].to(u.km)
-        ceiling = self._take_closest(
-            altitude_list.to(self.stat_description["avg"]["Altitude"].unit),
-            (self.stat_description["avg"]["Altitude"][0])
-            * self.stat_description["avg"]["Altitude"].unit,
-        )
+        floor, ceiling = self._get_data_altitude_range(rayleigh_scattering_altitude_bins)
         altitude = rayleigh_scattering_altitude_bins.to(u.km)
-        if ceiling.to_value(u.km) > 7.0:
-            altitude_middle = np.arange(7.0, ceiling.to_value(u.km), 1)
-            altitude = (
-                np.concatenate((altitude.to_value(u.km), altitude_middle))
-            ) * rayleigh_scattering_altitude_bins.unit
+        altitude = altitude[altitude < ceiling]
 
         interpolation_centers = (altitude[:-1] + altitude[1:]) / 2
-        temperature_lower = (
-            self._interpolate_cubic(
-                self.stat_description["avg"]["Altitude"].to(u.km),
-                self.stat_description["avg"]["Temperature"],
-                interpolation_centers.to(u.km),
-            )
-            * self.stat_description["avg"]["Temperature"].unit
-        )
-        relative_humidity_lower = (
-            self._interpolate_cubic(
-                self.stat_description["avg"]["Altitude"].to(u.km),
-                self.stat_description["avg"]["Relative humidity"],
-                interpolation_centers.to(u.km),
-            )
-            * self.stat_description["avg"]["Relative humidity"].unit
-        )
-        pressure_lower = (
-            self._interpolate_cubic(
-                self.stat_description["avg"]["Altitude"].to(u.km),
-                self.stat_description["avg"]["Pressure"],
-                interpolation_centers.to(u.km),
-            )
-            * self.stat_description["avg"]["Pressure"].unit
-        )
+        (
+            temperature_lower,
+            relative_humidity_lower,
+            pressure_lower,
+            density_lower,
+        ) = self._create_profile(interpolation_centers)
 
         # Concatenate with reference atmosphere
         if reference_atmosphere:
             reference_atmosphere_table = self._pick_up_reference_atmosphere(
                 ceiling, floor, reference_atmosphere
             )
             length_of_columns = len(reference_atmosphere_table)
@@ -470,28 +464,30 @@
         else:
             logger.info(
                 "Since the reference atmosphere was not provided, the resulting atmospheric model will be constrained to the extent of the provided meteorological data."
             )
             temperature = temperature_lower
             pressure = pressure_lower
             relative_humidity = relative_humidity_lower
+
         t = QTable(
             [altitude[1:], pressure, temperature, relative_humidity],
             names=("altitude", "pressure", "temperature", "relative_humidity"),
         )
         t.sort("altitude")
         bin_widths = np.diff(np.sort(altitude))
         t["bin_widths"] = bin_widths
         mask = t["altitude"] > floor
         wavelength_range = (
             np.arange(wavelength_min.to_value(u.nm), wavelength_max.to_value(u.nm), 1) * u.nm
         )
-        rayleigh_extinction_table = Table(names=wavelength_range)
-        col_alt_max = Column(name="altitude_max")
-        col_alt_min = Column(name="altitude_min")
+        aod_units = len(wavelength_range) * [u.dimensionless_unscaled]
+        rayleigh_extinction_table = Table(names=wavelength_range, units=aod_units)
+        col_alt_max = Column(name="altitude_max", unit=u.km)
+        col_alt_min = Column(name="altitude_min", unit=u.km)
         rayleigh_extinction_table.add_columns([col_alt_max, col_alt_min], indexes=[0, 0])
         aod_dict = {
             aod: 0
             for aod in np.arange(wavelength_min.to_value(u.nm), wavelength_max.to_value(u.nm))
         }
         for row in t[mask]:
             new_row = []
@@ -508,7 +504,76 @@
                 beta = rayleigh.beta
                 aod = row["bin_widths"] * beta
                 aod_dict[wavelength.to_value(u.nm)] += aod
                 new_row.append(aod_dict[wavelength.to_value(u.nm)])
             rayleigh_extinction_table.add_row(new_row)
         rayleigh_extinction_table.write(rayleigh_extinction_file, overwrite=True)
         return rayleigh_extinction_file
+
+    def convert_to_simtel_compatible(self, input_ecsv_file, output_file, observation_altitude):
+        """
+        Converts an ecsv file of an extinction profile to a format digestible by sim_telarray.
+        Parameters:
+        -----------
+        input_ecsv_file : string
+            Name of the input extinction profile file in ecsv format.
+        output_file : string
+            Name of the output extinction profile file in simtel digestible format.
+        observation_altitude : quantity
+            Starting altitude measured from sea level.
+        """
+        extinction_table = QTable.read(input_ecsv_file)
+        with open(output_file, "w") as f:
+            H2 = observation_altitude.to_value(u.km)
+            H1 = extinction_table["altitude_max"].to_value(u.km)
+            list_of_altitude_bins = f"# H2= {H2:.3f}, H1= "
+            for height in H1:
+                list_of_altitude_bins += f"{height:.3f}\t"
+            list_of_altitude_bins += "\n"
+            f.writelines(list_of_altitude_bins)
+            for wl in extinction_table.columns:
+                if wl not in ("altitude_max", "altitude_min"):
+                    file_line = [str(wl).split(" ")[0], "\t"]
+                    for aod in extinction_table[wl]:
+                        file_line += [f"{aod:.6f}", "\t"]
+                    file_line += ["\n"]
+                    f.writelines(file_line)
+
+    def timeseries_analysis(self, outfile, altitude_list=STD_CORSIKA_ALTITUDE_PROFILE):
+        """
+        Analyses timeseries of meteorological data.
+        It produces an astropy table with the scaled exponential density at 15km a.s.l. as a function of the MJD.
+        This timeseries is used for the identification of seasons.
+        outfile : string
+            Name of the produced file where the table is stored.
+        altitude_list : Quantity
+            Tuple with the altitudes that the atmospheric parameters will be calculated. Units of length.
+        """
+
+        output_table = QTable()
+        tables = []
+        floor = 1 * u.km
+        ceiling = 20 * u.km
+        altitude = altitude_list[
+            (altitude_list.to_value() >= floor.to_value(altitude_list.unit))
+            & (altitude_list.to_value() < ceiling.to_value(altitude_list.unit))
+        ]
+
+        self.data["MJD"] = self.data["Timestamp"].mjd
+        test_table = self.data.group_by("MJD")
+        indices = test_table.groups.indices
+        for first, second in zip(indices, indices[1:]):
+            t = test_table[first:second]
+            n_exp = (
+                self._interpolate_cubic(
+                    t["Altitude"],
+                    t["Exponential Density"],
+                    altitude,
+                )
+                * u.dimensionless_unscaled
+            )
+            current_table = QTable([n_exp, altitude], names=("n_exp", "altitude"))
+            current_table["mjd"] = t["MJD"][1]
+            mask = current_table["altitude"] == 15000 * u.m
+            tables.append(current_table[mask])
+        output_table = vstack(tables)
+        output_table.write(outfile, overwrite=True)
```

### Comparing `molecularprofiles-0.5.6/src/molecularprofiles/utils/constants.py` & `molecularprofiles-0.5.7/src/molecularprofiles/utils/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # standard atmosphere thermodynamic values
 STD_NUMBER_DENSITY = (
     2.546899e19 / u.cm**3
 )  # [cm^-3] molecular number density for standard air conditions
 STD_AIR_PRESSURE = 1013.25 * u.hPa  # [hPa]   standard air pressure
 STD_AIR_TEMPERATURE = 288.15 * u.K  # [K]     standard air temperature
 STD_AIR_DENSITY = 1.225 * u.kg / u.m**3  # [kg/m^3] standard air density
-DENSITY_SCALE_HEIGHT = 9500.0 * u.km  # [km]    density scale hight for La Palma Winter
+DENSITY_SCALE_HEIGHT = 9500.0 * u.m  # [km]    density scale hight for La Palma Winter
 STD_RELATIVE_HUMIDITY = 45.9 * u.percent  # [%]     standard air rel. humidity
 # atmospheric composition
 NITROGEN_RATIO = 0.78084 * u.dimensionless_unscaled
 OXYGEN_RATIO = 0.20946 * u.dimensionless_unscaled
 ARGON_RATIO = 0.00934 * u.dimensionless_unscaled
 GAS_CONSTANT = 8.31451 * u.J / (u.K * u.mol)  # gas constant [J/mol/K]
 MOLAR_MASS_WATER_VAPOR = 0.018015 * u.kg / u.mol  # molar mass of water vapor [kg/mol]
```

### Comparing `molecularprofiles-0.5.6/src/molecularprofiles/utils/grib_utils.py` & `molecularprofiles-0.5.7/src/molecularprofiles/utils/grib_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,22 +163,16 @@
 
     Returns
     -------
     astropy.table.Table
         Table with grib file data gridded in isobaric levels
     """
 
-    logger.debug("Working with %s", filename)
-    logger.debug("Getting all variable names...")
     variable_names, variable_short_names = get_gribfile_variables(filename)
-    logger.info("Indexing the file %s (this might take a while...)", filename)
-    grib_file = pg.index(filename, "shortName", "typeOfLevel")
-    logger.debug(
-        "Selecting the parameters information for %s (this might take a while...)", filename
-    )
+    grib_file = pg.open(filename)
     gpm = u.def_unit("gpm", u.m)
     u.add_enabled_units([gpm])
     data = Table()
     for short_name in variable_short_names:
         if short_name == "unknown":
             continue
         var = grib_file.select(shortName=short_name, typeOfLevel="isobaricInhPa")
@@ -207,14 +201,15 @@
     astropy.table.Table
         Table with grib data
     Returns
     -------
     astropy.table.Table
         Extended table with grib data and additional quantities
     """
+
     logger.debug("Check for gaps in relative humidity and fill them if neccessary")
     data["Relative humidity"] = data["Relative humidity"].filled(0)
     logger.debug("Compute altitude from geopotential")
     if "Geopotential height" in data.keys():
         data["Altitude"] = get_altitude_from_geopotential_height(
             data["Geopotential height"], data["Latitude"]
         )
@@ -293,13 +288,14 @@
     Merge ecsv files
 
     Parameters
     ----------
     data_path: path-like
         Path to the folder with GRIB/GRIB2 data files
     """
-    merged_data = Table()
+    tables = []
     for tfile in os.listdir(data_path):
         if tfile.endswith(".ecsv"):
-            data = Table.read(f"{data_path}/{tfile}")
-            merged_data = vstack([merged_data, data])
+            tables.append(Table.read(f"{data_path}/{tfile}"))
+    merged_data = vstack(tables)
+    del tables
     save_grib_table(merged_data, f"{data_path}/merged_file.ecsv")
```

### Comparing `molecularprofiles-0.5.6/src/molecularprofiles/utils/humidity.py` & `molecularprofiles-0.5.7/src/molecularprofiles/utils/humidity.py`

 * *Files identical despite different names*

### Comparing `molecularprofiles-0.5.6/src/molecularprofiles/utils/rayleigh.py` & `molecularprofiles-0.5.7/src/molecularprofiles/utils/rayleigh.py`

 * *Files identical despite different names*

### Comparing `molecularprofiles-0.5.6/src/molecularprofiles.egg-info/PKG-INFO` & `molecularprofiles-0.5.7/src/molecularprofiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.5.6
+Version: 0.5.7
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `molecularprofiles-0.5.6/src/molecularprofiles.egg-info/SOURCES.txt` & `molecularprofiles-0.5.7/src/molecularprofiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

