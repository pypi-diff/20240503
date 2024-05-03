# Comparing `tmp/aixweather-0.1.6.tar.gz` & `tmp/aixweather-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixweather-0.1.6.tar", last modified: Thu May  2 16:25:20 2024, max compression
+gzip compressed data, was "aixweather-0.1.7.tar", last modified: Fri May  3 16:32:51 2024, max compression
```

## Comparing `aixweather-0.1.6.tar` & `aixweather-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/AixWeather.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8385 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1526 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      233 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-02 15:56:22.000000 aixweather-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8385 2024-05-02 16:25:20.808354 aixweather-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6882 2024-05-02 15:56:22.000000 aixweather-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-02 16:12:55.000000 aixweather-0.1.6/aixweather/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/core_data_format_2_output_file/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27093 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_epw_energyplus.py
--rw-rw-rw-   0 root         (0) root         (0)    12087 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_mos_TMY3.py
--rw-rw-rw-   0 root         (0) root         (0)     5031 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/unconverted_to_x.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/data_quality_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/imports/
--rw-rw-rw-   0 root         (0) root         (0)    12879 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/DWD.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/EPW.py
--rw-rw-rw-   0 root         (0) root         (0)     4658 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/ERC.py
--rw-rw-rw-   0 root         (0) root         (0)     5597 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/TRY.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/custom_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/utils_import.py
--rw-rw-rw-   0 root         (0) root         (0)    15038 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/project_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/transformation_functions/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5321 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/auxiliary.py
--rw-rw-rw-   0 root         (0) root         (0)     9673 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/pass_through_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/time_observation_transformations.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/unit_conversions.py
--rw-rw-rw-   0 root         (0) root         (0)    11311 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/variable_transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/aixweather/transformation_to_core_data/
--rw-rw-rw-   0 root         (0) root         (0)    13247 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/DWD.py
--rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/EPW.py
--rw-rw-rw-   0 root         (0) root         (0)     4022 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/ERC.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/TRY.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/custom_file.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 16:25:20.808354 aixweather-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-05-02 15:56:23.000000 aixweather-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3337 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_DWD_forecast.py
--rw-rw-rw-   0 root         (0) root         (0)     3245 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_DWD_historical.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_EPW.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_ERC.py
--rw-rw-rw-   0 root         (0) root         (0)     2184 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_TRY.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2024-05-02 15:56:24.000000 aixweather-0.1.6/tests/test_output_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.533656 aixweather-0.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.529656 aixweather-0.1.7/AixWeather.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8432 2024-05-03 16:32:51.000000 aixweather-0.1.7/AixWeather.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-03 16:32:51.000000 aixweather-0.1.7/AixWeather.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:32:51.000000 aixweather-0.1.7/AixWeather.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-03 16:32:51.000000 aixweather-0.1.7/AixWeather.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-03 16:32:51.000000 aixweather-0.1.7/AixWeather.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-03 15:54:37.000000 aixweather-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8432 2024-05-03 16:32:51.533656 aixweather-0.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6882 2024-05-03 15:54:37.000000 aixweather-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.525656 aixweather-0.1.7/aixweather/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-03 16:24:29.000000 aixweather-0.1.7/aixweather/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.529656 aixweather-0.1.7/aixweather/core_data_format_2_output_file/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/core_data_format_2_output_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27093 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/core_data_format_2_output_file/to_epw_energyplus.py
+-rw-rw-rw-   0 root         (0) root         (0)    12087 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/core_data_format_2_output_file/to_mos_TMY3.py
+-rw-rw-rw-   0 root         (0) root         (0)     5031 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/core_data_format_2_output_file/unconverted_to_x.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/data_quality_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.529656 aixweather-0.1.7/aixweather/imports/
+-rw-rw-rw-   0 root         (0) root         (0)    12879 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/imports/DWD.py
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/imports/EPW.py
+-rw-rw-rw-   0 root         (0) root         (0)     4658 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/imports/ERC.py
+-rw-rw-rw-   0 root         (0) root         (0)     5691 2024-05-03 16:24:29.000000 aixweather-0.1.7/aixweather/imports/TRY.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/imports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/imports/custom_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/imports/utils_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    15038 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/project_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.529656 aixweather-0.1.7/aixweather/transformation_functions/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5321 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_functions/auxiliary.py
+-rw-rw-rw-   0 root         (0) root         (0)     9673 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_functions/pass_through_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_functions/time_observation_transformations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_functions/unit_conversions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11311 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_functions/variable_transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.529656 aixweather-0.1.7/aixweather/transformation_to_core_data/
+-rw-rw-rw-   0 root         (0) root         (0)    13247 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_to_core_data/DWD.py
+-rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_to_core_data/EPW.py
+-rw-rw-rw-   0 root         (0) root         (0)     4022 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_to_core_data/ERC.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_to_core_data/TRY.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_to_core_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2024-05-03 15:54:37.000000 aixweather-0.1.7/aixweather/transformation_to_core_data/custom_file.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 16:32:51.533656 aixweather-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2024-05-03 15:54:38.000000 aixweather-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:32:51.529656 aixweather-0.1.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3337 2024-05-03 15:54:38.000000 aixweather-0.1.7/tests/test_DWD_forecast.py
+-rw-rw-rw-   0 root         (0) root         (0)     3245 2024-05-03 15:54:38.000000 aixweather-0.1.7/tests/test_DWD_historical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-03 15:54:38.000000 aixweather-0.1.7/tests/test_EPW.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-03 15:54:38.000000 aixweather-0.1.7/tests/test_ERC.py
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2024-05-03 15:54:38.000000 aixweather-0.1.7/tests/test_TRY.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2024-05-03 15:54:39.000000 aixweather-0.1.7/tests/test_output_functions.py
```

### Comparing `aixweather-0.1.6/AixWeather.egg-info/PKG-INFO` & `aixweather-0.1.7/AixWeather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AixWeather
-Version: 0.1.6
+Version: 0.1.7
 Summary: A weather data generation tool for building energy system simulations.Pull, Transform, Export.
 Home-page: https://github.com/RWTH-EBC/AixWeather
-Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.6.tar.gz
+Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.7.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: ebc-abos@eonerc.rwth-aachen.de
 License: BSD 3-Clause
 Keywords: weather,BES,converter,simulation,building,energy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
@@ -27,14 +27,15 @@
 Requires-Dist: shapely~=2.0.3; extra == "try"
 Provides-Extra: dwd-forecast
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "dwd-forecast"
 Provides-Extra: full
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "full"
 Requires-Dist: geopandas~=0.14.0; extra == "full"
 Requires-Dist: geopy~=2.4.0; extra == "full"
+Requires-Dist: shapely~=2.0.3; extra == "full"
 
 ![E.ON EBC RWTH Aachen University](./docs/source/_static/EBC_Logo.png)
 
 [![pylint](https://rwth-ebc.github.io/AixWeather//main//pylint/pylint.svg )](https://rwth-ebc.github.io/AixWeather//main//pylint/pylint.html)
 [![documentation](https://rwth-ebc.github.io/AixWeather//main//docs/doc.svg)](https://rwth-ebc.github.io/AixWeather//main//docs/index.html)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
```

### Comparing `aixweather-0.1.6/AixWeather.egg-info/SOURCES.txt` & `aixweather-0.1.7/AixWeather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/LICENSE` & `aixweather-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/PKG-INFO` & `aixweather-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AixWeather
-Version: 0.1.6
+Version: 0.1.7
 Summary: A weather data generation tool for building energy system simulations.Pull, Transform, Export.
 Home-page: https://github.com/RWTH-EBC/AixWeather
-Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.6.tar.gz
+Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.7.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: ebc-abos@eonerc.rwth-aachen.de
 License: BSD 3-Clause
 Keywords: weather,BES,converter,simulation,building,energy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
@@ -27,14 +27,15 @@
 Requires-Dist: shapely~=2.0.3; extra == "try"
 Provides-Extra: dwd-forecast
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "dwd-forecast"
 Provides-Extra: full
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "full"
 Requires-Dist: geopandas~=0.14.0; extra == "full"
 Requires-Dist: geopy~=2.4.0; extra == "full"
+Requires-Dist: shapely~=2.0.3; extra == "full"
 
 ![E.ON EBC RWTH Aachen University](./docs/source/_static/EBC_Logo.png)
 
 [![pylint](https://rwth-ebc.github.io/AixWeather//main//pylint/pylint.svg )](https://rwth-ebc.github.io/AixWeather//main//pylint/pylint.html)
 [![documentation](https://rwth-ebc.github.io/AixWeather//main//docs/doc.svg)](https://rwth-ebc.github.io/AixWeather//main//docs/index.html)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
```

### Comparing `aixweather-0.1.6/README.md` & `aixweather-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_epw_energyplus.py` & `aixweather-0.1.7/aixweather/core_data_format_2_output_file/to_epw_energyplus.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_mos_TMY3.py` & `aixweather-0.1.7/aixweather/core_data_format_2_output_file/to_mos_TMY3.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/core_data_format_2_output_file/unconverted_to_x.py` & `aixweather-0.1.7/aixweather/core_data_format_2_output_file/unconverted_to_x.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/data_quality_checks.py` & `aixweather-0.1.7/aixweather/data_quality_checks.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/definitions.py` & `aixweather-0.1.7/aixweather/definitions.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/imports/DWD.py` & `aixweather-0.1.7/aixweather/imports/DWD.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/imports/EPW.py` & `aixweather-0.1.7/aixweather/imports/EPW.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/imports/ERC.py` & `aixweather-0.1.7/aixweather/imports/ERC.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/imports/TRY.py` & `aixweather-0.1.7/aixweather/imports/TRY.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 import DWD TRY data
 """
 
+import logging
 import re
-import pandas as pd
 import random
+import pandas as pd
 
 from aixweather.imports.utils_import import MetaData
 
+logger = logging.getLogger(__name__)
 
 def _handle_TRY_type(path: str) -> tuple:
     """
     Determine the TRY format type based on the provided file path.
 
     Args:
         path (str): The file path to the TRY dataset file.
@@ -97,18 +99,17 @@
     hoehenlage_line = next(line for line in header_lines if "Hoehenlage" in line)
     hoehenlage = int(re.search(r":\s*(\d+) Meter", hoehenlage_line).group(1))
 
     try:
         import geopandas as gpd
         from geopy.geocoders import Nominatim
         from shapely.geometry import Point
-    except ImportError as err:
-        print("Optional dependency 'TRY' not installed, "
-              "skipping metadata of TRY. ImportError:", err)
-        return meta
+    except ImportError:
+        raise ImportError("Optional dependency 'TRY' not installed. Conversion of longitude and "
+                          "latitude not possible and hence no radiation transformation.")
 
     ### convert latitude and longitude
     # Create a GeoDataFrame with the provided coordinates
     # (using pyproj directly led to wrong calculation)
     gdf = gpd.GeoDataFrame(
         {"geometry": [Point(rechtswert, hochwert)]},
         crs="EPSG:3034",  # Original coordinate system
```

### Comparing `aixweather-0.1.6/aixweather/imports/custom_file.py` & `aixweather-0.1.7/aixweather/imports/custom_file.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/imports/utils_import.py` & `aixweather-0.1.7/aixweather/imports/utils_import.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/project_class.py` & `aixweather-0.1.7/aixweather/project_class.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_functions/auxiliary.py` & `aixweather-0.1.7/aixweather/transformation_functions/auxiliary.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_functions/pass_through_handling.py` & `aixweather-0.1.7/aixweather/transformation_functions/pass_through_handling.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_functions/time_observation_transformations.py` & `aixweather-0.1.7/aixweather/transformation_functions/time_observation_transformations.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_functions/unit_conversions.py` & `aixweather-0.1.7/aixweather/transformation_functions/unit_conversions.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_functions/variable_transformations.py` & `aixweather-0.1.7/aixweather/transformation_functions/variable_transformations.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_to_core_data/DWD.py` & `aixweather-0.1.7/aixweather/transformation_to_core_data/DWD.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_to_core_data/EPW.py` & `aixweather-0.1.7/aixweather/transformation_to_core_data/EPW.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_to_core_data/ERC.py` & `aixweather-0.1.7/aixweather/transformation_to_core_data/ERC.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_to_core_data/TRY.py` & `aixweather-0.1.7/aixweather/transformation_to_core_data/TRY.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_to_core_data/__init__.py` & `aixweather-0.1.7/aixweather/transformation_to_core_data/__init__.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/aixweather/transformation_to_core_data/custom_file.py` & `aixweather-0.1.7/aixweather/transformation_to_core_data/custom_file.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/setup.py` & `aixweather-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         "shapely~=2.0.3"
     ],
     "DWD_forecast": ["wetterdienst>=0.65.0,<=0.72.0"],
     "full": [
         "wetterdienst>=0.65.0,<=0.72.0",
         "geopandas~=0.14.0",
         "geopy~=2.4.0",
+        "shapely~=2.0.3",
     ]
 }
 
 
 # Add all open-source packages to setup-requires
 SETUP_REQUIRES = INSTALL_REQUIRES.copy()
```

### Comparing `aixweather-0.1.6/tests/test_DWD_forecast.py` & `aixweather-0.1.7/tests/test_DWD_forecast.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/tests/test_DWD_historical.py` & `aixweather-0.1.7/tests/test_DWD_historical.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/tests/test_EPW.py` & `aixweather-0.1.7/tests/test_EPW.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/tests/test_ERC.py` & `aixweather-0.1.7/tests/test_ERC.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/tests/test_TRY.py` & `aixweather-0.1.7/tests/test_TRY.py`

 * *Files identical despite different names*

### Comparing `aixweather-0.1.6/tests/test_output_functions.py` & `aixweather-0.1.7/tests/test_output_functions.py`

 * *Files identical despite different names*

