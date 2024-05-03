# Comparing `tmp/hhnk_research_tools-2023.4.tar.gz` & `tmp/hhnk_research_tools-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk_research_tools-2023.4.tar", last modified: Thu Nov  9 12:17:27 2023, max compression
+gzip compressed data, was "hhnk_research_tools-2024.1.tar", last modified: Fri May  3 10:45:14 2024, max compression
```

## Comparing `hhnk_research_tools-2023.4.tar` & `hhnk_research_tools-2024.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:25.742179 hhnk_research_tools-2023.4/
--rw-rw-rw-   0        0        0      596 2023-11-09 12:17:27.479405 hhnk_research_tools-2023.4/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-23 10:51:35.000000 hhnk_research_tools-2023.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:25.915182 hhnk_research_tools-2023.4/hhnk_research_tools/
--rw-rw-rw-   0        0        0     2247 2023-11-07 09:40:46.000000 hhnk_research_tools-2023.4/hhnk_research_tools/__init__.py
--rw-rw-rw-   0        0        0     5886 2023-11-06 14:18:34.000000 hhnk_research_tools-2023.4/hhnk_research_tools/dataframe_functions.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:26.167186 hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/
--rw-rw-rw-   0        0        0        0 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/__init__.py
--rw-rw-rw-   0        0        0     2623 2023-11-06 14:17:04.000000 hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/file_class.py
--rw-rw-rw-   0        0        0     6600 2023-11-09 12:13:04.000000 hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/folder_file_classes.py
--rw-rw-rw-   0        0        0     6070 2023-11-06 14:19:34.000000 hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/sqlite_class.py
--rw-rw-rw-   0        0        0     8845 2023-11-06 14:19:34.000000 hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/threedi_schematisation.py
--rw-rw-rw-   0        0        0     4667 2023-11-06 14:18:40.000000 hhnk_research_tools-2023.4/hhnk_research_tools/general_functions.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:26.247187 hhnk_research_tools-2023.4/hhnk_research_tools/gis/
--rw-rw-rw-   0        0        0        0 2023-08-18 09:53:48.000000 hhnk_research_tools-2023.4/hhnk_research_tools/gis/__init__.py
--rw-rw-rw-   0        0        0    18429 2023-11-06 14:19:35.000000 hhnk_research_tools-2023.4/hhnk_research_tools/gis/raster.py
--rw-rw-rw-   0        0        0     1427 2023-11-06 14:17:42.000000 hhnk_research_tools-2023.4/hhnk_research_tools/gis/vector.py
--rw-rw-rw-   0        0        0     2012 2023-11-06 14:18:35.000000 hhnk_research_tools-2023.4/hhnk_research_tools/processes.py
--rw-rw-rw-   0        0        0    19114 2023-11-06 14:18:38.000000 hhnk_research_tools-2023.4/hhnk_research_tools/raster_functions.py
--rw-rw-rw-   0        0        0    11302 2023-11-06 14:18:39.000000 hhnk_research_tools-2023.4/hhnk_research_tools/sql_functions.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:26.769196 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/
--rw-rw-rw-   0        0        0      149 2023-11-06 14:17:43.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/__init__.py
--rw-rw-rw-   0        0        0      879 2023-11-06 14:17:45.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/call_api.py
--rw-rw-rw-   0        0        0     1999 2023-11-06 14:17:46.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/geometry_functions.py
--rw-rw-rw-   0        0        0     6327 2023-11-06 14:19:35.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/grid.py
--rw-rw-rw-   0        0        0      664 2023-11-06 14:17:49.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/read_api_file.py
--rw-rw-rw-   0        0        0      904 2023-11-06 14:17:51.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/threediresult_loader.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:26.940199 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/variables/
--rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/variables/__init__.py
--rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/variables/gridadmin.py
--rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/variables/rain_dataframe.py
--rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/variables/results_mapping.py
--rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.4/hhnk_research_tools/threedi/variables/variables_container.py
--rw-rw-rw-   0        0        0     1870 2023-11-06 14:19:01.000000 hhnk_research_tools-2023.4/hhnk_research_tools/variables.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:27.172202 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/
--rw-rw-rw-   0        0        0       82 2023-11-06 14:18:47.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:27.420207 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/
--rw-rw-rw-   0        0        0        0 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/__init__.py
--rw-rw-rw-   0        0        0    70142 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg
--rw-rw-rw-   0        0        0    64399 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg
--rw-rw-rw-   0        0        0    64209 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg
--rw-rw-rw-   0        0        0    69232 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg
--rw-rw-rw-   0        0        0     5096 2023-11-06 14:18:17.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/wss_calculations.py
--rw-rw-rw-   0        0        0     4162 2023-11-06 14:17:56.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/wss_loading.py
--rw-rw-rw-   0        0        0     6542 2023-11-06 14:18:04.000000 hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/wss_main.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:17:25.985183 hhnk_research_tools-2023.4/hhnk_research_tools.egg-info/
--rw-rw-rw-   0        0        0      596 2023-11-09 12:17:25.000000 hhnk_research_tools-2023.4/hhnk_research_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1947 2023-11-09 12:17:25.000000 hhnk_research_tools-2023.4/hhnk_research_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-09 12:17:25.000000 hhnk_research_tools-2023.4/hhnk_research_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-11-09 12:17:25.000000 hhnk_research_tools-2023.4/hhnk_research_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-09 12:17:27.528127 hhnk_research_tools-2023.4/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-08-16 10:01:39.000000 hhnk_research_tools-2023.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:14.119443 hhnk_research_tools-2024.1/
+-rw-rw-rw-   0        0        0      546 2024-05-03 10:45:14.114443 hhnk_research_tools-2024.1/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-23 10:51:35.000000 hhnk_research_tools-2024.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:13.606647 hhnk_research_tools-2024.1/hhnk_research_tools/
+-rw-rw-rw-   0        0        0     2587 2024-04-29 14:14:02.000000 hhnk_research_tools-2024.1/hhnk_research_tools/__init__.py
+-rw-rw-rw-   0        0        0     5886 2023-11-06 14:18:34.000000 hhnk_research_tools-2024.1/hhnk_research_tools/dataframe_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:13.750647 hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/
+-rw-rw-rw-   0        0        0        0 2023-05-10 15:38:56.000000 hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/__init__.py
+-rw-rw-rw-   0        0        0     3021 2023-11-23 14:43:24.000000 hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/file_class.py
+-rw-rw-rw-   0        0        0     7483 2024-04-16 09:14:24.000000 hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/folder_file_classes.py
+-rw-rw-rw-   0        0        0     6120 2024-04-30 11:23:31.000000 hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/sqlite_class.py
+-rw-rw-rw-   0        0        0     8862 2023-11-30 10:30:40.000000 hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/threedi_schematisation.py
+-rw-rw-rw-   0        0        0     5066 2023-11-23 14:43:25.000000 hhnk_research_tools-2024.1/hhnk_research_tools/general_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:13.786651 hhnk_research_tools-2024.1/hhnk_research_tools/gis/
+-rw-rw-rw-   0        0        0        0 2023-08-18 09:53:48.000000 hhnk_research_tools-2024.1/hhnk_research_tools/gis/__init__.py
+-rw-rw-rw-   0        0        0    22564 2024-04-08 09:52:19.000000 hhnk_research_tools-2024.1/hhnk_research_tools/gis/raster.py
+-rw-rw-rw-   0        0        0    20346 2024-02-05 15:58:45.000000 hhnk_research_tools-2024.1/hhnk_research_tools/gis/raster_calculator.py
+-rw-rw-rw-   0        0        0     1427 2023-11-06 14:17:42.000000 hhnk_research_tools-2024.1/hhnk_research_tools/gis/vector.py
+-rw-rw-rw-   0        0        0     2012 2023-11-06 14:18:35.000000 hhnk_research_tools-2024.1/hhnk_research_tools/processes.py
+-rw-rw-rw-   0        0        0    19325 2024-01-12 09:00:32.000000 hhnk_research_tools-2024.1/hhnk_research_tools/raster_functions.py
+-rw-rw-rw-   0        0        0    11311 2024-03-20 13:32:25.000000 hhnk_research_tools-2024.1/hhnk_research_tools/sql_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:13.829655 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/
+-rw-rw-rw-   0        0        0      149 2023-11-06 14:17:43.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/__init__.py
+-rw-rw-rw-   0        0        0      927 2023-11-30 10:32:37.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/call_api.py
+-rw-rw-rw-   0        0        0     1999 2023-11-06 14:17:46.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/geometry_functions.py
+-rw-rw-rw-   0        0        0     6327 2023-11-06 14:19:35.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/grid.py
+-rw-rw-rw-   0        0        0      664 2023-11-06 14:17:49.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/read_api_file.py
+-rw-rw-rw-   0        0        0      904 2023-11-06 14:17:51.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/threediresult_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:13.869651 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/variables/
+-rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/variables/__init__.py
+-rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/variables/gridadmin.py
+-rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/variables/rain_dataframe.py
+-rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/variables/results_mapping.py
+-rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-2024.1/hhnk_research_tools/threedi/variables/variables_container.py
+-rw-rw-rw-   0        0        0     1870 2023-11-06 14:19:01.000000 hhnk_research_tools-2024.1/hhnk_research_tools/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:13.906445 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/
+-rw-rw-rw-   0        0        0       82 2023-11-06 14:18:47.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:14.103444 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/
+-rw-rw-rw-   0        0        0        0 2023-06-22 10:20:37.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/__init__.py
+-rw-rw-rw-   0        0        0    70142 2023-06-22 10:20:37.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg
+-rw-rw-rw-   0        0        0    64399 2023-06-22 10:20:37.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg
+-rw-rw-rw-   0        0        0    64209 2023-06-22 10:20:37.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg
+-rw-rw-rw-   0        0        0    69232 2023-06-22 10:20:37.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg
+-rw-rw-rw-   0        0        0     5096 2023-11-06 14:18:17.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/wss_calculations.py
+-rw-rw-rw-   0        0        0     4162 2023-11-06 14:17:56.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/wss_loading.py
+-rw-rw-rw-   0        0        0     6677 2024-04-03 11:30:23.000000 hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/wss_main.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:45:14.111442 hhnk_research_tools-2024.1/hhnk_research_tools.egg-info/
+-rw-rw-rw-   0        0        0      546 2024-05-03 10:45:13.000000 hhnk_research_tools-2024.1/hhnk_research_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1992 2024-05-03 10:45:13.000000 hhnk_research_tools-2024.1/hhnk_research_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 10:45:13.000000 hhnk_research_tools-2024.1/hhnk_research_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-03 10:45:13.000000 hhnk_research_tools-2024.1/hhnk_research_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 10:45:14.119443 hhnk_research_tools-2024.1/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-08-16 10:01:39.000000 hhnk_research_tools-2024.1/setup.py
```

### Comparing `hhnk_research_tools-2023.4/PKG-INFO` & `hhnk_research_tools-2024.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 Metadata-Version: 2.1
 Name: hhnk_research_tools
-Version: 2023.4
+Version: 2024.1
 Summary: General tools for analysis, data manipulation and threedi interaction for analysis of water systems
 Home-page: https://github.com/HHNK/hhnk-research-tools
 Author: Wietse van Gerwen
 Author-email: w.vangerwen@hhnk.nl
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HHNK/hhnk-research-tools/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-
-UNKNOWN
-
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/__init__.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-from hhnk_research_tools.gis.raster import Raster, RasterMetadata
+# hhnk_research_tools/__init__.py
+from typing import TYPE_CHECKING
+
+from hhnk_research_tools.gis.raster import Raster, RasterMetadata  # noqa: F401
+
+if TYPE_CHECKING:
+    # TODO zou moeten werken met typehints van imports. Maar vraag is maar of het werkt.
+    import hhnk_research_tools as hrt
+
 import hhnk_research_tools.threedi as threedi
 import hhnk_research_tools.variables as variables
 import hhnk_research_tools.waterschadeschatter.resources
 from hhnk_research_tools.dataframe_functions import (
     df_add_geometry_to_gdf,
     df_convert_to_gdf,
     gdf_write_to_csv,
@@ -30,16 +38,17 @@
     dict_to_class,
     ensure_file_path,
     get_functions,
     get_pkg_resource_path,
     get_uuid,
     get_variables,
     load_source,
+    time_delta,
 )
-
+from hhnk_research_tools.gis.raster_calculator import RasterBlocks, RasterCalculatorV2
 from hhnk_research_tools.raster_functions import (
     RasterCalculator,
     build_vrt,
     create_meta_from_gdf,
     create_new_raster_file,
     dx_dy_between_rasters,
     gdf_to_raster,
@@ -62,12 +71,12 @@
 from hhnk_research_tools.threedi.call_api import call_threedi_api
 from hhnk_research_tools.threedi.read_api_file import read_api_file
 from hhnk_research_tools.waterschadeschatter.wss_main import Waterschadeschatter
 
 # TODO how does this versioning work?
 # Threedigrid version number is automatic updated with zest.releaser. Geopandas uses versioneer.py.
 # the version number in setup.py is updated using the find_version()
-__version__ = "2023.4"
+__version__ = "2024.1"
 
 __doc__ = """
 General toolbox for loading, converting and saving serval datatypes.
 """
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/dataframe_functions.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/file_class.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/file_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,50 +14,46 @@
     def __init__(self, base=None):
         self._base = base
         self.path = Path(str(base)).absolute().resolve()
 
     # decorated properties
     @property
     def base(self):
-        """path as posix string (foreward slashes)"""
+        """Path as posix string (foreward slashes)"""
         return self.path.as_posix()
 
     @property
     def name(self):
-        """name with suffix"""
+        """Name with suffix"""
         return self.path.name
 
-    @property
-    def parent(self):
-        return self.path.parent
-
     # TODO remove in future release
     @property
     def pl(self):
         import warnings
 
         warnings.warn(
-            ".pl is deprecated and will be removed in a future release. Please use .path instead",
+            ".pl is deprecated since v2023.4 and will be removed in a future release. Please use .path instead",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.path
 
     @property
     def path_if_exists(self):
-        """return filepath if the file exists otherwise return None"""
+        """Return filepath if the file exists otherwise return None"""
         if self.exists():
             return str(self.path)
         return None
 
     # def is_file(self):
     #     return self.path.suffix != ""
 
     def exists(self):
-        """dont return true on empty path."""
+        """Dont return true on empty path."""
         if not self._base:
             return False
         return self.path.exists()
 
     def __str__(self):
         return self.base
 
@@ -79,24 +75,38 @@
 
     def unlink(self, missing_ok=True):
         self.path.unlink(missing_ok=missing_ok)
 
     def read_json(self):
         if self.path.suffix == ".json":
             return json.loads(self.path.read_text())
-        raise Exception(f"{self.name} is not a json.")
+        raise TypeError(f"{self.name} is not a json.")
 
     def ensure_file_path(self):
         ensure_file_path(self.path)
 
+    @property
+    def parent(self):
+        """Return hrt.Folder instance. Import needs to happen here
+        to prevent circular imports.
+        """
+        from hhnk_research_tools.folder_file_classes.folder_file_classes import Folder
+
+        return Folder(self.path.parent)
+
     def __repr__(self):
         repr_str = f"""{self.path.name} @ {self.path}
 exists: {self.exists()}
 type: {type(self)}
 functions: {get_functions(self)}
 variables: {get_variables(self)}
 """
         return repr_str
 
-    def view_name_with_parents(self, parents=0):
+    def view_name_with_parents(self, parents: int = 0):
+        """Display name of file with number of parents
+
+        parents (int): defaults to 0
+            number of parents to show
+        """
         parents = min(len(self.path.parts) - 2, parents)  # avoids index-error
-        return self.base.split(self.path.parents[parents].as_posix())[-1]
+        return self.base.split(self.path.parents[parents].as_posix(), maxsplit=1)[-1]
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/folder_file_classes.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/folder_file_classes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # %%
 import types
+import warnings
 from pathlib import Path
 
 import fiona
 import geopandas as gpd
 
 from hhnk_research_tools import Raster
 from hhnk_research_tools.folder_file_classes.file_class import BasePath, File
 from hhnk_research_tools.folder_file_classes.sqlite_class import Sqlite
 from hhnk_research_tools.general_functions import get_functions, get_variables
 
+# %%
+
 
 class Folder(BasePath):
     """Base folder class for creating, deleting and see if folder exists"""
 
     def __init__(self, base, create=False):
         super().__init__(base)
 
@@ -45,36 +48,61 @@
     #     return [i for i in self.paths if i not in self.folders]
 
     # @property
     # def folders_list(self):
     #     """Check if paths are instance of Folder."""
     #     return [i for i in self.paths if not isinstance(getattr(self, i), Folder)]
 
+    @property
+    def parent(self):
+        """Return hrt.Folder instance. Import needs to happen here
+        to prevent circular imports.
+        """
+        return Folder(self.path.parent)
+
     def create(self, parents=False, verbose=False):
         """Create folder, if parents==False path wont be
-        created if parent doesnt exist."""
+        created if parent doesnt exist.
+        """
+        warnings.warn(
+            ".create is deprecated v2024.1 and will be removed in a future release. Please use .mkdir instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+        self.mkdir(parents=parents, verbose=verbose)
+
+    def mkdir(self, parents=False, verbose=False):
+        """Create folder and parents
+
+        Parameters
+        ----------
+        parents; Bool
+            False: dont create if parent don't exist.
+            True: also create parents.
+        """
         if not parents:
-            if not self.path.parent.exists():
+            if not self.parent.exists():
                 if verbose:
                     print(f"'{self.path}' not created, parent does not exist.")
                 return
         self.path.mkdir(parents=parents, exist_ok=True)
 
     def find_ext(self, ext: list):
-        """finds files with a certain extension"""
+        """Find files with a certain extension"""
         if type(ext) == str:
             ext = [ext]
         file_list = []
         for e in ext:
             file_list += [i for i in self.path.glob(f"*.{e.replace('.','')}")]
         return file_list
 
     def full_path(self, name, return_only_file_class=False):
         """
-        returns the full path of a file or a folder when only a name is known.
+        Return the full path of a file or a folder when only a name is known.
         Will return the object based on suffix
 
         return_only_file_class (bool): only return file class, can speed up
             some functions because hrt.Raster initialization takes some time.
         """
         name = str(name)
         if name.startswith("\\") or name.startswith("/"):
@@ -96,22 +124,25 @@
             elif filepath.suffix in [".sqlite"]:
                 new_file = Sqlite(filepath)
             else:
                 new_file = File(filepath)
         return new_file
 
     def add_file(self, objectname, filename):
-        """"""
+        """Add file as attribute. type is determined by filename extension."""
         new_file = self.full_path(filename)
 
         self.files[objectname] = new_file
         setattr(self, objectname, new_file)
+        return new_file
 
     def unlink_contents(self, names=[], rmfiles=True, rmdirs=False):
-        """unlink all content when names is an empty list. Otherwise just remove the names."""
+        """Unlink all content when names is an empty list.
+        Otherwise just remove the names.
+        """
         if not names:
             names = self.content
         for name in names:
             pathname = self.path / name
             try:
                 if pathname.exists():
                     # FIXME rmdir is only allowed for empty dirs
@@ -144,21 +175,21 @@
     def __init__(self, base):
         super().__init__(base)
 
         self.layerlist = []
         self.layers = types.SimpleNamespace()  # empty class
 
     def load(self, layer=None):
-        if layer == None:
+        if layer is None:
             avail_layers = self.available_layers()
             if len(avail_layers) == 1:
                 layer = avail_layers[0]
             else:
                 layer = input(f"Select layer [{avail_layers}]:")
-        return gpd.read_file(self.base, layer=layer)
+        return gpd.read_file(self.path, layer=layer, engine="pyogrio")
 
     def add_layer(self, name: str):
         """Predefine layers so we can write output to that layer."""
         if name not in self.layerlist:
             new_layer = FileGDBLayer(name, parent=self)
             self.layerlist.append(name)
             setattr(self.layers, name, new_layer)
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/sqlite_class.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/sqlite_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# %%
 import os
 import sqlite3
 
 import pandas as pd
 
 import hhnk_research_tools as hrt
 from hhnk_research_tools.folder_file_classes.file_class import File
@@ -15,18 +16,19 @@
     def connect(self):
         if self.exists():
             return self.create_sqlite_connection()
         else:
             return None
 
     def create_sqlite_connection(self):
-        """Create connection to database. On windows with conda envs this requires the mod_spatialaite extension
+        r"""Create connection to database. On windows with conda envs this requires the mod_spatialaite extension
         to be installed explicitly. The location of this extension is stored in
         hhnk_research_tools.variables.MOD_SPATIALITE_PATH (C:\ProgramData\Anaconda3\mod_spatialite-5.0.1-win-amd64)
-        and can be downloaded from http://www.gaia-gis.it/gaia-sins/windows-bin-amd64/"""
+        and can be downloaded from http://www.gaia-gis.it/gaia-sins/windows-bin-amd64/
+        """
         try:
             conn = sqlite3.connect(self.path)
             conn.enable_load_extension(True)
             conn.execute("SELECT load_extension('mod_spatialite')")
             return conn
         except sqlite3.OperationalError as e:
             if e.args[0] == "The specified module could not be found.\r\n":
@@ -44,15 +46,15 @@
                     )
                     raise e from None
 
         except Exception as e:
             raise e from None
 
     def read_table(self, table_name: str, id_col: str = None, columns: list = []):
-        """read table as (geo)dataframe. If there is a geometry column
+        """Read table as (geo)dataframe. If there is a geometry column
         then it will load as a gdf in epsg 28992.
         Run .list_tables to get an overview over available (v2) tables
         table_name: table in sqlite
         id_col: sets the index of the dataframe to this column
         columns: filter columns that are returned
         """
         conn = None
@@ -103,22 +105,27 @@
             raise e from None
         finally:
             if kill_connection and conn is not None:
                 conn.close()
 
     def execute_sql_changes(self, query, conn=None):
         """
-        Takes a query that changes the database and tries
+        Take a query that changes the database and try
         to execute it. On success, changes are committed.
-        On a failure, rolls back to the state before
-        the query was executed that caused the error
+        On a failure, roll back to the state before
+        execution.
 
         The explicit begin and commit statements are necessary
         to make sure we can roll back the transaction
         """
+
+        # Dont execute empty str.
+        if query in [None, ""]:
+            return
+
         kill_connection = conn is None  # Only kill connection when it was not provided as input
         try:
             if conn is None:
                 conn = self.connect()
             try:
                 conn.executescript(f"BEGIN; {query}; COMMIT")
             except Exception as e:
@@ -128,17 +135,15 @@
             raise e from None
         finally:
             if kill_connection and conn is not None:
                 conn.close()
 
     # TODO was sql_table_exists
     def sql_table_info(self, table_name, conn=None):
-        """
-        Returns table info if it exists
-        """
+        """Return table info if it exists"""
         query = f"""PRAGMA table_info({table_name})"""
         df = self.execute_sql_selection(query=query, conn=conn)
         return df
 
     def list_tables(self):
         """Get a list of all v2 tables."""
         query = """SELECT name
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/folder_file_classes/threedi_schematisation.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/folder_file_classes/threedi_schematisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,24 +53,24 @@
 
     @property
     def database_path(self):
         return str(self.database)
 
     @property
     def sqlite_paths(self):
-        """returns all sqlites in folder"""
+        """Return all sqlites in folder"""
         return self.find_ext("sqlite")
 
     @property
     def sqlite_names(self):
-        """returns all sqlites in folder"""
+        """Return all sqlites in folder"""
         return [sp.stem for sp in self.sqlite_paths]
 
     def model_path(self, idx=0, name=None):
-        """finds a model using an index"""
+        """Find a model using an index"""
         if name:
             try:
                 idx = self.sqlite_names.index(name)
             except Exception:
                 raise ValueError("name of sqlite given, but cannot be found")
         if len(self.sqlite_paths) >= 1:
             return self.sqlite_paths[idx]
@@ -111,26 +111,27 @@
             if len(tifs) == 0:
                 tifs = [""]
             return File(tifs[0])
 
         def get_raster_path(self, table_name, col_name):
             """Read the sqlite to check which rasters are used in the model.
             This only works for models from Klondike release onwards, where we only have
-            one global settings row."""
+            one global settings row.
+            """
 
             if self.caller.database.exists():
                 df = hrt.sqlite_table_to_df(database_path=self.caller.database.path, table_name=table_name)
                 # if len(df) > 1:
                 # print(f"{table_name} has more than 1 row. Choosing the first row for the rasters.")
                 if len(df) == 0:
                     raster_name = None
                 else:
                     raster_name = df.iloc[0][col_name]
 
-                if raster_name == None:
+                if raster_name is None:
                     raster_path = ""
                 else:
                     raster_path = self.caller.full_path(raster_name)
             else:
                 raster_path = ""
             return Raster(raster_path)
 
@@ -144,15 +145,16 @@
     initial_wlvl_2d - {self.initial_wlvl_2d.name}
     dem_50cm - {self.dem_50cm.name}
 """
 
 
 class ThreediResult(Folder):
     """Result of threedi simulation. Base files are .nc and .h5.
-    Use .grid to access GridH5ResultAdmin and .admin to access GridH5Admin"""
+    Use .grid to access GridH5ResultAdmin and .admin to access GridH5Admin
+    """
 
     def __init__(self, base, create=False):
         super().__init__(base, create=create)
 
         # Files
         self.add_file("grid_path", "results_3di.nc")
         self.add_file("admin_path", "gridadmin.h5")
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/general_functions.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/general_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import importlib
 import importlib.resources as pkg_resources  # Load resource from package
 import inspect
 import sys
 from pathlib import Path
+from typing import Union
 from uuid import uuid4
 
 import geopandas as gpd
 
 
 def get_functions(cls, stringify=True):
     """Get a string with functions (methods) in a class."""
@@ -27,16 +28,16 @@
     if stringify:
         variables = " ".join(variables)
     return variables
 
 
 def ensure_file_path(filepath):
     # TODO add to file class? still needed?
-    """
-    Functions makes sure all folders in a given file path exist. Creates them if they don't.
+    """Make sure all folders in a given file path exist.
+    Creates them if they don't.
     """
     try:
         path = Path(filepath)
         path.parent.mkdir(parents=True, exist_ok=True)
     except Exception as e:
         raise e from None
 
@@ -53,28 +54,31 @@
                     print(f"    {layer}")
                 gdf = gpd.read_file(str(gdb), layer=layer)
 
                 gdf.to_file(str(gpkg), layer=layer, driver="GPKG")
 
 
 def check_create_new_file(
-    output_file: str, overwrite: bool = False, input_files: list = [], check_is_file=True
+    output_file: Union[Path, str],
+    overwrite: bool = False,
+    input_files: list = [],
+    check_is_file=True,
 ) -> bool:
     """
     Check if we should continue to create a new file.
 
     output_file: The file under evaluation
     overwrite: When overwriting is True the output_file will be removed.
     input_files: if input files are provided the edit time of the input will be
                  compared to the output. If edit time is after the output, it will
                  recreate the output.
     check_is_file: check if output_file is a file
     """
     create = False
-    output_file = Path(str(output_file))
+    output_file = Path(str(output_file))  # noqa
 
     # Als geen suffix (dus geen file), dan error
     if check_is_file:  #
         if not output_file.suffix:
             raise TypeError(f"{output_file} is not a file.")
 
     # Rasterize regions
@@ -98,19 +102,19 @@
                         output_file.unlink()
                         create = True
                         break
     return create
 
 
 def load_source(name: str, path: str):
-    """
-    Load python file as module.
+    """Load python file as module.
 
     Replacement for deprecated imp.load_source()
-    Inspiration from https://github.com/cuthbertLab/music21/blob/master/music21/test/commonTest.py"""
+    Inspiration from https://github.com/cuthbertLab/music21/blob/master/music21/test/commonTest.py
+    """
     spec = importlib.util.spec_from_file_location(name, str(path))
     if spec is None or spec.loader is None:
         raise FileNotFoundError(f"No such file or directory: {path!r}")
     if name in sys.modules:
         module = sys.modules[name]
     else:
         module = importlib.util.module_from_spec(spec)
@@ -119,27 +123,37 @@
         sys.modules[name] = module
     spec.loader.exec_module(module)
 
     return module
 
 
 def get_uuid(chars=8):
-    """max chars = 36"""
+    """Max chars is 36"""
     return str(uuid4())[:chars]
 
 
 def get_pkg_resource_path(package_resource, name) -> Path:
-    """return path to resource in a python package, so it can be loaded"""
+    """Return path to resource in a python package, so it can be loaded"""
     with pkg_resources.path(package_resource, name) as p:
         return p.absolute().resolve()
 
 
-def current_time(time_format="%H:%M:%S"):
+def current_time(time_format="%H:%M:%S", date: bool = False):
+    if date is True:
+        time_format = "%Y%m%d_%H%M%S_%f"
     return datetime.datetime.now().strftime(time_format)
 
 
+def time_delta(start_time: datetime.datetime):
+    """Difference between starttime in seconds.
+
+    start_time (datetime.datetime): get by using datetime.datetime.now()
+    """
+    return round((datetime.datetime.now() - start_time).total_seconds(), 2)
+
+
 class dict_to_class(dict):
     """dot.notation access to dictionary attributes"""
 
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/gis/raster.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/gis/raster.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,20 @@
 from scipy import ndimage
 from shapely import geometry
 
 import hhnk_research_tools as hrt
 from hhnk_research_tools.folder_file_classes.file_class import File
 from hhnk_research_tools.general_functions import get_functions, get_variables
 
+# If anything goes wrong in gdal, make sure we raise the errors instead
+# of silenty ignoring the issues.
+gdal.UseExceptions()
 
+
+# %%
 class Raster(File):
     def __init__(self, base, min_block_size=1024):
         super().__init__(base)
 
         self.source_set = False  # Tracks if the source exist on the system.
         self._array = None
         self.min_block_size = min_block_size
@@ -33,34 +38,41 @@
             return self._array
 
     @array.setter
     def array(self, raster_array, window=None, band_nr=1):
         self._array = raster_array
 
     def _read_array(self, band=None, window=None):
+        # TODO hidden to public?
         """window=[x0, y0, x1, y1]--oud.
         window=[x0, y0, xsize, ysize]
-        x0, y0 is left top corner!!"""
-        if band == None:
+        x0, y0 is left top corner!!
+        """
+        if band is None:
             gdal_src = self.open_gdal_source_read()
             band = gdal_src.GetRasterBand(1)
 
         if window is not None:
             raster_array = band.ReadAsArray(
-                xoff=int(window[0]), yoff=int(window[1]), win_xsize=int(window[2]), win_ysize=int(window[3])
+                xoff=int(window[0]),
+                yoff=int(window[1]),
+                win_xsize=int(window[2]),
+                win_ysize=int(window[3]),
             )
         else:
             raster_array = band.ReadAsArray()
 
         band.FlushCache()  # close file after writing
         band = None
 
         return raster_array
 
     def get_array(self, window=None, band_count=None):
+        # TODO hoe deze gebruiken tov _read_array? is het nuttig om
+        # array ook in cls weg te schrijven.
         try:
             if band_count is None:
                 band_count = self.band_count
 
             gdal_src = self.open_gdal_source_read()
             if band_count == 1:
                 raster_array = self._read_array(band=gdal_src.GetRasterBand(1), window=window)
@@ -82,25 +94,24 @@
             raise e from None
 
     @property
     def source(self):
         if super().exists():
             if not self.source_set:
                 self.source = True  # call source.setter
-                return self.open_gdal_source_read()
-            else:
-                return self.open_gdal_source_read()
+            return self.open_gdal_source_read()
         else:
             return False
 
     @source.setter
     def source(self, value):
         """If source does not exist it will not be set.
         Bit clunky. But it should work that if it exists it will only be set once.
-        Otherwise it will not set."""
+        Otherwise it will not set.
+        """
         if super().exists():  # cannot use self.exists here.
             # Needs to be first otherwise we end in a loop when settings metadata/nodata/band_count
             self.source_set = True
 
             gdal_src = self.open_gdal_source_read()
 
             self._metadata = RasterMetadata(gdal_src=gdal_src)
@@ -111,17 +122,15 @@
         """usage;
         with self.open_gdal_source_read() as gdal_src: doesnt work.
         just dont write it to the class, and it should be fine..
         """
         return gdal.Open(self.base, gdal.GA_ReadOnly)
 
     def open_gdal_source_write(self):
-        """
-        open source with write access
-        """
+        """Open source with write access"""
         return gdal.Open(self.base, gdal.GA_Update)
 
     def unlink(self, missing_ok=True):
         """Remove raster if it exists, reset source."""
         self.path.unlink(missing_ok=missing_ok)
         if not self.exists():
             self.source_set = False
@@ -162,32 +171,37 @@
     def shape(self):
         return self.metadata.shape
 
     @property
     def pixelarea(self):
         return self.metadata.pixelarea
 
-    def statistics(self, approve_ok=True, force=True):
-        """approve_ok: reads stats from xml if available.
+    def statistics(self, approve_ok=True, force=True) -> dict:
+        """
+        Parameters
+        ----------
+        approve_ok: reads stats from xml if available.
         force: calculates stats, might be slow.
-        returns [min, max, mean, std]"""
+        returns [min, max, mean, std]
+        """
         raster_src = self.open_gdal_source_read()
         stats = raster_src.GetRasterBand(1).GetStatistics(approve_ok, force)  # [min, max, mean, std]
         d = 6  # decimals
         return {
             "min": np.round(stats[0], d),
             "max": np.round(stats[1], d),
             "mean": np.round(stats[2], d),
             "std": np.round(stats[3], d),
         }
 
     def generate_blocks(self, blocksize_from_source: bool = False) -> pd.DataFrame:
         """Generate blocks with the blocksize of the band.
         These blocks can be used as window to load the raster iteratively.
-        from_source (bool): read
+        blocksize_from_source (bool): read the blocksize from the source raster
+            if its bigger than min_blocksize, use that.
         """
 
         if blocksize_from_source:
             gdal_src = self.open_gdal_source_read()
             band = gdal_src.GetRasterBand(1)
             block_height, block_width = band.GetBlockSize()
             band.FlushCache()  # close file after writing
@@ -289,14 +303,98 @@
         for idx, block_row in self.blocks.iterrows():
             window = block_row["window_readarray"]
             yield idx, window, block_row
 
     def to_file(self):
         pass
 
+    def build_vrt(self, overwrite: bool, bounds, input_files: list, resolution="highest", bandlist=[1]):
+        """Build vrt from input files.
+        overwrite (bool)
+        bounds (np.array): format should be; (xmin, ymin, xmax, ymax)
+            if None will use input files.
+        input_files (list): list of paths to input rasters
+        resolution: "highest"|"lowest"|"average"
+            instead of "user" option, provide a float for manual target_resolution
+        bandList: doesnt work as expected, passing [1] works.
+        """
+        if hrt.check_create_new_file(output_file=self.path, overwrite=overwrite):
+            # Set inputfiles to list of strings.
+            if type(input_files) != list:
+                input_files = [str(input_files)]
+            else:
+                input_files = [str(i) for i in input_files]
+
+            if type(resolution) in (float, int):
+                kwargs = {}
+                xRes = resolution
+                yRes = resolution
+                resolution = "user"
+            else:
+                xRes = None
+                yRes = None
+
+            # Check resolution of input files
+            input_resolutions = []
+            for r in input_files:
+                r = Raster(r)
+                input_resolutions.append(r.metadata.pixel_width)
+            if len(np.unique(input_resolutions)) > 1:
+                raise Exception(
+                    f"Multiple resolutions ({input_resolutions}) found in input_files. We cannot handle that yet."
+                )
+
+            # Build vrt
+            vrt_options = gdal.BuildVRTOptions(
+                resolution=resolution,
+                separate=False,
+                resampleAlg="nearest",
+                addAlpha=False,
+                outputBounds=bounds,
+                bandList=bandlist,
+                xRes=xRes,
+                yRes=yRes,
+            )
+            ds = gdal.BuildVRT(destName=str(self.path), srcDSOrSrcDSTab=input_files, options=vrt_options)
+            ds.FlushCache()
+
+    # FIXME hoe hier het beste omgaan met Folder zonder circular imports?
+    # def build_vrt_from_folder(self, folder_path):
+    #     """"""
+    #     raster_folder = Folder(raster_folder)
+    #     output_path = raster_folder.full_path(f'{vrt_name}.vrt')
+
+    #     if output_path.exists() and not overwrite:
+    #         print(f'vrt already exists: {output_path}')
+    #         return
+
+    #     tifs_list = [str(i) for i in raster_folder.find_ext(["tif", "tiff"])]
+
+    def write_array(self, array, window, band=None):
+        """Note that providing the band may be faster.
+
+        array (np.array([])): block or raster array
+        window (list): [x0, y0, xsize, ysize]
+        x0, y0 is left top corner!!
+        """
+        flushband = False
+        if band is None:
+            gdal_src = self.open_gdal_source_write()
+            band = gdal_src.GetRasterBand(1)
+            flushband = True
+        else:
+            print("At this point just use band.WriteArray, no need for this function.")
+
+        band.WriteArray(array, xoff=window[0], yoff=window[1])
+
+        if flushband:
+            # Only flush band if it was not provided
+            # band.FlushCache()  # close file after writing
+            band = None
+
     def __iter__(self):
         if not hasattr(self, "blocks"):
             _ = self.generate_blocks()
 
         for idx, block_row in self.blocks.iterrows():
             window = block_row["window_readarray"]
             block = self._read_array(window=window)
@@ -321,16 +419,17 @@
 
 functions: {get_functions(self)}
 variables: {get_variables(self)}
 """
 
     def create(self, metadata, nodata, datatype=None, create_options=None, verbose=False, overwrite=False):
         """Create empty raster
-        metadata : RasterMetadata instance
-        nodata: int
+
+        metadata (RasterMetadata): metadata
+        nodata (int): nodata value
         """
         # Check if function should continue.
         if verbose:
             print(f"creating output raster: {self.path}")
         target_ds = hrt.create_new_raster_file(
             file_name=self.path,
             nodata=nodata,
@@ -343,35 +442,37 @@
 
         # Reset source, if raster is deleted and recreated with different resolution
         # this would otherwise cause issues.
         self.source_set = False
         self.source = None  # Update raster now it exists
 
     def sum(self):
-        """calculate sum of raster"""
+        """Calculate sum of raster"""
         raster_sum = 0
         for window, block in self:
-            block[block == self.nodata] = np.nan
+            block[block == self.nodata] = 0
             raster_sum += np.nansum(block)
         return raster_sum
 
 
 class RasterMetadata:
     """Metadata object of a raster. Resolution can be changed
     so that a new raster with another resolution can be created.
 
     Metadata can be created by supplying either:
     1. gdal_src
     2. res, bounds
     """
 
-    def __init__(self, gdal_src=None, res=None, bounds_dict=None, proj="epsg:28992"):
-        """gdal_src = gdal.Open(raster_source)
+    def __init__(self, gdal_src=None, res: float = None, bounds_dict=None, proj="epsg:28992"):
+        """
+        gdal_src = gdal.Open(raster_source)
         bounds = {"minx":, "maxx":, "miny":, "maxy":}
-        Projection only implemented for epsg:28992"""
+        Projection only implemented for epsg:28992
+        """
 
         if gdal_src is not None:
             self.proj = gdal_src.GetProjection()
             self.georef = gdal_src.GetGeoTransform()
 
             self.x_res = gdal_src.RasterXSize
             self.y_res = gdal_src.RasterYSize
@@ -417,28 +518,33 @@
     def bounds(self):
         return [self.x_min, self.x_max, self.y_min, self.y_max]
 
     # TODO deprecated. Remove in future release.
     @property
     def bounds_dl(self):
         """Lizard v3 bounds"""
-        raise Exception("use .bbox instead. lizard v4 api no longer suppers bounds_dl")
+        raise Exception("use .bbox instead. lizard v4 api no longer supports bounds_dl")
         return {
             "west": self.x_min,
             "south": self.y_min,
             "east": self.x_max,
             "north": self.y_max,
         }
 
     @property
     def bbox(self):
         """Lizard v4 bbox; str(x1, y1, x2, y2)"""
         return f"{self.x_min}, {self.y_min}, {self.x_max}, {self.y_max}"
 
     @property
+    def bbox_gdal(self):
+        """Gdal takes bbox as list, for instance in vrt creation."""
+        return [self.x_min, self.y_min, self.x_max, self.y_max]
+
+    @property
     def shape(self):
         return [self.y_res, self.x_res]
 
     @property
     def pixelarea(self):
         return abs(self.georef[1] * self.georef[5])
 
@@ -448,15 +554,15 @@
             proj_str = self.proj.split("AUTHORITY")[-1][2:-3].split('","')
             return f"{proj_str[0]}:{proj_str[1]}"
         except:
             return None
 
     def _update_georef(self, resolution):
         def res_str(georef_i):
-            """make sure negative values are kept."""
+            """Make sure negative values are kept."""
             if georef_i == self.pixel_width:
                 return resolution
             if georef_i == -self.pixel_width:
                 return -resolution
 
         georef_new = list(self.georef)
         georef_new[1] = res_str(georef_new[1])
@@ -473,16 +579,23 @@
             print(f"updated metadata resolution from {resolution_current}m to {resolution_new}m")
         else:
             raise Exception(
                 f"New resolution ({resolution_new}) can currently only be smaller than old resolution ({resolution_current})"
             )
 
     def __repr__(self):
-        funcs = "." + " .".join(
-            [i for i in dir(self) if not i.startswith("_") and hasattr(inspect.getattr_static(self, i), "__call__")]
+        funcs = (
+            "."
+            + " .".join(
+                [
+                    i
+                    for i in dir(self)
+                    if not i.startswith("_") and hasattr(inspect.getattr_static(self, i), "__call__")
+                ]
+            )
         )  # getattr resulted in RecursionError. https://stackoverflow.com/questions/1091259/how-to-test-if-a-class-attribute-is-an-instance-method
         variables = "." + " .".join(
             [
                 i
                 for i in dir(self)
                 if not i.startswith("__") and not hasattr(inspect.getattr_static(self, i), "__call__")
             ]
@@ -493,16 +606,17 @@
 .georef : {self.georef}
 .bounds : {self.bounds}
 .pixel_width : {self.pixel_width}
 ----
 {repr_str}"""
 
     def __getitem__(self, item):
-        """metadata was a dict previously. This makes it that items from
-        the class can be accessed like a dict."""
+        """Metadata was a dict previously. This makes it that items from
+        the class can be accessed like a dict.
+        """
         return getattr(self, item)
 
 
 if __name__ == "__main__":
     dem_path = Path(
         r"G:\02_Werkplaatsen\06_HYD\Projecten\HKC16015 Wateropgave 2.0\11. DCMB\hhnk-modelbuilder-master\data\fixed_data\DEM\DEM_AHN4_int.vrt"
     )
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/gis/vector.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/gis/vector.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/processes.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/processes.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/raster_functions.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/raster_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # %%
+import datetime
 import json
 import types
 
 import numpy as np
+from IPython.display import display
 from osgeo import gdal, ogr
 
 from hhnk_research_tools.folder_file_classes.folder_file_classes import Folder
 from hhnk_research_tools.general_functions import (
     check_create_new_file,
     ensure_file_path,
 )
@@ -219,15 +221,16 @@
             check_is_file = False
         else:
             check_is_file = True
         if (
             check_create_new_file(output_file=file_name, overwrite=overwrite, check_is_file=check_is_file)
             or driver == "MEM"
         ):
-            target_ds = gdal.GetDriverByName(driver).Create(
+            gdal_driver = gdal.GetDriverByName(driver)
+            target_ds = gdal_driver.Create(
                 str(file_name),
                 meta.x_res,
                 meta.y_res,
                 num_bands,
                 datatype,
                 options=create_options,
             )
@@ -277,16 +280,19 @@
             target_ds = None
     except Exception as e:
         raise e
 
 
 def build_vrt(raster_folder, vrt_name="combined_rasters", bandlist=[1], bounds=None, overwrite=False):
     """create vrt from all rasters in a folder.
-    bounds=(xmin, ymin, xmax, ymax)
-    bandList doesnt work as expected."""
+
+    raster_folder (str)
+    bounds (np.array): format should be; (xmin, ymin, xmax, ymax),
+        if None will use input files.
+    bandList doesnt work as expected, passing [1] works."""
     raster_folder = Folder(raster_folder)
     output_path = raster_folder.full_path(f"{vrt_name}.vrt")
 
     if output_path.exists() and not overwrite:
         print(f"vrt already exists: {output_path}")
         return
 
@@ -414,49 +420,50 @@
         x1, x2, y1, y2 = raster1.metadata.bounds
         xx1, xx2, yy1, yy2 = raster2.metadata.bounds
         bounds_diff = x1 - xx1, y1 - yy1, xx2 - x2, yy2 - y2  # subtract bounds
         check_arr = np.array([i <= 0 for i in bounds_diff])  # check if values <=0
 
         # If all are true (or all false) we know that the rasters fully overlap.
         if raster1.metadata.pixel_width != raster2.metadata.pixel_width:
-            raise Exception("""Rasters do not have equal resolution""")
+            raise Exception("Rasters do not have equal resolution")
 
         if np.all(check_arr):
             # In this case raster1 is the bigger raster.
             return raster1, raster2, {"raster1": "big", "raster2": "small"}
         elif np.all(~check_arr):
             # In this case raster2 is the bigger raster
             return raster2, raster1, {"raster1": "small", "raster2": "big"}
         else:
-            raise Exception("""Raster bounds do not overlap. We cannot use this.""")
+            raise Exception("Raster bounds do not overlap. We cannot use this.")
 
     def create(self, overwrite=False) -> bool:
         """Create empty output raster
-        returns bool wether the rest of the function should continue"""
+        returns bool wether the rest of the function should continue
+        """
         # Check if function should continue.
         cont = True
         if not overwrite and self.raster_out.exists():
             cont = False
 
-        if cont == True:
+        if cont is True:
             if self.verbose:
                 print(f"creating output raster: {self.raster_out.path}")
             target_ds = create_new_raster_file(
                 file_name=self.raster_out.path,
                 nodata=self.output_nodata,
                 meta=self.raster_small.metadata,
             )
             target_ds = None
         else:
             if self.verbose:
                 print(f"output raster already exists: {self.raster_out.path}")
         return cont
 
     def run(self, overwrite=False, **kwargs):
-        """loop over the small raster blocks, load both arrays and apply a custom function to it."""
+        """Loop over the small raster blocks, load both arrays and apply a custom function to it."""
         cont = self.create(overwrite=overwrite)
 
         if cont:
             target_ds = self.raster_out.open_gdal_source_write()
             band_out = target_ds.GetRasterBand(1)
 
             for idx, block_row in self.blocks_df.iterrows():
@@ -480,18 +487,18 @@
 
             band_out.FlushCache()  # close file after writing
             band_out = None
             target_ds = None
 
 
 def reproject(src: Raster, target_res: float, output_path: str):
-    """
-    src : hrt.Raster
+    """src : hrt.Raster
     output_path : str
-    meta_new : hrt.core"""
+    meta_new : hrt.core
+    """
     # https://svn.osgeo.org/gdal/trunk/autotest/alg/reproject.py
     src.metadata.update_resolution(target_res)
 
     src_ds = src.source
     dst_ds = create_new_raster_file(file_name=output_path, nodata=src.nodata, meta=src.metadata)
 
     if dst_ds is not None:
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/sql_functions.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/sql_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,19 @@
         return query
     except Exception as e:
         raise e from None
 
 
 # TODO REMOVE
 def create_sqlite_connection(database_path):
-    """Create connection to database. On windows with conda envs this requires the mod_spatialaite extension
+    r"""Create connection to database. On windows with conda envs this requires the mod_spatialaite extension
     to be installed explicitly. The location of this extension is stored in
     hhnk_research_tools.variables.MOD_SPATIALITE_PATH (C:\ProgramData\Anaconda3\mod_spatialite-5.0.1-win-amd64)
-    and can be downloaded from http://www.gaia-gis.it/gaia-sins/windows-bin-amd64/"""
+    and can be downloaded from http://www.gaia-gis.it/gaia-sins/windows-bin-amd64/
+    """
     try:
         conn = sqlite3.connect(database_path)
         conn.enable_load_extension(True)
         conn.execute("SELECT load_extension('mod_spatialite')")
         return conn
     except sqlite3.OperationalError as e:
         if e.args[0] == "The specified module could not be found.\r\n":
@@ -119,17 +120,15 @@
 
     except Exception as e:
         raise e from None
 
 
 # TODO REMOVE
 def sql_table_exists(database_path, table_name):
-    """
-    Checks if a table name exists in the specified database
-    """
+    """Check if a table name exists in the specified database"""
     try:
         query = f"""PRAGMA table_info({table_name})"""
         df = execute_sql_selection(query=query, database_path=database_path)
         return not df.empty
     except Exception as e:
         raise e from None
 
@@ -151,14 +150,15 @@
     except Exception as e:
         raise e from None
     finally:
         if kill_connection and conn is not None:
             conn.close()
 
 
+# TODO REMOVE
 def execute_sql_changes(query, database=None, conn=None):
     """
     Takes a query that changes the database and tries
     to execute it. On success, changes are committed.
     On a failure, rolls back to the state before
     the query was executed that caused the error
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/threedi/call_api.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/threedi/call_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import time
 
-from threedi_api_client.openapi import ApiException
-
 
 def call_threedi_api(func, max_retries=60, **kwargs):
-    """add something to simulation, if apiexcetion is raised sleep on it and try again."""
+    """Add something to simulation, if apiexcetion is raised sleep on it and try again."""
+    from threedi_api_client.openapi import ApiException  # Import here so its not a forced dependency
 
     for i in range(max_retries):
         try:
             # check if data is dict
             if "data" in kwargs.keys():
                 if type(kwargs["data"]) != dict:
                     print("OJEE... data is geen dict {func}")
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/threedi/geometry_functions.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/threedi/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/threedi/grid.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/threedi/grid.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/threedi/read_api_file.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/threedi/read_api_file.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/threedi/threediresult_loader.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/threedi/threediresult_loader.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/variables.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/variables.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg` & `hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg` & `hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg` & `hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg` & `hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/wss_calculations.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/wss_calculations.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/wss_loading.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/wss_loading.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools/waterschadeschatter/wss_main.py` & `hhnk_research_tools-2024.1/hhnk_research_tools/waterschadeschatter/wss_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # %%
 from osgeo import gdal
 
 import hhnk_research_tools as hrt
 import hhnk_research_tools.waterschadeschatter.wss_calculations as wss_calculations
 import hhnk_research_tools.waterschadeschatter.wss_loading as wss_loading
+from hhnk_research_tools.gis.raster import Raster
 
 gdal.UseExceptions()
 
 DMG_NODATA = 0
 
 
 class Waterschadeschatter:
@@ -33,16 +34,16 @@
         depth_file,
         landuse_file,
         wss_settings,
         min_block_size=2048,
     ):
         self.wss_settings = wss_settings
         self.min_block_size = min_block_size
-        self.lu_raster = hrt.Raster(landuse_file)
-        self.depth_raster = hrt.Raster(depth_file, self.min_block_size)
+        self.lu_raster = Raster(landuse_file)
+        self.depth_raster = Raster(depth_file, self.min_block_size)
         self.gamma_inundatiediepte = None
 
         self.validate()
 
         # Inladen configuratie
         self.dmg_table_landuse, self.dmg_table_general = wss_loading.read_dmg_table_config(self.wss_settings)
 
@@ -60,15 +61,15 @@
         indices = {}
         indices["herstelperiode"] = self.dmg_table_general["herstelperiode"].index(self.wss_settings["herstelperiode"])
         indices["maand"] = self.dmg_table_general["maand"].index(self.wss_settings["maand"])
         return indices
 
     def run(
         self,
-        output_raster: hrt.Raster,
+        output_raster: Raster,
         calculation_type="sum",
         verbose=False,
         overwrite=False,
     ):
         """
         Calculation type options: 'sum','direct','indirect'
         """
@@ -104,14 +105,15 @@
             window_lu = window_depth.copy()
             window_lu[0] += dx_min
             window_lu[1] += dy_min
 
             lu_block = self.lu_raster._read_array(window=window_lu)
             lu_block = lu_block.astype(int)
             lu_block[lu_block == self.lu_raster.nodata] = 0
+            # TODO np.all(self.polder==folder.dst.tmp.polder.nodata) is mogelijk net iets sneller.
             if lu_block.mean() != 0:
                 # Load depth
                 depth_block = self.depth_raster._read_array(window=window_depth)
                 # depth_mask = depth_block==self.depth_raster.nodata
                 # depth_block[depth_mask] = np.nan #Schadetabel loopt vanaf -0.01cm
 
                 # Calculate damage
@@ -172,12 +174,12 @@
             depth_file=depth_file,
             landuse_file=landuse_file,
             wss_settings=wss_settings,
         )
 
         # Berkenen schaderaster
         self.run(
-            output_raster=hrt.Raster(output_file),
+            output_raster=Raster(output_file),
             calculation_type="sum",
             verbose=True,
             overwrite=False,
         )
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools.egg-info/PKG-INFO` & `hhnk_research_tools-2024.1/hhnk_research_tools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 Metadata-Version: 2.1
-Name: hhnk-research-tools
-Version: 2023.4
+Name: hhnk_research_tools
+Version: 2024.1
 Summary: General tools for analysis, data manipulation and threedi interaction for analysis of water systems
 Home-page: https://github.com/HHNK/hhnk-research-tools
 Author: Wietse van Gerwen
 Author-email: w.vangerwen@hhnk.nl
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HHNK/hhnk-research-tools/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-
-UNKNOWN
-
```

### Comparing `hhnk_research_tools-2023.4/hhnk_research_tools.egg-info/SOURCES.txt` & `hhnk_research_tools-2024.1/hhnk_research_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 hhnk_research_tools/folder_file_classes/__init__.py
 hhnk_research_tools/folder_file_classes/file_class.py
 hhnk_research_tools/folder_file_classes/folder_file_classes.py
 hhnk_research_tools/folder_file_classes/sqlite_class.py
 hhnk_research_tools/folder_file_classes/threedi_schematisation.py
 hhnk_research_tools/gis/__init__.py
 hhnk_research_tools/gis/raster.py
+hhnk_research_tools/gis/raster_calculator.py
 hhnk_research_tools/gis/vector.py
 hhnk_research_tools/threedi/__init__.py
 hhnk_research_tools/threedi/call_api.py
 hhnk_research_tools/threedi/geometry_functions.py
 hhnk_research_tools/threedi/grid.py
 hhnk_research_tools/threedi/read_api_file.py
 hhnk_research_tools/threedi/threediresult_loader.py
```

### Comparing `hhnk_research_tools-2023.4/setup.py` & `hhnk_research_tools-2024.1/setup.py`

 * *Files identical despite different names*

