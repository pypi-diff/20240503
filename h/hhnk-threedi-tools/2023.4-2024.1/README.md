# Comparing `tmp/hhnk-threedi-tools-2023.4.tar.gz` & `tmp/hhnk_threedi_tools-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk-threedi-tools-2023.4.tar", last modified: Thu Nov  9 12:25:03 2023, max compression
+gzip compressed data, was "hhnk_threedi_tools-2024.1.tar", last modified: Fri May  3 11:05:26 2024, max compression
```

## Comparing `hhnk-threedi-tools-2023.4.tar` & `hhnk_threedi_tools-2024.1.tar`

### file list

```diff
@@ -1,334 +1,338 @@
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:42.371443 hhnk-threedi-tools-2023.4/
--rw-rw-rw-   0        0        0      245 2023-06-19 15:02:38.000000 hhnk-threedi-tools-2023.4/MANIFEST.in
--rw-rw-rw-   0        0        0      578 2023-11-09 12:25:03.211641 hhnk-threedi-tools-2023.4/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-11-01 09:17:51.000000 hhnk-threedi-tools-2023.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:42.402444 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/
--rw-rw-rw-   0        0        0     1439 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:42.713449 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/
--rw-rw-rw-   0        0        0       50 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:43.184457 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/__init__.py
--rw-rw-rw-   0        0        0    41098 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/calculation.py
--rw-rw-rw-   0        0        0    90970 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/calculation_gui_class.py
--rw-rw-rw-   0        0        0     2833 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/download_functions.py
--rw-rw-rw-   0        0        0    70874 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/download_gui_class.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:43.833468 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/__init__.py
--rw-rw-rw-   0        0        0    28944 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/bank_levels.py
--rw-rw-rw-   0        0        0     5699 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/grid_result_metadata.py
--rw-rw-rw-   0        0        0    21409 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/model_state.py
--rw-rw-rw-   0        0        0    17114 2023-11-09 12:12:00.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/one_d_two_d.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:44.068472 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/sqlite/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/sqlite/__init__.py
--rw-rw-rw-   0        0        0    30415 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py
--rw-rw-rw-   0        0        0     8123 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/sqlite/structure_control.py
--rw-rw-rw-   0        0        0    13564 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/zero_d_one_d.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:44.503479 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/
--rw-rw-rw-   0        0        0        0 2022-04-12 14:08:35.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/__init__.py
--rw-rw-rw-   0        0        0     6726 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py
--rw-rw-rw-   0        0        0     8218 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_main.py
--rw-rw-rw-   0        0        0    10558 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py
--rw-rw-rw-   0        0        0    15205 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py
--rw-rw-rw-   0        0        0     1807 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py
--rw-rw-rw-   0        0        0     1994 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py
--rw-rw-rw-   0        0        0     5083 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py
--rw-rw-rw-   0        0        0     3181 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py
--rw-rw-rw-   0        0        0     4062 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py
--rw-rw-rw-   0        0        0     6016 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/folder_helpers.py
--rw-rw-rw-   0        0        0    22442 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/folders.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:44.629481 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/result_rasters/
--rw-rw-rw-   0        0        0        0 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/result_rasters/__init__.py
--rw-rw-rw-   0        0        0     9868 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/result_rasters/calculate_raster.py
--rw-rw-rw-   0        0        0     9618 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:44.966487 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/
--rw-rw-rw-   0        0        0        0 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/__init__.py
--rw-rw-rw-   0        0        0     4426 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/migrate.py
--rw-rw-rw-   0        0        0     5581 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/model_backup.py
--rw-rw-rw-   0        0        0    14635 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/model_splitter.py
--rw-rw-rw-   0        0        0     9149 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/upload.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:45.138489 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/external/
--rw-rw-rw-   0        0        0        0 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/external/__init__.py
--rw-rw-rw-   0        0        0    31990 2023-11-06 13:42:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/external/downloader.py
--rw-rw-rw-   0        0        0    44747 2023-11-06 13:43:08.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/external/threedi_calls.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:45.235491 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/qgis/
--rw-rw-rw-   0        0        0      156 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/qgis/__init__.py
--rw-rw-rw-   0        0        0    13998 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/qgis/layer_structure.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:45.864501 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:45.935503 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/__pycache__/
--rw-rw-rw-   0        0        0      167 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      171 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9293 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/model_settings.xlsx
--rw-rw-rw-   0        0        0     9664 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/model_settings_default.xlsx
--rw-rw-rw-   0        0        0    12764 2023-01-09 08:28:05.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/precipitation_frequency.xlsx
--rw-rw-rw-   0        0        0  2080345 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif
--rw-rw-rw-   0        0        0     1167 2023-10-18 09:31:35.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif.aux.xml
--rw-rw-rw-   0        0        0    43028 2023-11-01 10:20:42.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_structure.csv
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:45.982504 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:46.096505 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/
--rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_cross_sections.qml
--rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_flowlines.qml
--rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_watergangen.qml
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:46.241508 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/grid/
--rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/grid/cells.qml
--rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/grid/lines.qml
--rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/grid/nodes.qml
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:49.011554 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/
--rw-rw-rw-   0        0        0     1572 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Landgebruik (v1801c).qml
--rw-rw-rw-   0        0        0     5072 2023-11-01 10:20:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Luchtfoto Actueel Ortho 25cm RGB.qml
--rw-rw-rw-   0        0        0     5052 2023-11-01 10:20:44.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/brtachtergrondkaartgrijs.qml
--rw-rw-rw-   0        0        0     6634 2023-11-01 10:20:44.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast.qml
--rw-rw-rw-   0        0        0     6664 2023-11-01 10:20:44.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast_correctie.qml
--rw-rw-rw-   0        0        0     6622 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas.qml
--rw-rw-rw-   0        0        0     6652 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas_correctie.qml
--rw-rw-rw-   0        0        0     3558 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/geen_schade.qml
--rw-rw-rw-   0        0        0     1797 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatiediepte.qml
--rw-rw-rw-   0        0        0     4392 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0010.qml
--rw-rw-rw-   0        0        0     4173 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0100.qml
--rw-rw-rw-   0        0        0     7578 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T1000.qml
--rw-rw-rw-   0        0        0    11908 2023-11-01 10:20:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/maskerkaart.qml
--rw-rw-rw-   0        0        0    16130 2023-11-01 10:20:46.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/peilgebieden.qml
--rw-rw-rw-   0        0        0    10960 2023-11-01 10:20:46.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon.qml
--rw-rw-rw-   0        0        0    10967 2023-11-01 10:20:46.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon_wit.qml
--rw-rw-rw-   0        0        0    47288 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/ruimtekaart.qml
--rw-rw-rw-   0        0        0    15789 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied.qml
--rw-rw-rw-   0        0        0    15789 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_correctie.qml
--rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast.qml
--rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast_correctie.qml
--rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas.qml
--rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas_correctie.qml
--rw-rw-rw-   0        0        0     9533 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/waterlevel.qml
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:49.232558 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/
--rw-rw-rw-   0        0        0    30275 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_amount.qml
--rw-rw-rw-   0        0        0    15023 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_dry_category.qml
--rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/grid_nodes_2d.qml
--rw-rw-rw-   0        0        0     2726 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterdepth.qml
--rw-rw-rw-   0        0        0     2377 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterlevel.qml
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:49.755566 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/
--rw-rw-rw-   0        0        0    78145 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_depth.qml
--rw-rw-rw-   0        0        0   156909 2023-11-01 10:20:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_width.qml
--rw-rw-rw-   0        0        0    11958 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/controlled_structs.qml
--rw-rw-rw-   0        0        0    24563 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_duplicates.qml
--rw-rw-rw-   0        0        0    33286 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_no_vertex.qml
--rw-rw-rw-   0        0        0     2618 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/dewatering_depth.qml
--rw-rw-rw-   0        0        0     1989 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/isolated_channels.qml
--rw-rw-rw-   0        0        0    10982 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/structs_channel.qml
--rw-rw-rw-   0        0        0     7480 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/watersurface_area.qml
--rw-rw-rw-   0        0        0    10686 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/weir_height.qml
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:58.979720 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/
--rw-rw-rw-   0        0        0     5194 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_aquaduct.qml
--rw-rw-rw-   0        0        0    33764 2023-11-01 10:20:48.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_brug.qml
--rw-rw-rw-   0        0        0    46543 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_duiker.qml
--rw-rw-rw-   0        0        0    13222 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_gemaal.qml
--rw-rw-rw-   0        0        0    27700 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_sluis.qml
--rw-rw-rw-   0        0        0    53506 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_stuw.qml
--rw-rw-rw-   0        0        0    21540 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vaste_dam.qml
--rw-rw-rw-   0        0        0    11620 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vispassage.qml
--rw-rw-rw-   0        0        0    33715 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/HDB_stuw_automatisch.qml
--rw-rw-rw-   0        0        0     7684 2023-11-01 10:20:49.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_lijn.qml
--rw-rw-rw-   0        0        0    15803 2023-11-01 10:20:50.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_punt.qml
--rw-rw-rw-   0        0        0    20972 2023-11-01 10:20:50.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bodemhoogte_kunstwerken.qml
--rw-rw-rw-   0        0        0    11409 2023-11-01 10:20:50.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/boezem.qml
--rw-rw-rw-   0        0        0    45734 2023-11-01 10:20:50.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_niet_in_model.qml
--rw-rw-rw-   0        0        0    45760 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_wel_in_model.qml
--rw-rw-rw-   0        0        0     9432 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/channel_surface_from_profiles.qml
--rw-rw-rw-   0        0        0     9340 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dam.qml
--rw-rw-rw-   0        0        0    14944 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_gw_pro.qml
--rw-rw-rw-   0        0        0    18273 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_waterdeel.qml
--rw-rw-rw-   0        0        0    21856 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_crosssection.qml
--rw-rw-rw-   0        0        0    25112 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_output_channel.qml
--rw-rw-rw-   0        0        0     6891 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem.qml
--rw-rw-rw-   0        0        0     4910 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem_hillshade.qml
--rw-rw-rw-   0        0        0     2619 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/drooglegging.qml
--rw-rw-rw-   0        0        0    15096 2023-11-01 10:20:51.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker,_syphon,_hevel_(lijn).qml
--rw-rw-rw-   0        0        0    28513 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_bob.qml
--rw-rw-rw-   0        0        0    30808 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_doorstroomafmeting.qml
--rw-rw-rw-   0        0        0    16231 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_syphon_hevel.qml
--rw-rw-rw-   0        0        0    60798 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_niet_in_model.qml
--rw-rw-rw-   0        0        0    60802 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_wel_in_model.qml
--rw-rw-rw-   0        0        0    25449 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_lijn.qml
--rw-rw-rw-   0        0        0    27914 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_punt.qml
--rw-rw-rw-   0        0        0     6882 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/friction.qml
--rw-rw-rw-   0        0        0     5559 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/geisoleerde_watergangen.qml
--rw-rw-rw-   0        0        0    44016 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_niet_in_model.qml
--rw-rw-rw-   0        0        0    13458 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_peilafwijking.qml
--rw-rw-rw-   0        0        0    44020 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_wel_in_model.qml
--rw-rw-rw-   0        0        0    21867 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemeten_niet_in_model.qml
--rw-rw-rw-   0        0        0    19432 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gestuurde_kunstwerken.qml
--rw-rw-rw-   0        0        0    12551 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_kunstwerken.qml
--rw-rw-rw-   0        0        0    12053 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_watergang_segmenten.qml
--rw-rw-rw-   0        0        0    38443 2023-11-01 10:20:52.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_duikers_op_peilgrens.qml
--rw-rw-rw-   0        0        0    23645 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_gemalen_op_peilgrens.qml
--rw-rw-rw-   0        0        0     8444 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_levee_overstromingsmodel.qml
--rw-rw-rw-   0        0        0    29529 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_stuwen_op_peilgrens.qml
--rw-rw-rw-   0        0        0    89775 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hydro_deelgebieden_(hdb).qml
--rw-rw-rw-   0        0        0     6842 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/infiltration.qml
--rw-rw-rw-   0        0        0     9964 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/kzk.qml
--rw-rw-rw-   0        0        0    15707 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/levee_30_cm_boven_max_peil.qml
--rw-rw-rw-   0        0        0     6540 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/luchtfoto_actueel_ortho_25cm_rgb.qml
--rw-rw-rw-   0        0        0     8715 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_lines.qml
--rw-rw-rw-   0        0        0     8500 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_points.qml
--rw-rw-rw-   0        0        0    10673 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ernstig.qml
--rw-rw-rw-   0        0        0    10675 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_naar_kijken.qml
--rw-rw-rw-   0        0        0    10690 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ter_info.qml
--rw-rw-rw-   0        0        0     1657 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/openstreetmap.qml
--rw-rw-rw-   0        0        0     6927 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/opmerkingen.qml
--rw-rw-rw-   0        0        0   145908 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo).qml
--rw-rw-rw-   0        0        0    61961 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo_huidig).qml
--rw-rw-rw-   0        0        0    43564 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebied_aanname_streefpeil.qml
--rw-rw-rw-   0        0        0    37659 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebieden_(datacheck).qml
--rw-rw-rw-   0        0        0    72597 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo).qml
--rw-rw-rw-   0        0        0    34786 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo_huidig).qml
--rw-rw-rw-   0        0        0    24754 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/polder_polygon.qml
--rw-rw-rw-   0        0        0     6666 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ggg.qml
--rw-rw-rw-   0        0        0     6666 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ghg.qml
--rw-rw-rw-   0        0        0     6780 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_glg.qml
--rw-rw-rw-   0        0        0    27502 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuw_aanname_breedte.qml
--rw-rw-rw-   0        0        0    47966 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_niet_in_model.qml
--rw-rw-rw-   0        0        0    47970 2023-11-01 10:20:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_wel_in_model.qml
--rw-rw-rw-   0        0        0     6857 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions.qml
--rw-rw-rw-   0        0        0    12238 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions_view.qml
--rw-rw-rw-   0        0        0     5498 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral.qml
--rw-rw-rw-   0        0        0    10994 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral_view.qml
--rw-rw-rw-   0        0        0    11645 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_boundary_conditions.qml
--rw-rw-rw-   0        0        0     9996 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_lateral.qml
--rw-rw-rw-   0        0        0    11540 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_aggregation_settings.qml
--rw-rw-rw-   0        0        0    17656 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_channel.qml
--rw-rw-rw-   0        0        0    21232 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_connection_nodes.qml
--rw-rw-rw-   0        0        0     7617 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_definition.qml
--rw-rw-rw-   0        0        0    15527 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location.qml
--rw-rw-rw-   0        0        0    23555 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location_view.qml
--rw-rw-rw-   0        0        0    27193 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert.qml
--rw-rw-rw-   0        0        0    47426 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert_view.qml
--rw-rw-rw-   0        0        0     8046 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_dem_average_area.qml
--rw-rw-rw-   0        0        0    53502 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_global_settings.qml
--rw-rw-rw-   0        0        0    21490 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement.qml
--rw-rw-rw-   0        0        0    27705 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement_area.qml
--rw-rw-rw-   0        0        0    27896 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_groundwater.qml
--rw-rw-rw-   0        0        0    31655 2023-11-01 10:20:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface.qml
--rw-rw-rw-   0        0        0     6403 2023-11-01 10:20:55.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface_map.qml
--rw-rw-rw-   0        0        0    12028 2023-11-01 10:20:55.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_interflow.qml
--rw-rw-rw-   0        0        0    39633 2023-11-01 10:20:55.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_levee.qml
--rw-rw-rw-   0        0        0    17417 2023-11-01 10:20:55.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole.qml
--rw-rw-rw-   0        0        0    45493 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole_view.qml
--rw-rw-rw-   0        0        0    26442 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_numerical_settings.qml
--rw-rw-rw-   0        0        0    10463 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_obstacle.qml
--rw-rw-rw-   0        0        0    18741 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice.qml
--rw-rw-rw-   0        0        0    62499 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice_view.qml
--rw-rw-rw-   0        0        0    23573 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe.qml
--rw-rw-rw-   0        0        0    60552 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe_view.qml
--rw-rw-rw-   0        0        0    16415 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation.qml
--rw-rw-rw-   0        0        0    24185 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_point_view.qml
--rw-rw-rw-   0        0        0    28752 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_view.qml
--rw-rw-rw-   0        0        0     8555 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_simple_infiltration.qml
--rw-rw-rw-   0        0        0    16667 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface.qml
--rw-rw-rw-   0        0        0     7487 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_map.qml
--rw-rw-rw-   0        0        0    10465 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_parameters.qml
--rw-rw-rw-   0        0        0    18641 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir.qml
--rw-rw-rw-   0        0        0    62454 2023-11-01 10:20:56.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir_view.qml
--rw-rw-rw-   0        0        0    11236 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_windshielding.qml
--rw-rw-rw-   0        0        0    28738 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_niet_in_model.qml
--rw-rw-rw-   0        0        0    25998 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_wel_in_model.qml
--rw-rw-rw-   0        0        0    11163 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_loose.qml
--rw-rw-rw-   0        0        0    11043 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.qml
--rw-rw-rw-   0        0        0     1202 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.sld
--rw-rw-rw-   0        0        0    67455 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.qml
--rw-rw-rw-   0        0        0    33473 2023-11-01 10:20:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.sld
--rw-rw-rw-   0        0        0   100574 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.qml
--rw-rw-rw-   0        0        0    51192 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.sld
--rw-rw-rw-   0        0        0    11410 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.qml
--rw-rw-rw-   0        0        0     1271 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.sld
--rw-rw-rw-   0        0        0    14996 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.qml
--rw-rw-rw-   0        0        0     3690 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.sld
--rw-rw-rw-   0        0        0    22539 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.qml
--rw-rw-rw-   0        0        0     3663 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.sld
--rw-rw-rw-   0        0        0     1747 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.qml
--rw-rw-rw-   0        0        0      705 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.sld
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:59.586730 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/
--rw-rw-rw-   0        0        0    21226 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__default.qml
--rw-rw-rw-   0        0        0    92565 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__detailed.qml
--rw-rw-rw-   0        0        0     8911 2023-11-01 10:20:58.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/discharge.qml
--rw-rw-rw-   0        0        0    29841 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_kunstwerken.qml
--rw-rw-rw-   0        0        0    42981 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_watergangen.qml
--rw-rw-rw-   0        0        0    12056 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_end_rain_min_1.qml
--rw-rw-rw-   0        0        0    82279 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__default.qml
--rw-rw-rw-   0        0        0    18046 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__original.qml
--rw-rw-rw-   0        0        0    12051 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_sum_start_sum.qml
--rw-rw-rw-   0        0        0    12053 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_start_rain_vs_start_sum.qml
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:59.817734 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/__init__.py
--rw-rw-rw-   0        0        0    42269 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten.qpt
--rw-rw-rw-   0        0        0    42681 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten2.qpt
--rw-rw-rw-   0        0        0    42333 2023-11-01 10:20:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten_landscape.qpt
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:00.001737 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:00.423744 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/
--rw-rw-rw-   0        0        0      163 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      167 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    14142 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc
--rw-rw-rw-   0        0        0    15662 2023-11-06 13:43:46.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc
--rw-rw-rw-   0        0        0    12108 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc
--rw-rw-rw-   0        0        0    12557 2023-11-06 13:43:47.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:01.006754 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:01.227757 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     1986 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb
--rw-rw-rw-   0        0        0     5495 2023-04-11 15:21:12.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb
--rw-rw-rw-   0        0        0     1963 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb
--rw-rw-rw-   0        0        0     5026 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb
--rw-rw-rw-   0        0        0    23873 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb
--rw-rw-rw-   0        0        0     6876 2023-11-01 09:17:53.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb
--rw-rw-rw-   0        0        0     2090 2023-06-21 07:55:43.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:01.630764 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/
--rw-rw-rw-   0        0        0      179 2022-01-31 10:15:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      177 2022-06-29 11:24:40.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1323 2023-11-06 08:43:16.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/net.cpython-39.pyc
--rw-rw-rw-   0        0        0      847 2023-06-21 10:23:54.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc
--rw-rw-rw-   0        0        0     6121 2023-04-25 11:04:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc
--rw-rw-rw-   0        0        0     6280 2023-11-06 13:38:11.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc
--rw-rw-rw-   0        0        0      300 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/constants.py
--rw-rw-rw-   0        0        0      462 2023-07-18 09:43:59.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/notebook_data.json
--rw-rw-rw-   0        0        0      598 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/notebook_setup.py
--rw-rw-rw-   0        0        0     7322 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/run.py
--rw-rw-rw-   0        0        0    20260 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/queries.py
--rw-rw-rw-   0        0        0    25162 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/queries_general_checks.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:02.458778 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/__init__.py
--rw-rw-rw-   0        0        0     1850 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/api_settings.py
--rw-rw-rw-   0        0        0      256 2023-11-06 13:43:39.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/backups_table_names.py
--rw-rw-rw-   0        0        0     1043 2023-11-06 13:43:45.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/bank_levels.py
--rw-rw-rw-   0        0        0     1649 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/database_aliases.py
--rw-rw-rw-   0        0        0     2601 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/database_variables.py
--rw-rw-rw-   0        0        0      134 2023-05-06 10:58:04.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/datachecker_variables.py
--rw-rw-rw-   0        0        0      162 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/default_variables.py
--rw-rw-rw-   0        0        0      130 2023-05-06 07:30:57.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/definitions.py
--rw-rw-rw-   0        0        0      618 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/model_state.py
--rw-rw-rw-   0        0        0      953 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/one_d_two_d.py
--rw-rw-rw-   0        0        0      830 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/sqlite.py
--rw-rw-rw-   0        0        0      254 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/weirs.py
--rw-rw-rw-   0        0        0     1777 2023-11-09 12:12:01.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/zero_d_one_d.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:24:42.610447 hhnk-threedi-tools-2023.4/hhnk_threedi_tools.egg-info/
--rw-rw-rw-   0        0        0      578 2023-11-09 12:24:41.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    21873 2023-11-09 12:24:41.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-09 12:24:41.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-11-09 12:24:41.000000 hhnk-threedi-tools-2023.4/hhnk_threedi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-09 12:25:03.233055 hhnk-threedi-tools-2023.4/setup.cfg
--rw-rw-rw-   0        0        0     1659 2023-06-21 07:43:33.000000 hhnk-threedi-tools-2023.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:02.996787 hhnk-threedi-tools-2023.4/tests/
-drwxrwxrwx   0        0        0        0 2023-11-09 12:25:03.170790 hhnk-threedi-tools-2023.4/tests/notebooks/
--rw-rw-rw-   0        0        0        0 2023-11-01 09:17:54.000000 hhnk-threedi-tools-2023.4/tests/notebooks/__init__.py
--rw-rw-rw-   0        0        0      620 2023-11-01 09:17:54.000000 hhnk-threedi-tools-2023.4/tests/notebooks/notebook_setup.py
--rw-rw-rw-   0        0        0     3330 2023-11-01 09:17:54.000000 hhnk-threedi-tools-2023.4/tests/notebooks/rtest_lizardapi.py
--rw-rw-rw-   0        0        0      569 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/notebooks/rtest_notebooks.py
--rw-rw-rw-   0        0        0     1258 2023-11-01 10:21:00.000000 hhnk-threedi-tools-2023.4/tests/notebooks/rtest_upload_schema.py
--rw-rw-rw-   0        0        0     4365 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_bank_level_check.py
--rw-rw-rw-   0        0        0     2220 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_calculation_gui.py
--rw-rw-rw-   0        0        0     2936 2023-11-02 07:34:41.000000 hhnk-threedi-tools-2023.4/tests/test_folder_structures.py
--rw-rw-rw-   0        0        0     2120 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_klimaatsommen_prep.py
--rw-rw-rw-   0        0        0     2209 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_modelsplitter.py
--rw-rw-rw-   0        0        0     1983 2023-11-01 09:20:20.000000 hhnk-threedi-tools-2023.4/tests/test_one_d_two_d.py
--rw-rw-rw-   0        0        0     2121 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_result_rasters.py
--rw-rw-rw-   0        0        0     1182 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_schema_migration.py
--rw-rw-rw-   0        0        0     5225 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_sqlite.py
--rw-rw-rw-   0        0        0     1078 2023-11-01 09:17:55.000000 hhnk-threedi-tools-2023.4/tests/test_zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.831014 hhnk_threedi_tools-2024.1/
+-rw-rw-rw-   0        0        0      245 2023-06-19 15:02:38.000000 hhnk_threedi_tools-2024.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      528 2024-05-03 11:05:26.808031 hhnk_threedi_tools-2024.1/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-11-01 09:17:51.000000 hhnk_threedi_tools-2024.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.758926 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/
+-rw-rw-rw-   0        0        0     1590 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.826929 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/
+-rw-rw-rw-   0        0        0       50 2021-12-13 08:25:18.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.864928 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/__init__.py
+-rw-rw-rw-   0        0        0    41016 2024-05-03 11:04:02.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/calculation.py
+-rw-rw-rw-   0        0        0    90970 2023-11-16 09:48:32.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/calculation_gui_class.py
+-rw-rw-rw-   0        0        0     2833 2023-11-09 12:12:00.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/download_functions.py
+-rw-rw-rw-   0        0        0    71229 2024-05-03 11:04:02.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/download_gui_class.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.893927 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/__init__.py
+-rw-rw-rw-   0        0        0    29344 2024-04-29 15:28:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/bank_levels.py
+-rw-rw-rw-   0        0        0     5673 2024-03-20 13:17:39.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/grid_result_metadata.py
+-rw-rw-rw-   0        0        0    21409 2023-11-09 12:12:00.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/model_state.py
+-rw-rw-rw-   0        0        0     9532 2024-03-20 13:17:39.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/one_d_two_d.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.906930 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/sqlite/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/sqlite/__init__.py
+-rw-rw-rw-   0        0        0    30425 2024-05-03 11:04:02.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py
+-rw-rw-rw-   0        0        0     8139 2024-05-03 11:04:02.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/sqlite/structure_control.py
+-rw-rw-rw-   0        0        0    13636 2024-04-29 07:35:33.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.954310 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/
+-rw-rw-rw-   0        0        0        0 2022-04-12 14:08:35.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     6726 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py
+-rw-rw-rw-   0        0        0     8218 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_main.py
+-rw-rw-rw-   0        0        0    10659 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py
+-rw-rw-rw-   0        0        0    15205 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py
+-rw-rw-rw-   0        0        0     1807 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py
+-rw-rw-rw-   0        0        0     1994 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py
+-rw-rw-rw-   0        0        0     5083 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py
+-rw-rw-rw-   0        0        0     3181 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py
+-rw-rw-rw-   0        0        0     4062 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py
+-rw-rw-rw-   0        0        0     6016 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/folder_helpers.py
+-rw-rw-rw-   0        0        0    21577 2024-05-03 11:04:02.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/folders.py
+-rw-rw-rw-   0        0        0     3364 2023-11-22 08:54:11.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/folders_modelbuilder.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.963150 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/result_rasters/
+-rw-rw-rw-   0        0        0        0 2023-06-13 10:35:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/result_rasters/__init__.py
+-rw-rw-rw-   0        0        0     9912 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/result_rasters/calculate_raster.py
+-rw-rw-rw-   0        0        0    17840 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:23.989054 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/
+-rw-rw-rw-   0        0        0        0 2023-11-01 09:17:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/__init__.py
+-rw-rw-rw-   0        0        0     4426 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/migrate.py
+-rw-rw-rw-   0        0        0     5581 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/model_backup.py
+-rw-rw-rw-   0        0        0    14546 2024-04-30 11:49:16.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/model_splitter.py
+-rw-rw-rw-   0        0        0     9149 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/upload.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.000481 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/external/
+-rw-rw-rw-   0        0        0        0 2023-11-01 09:17:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/external/__init__.py
+-rw-rw-rw-   0        0        0    31990 2023-11-17 12:01:34.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/external/downloader.py
+-rw-rw-rw-   0        0        0    44747 2023-11-06 13:43:08.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/external/threedi_calls.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.035956 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/qgis/
+-rw-rw-rw-   0        0        0      156 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/qgis/__init__.py
+-rw-rw-rw-   0        0        0    13998 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/qgis/layer_structure.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.148478 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.172245 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/__pycache__/
+-rw-rw-rw-   0        0        0      167 2022-07-14 07:53:38.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      171 2022-07-06 13:22:12.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9293 2023-11-01 09:17:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/model_settings.xlsx
+-rw-rw-rw-   0        0        0     9664 2023-11-01 09:17:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/model_settings_default.xlsx
+-rw-rw-rw-   0        0        0    12764 2023-01-09 08:28:05.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/precipitation_frequency.xlsx
+-rw-rw-rw-   0        0        0  2080345 2021-12-13 08:25:18.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif
+-rw-rw-rw-   0        0        0     1167 2023-10-18 09:31:35.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif.aux.xml
+-rw-rw-rw-   0        0        0    43036 2024-05-03 11:04:02.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_structure.csv
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.192528 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.208259 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/
+-rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_cross_sections.qml
+-rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_flowlines.qml
+-rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_watergangen.qml
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.222544 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/grid/
+-rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/grid/cells.qml
+-rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/grid/lines.qml
+-rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/grid/nodes.qml
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.352826 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/
+-rw-rw-rw-   0        0        0     1572 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Landgebruik (v1801c).qml
+-rw-rw-rw-   0        0        0     5072 2023-11-01 10:20:43.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Luchtfoto Actueel Ortho 25cm RGB.qml
+-rw-rw-rw-   0        0        0     5052 2023-11-01 10:20:44.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/brtachtergrondkaartgrijs.qml
+-rw-rw-rw-   0        0        0     6634 2023-11-01 10:20:44.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast.qml
+-rw-rw-rw-   0        0        0     6664 2023-11-01 10:20:44.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast_correctie.qml
+-rw-rw-rw-   0        0        0     6622 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas.qml
+-rw-rw-rw-   0        0        0     6652 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas_correctie.qml
+-rw-rw-rw-   0        0        0     3558 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/geen_schade.qml
+-rw-rw-rw-   0        0        0     1797 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatiediepte.qml
+-rw-rw-rw-   0        0        0     4392 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0010.qml
+-rw-rw-rw-   0        0        0     4173 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0100.qml
+-rw-rw-rw-   0        0        0     7578 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T1000.qml
+-rw-rw-rw-   0        0        0    11908 2023-11-01 10:20:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/maskerkaart.qml
+-rw-rw-rw-   0        0        0    16130 2023-11-01 10:20:46.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/peilgebieden.qml
+-rw-rw-rw-   0        0        0    10960 2023-11-01 10:20:46.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon.qml
+-rw-rw-rw-   0        0        0    10967 2023-11-01 10:20:46.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon_wit.qml
+-rw-rw-rw-   0        0        0    47288 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/ruimtekaart.qml
+-rw-rw-rw-   0        0        0    15789 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied.qml
+-rw-rw-rw-   0        0        0    15789 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_correctie.qml
+-rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast.qml
+-rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast_correctie.qml
+-rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas.qml
+-rw-rw-rw-   0        0        0    15687 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas_correctie.qml
+-rw-rw-rw-   0        0        0     9533 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/waterlevel.qml
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.408911 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/
+-rw-rw-rw-   0        0        0    30275 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_amount.qml
+-rw-rw-rw-   0        0        0    15023 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_dry_category.qml
+-rw-rw-rw-   0        0        0     1443 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/grid_nodes_2d.qml
+-rw-rw-rw-   0        0        0     2726 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterdepth.qml
+-rw-rw-rw-   0        0        0     2377 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterlevel.qml
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:24.572706 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/
+-rw-rw-rw-   0        0        0    78145 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_depth.qml
+-rw-rw-rw-   0        0        0   156909 2023-11-01 10:20:47.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_width.qml
+-rw-rw-rw-   0        0        0    11958 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/controlled_structs.qml
+-rw-rw-rw-   0        0        0    24563 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_duplicates.qml
+-rw-rw-rw-   0        0        0    33286 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_no_vertex.qml
+-rw-rw-rw-   0        0        0     2618 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/dewatering_depth.qml
+-rw-rw-rw-   0        0        0     1989 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/isolated_channels.qml
+-rw-rw-rw-   0        0        0    10982 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/structs_channel.qml
+-rw-rw-rw-   0        0        0     7480 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/watersurface_area.qml
+-rw-rw-rw-   0        0        0    10686 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/weir_height.qml
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:25.977916 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/
+-rw-rw-rw-   0        0        0     5194 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_aquaduct.qml
+-rw-rw-rw-   0        0        0    33764 2023-11-01 10:20:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_brug.qml
+-rw-rw-rw-   0        0        0    46543 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_duiker.qml
+-rw-rw-rw-   0        0        0    13222 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_gemaal.qml
+-rw-rw-rw-   0        0        0    27700 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_sluis.qml
+-rw-rw-rw-   0        0        0    53506 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_stuw.qml
+-rw-rw-rw-   0        0        0    21540 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vaste_dam.qml
+-rw-rw-rw-   0        0        0    11620 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vispassage.qml
+-rw-rw-rw-   0        0        0    33715 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/HDB_stuw_automatisch.qml
+-rw-rw-rw-   0        0        0     7684 2023-11-01 10:20:49.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_lijn.qml
+-rw-rw-rw-   0        0        0    15803 2023-11-01 10:20:50.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_punt.qml
+-rw-rw-rw-   0        0        0    20972 2023-11-01 10:20:50.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bodemhoogte_kunstwerken.qml
+-rw-rw-rw-   0        0        0    11409 2023-11-01 10:20:50.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/boezem.qml
+-rw-rw-rw-   0        0        0    45734 2023-11-01 10:20:50.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_niet_in_model.qml
+-rw-rw-rw-   0        0        0    45760 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_wel_in_model.qml
+-rw-rw-rw-   0        0        0     9432 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/channel_surface_from_profiles.qml
+-rw-rw-rw-   0        0        0     9340 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dam.qml
+-rw-rw-rw-   0        0        0    14944 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_gw_pro.qml
+-rw-rw-rw-   0        0        0    18273 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_waterdeel.qml
+-rw-rw-rw-   0        0        0    21856 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_crosssection.qml
+-rw-rw-rw-   0        0        0    25112 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_output_channel.qml
+-rw-rw-rw-   0        0        0     6891 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem.qml
+-rw-rw-rw-   0        0        0     4910 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem_hillshade.qml
+-rw-rw-rw-   0        0        0     2619 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/drooglegging.qml
+-rw-rw-rw-   0        0        0    15096 2023-11-01 10:20:51.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker,_syphon,_hevel_(lijn).qml
+-rw-rw-rw-   0        0        0    28513 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_bob.qml
+-rw-rw-rw-   0        0        0    30808 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_doorstroomafmeting.qml
+-rw-rw-rw-   0        0        0    16231 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_syphon_hevel.qml
+-rw-rw-rw-   0        0        0    60798 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_niet_in_model.qml
+-rw-rw-rw-   0        0        0    60802 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_wel_in_model.qml
+-rw-rw-rw-   0        0        0    25449 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_lijn.qml
+-rw-rw-rw-   0        0        0    27914 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_punt.qml
+-rw-rw-rw-   0        0        0     6882 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/friction.qml
+-rw-rw-rw-   0        0        0     5559 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/geisoleerde_watergangen.qml
+-rw-rw-rw-   0        0        0    44016 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_niet_in_model.qml
+-rw-rw-rw-   0        0        0    13458 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_peilafwijking.qml
+-rw-rw-rw-   0        0        0    44020 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_wel_in_model.qml
+-rw-rw-rw-   0        0        0    21867 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemeten_niet_in_model.qml
+-rw-rw-rw-   0        0        0    19432 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gestuurde_kunstwerken.qml
+-rw-rw-rw-   0        0        0    12551 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_kunstwerken.qml
+-rw-rw-rw-   0        0        0    12053 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_watergang_segmenten.qml
+-rw-rw-rw-   0        0        0    38443 2023-11-01 10:20:52.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_duikers_op_peilgrens.qml
+-rw-rw-rw-   0        0        0    23645 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_gemalen_op_peilgrens.qml
+-rw-rw-rw-   0        0        0     8444 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_levee_overstromingsmodel.qml
+-rw-rw-rw-   0        0        0    29529 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_stuwen_op_peilgrens.qml
+-rw-rw-rw-   0        0        0    89775 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hydro_deelgebieden_(hdb).qml
+-rw-rw-rw-   0        0        0     6842 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/infiltration.qml
+-rw-rw-rw-   0        0        0     9964 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/kzk.qml
+-rw-rw-rw-   0        0        0    15707 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/levee_30_cm_boven_max_peil.qml
+-rw-rw-rw-   0        0        0     6540 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/luchtfoto_actueel_ortho_25cm_rgb.qml
+-rw-rw-rw-   0        0        0     8715 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_lines.qml
+-rw-rw-rw-   0        0        0     8500 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_points.qml
+-rw-rw-rw-   0        0        0    10673 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ernstig.qml
+-rw-rw-rw-   0        0        0    10675 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_naar_kijken.qml
+-rw-rw-rw-   0        0        0    10690 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ter_info.qml
+-rw-rw-rw-   0        0        0     1657 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/openstreetmap.qml
+-rw-rw-rw-   0        0        0     6927 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/opmerkingen.qml
+-rw-rw-rw-   0        0        0   145908 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo).qml
+-rw-rw-rw-   0        0        0    61961 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo_huidig).qml
+-rw-rw-rw-   0        0        0    43564 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebied_aanname_streefpeil.qml
+-rw-rw-rw-   0        0        0    37659 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebieden_(datacheck).qml
+-rw-rw-rw-   0        0        0    72597 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo).qml
+-rw-rw-rw-   0        0        0    34786 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo_huidig).qml
+-rw-rw-rw-   0        0        0    24754 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/polder_polygon.qml
+-rw-rw-rw-   0        0        0     6666 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ggg.qml
+-rw-rw-rw-   0        0        0     6666 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ghg.qml
+-rw-rw-rw-   0        0        0     6780 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_glg.qml
+-rw-rw-rw-   0        0        0    27502 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuw_aanname_breedte.qml
+-rw-rw-rw-   0        0        0    47966 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_niet_in_model.qml
+-rw-rw-rw-   0        0        0    47970 2023-11-01 10:20:53.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_wel_in_model.qml
+-rw-rw-rw-   0        0        0     6857 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions.qml
+-rw-rw-rw-   0        0        0    12238 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions_view.qml
+-rw-rw-rw-   0        0        0     5498 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral.qml
+-rw-rw-rw-   0        0        0    10994 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral_view.qml
+-rw-rw-rw-   0        0        0    11645 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_boundary_conditions.qml
+-rw-rw-rw-   0        0        0     9996 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_lateral.qml
+-rw-rw-rw-   0        0        0    11540 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_aggregation_settings.qml
+-rw-rw-rw-   0        0        0    17656 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_channel.qml
+-rw-rw-rw-   0        0        0    21232 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_connection_nodes.qml
+-rw-rw-rw-   0        0        0     7617 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_definition.qml
+-rw-rw-rw-   0        0        0    15527 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location.qml
+-rw-rw-rw-   0        0        0    23555 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location_view.qml
+-rw-rw-rw-   0        0        0    27193 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert.qml
+-rw-rw-rw-   0        0        0    47426 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert_view.qml
+-rw-rw-rw-   0        0        0     8046 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_dem_average_area.qml
+-rw-rw-rw-   0        0        0    53502 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_global_settings.qml
+-rw-rw-rw-   0        0        0    21490 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement.qml
+-rw-rw-rw-   0        0        0    27705 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement_area.qml
+-rw-rw-rw-   0        0        0    27896 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_groundwater.qml
+-rw-rw-rw-   0        0        0    31655 2023-11-01 10:20:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface.qml
+-rw-rw-rw-   0        0        0     6403 2023-11-01 10:20:55.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface_map.qml
+-rw-rw-rw-   0        0        0    12028 2023-11-01 10:20:55.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_interflow.qml
+-rw-rw-rw-   0        0        0    39633 2023-11-01 10:20:55.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_levee.qml
+-rw-rw-rw-   0        0        0    17417 2023-11-01 10:20:55.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole.qml
+-rw-rw-rw-   0        0        0    45493 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole_view.qml
+-rw-rw-rw-   0        0        0    26442 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_numerical_settings.qml
+-rw-rw-rw-   0        0        0    10463 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_obstacle.qml
+-rw-rw-rw-   0        0        0    18741 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice.qml
+-rw-rw-rw-   0        0        0    62499 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice_view.qml
+-rw-rw-rw-   0        0        0    23573 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe.qml
+-rw-rw-rw-   0        0        0    60552 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe_view.qml
+-rw-rw-rw-   0        0        0    16415 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation.qml
+-rw-rw-rw-   0        0        0    24185 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_point_view.qml
+-rw-rw-rw-   0        0        0    28752 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_view.qml
+-rw-rw-rw-   0        0        0     8555 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_simple_infiltration.qml
+-rw-rw-rw-   0        0        0    16667 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface.qml
+-rw-rw-rw-   0        0        0     7487 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_map.qml
+-rw-rw-rw-   0        0        0    10465 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_parameters.qml
+-rw-rw-rw-   0        0        0    18641 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir.qml
+-rw-rw-rw-   0        0        0    62454 2023-11-01 10:20:56.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir_view.qml
+-rw-rw-rw-   0        0        0    11236 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_windshielding.qml
+-rw-rw-rw-   0        0        0    28738 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_niet_in_model.qml
+-rw-rw-rw-   0        0        0    25998 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_wel_in_model.qml
+-rw-rw-rw-   0        0        0    11163 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_loose.qml
+-rw-rw-rw-   0        0        0    11043 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.qml
+-rw-rw-rw-   0        0        0     1202 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.sld
+-rw-rw-rw-   0        0        0    67455 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.qml
+-rw-rw-rw-   0        0        0    33473 2023-11-01 10:20:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.sld
+-rw-rw-rw-   0        0        0   100574 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.qml
+-rw-rw-rw-   0        0        0    51192 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.sld
+-rw-rw-rw-   0        0        0    11410 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.qml
+-rw-rw-rw-   0        0        0     1271 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.sld
+-rw-rw-rw-   0        0        0    14996 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.qml
+-rw-rw-rw-   0        0        0     3690 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.sld
+-rw-rw-rw-   0        0        0    22539 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.qml
+-rw-rw-rw-   0        0        0     3663 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.sld
+-rw-rw-rw-   0        0        0     1747 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.qml
+-rw-rw-rw-   0        0        0      705 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.sld
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.107968 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/
+-rw-rw-rw-   0        0        0    21226 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__default.qml
+-rw-rw-rw-   0        0        0    92565 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__detailed.qml
+-rw-rw-rw-   0        0        0     8911 2023-11-01 10:20:58.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/discharge.qml
+-rw-rw-rw-   0        0        0    29841 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_kunstwerken.qml
+-rw-rw-rw-   0        0        0    42981 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_watergangen.qml
+-rw-rw-rw-   0        0        0    12056 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_end_rain_min_1.qml
+-rw-rw-rw-   0        0        0    82279 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__default.qml
+-rw-rw-rw-   0        0        0    18046 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__original.qml
+-rw-rw-rw-   0        0        0    12051 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_sum_start_sum.qml
+-rw-rw-rw-   0        0        0    12053 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_start_rain_vs_start_sum.qml
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.139795 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/__init__.py
+-rw-rw-rw-   0        0        0    42269 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten.qpt
+-rw-rw-rw-   0        0        0    42681 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten2.qpt
+-rw-rw-rw-   0        0        0    42333 2023-11-01 10:20:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten_landscape.qpt
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.159275 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.283350 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/
+-rw-rw-rw-   0        0        0      163 2022-07-14 07:53:38.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      167 2022-07-06 13:21:07.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14142 2022-07-14 07:53:38.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc
+-rw-rw-rw-   0        0        0    15533 2023-11-21 12:37:18.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12108 2022-07-14 07:53:38.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc
+-rw-rw-rw-   0        0        0    12567 2024-04-30 10:17:48.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.435354 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.460117 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     1986 2023-01-23 09:53:44.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     5495 2023-04-11 15:21:12.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     1976 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb
+-rw-rw-rw-   0        0        0     4996 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb
+-rw-rw-rw-   0        0        0    23402 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb
+-rw-rw-rw-   0        0        0     6306 2023-12-19 13:51:26.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb
+-rw-rw-rw-   0        0        0     2106 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.534450 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/
+-rw-rw-rw-   0        0        0      179 2022-01-31 10:15:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      177 2022-06-29 11:24:40.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1323 2023-11-06 08:43:16.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/net.cpython-39.pyc
+-rw-rw-rw-   0        0        0      847 2023-06-21 10:23:54.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6121 2023-04-25 11:04:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6280 2024-04-29 14:29:23.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc
+-rw-rw-rw-   0        0        0      304 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/constants.py
+-rw-rw-rw-   0        0        0      462 2023-07-18 09:43:59.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/notebook_data.json
+-rw-rw-rw-   0        0        0      598 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/notebook_setup.py
+-rw-rw-rw-   0        0        0     7362 2024-04-29 13:31:19.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/run.py
+-rw-rw-rw-   0        0        0    20085 2023-11-21 12:35:25.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/queries.py
+-rw-rw-rw-   0        0        0    25166 2024-04-30 10:17:30.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/queries_general_checks.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.651641 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/__init__.py
+-rw-rw-rw-   0        0        0     1850 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/api_settings.py
+-rw-rw-rw-   0        0        0      256 2023-11-06 13:43:39.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/backups_table_names.py
+-rw-rw-rw-   0        0        0     1043 2023-11-06 13:43:45.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/bank_levels.py
+-rw-rw-rw-   0        0        0     1649 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/database_aliases.py
+-rw-rw-rw-   0        0        0     2601 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/database_variables.py
+-rw-rw-rw-   0        0        0      134 2023-05-06 10:58:04.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/datachecker_variables.py
+-rw-rw-rw-   0        0        0      162 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/default_variables.py
+-rw-rw-rw-   0        0        0      130 2023-05-06 07:30:57.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/definitions.py
+-rw-rw-rw-   0        0        0      618 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/model_state.py
+-rw-rw-rw-   0        0        0      928 2023-12-19 13:51:26.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/one_d_two_d.py
+-rw-rw-rw-   0        0        0      830 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/sqlite.py
+-rw-rw-rw-   0        0        0      254 2021-12-13 08:25:22.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/weirs.py
+-rw-rw-rw-   0        0        0     1777 2023-11-09 12:12:01.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.804780 hhnk_threedi_tools-2024.1/hhnk_threedi_tools.egg-info/
+-rw-rw-rw-   0        0        0      528 2024-05-03 11:05:23.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    22028 2024-05-03 11:05:23.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 11:05:23.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-03 11:05:23.000000 hhnk_threedi_tools-2024.1/hhnk_threedi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 11:05:26.831014 hhnk_threedi_tools-2024.1/setup.cfg
+-rw-rw-rw-   0        0        0     1659 2023-06-21 07:43:33.000000 hhnk_threedi_tools-2024.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.724743 hhnk_threedi_tools-2024.1/tests/
+drwxrwxrwx   0        0        0        0 2024-05-03 11:05:26.789781 hhnk_threedi_tools-2024.1/tests/notebooks/
+-rw-rw-rw-   0        0        0        0 2023-11-01 09:17:54.000000 hhnk_threedi_tools-2024.1/tests/notebooks/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-11-01 09:17:54.000000 hhnk_threedi_tools-2024.1/tests/notebooks/notebook_setup.py
+-rw-rw-rw-   0        0        0     3330 2023-11-01 09:17:54.000000 hhnk_threedi_tools-2024.1/tests/notebooks/rtest_lizardapi.py
+-rw-rw-rw-   0        0        0      569 2023-11-01 09:17:55.000000 hhnk_threedi_tools-2024.1/tests/notebooks/rtest_notebooks.py
+-rw-rw-rw-   0        0        0     1258 2023-11-01 10:21:00.000000 hhnk_threedi_tools-2024.1/tests/notebooks/rtest_upload_schema.py
+-rw-rw-rw-   0        0        0     4265 2024-04-29 15:35:27.000000 hhnk_threedi_tools-2024.1/tests/test_bank_level_check.py
+-rw-rw-rw-   0        0        0     2001 2023-11-21 12:35:25.000000 hhnk_threedi_tools-2024.1/tests/test_calculation_gui.py
+-rw-rw-rw-   0        0        0     1672 2023-11-22 11:49:44.000000 hhnk_threedi_tools-2024.1/tests/test_create_schematisation_rasters.py
+-rw-rw-rw-   0        0        0     2913 2023-11-21 12:35:25.000000 hhnk_threedi_tools-2024.1/tests/test_folder_structures.py
+-rw-rw-rw-   0        0        0     2177 2024-04-29 07:35:33.000000 hhnk_threedi_tools-2024.1/tests/test_klimaatsommen_prep.py
+-rw-rw-rw-   0        0        0     1840 2023-11-21 12:35:26.000000 hhnk_threedi_tools-2024.1/tests/test_layer_structure.py
+-rw-rw-rw-   0        0        0     2138 2024-04-30 07:33:49.000000 hhnk_threedi_tools-2024.1/tests/test_modelsplitter.py
+-rw-rw-rw-   0        0        0     1669 2024-03-20 13:17:39.000000 hhnk_threedi_tools-2024.1/tests/test_netcdf_to_gridgpkg.py
+-rw-rw-rw-   0        0        0     1737 2024-03-20 13:17:39.000000 hhnk_threedi_tools-2024.1/tests/test_one_d_two_d.py
+-rw-rw-rw-   0        0        0     1870 2023-12-19 13:51:27.000000 hhnk_threedi_tools-2024.1/tests/test_result_rasters.py
+-rw-rw-rw-   0        0        0     1182 2023-11-21 12:35:26.000000 hhnk_threedi_tools-2024.1/tests/test_schema_migration.py
+-rw-rw-rw-   0        0        0     5062 2023-12-19 13:51:27.000000 hhnk_threedi_tools-2024.1/tests/test_sqlite.py
+-rw-rw-rw-   0        0        0     1070 2023-11-21 12:35:26.000000 hhnk_threedi_tools-2024.1/tests/test_zero_d_one_d.py
```

### Comparing `hhnk-threedi-tools-2023.4/PKG-INFO` & `hhnk_threedi_tools-2024.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 Metadata-Version: 2.1
 Name: hhnk-threedi-tools
-Version: 2023.4
+Version: 2024.1
 Summary: HHNK watersystemen analysis tools
 Home-page: https://github.com/threedi/hhnk-threedi-tools
 Author: Wietse van Gerwen, Laure Ravier
 Author-email: w.vangerwen@hhnk.nl
 Maintainer: Wietse van Gerwen
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/threedi/hhnk-threedi-tools/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-
-UNKNOWN
-
```

### Comparing `hhnk-threedi-tools-2023.4/README.md` & `hhnk_threedi_tools-2024.1/README.md`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/__init__.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from osgeo import gdal
 
 import hhnk_threedi_tools.core
 import hhnk_threedi_tools.qgis
 import hhnk_threedi_tools.resources
 
 # checks
-from hhnk_threedi_tools.core.checks.bank_levels import (
-    BankLevelTest,
-)
+from hhnk_threedi_tools.core.checks.bank_levels import BankLevelTest
 
 # FIXME TypeError: metaclass conflict: the metaclass of a derived class must be a (non-strict) subclass of the metaclasses of all its bases
 from hhnk_threedi_tools.core.checks.one_d_two_d import OneDTwoDTest
 from hhnk_threedi_tools.core.checks.sqlite.sqlite_main import SqliteCheck  # FIXME
 from hhnk_threedi_tools.core.checks.zero_d_one_d import ZeroDOneDTest
 from hhnk_threedi_tools.core.folders import Folders
+from hhnk_threedi_tools.core.folders_modelbuilder import FoldersModelbuilder
+from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import NetcdfToGPKG
 from hhnk_threedi_tools.core.schematisation import (
     migrate,
     model_backup,
     model_splitter,
     upload,
 )
 from hhnk_threedi_tools.core.schematisation.migrate import MigrateSchema
@@ -46,8 +46,8 @@
     add_notebook_paths,
     copy_notebooks,
     open_server,
     read_notebook_json,
     write_notebook_json,
 )
 
-__version__ = "2023.4"
+__version__ = "2024.1"
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/calculation.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -730,16 +730,15 @@
             with open(filepath, "rb") as file:
                 response = requests.put(upload_result.put_url, data=file)
                 return response
 
         filename = f"boundaryconditions_{self.model_id}.json"
 
         output_path = Path(self.output_folder).joinpath("tempfiles", filename)
-        output_path.parent.parent.mkdir(exist_ok=True)
-        output_path.parent.mkdir(exist_ok=True)  # Create parent folder
+        output_path.parent.mkdir(parents=True, exist_ok=True)  # Create parent folder
 
         if not output_path.exists():
             save_json(output_path, self.data.boundaries)
 
         if self.data.boundaries == []:
             print("Info: Boundary file is empty, file not uploaded")
             return "Info: Boundary file is empty, file not uploaded"
@@ -870,16 +869,16 @@
         if output_folder_sqlite is None:
             return "define self.output_folder first"
 
         if self.model is None:
             return "define self.model_id first"
 
         output_path = Path(output_folder_sqlite).joinpath("tempfiles", f"model_{self.model_id}.zip")
-        output_path.parent.parent.mkdir(exist_ok=True)
-        output_path.parent.mkdir(exist_ok=True)  # Create parent folder
+        output_path.parent.mkdir(parents=True, exist_ok=True)  # Create parent folder
+
         if not output_path.with_suffix("").exists():
             if not output_path.exists():
                 sqlite_dnwld = self._add_to_simulation(
                     self.threedi_api.schematisations_revisions_sqlite_download,
                     id=int(self.revision_id),
                     schematisation_pk=int(self.schema_id),
                 )
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/calculation_gui_class.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/calculation_gui_class.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/download_functions.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/download_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/api/download_gui_class.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/api/download_gui_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,25 +598,34 @@
                 # Create destination folder
                 if not os.path.exists(output_folder) and output_folder != "":
                     os.mkdir(output_folder)
                 #             print('Created folder: ' + output_folder.rsplit('/')[-1])
 
                 # add some variables to overview
                 for index, key in enumerate(download_urls):
-                    self.vars.output_df = self.vars.output_df.append(
-                        {
-                            "id": scenario_id,
-                            "name": scenario_name,
-                            "uuid": scenario.uuid,
-                            "scenario_download_url": download_urls[key],
-                            "output_folder": output_folder,
-                        },
+                    self.vars.output_df = pd.concat(
+                        [
+                            self.vars.output_df,
+                            pd.DataFrame(
+                                pd.Series(
+                                    {
+                                        "id": scenario_id,
+                                        "name": scenario_name,
+                                        "uuid": scenario.uuid,
+                                        "scenario_download_url": download_urls[key],
+                                        "output_folder": output_folder,
+                                    }
+                                )
+                            ).T,
+                        ],
                         ignore_index=True,
                     )
 
+                    # %%
+
                 # Download files
                 if self.vars.scenario_result_type == "lizard":
                     download_functions.start_download(
                         download_urls.values(),
                         output_folder,
                         api_key=dl.get_api_key(),
                         automatic_download=1,
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/bank_levels.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/bank_levels.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Created on Thu Aug 19 09:04:52 2021
 
 @author: chris.kerklaan
 
 Bank level testing made into an object to have more overview
 
 """
+
 import geopandas as gpd
 import hhnk_research_tools as hrt
 import numpy as np
 import pandas as pd
 from hhnk_research_tools.threedi.geometry_functions import extract_boundary_from_polygon
 from hhnk_research_tools.threedi.grid import Grid
 
@@ -297,39 +298,47 @@
 
 
 def get_manhole_information(
     intersections: gpd.GeoDataFrame,
     diverging_wl_nodes: gpd.GeoDataFrame,
     manholes: gpd.GeoDataFrame,
 ):
-    """Uses the manhole table from the sqlite and the 1d2d flowlines that originate from a connection node.
+    """Use the manhole table from the sqlite and the 1d2d flowlines that originate from a connection node.
     If the connection node is not already a manhole, they are added to the list. This function generates the
     dataframe from which the sql code can be made"""
     try:
         node_ids_without_manholes = conn_nodes_without_manholes(intersections, manholes)
         # Combine the three lists: manholes, connection nodes with 1d2d flowline and connection nodes in wrong area
         # Manholes from model
         all_manholes = manholes.copy()
         all_manholes[already_manhole_col] = True
         # default manhole type, if manhole is added through other procedure,
         # this script doesnt know why it was added
-        all_manholes[type_col] = unknown_val
+        all_manholes["type"] = "unknown"
 
         # Update current manholes with the type of manhole from intersections.
         all_manholes.set_index(a_man_conn_id, drop=False, inplace=True)
-        all_manholes.update(intersections.set_index(node_id_col)[type_col])
-        # Add new manholes that are not yet in sqlite (rename is needed because of difference in column names)
-        all_manholes = all_manholes.append(node_ids_without_manholes.rename(columns={node_id_col: a_man_conn_id}))
+
+        # FIXME added calc nodes do not have a connection node id. We filter them here to get rid of
+        # ValueError: cannot reindex on an axis with duplicate labels. Take this into account on refactor.
+        intersections2 = intersections[intersections["node_type"] != "added_calculation"].copy()
+        all_manholes.update(intersections2.set_index(node_id_col)["type"])
+
+        # # Add new manholes that are not yet in sqlite (rename is needed because of difference in column names)
+        all_manholes = pd.concat(
+            [all_manholes, node_ids_without_manholes.rename(columns={node_id_col: a_man_conn_id})]
+        )
+
         # check if nodes in wrong area (different initial waterlevel than rest in area) don't have manhole yet
         nodes_with_divergent_initial_wtrlvl_no_manhole = diverging_wl_nodes[
             ~diverging_wl_nodes[a_conn_node_id].isin(all_manholes[a_man_conn_id])
         ].copy()
         nodes_with_divergent_initial_wtrlvl_no_manhole[already_manhole_col] = False
         # also add these to the list
-        all_manholes = all_manholes.append(nodes_with_divergent_initial_wtrlvl_no_manhole, ignore_index=True)
+        all_manholes = pd.concat([all_manholes, nodes_with_divergent_initial_wtrlvl_no_manhole], ignore_index=True)
         # Drop duplicates that are introduced by nodes_with_divergent_initial_wtrlvl_no_manhole
         all_manholes = (
             all_manholes.sort_values(drain_level_col, ascending=False).drop_duplicates(a_conn_node_id).sort_index()
         )
         all_manholes.reset_index(drop=True, inplace=True)
         all_manholes.crs = f"EPSG:{DEF_TRGT_CRS}"
         # all_manholes_gdf = gpd.GeoDataFrame(all_manholes, crs=f"EPSG:{DEF_TRGT_CRS}")
@@ -470,16 +479,19 @@
             nodes_in_same_area = nodes_with_fixeddrainage_id[nodes_with_fixeddrainage_id[peil_id_col] == p_id]
 
             # Find the most occuring value of initial waterlevel, this is considered the initial
             # waterlevel in the area specified by p_id
             init_waterlevel_mode = nodes_in_same_area[initial_waterlevel_col].mode().values[0]
 
             # Find which nodes have a different waterlevel than the initial waterlevel
-            diverging_nodes = diverging_nodes.append(
-                nodes_in_same_area[nodes_in_same_area[initial_waterlevel_col] != init_waterlevel_mode],
+            diverging_nodes = pd.concat(
+                [
+                    diverging_nodes,
+                    nodes_in_same_area[nodes_in_same_area[initial_waterlevel_col] != init_waterlevel_mode],
+                ],
                 ignore_index=True,
             )
 
         # Clean up dataframe and add columns so it can be used in the sql creation for manholes on these nodes.
         diverging_nodes = diverging_nodes[[a_conn_node_id, initial_waterlevel_col, storage_area_col, df_geo_col]]
         diverging_nodes[drain_level_col] = np.nan
         diverging_nodes[code_col] = diverging_nodes[a_conn_node_id].apply(lambda x: f"{a_conn_node_id}_" + str(x))
@@ -604,17 +616,15 @@
         cross_loc_new_all.loc[cross_loc_levee.index, "new_bank_level"] = cross_loc_levee["levee_height"].astype(float)
         cross_loc_new_all.loc[cross_loc_levee.index, "bank_level_source"] = "levee_height"
 
         # Cross locations that are associated with peilgrenzen get a special label for recognition (values are already set)
         cross_loc_new_all.loc[
             (cross_loc_new_all.index.isin(cross_loc_fixeddrainage.index)),
             "bank_level_source",
-        ] = (
-            cross_loc_new_all["bank_level_source"] + "_fixeddrainage"
-        )
+        ] = cross_loc_new_all["bank_level_source"] + "_fixeddrainage"
 
         # Calculate difference between new and old bank level
         cross_loc_new_all["bank_level_diff"] = np.round(
             cross_loc_new_all["new_bank_level"] - cross_loc_new_all["bank_level"], 2
         )
 
         # reorder columns
@@ -661,15 +671,15 @@
     return all_channels
 
 
 # %%
 if __name__ == "__main__":
     from pathlib import Path
 
-    TEST_MODEL = Path(__file__).parent.parent.parent.parent / "tests/data/model_test/"
+    TEST_MODEL = Path(__file__).parent.parent.parent.parent.full_path(r"tests/data/model_test/")
     if not TEST_MODEL.exists():
         raise Exception(f"{TEST_MODEL} doesnt exist")
 
     self = BankLevelTest(Folders(TEST_MODEL))
     self.import_data()
     self.run()
     # self.manhole_information()
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/grid_result_metadata.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/grid_result_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # %%
 import numpy as np
 import pandas as pd
 from threedigrid.admin.gridresultadmin import GridH5ResultAdmin
 
 
 def calculate_rain_days(rain):
-    """
-    Calculates days dry before and after rain
-    """
+    """Calculate days dry before and after rain"""
     detected_rain = [i for i, e in enumerate(rain) if e > 1e-5]
     # Collect indexes of items in rain where rain falls (every index represents an hour)
     if detected_rain:
         # Detected rain[0] is the first index where rain occurs, so the last dry
         # item is one before that. Dividing by 24 converts to days
         dry_days_start = max(0, (detected_rain[0] - 1) / 24)
         # Detected rain[-1] is the first index where rain occurs, so the last dry
@@ -19,17 +17,15 @@
         dry_days_end = max(0, (len(rain) - detected_rain[-1] - 1) / 24)
         return detected_rain, dry_days_start, dry_days_end
     else:
         raise Exception(f"Geen regen gedetecteerd in 3di scenario")
 
 
 def get_rain_properties(results):
-    """
-    Calculates the rain scenario used for this result
-    """
+    """Calculate the rain scenario used for this result"""
     try:
         # Calculates the mean of steps between timestamps (in seconds), then converts to minutes
         dt = round(np.mean(np.diff(results.nodes.timestamps)) / 60, 0)
         # Timestep is list of time passed between timestamp and start in minutes
         timestep = results.nodes.timestamps / 60
         # Calculates rain per node between 0 and end of scenario at every step of size dt / 60 (so every hour)
         rain_1d_list = (
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/model_state.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/model_state.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # %%
 # -*- coding: utf-8 -*-
 """
 Created on Tue Aug 24 14:11:45 2021
 
 @author: chris.kerklaan
 """
+
 # Third-party imports
 from pathlib import Path
 
 import fiona
 import geopandas as gpd
 
 # research-tools
@@ -173,15 +174,15 @@
                             exist = False
         return exist
 
     def run_controlled_structures(self, overwrite=False):
         """Create leayer with structure control in schematisation"""
         self.structure_control = StructureControl(
             model=self.fenv.model.schema_base.database,
-            hdb_control_layer=self.fenv.source_data.hdb.layers.sturing_3di,
+            hdb_control_layer=self.fenv.source_data.hdb.layers.sturing_kunstwerken,
             output_file=self.output_fd.gestuurde_kunstwerken.base,
         )
         self.structure_control.run(overwrite=overwrite)
 
     def run_dem_max_value(self):
         stats = self.dem.statistics(approve_ok=False, force=True)
         if stats["max"] > DEM_MAX_VALUE:
@@ -393,16 +394,16 @@
             model=self.model,
             channel_profile_file=self.channels_from_profiles,
             fixeddrainage_layer=self.fenv.source_data.datachecker.layers.fixeddrainagelevelarea,
             damo_layer=self.fenv.source_data.damo.layers.waterdeel,
         )
         fixeddrainage = calc_area(fixeddrainage, modelbuilder_waterdeel, damo_waterdeel, conn_nodes_geo)
         result_txt = """Gebied open water BGT: {} ha\nGebied open water model: {} ha""".format(
-            round(fixeddrainage.sum()[watersurface_waterdeel_area] / 10000, 2),
-            round(fixeddrainage.sum()[watersurface_model_area] / 10000, 2),
+            round(fixeddrainage[watersurface_waterdeel_area].sum() / 10000, 2),
+            round(fixeddrainage[watersurface_model_area].sum() / 10000, 2),
         )
         self.results["watersurface_area"] = {
             "fixeddrainage": fixeddrainage,
             "result_txt": result_txt,
         }
         return fixeddrainage, result_txt
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/sqlite/structure_control.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/sqlite/structure_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     basis van de v2_control_table. Per kunstwerk worden actiewaarden opgevraagd. Per gevonden gestuurd kunstwerk
     wordt ook relevante informatie uit de HDB database toegevoegd, zoals het streefpeil en minimale en maximale kruin
     hoogtes.
     """
 
     def __init__(self, model: hrt.Sqlite, hdb_control_layer: hrt.FileGDBLayer, output_file: str):
         self.model = model  # folder.model.schema_base.database
-        self.hdb_control_layer = hdb_control_layer  # folder.source_data.hdb.layers.sturing_3di
+        self.hdb_control_layer = hdb_control_layer  # folder.source_data.hdb.layers.sturing_kunstwerken
         self.output_file = Path(output_file)  # folder.output.sqlite_tests.gestuurde_kunstwerken.base
 
         self.layers = self.Layers()
 
     class Layers:
         def __init__(self):
             # Raw results
@@ -178,11 +178,11 @@
         TEST_MODEL = Path(__file__).parents[i].absolute() / "tests/data/model_test/"
         folder = Folders(TEST_MODEL)
         if folder.exists():
             break
 
     self = StructureControl(
         model=folder.model.schema_base.database,
-        hdb_control_layer=folder.source_data.hdb.layers.sturing_3di,
+        hdb_control_layer=folder.source_data.hdb.layers.sturing_kunstwerken,
         output_file=folder.output.sqlite_tests.gestuurde_kunstwerken.path,
     )
     self.run(overwrite=True)
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/checks/zero_d_one_d.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/zero_d_one_d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Aug 20 16:09:34 2021
 
 @author: chris.kerklaan
 """
+
 # Third-party imports
 import hhnk_research_tools as hrt
 import pandas as pd
 from hhnk_research_tools.threedi.geometry_functions import coordinates_to_points
 from hhnk_research_tools.variables import (
     DEF_TRGT_CRS,
     all_1d,
@@ -151,17 +152,21 @@
                 threedi_result=self.grid_result,
                 structure_name=res_channels,
                 wtrlvl_nodes_at_timesteps=wtrlvl_nodes_at_timesteps,
                 t_end=T_end,
             )
 
             # Find all connection nodes from channels that are primary and combine in list without duplicates
-            primary_nodes_series = channels_gdf.loc[channels_gdf.zoom_cat == 4, start_node_col].append(
-                channels_gdf.loc[channels_gdf.zoom_cat == 4, end_node_col]
+            primary_nodes_series = pd.concat(
+                [
+                    channels_gdf.loc[channels_gdf.zoom_cat == 4, start_node_col],
+                    channels_gdf.loc[channels_gdf.zoom_cat == 4, end_node_col],
+                ]
             )
+
             primary_nodes = primary_nodes_series.unique().tolist()
 
             culvert_gdf = create_structure_gdf(
                 threedi_result=self.grid_result,
                 structure_name=res_culverts,
                 wtrlvl_nodes_at_timesteps=wtrlvl_nodes_at_timesteps,
                 t_end=T_end,
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_main.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_main.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,64 +3,66 @@
 
 import geopandas as gpd
 import hhnk_research_tools as hrt
 import pandas as pd
 
 from hhnk_threedi_tools import Folders
 from hhnk_threedi_tools.core.result_rasters.calculate_raster import BaseCalculatorGPKG
-from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import ThreediGrid
+from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import NetcdfToGPKG
 
 
 class KlimaatsommenPrep:
     """Postprocessing of climate scenarios. This object will turn the
     raw netcdf results into depth and damage rasters for each scenario.
     """
 
     def __init__(
         self,
         folder: Folders,
         batch_name: str,
         cfg_file="cfg_lizard.cfg",
         landuse_file: str = r"\\corp.hhnk.nl\data\Hydrologen_data\Data\01.basisgegevens\rasters\landgebruik\landuse2019_tiles\combined_rasters.vrt",
+        min_block_size=1024,
         verify=True,
     ):
-        if type(cfg_file) == str:
+        if isinstance(cfg_file, str):
             cfg_file = hrt.get_pkg_resource_path(package_resource=hrt.waterschadeschatter.resources, name=cfg_file)
             if not cfg_file.exists():
-                raise Exception(f"{cfg_file} doesnt exist.")
+                raise FileNotFoundError(f"{cfg_file} doesnt exist.")
 
         self.folder = folder
         self.batch_fd = self.folder.threedi_results.batch[batch_name]
 
         self.cfg_file = cfg_file
         self.landuse_file = landuse_file
+        self.min_block_size = min_block_size
 
         if verify:
             self.verify_input()
 
     def verify_input(self):
         """Verify if we can run"""
         if not self.batch_fd.exists():
-            raise Exception(f"INPUTERROR - {self.batch_fd.name} missing")
+            raise FileNotFoundError(f"INPUTERROR - batchfolder {self.batch_fd.name} missing")
 
         netcdf_missing = [
             name
             for name in self.batch_fd.downloads.names
             if not getattr(self.batch_fd.downloads, name).netcdf.grid_path.exists()
         ]
         if any(netcdf_missing):
-            raise Exception(f"INPUTERROR - netcdf missing for scenarios; {netcdf_missing}")
+            raise FileNotFoundError(f"INPUTERROR - netcdf missing for scenarios; {netcdf_missing}")
 
         h5_missing = [
             name
             for name in self.batch_fd.downloads.names
             if not getattr(self.batch_fd.downloads, name).netcdf.admin_path.exists()
         ]
         if any(h5_missing):
-            raise Exception(f"INPUTERROR - h5 missing for scenarios; {h5_missing}")
+            raise FileNotFoundError(f"INPUTERROR - h5 missing for scenarios; {h5_missing}")
         return True
 
     def get_dem(self):
         """Update dem resolution to 0.5m
         #Get the dem. If dem doesnt have correct resolution it will be reprojected to 0.5m
         """
         dem = self.folder.model.schema_base.rasters.dem
@@ -73,67 +75,71 @@
             dem = hrt.Raster(new_dem_path)
             return dem
         else:
             return dem
 
     def get_scenario(self, name):
         """Get individual threediresult of a scenario.
-        (e.g. netcdf folder of blok_gxg_T10)"""
+        (e.g. netcdf folder of blok_gxg_T10)
+        """
         scenario = getattr((self.batch_fd.downloads), name)
         return scenario
 
     def netcdf_to_grid(
         self,
         threedi_result,
-        corrected_col_name="wlvl_max_replaced",
-        grid_raw_filename="grid_raw.gpkg",
-        grid_corr_filename="grid_corr.gpkg",
+        grid_filename="grid_wlvl.gpkg",
         overwrite=False,
     ):
-        """Transform netcdf to grid gpkg and apply wlvl correction"""
+        """Transform netcdf to grid gpkg and apply wlvl correction
+        output will be stored in wlvl_corr_max column
+        """
         # Select result
-        threedigrid = ThreediGrid(
+        netcdf_gpkg = NetcdfToGPKG.from_folder(
             folder=self.folder,
             threedi_result=threedi_result,
-            grid_raw_filename=grid_raw_filename,
-            grid_corr_filename=grid_corr_filename,
         )
 
         # Convert netcdf to grid gpkg
-        threedigrid.netcdf_to_grid_gpkg(overwrite=overwrite)
-
-        # Replace waterlevel of selected cells with avg of neighbours.
-        threedigrid.waterlevel_correction(output_col=corrected_col_name, overwrite=overwrite)
+        netcdf_gpkg.run(
+            output_file=threedi_result.full_path(grid_filename),
+            timesteps_seconds=["max"],
+            overwrite=overwrite,
+        )
 
     def calculate_raster(
         self,
         scenario_raster,
-        threedi_result,
-        mode,
-        grid_filename="grid_corr.gpkg",
-        wlvl_col_name="wlvl_max_replaced",
+        threedi_result: hrt.ThreediResult,
+        mode: str,
+        grid_filename: str = "grid_wlvl.gpkg",
+        wlvl_col_name: str = "wlvl_corr_max",
         overwrite=False,
     ):
-        """mode options are: "MODE_WDEPTH", "MODE_WLVL" """
+        """Mode options are: 'MODE_WDEPTH', 'MODE_WLVL'"""
         grid_gdf = threedi_result.full_path(grid_filename).load()
 
-        calculator_kwargs = {"dem_path": self.dem.base, "grid_gdf": grid_gdf, "wlvl_column": wlvl_col_name}
+        calculator_kwargs = {
+            "dem_path": self.dem.base,
+            "grid_gdf": grid_gdf,
+            "wlvl_column": wlvl_col_name,
+        }
 
         output_file = scenario_raster
 
         # Init calculator
         with BaseCalculatorGPKG(**calculator_kwargs) as basecalc:
-            basecalc.run(output_file=output_file, mode=mode, overwrite=overwrite)
+            basecalc.run(output_file=output_file, mode=mode, min_block_size=self.min_block_size, overwrite=overwrite)
 
     def calculate_depth(
         self,
         scenario,
         threedi_result: hrt.ThreediResult,
-        grid_filename="grid_corr.gpkg",
-        wlvl_col_name="wlvl_max_replaced",
+        grid_filename: str,
+        wlvl_col_name="wlvl_corr_max",
         overwrite=False,
     ):
         scenario_raster = scenario.depth_max
         self.calculate_raster(
             scenario_raster=scenario_raster,
             threedi_result=threedi_result,
             mode="MODE_WDEPTH",
@@ -142,16 +148,16 @@
             overwrite=overwrite,
         )
 
     def calculate_wlvl(
         self,
         scenario,
         threedi_result: hrt.ThreediResult,
-        grid_filename="grid_corr.gpkg",
-        wlvl_col_name="wlvl_max_replaced",
+        grid_filename: str,
+        wlvl_col_name="wlvl_corr_max",
         overwrite=False,
     ):
         scenario_raster = scenario.wlvl_max
         self.calculate_raster(
             scenario_raster=scenario_raster,
             threedi_result=threedi_result,
             mode="MODE_WLVL",
@@ -173,15 +179,20 @@
             "dmg_type": "gem",
         }
 
         if output_raster.exists() and not overwrite:
             return
 
         # Calculation
-        wss = hrt.Waterschadeschatter(depth_file=depth_file, landuse_file=self.landuse_file, wss_settings=wss_settings)
+        wss = hrt.Waterschadeschatter(
+            depth_file=depth_file,
+            landuse_file=self.landuse_file,
+            wss_settings=wss_settings,
+            min_block_size=self.min_block_size,
+        )
 
         # Berekenen schaderaster
         wss.run(output_raster=output_raster, calculation_type="sum", overwrite=overwrite)
 
     def run(self, gridgpkg=True, depth=True, dmg=True, wlvl=False, overwrite=False, testing=False):
         try:
             self.dem = self.get_dem()
@@ -190,35 +201,39 @@
                 scenario = self.get_scenario(name=name)
                 threedi_result = scenario.netcdf
 
                 # Transform netcdf to grid gpkg
                 if gridgpkg:
                     self.netcdf_to_grid(
                         threedi_result=threedi_result,
-                        grid_raw_filename="grid_raw.gpkg",
-                        grid_corr_filename="grid_corr.gpkg",
+                        grid_filename="grid_wlvl.gpkg",
                         overwrite=overwrite,
                     )
 
                 # Diepterasters berekenen
                 if depth:
                     self.calculate_depth(
                         scenario=scenario,
                         threedi_result=threedi_result,
-                        grid_filename="grid_corr.gpkg",
+                        grid_filename="grid_wlvl.gpkg",
                         overwrite=overwrite,
                     )
 
                 # Schaderaster berekenen
                 if dmg:
                     self.calculate_damage(scenario=scenario, overwrite=overwrite)
 
                 # Waterlevelraster berekenen
                 if wlvl:
-                    self.calculate_wlvl(scenario=scenario, threedi_result=threedi_result, overwrite=overwrite)
+                    self.calculate_wlvl(
+                        scenario=scenario,
+                        threedi_result=threedi_result,
+                        grid_filename="grid_wlvl.gpkg",
+                        overwrite=overwrite,
+                    )
 
                 if testing:
                     # For pytests we dont need to run this 18 times
                     break
 
             self.create_scenario_metadata(overwrite=overwrite, testing=testing)
         except Exception as e:
@@ -231,30 +246,29 @@
         # Also bounds should be same.
 
         self.info_file = {}
 
         for raster_type in ["depth_max", "damage_total"]:
             self.info_file[raster_type] = self.batch_fd.full_path(f"{raster_type}_info.csv")
 
-            info_df = gpd.GeoDataFrame()
+            data = []
 
             # Get statistics for all 18 scenarios
             for name in self.batch_fd.downloads.names:
                 scenario = self.get_scenario(name=name)
 
-                info_row = self._scenario_metadata_row(scenario=scenario, raster_type=raster_type)
+                data += [self._scenario_metadata_row(scenario=scenario, raster_type=raster_type)]
                 # Add row to df
-                info_df = info_df.append(info_row, ignore_index=True)
 
                 if testing:
                     # For pytests we dont need to run this 18 times
                     break
 
             # Write to file
-
+            info_df = gpd.GeoDataFrame(data)
             info_df.set_index(["filename"], inplace=True)
             info_df.to_csv(self.info_file[raster_type].path, sep=";")
 
     def _scenario_metadata_row(self, scenario, raster_type) -> pd.Series:
         """Raster statistics for single scenario"""
         raster = getattr(scenario, raster_type)
 
@@ -276,15 +290,14 @@
 
 # %%
 if __name__ == "__main__":
     from pathlib import Path
 
     from hhnk_threedi_tools import Folders
 
-    # TEST_MODEL = Path(__file__).parent.parent.parent.parent / "tests/data/model_test/"
     TEST_MODEL = r"E:\02.modellen\model_test_v2"
     folder = Folders(TEST_MODEL)
 
     self = KlimaatsommenPrep(
         folder=folder,
         batch_name="batch_test2",
         cfg_file="cfg_lizard.cfg",
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/folder_helpers.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/folder_helpers.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/folders.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/folders.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,32 +81,32 @@
             folder = Folders('C:/Poldermodellen/Heiloo')
             
             folder.show
            
             Output: 
                 Heiloo @ C:/Poldermodellen/Heiloo
                                 Folders:	  
-                           				Folders
-                           				├── 01_source_data
-                           				├── 02_schematisation
-                           				├── 03_3di_results
-                           				└── 04_test_results
+                                    Folders
+                                    ├── 01_source_data
+                                    ├── 02_schematisation
+                                    ├── 03_3di_results
+                                    └── 04_test_results
                            
                                 Files:	[]
                                 Layers:	[]
         
             
             folder.source_data.show
             
             Output: 
             
                 01_Source_data @ C:/Poldermodellen/Heiloo/01_Source_data
                                     Folders:	  
-                               				source_data
-                               				└── modelbuilder
+                                        source_data
+                                        └── modelbuilder
                                
                                     Files:	['damo', 'hdb', 'datachecker', ...]
             
             
         {FOLDER_STRUCTURE}
 
         """
@@ -138,15 +138,15 @@
 
     @property
     def full_structure(self):
         return print(FOLDER_STRUCTURE)
 
     def to_file_dict(self):
         """
-        Returns dictionary containing paths to source files according to set project structure.
+        Return dictionary containing paths to source files according to set project structure.
 
             build_base_paths_dict(
                     polder_path (string: path to project folder (highest level))
                 )
         """
         return {
             "datachecker": self.source_data.datachecker.path_if_exists,
@@ -174,17 +174,15 @@
     def is_valid(self, folderpath):
         """Check if folder stucture is available in input folder."""
         SUB_FOLDERS = ["01_source_data", "02_schematisation", "03_3di_results", "04_test_results"]
         return all([Path(folderpath).joinpath(i).exists() for i in SUB_FOLDERS])
 
 
 class SourceDir(Folder):
-    """
-    Paths to source data (datachecker, DAMO, HDB)
-    """
+    """Path to source data (datachecker, DAMO, HDB)"""
 
     def __init__(self, base, create):
         super().__init__(os.path.join(base, "01_source_data"), create)
 
         # Folders
         self.modelbuilder = self.ModelbuilderPaths(self.base, create=create)
         self.peilgebieden = self.PeilgebiedenPaths(self.base, create=create)
@@ -194,15 +192,15 @@
             self.create_readme()
 
         # Files
         self.add_file("damo", "DAMO.gpkg")
         self.damo.add_layers(["DuikerSifonHevel", "waterdeel"])
 
         self.add_file("hdb", "HDB.gpkg")
-        self.hdb.add_layer("sturing_3di")
+        self.hdb.add_layer("sturing_kunstwerken")
 
         self.add_file("datachecker", "datachecker_output.gpkg")
         self.datachecker.add_layers(["fixeddrainagelevelarea", "culvert"])
 
         self.add_file("polder_polygon", POLDER_POLY)
         self.add_file("panden", "panden.gpkg")
 
@@ -252,15 +250,16 @@
                     self.add_file("peilgebieden", "peilgebieden.shp")
             self.add_file("geen_schade", "geen_schade.shp")
 
 
 class SchemaDirParent(Folder):
     """Parent folder with all model (schematisations) in it. These
     all share the same base schematisation, with only differences in
-    global settings or other things specific for that model"""
+    global settings or other things specific for that model
+    """
 
     def __init__(self, base, create):
         super().__init__(os.path.join(base, "02_schematisation"), create)
 
         self.revisions = self.ModelRevisionsParent(base=self.base, create=create)
         self.schema_base = hrt.ThreediSchematisation(base=self.base, name="00_basis", create=create)
         self.schema_list = ["schema_base"]
@@ -287,15 +286,15 @@
             if not self.settings_loaded:  # only read once. #FIXME test this, might cause issues.
                 self.settings_df = pd.read_excel(self.settings.base, engine="openpyxl")
                 self.settings_df = self.settings_df[self.settings_df["name"].notna()]
                 self.settings_df.set_index("name", drop=False, inplace=True)
                 self.settings_loaded = True
 
                 for item_name, row in self.settings_df.iterrows():
-                    if not pd.isnull(row["name"]):
+                    if not pd.isna(row["name"]):
                         self._add_modelpath(name=item_name)
         else:
             print(f"Tried to load {self.settings.base}, but it doesnt exist.")
 
     def create_readme(self):
         readme_txt = (
             "Expected files are:\n\n"
@@ -525,14 +524,15 @@
         class Outputd1d2d_revision(Folder):
             """Outputfolder 1d2d for a specific revision."""
 
             def __init__(self, base, create=True):
                 super().__init__(base, create=create)
 
                 self.add_file("grid_nodes_2d", "grid_nodes_2d.gpkg")
+                self.add_file("grid_wlvl", "grid_wlvl.gpkg")
                 self.add_file("stroming_1d2d_test", "stroming_1d2d_test.gpkg")
                 for T in [1, 3, 15]:
                     self.add_file(f"waterstand_T{T}", f"waterstand_T{T}.tif")
                     self.add_file(f"waterdiepte_T{T}", f"waterdiepte_T{T}.tif")
 
     # TODO hoort deze class hier nog? resultaten staan op een andere plek
     class OutputDirClimate(hrt.Folder):
@@ -542,39 +542,8 @@
             #     self.create()  # create outputfolder if parent exists
 
         @property
         def structure(self):
             return self.revision_structure("Climate")
 
 
-def create_tif_path(folder, filename):
-    """
-    Takes a folder name (ex: C:../output/Layers) and base filename (ex: raster) as arguments
-    and returns full path (ex: C:../output/Layers/raster.tif)
-    """
-    try:
-        full_path = os.path.join(folder, f"{filename}.tif")
-        return full_path
-    except Exception as e:
-        raise e from None
-
-
-def get_top_level_directories(folder, condition_test=None):
-    """
-    Resturns a list of all top level directories, can be filtered with a function (condition_test)
-    that returns a bool and takes one argument (directory)
-    """
-    return [
-        item
-        for item in (os.path.join(folder, d1) for d1 in os.listdir(folder))
-        if os.path.isdir(item) and (condition_test(item) if condition_test is not None else True)
-    ]
-
-
-def if_exists(path):
-    if path is None:
-        return None
-    else:
-        return path if os.path.exists(path) else None
-
-
 # %%
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/result_rasters/calculate_raster.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/result_rasters/calculate_raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # -*- coding: utf-8 -*-
 from pathlib import Path
 
 import hhnk_research_tools as hrt
 import numpy as np
 from osgeo import gdal
-from scipy.spatial import qhull
+from scipy.spatial import Delaunay
 from threedidepth import morton
 from threedigrid.admin.constants import NO_DATA_VALUE
 
 
 class BaseCalculatorGPKG:
     """Calculate interpolated rasters from a grid. The grid_gdf is
     created using the class ThreediGrid. Which converts the NetCDF
@@ -58,25 +58,25 @@
         return lookup_wlvl
 
     @property
     def delaunay(self):
         """
         Return a (delaunay, s1) tuple.
 
-        `delaunay` is a qhull.Delaunay object, and `s1` is an array of
+        `delaunay` is a scipy.spatial.Delaunay object, and `s1` is an array of
         waterlevels for the corresponding delaunay vertices.
         """
         try:
             return self.cache[self.DELAUNAY]
         except KeyError:
             points_grid = np.array(self.grid_gdf.centroid.apply(lambda x: [x.x, x.y]).to_list())
 
             # reorder a la lizard
             points_grid, wlvl = morton.reorder(points_grid, self.wlvl_raw)
-            delaunay = qhull.Delaunay(points_grid)
+            delaunay = Delaunay(points_grid)
             self.cache[self.DELAUNAY] = delaunay, wlvl
             return delaunay, wlvl
 
     def _get_points_mesh(self, window):
         """Create mesh grid points with coordinates every 0.5m with the input window.
         Point are created in the centre of the cell (0.5)
         Args:
@@ -102,21 +102,22 @@
         - The point is inside a grid cell
         - The point is inside the triangulation
         - The sum of weights of active (not 'no data' nodes) is more than half
           of the total weight of all nodes. Only active nodes are included in
           the interpolation.
 
         In all other cases, the waterlevel from the constant level method is
-        used."""
+        used.
+        """
         # start with the constant level result
         nodeid_block = self.nodeid_raster._read_array(window=window)
         # start with the constant level result
         # node_id_grid is 1d array of the node ids in the mesh grid
         nodeid_arr = nodeid_block.ravel()
-        # the waterlevel is known per nodeid. This loopuptable gets the waterlevel
+        # the waterlevel is known per nodeid. This lookuptable gets the waterlevel
         # per point in the mesh grid
         level = self.lookup_wlvl[nodeid_arr]
 
         # determine result raster cell centers and in which triangle they are
         points_mesh = self._get_points_mesh(window)
         delaunay, wlvl = self.delaunay
         simplices = delaunay.find_simplex(points_mesh)
@@ -125,38 +126,38 @@
         in_gridcell = nodeid_arr != 0
         in_triangle = simplices != -1
         in_interpol = in_gridcell & in_triangle
         points_int = points_mesh[in_interpol]
 
         # get the nodes and the transform for the corresponding triangles
         transform = delaunay.transform[simplices[in_interpol]]
-        vertices = delaunay.vertices[simplices[in_interpol]]
+        simplices = delaunay.simplices[simplices[in_interpol]]
 
         # calculate weight, see print(spatial.Delaunay.transform.__doc__) and
         # Wikipedia about barycentric coordinates
-        weight = np.empty(vertices.shape)
+        weight = np.empty(simplices.shape)
         weight[:, :2] = np.sum(transform[:, :2] * (points_int - transform[:, 2])[:, np.newaxis], 2)
         weight[:, 2] = 1 - weight[:, 0] - weight[:, 1]
 
         # set weight to zero when for inactive nodes
-        nodelevel = wlvl[vertices]
+        nodelevel = wlvl[simplices]
         weight[nodelevel == NO_DATA_VALUE] = 0
 
         # determine the sum of weights per result cell
         weight_sum = weight.sum(axis=1)
 
         # further subselect points suitable for interpolation
         suitable = weight_sum > 0.5
         weight = weight[suitable] / weight_sum[suitable][:, np.newaxis]
         nodelevel = nodelevel[suitable]
 
         # combine weight and nodelevel into result
         in_interpol_and_suitable = in_interpol.copy()
         in_interpol_and_suitable[in_interpol] &= suitable
-        level[in_interpol_and_suitable] = np.sum(weight * nodelevel, axis=1)
+        level[in_interpol_and_suitable] = np.sum(weight.astype(float) * nodelevel.astype(float), axis=1)
 
         # Return interpolated mesh grid
         return level.reshape(nodeid_block.shape)
 
     def block_calculate_delauney_wdepth(self, window):
         """depth=wlvl-dem"""
         # Read/create input
@@ -185,16 +186,16 @@
                 metadata=self.dem_raster.metadata,
                 datatype=gdal.GDT_Int32,
                 read_array=False,
             )
 
     def run(self, output_file, mode="MODE_WLVL", min_block_size=1024, overwrite=False):
         # Init rasters
-        self.nodeid_raster = hrt.Raster(Path(str(output_file)).parent / "nodeid.tif")
         self.output_raster = hrt.Raster(output_file)
+        self.nodeid_raster = self.output_raster.parent.full_path("nodeid.tif")
 
         create = hrt.check_create_new_file(output_file=self.output_raster.path, overwrite=overwrite)
 
         if create:
             # Create rasters
             self.output_raster.create(metadata=self.dem_raster.metadata, nodata=NO_DATA_VALUE)
             self.create_nodeid_raster()  # Nodeid raster for calculation
@@ -214,15 +215,15 @@
 
                 target_band.WriteArray(block_out, xoff=window[0], yoff=window[1])
             target_band.FlushCache()  # close file after writing
             target_band = None
             target_ds = None
 
     def __enter__(self):
-        "with BaseCalculatorGPKG(**args) as x. will call this func."
+        """With BaseCalculatorGPKG(**args) as x. will call this func."""
         self.cache = {}
         return self
 
     def __exit__(self, *args):
         self.cache = {}
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/checks/one_d_two_d.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,222 +1,231 @@
 # %%
 import geopandas as gpd
 import hhnk_research_tools as hrt
 import numpy as np
 import pandas as pd
-from shapely.geometry import box
+from hhnk_research_tools.variables import t_end_rain_col, t_end_sum_col, t_start_rain_col
+from shapely.geometry import LineString
 
-from hhnk_threedi_tools import Folders
+import hhnk_threedi_tools.core.checks.grid_result_metadata as grid_result_metadata
+from hhnk_threedi_tools.core.folders import Folders
+from hhnk_threedi_tools.core.result_rasters.calculate_raster import BaseCalculatorGPKG
+
+# Local imports
+from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import NetcdfToGPKG
+from hhnk_threedi_tools.variables.default_variables import DEF_TRGT_CRS
+from hhnk_threedi_tools.variables.one_d_two_d import (
+    content_type_col,
+    id_col,
+    kcu_col,
+    max_sfx,
+    one_d_two_d,
+    pump_capacity_m3_s_col,
+    q_m3_s_col,
+    spatialite_id_col,
+    suffixes_list,
+    two_d,
+    vel_m_s_col,
+)
 
 
-class ThreediGrid:
-    def __init__(
-        self,
-        threedi_result: hrt.ThreediResult,
-        folder: Folders = None,
-        waterdeel_path: str = None,
-        waterdeel_layer: str = "Waterdeel",
-        panden_path: str = None,
-        panden_layer: str = "panden",
-        grid_raw_filename="grid_raw.gpkg",
-        grid_corr_filename="grid_corr.gpkg",
-    ):
-        """
+class OneDTwoDTest:
+    TIMESTEPS = [1, 3, 15]  # hours, 1=start rain, 3=end rain, 15=end calculation
 
-        grid creation requires:
-            folder.source_data.damo
-            folder.source_data.panden
+    def __init__(self, folder: Folders, revision=0, dem_path=None):
+        self.folder = folder
+        self.revision = revision
 
-        Otherwise use waterdeel_path with waterdeel_layer
+        self.result_fd = self.folder.threedi_results.one_d_two_d[self.revision]
+        self.output_fd = self.folder.output.one_d_two_d[self.revision]
 
-        """
-        self.threedi_result = threedi_result
-        self.folder = folder
-        self.waterdeel_path = waterdeel_path
-        self.waterdeel_layer = waterdeel_layer
-        self.panden_path = panden_path
-        self.panden_layer = panden_layer
-
-        self.grid_path = self.threedi_result.full_path(grid_raw_filename)
-        self.grid_corr_path = self.threedi_result.full_path(grid_corr_filename)
-
-    @property
-    def grid(self):
-        return self.threedi_result.grid
-
-    def _load_water_gdf(self):
-        """Load waterdeel. if folder is defined as input we get if from there.
-        Otherwise the path needs to be provided"""
-        gdf = None
-        if self.folder is not None:
-            gdf = self.folder.source_data.damo.load(layer=self.waterdeel_layer)
-
-        elif self.waterdeel_path is not None:
-            if self.waterdeel_path.endswith(".gdb"):
-                gdf = gpd.read_file(self.waterdeel_path, layer=self.waterdeel_layer)
-            else:
-                gdf = gpd.read_file(self.waterdeel_path)
+        self.grid_result = self.result_fd.grid
 
-        else:
-            print("Couldnt load waterdeel. Ignoring it in correction.")
-        return gdf
+        (
+            rain,
+            detected_rain,
+            timestep,
+            days_dry_start,
+            days_dry_end,
+            self.timestep_df,
+        ) = grid_result_metadata.construct_scenario(self.grid_result)
 
-    def _load_pand_gdf(self):
-        """Load waterdeel. if folder is defined as input we get if from there.
-        Otherwise the path needs to be provided"""
-        gdf = None
-        if self.panden_path is None:
-            if self.folder is not None:
-                if self.folder.source_data.panden.exists():
-                    gdf = self.folder.source_data.panden.load(layer=self.panden_layer)
-
-        elif self.panden_path is not None:
-            if self.panden_path.endswith(".gdb"):
-                gdf = gpd.read_file(self.panden_path, layer=self.panden_layer)
-            else:
-                gdf = gpd.read_file(self.panden_path)
+        if dem_path:
+            self.dem = hrt.Raster(dem_path)
         else:
-            print("Couldnt load panden. Ignoring it in correction.")
-        return gdf
+            self.dem = self.folder.model.schema_base.rasters.dem
 
-    def netcdf_to_grid_gpkg(
-        self, replace_dem_below_perc=50, replace_water_above_perc=95, replace_pand_above_perc=99, overwrite=False
-    ):
+    @classmethod
+    def from_path(cls, path_to_polder, **kwargs):
+        return cls(Folders(path_to_polder), **kwargs)
+
+    def run_wlvl_depth_at_timesteps(self, overwrite=False):
+        """Transform netcdf to grid gpkg and apply wlvl correction
+        Then create waterlevel and depth rasters at 3 timesteps:
+        1h : start rain
+        3h : end rain
+        15h : end calculation
         """
-        ignore_dem_perc : if cell has no dem above this value waterlevels will be replaced
-        ignore_water_perc : if cell has water surface area above this value waterlevels will be replaced
+        netcdf_gpkg = NetcdfToGPKG.from_folder(folder=self.folder, threedi_result=self.result_fd)
 
-        create gpkg of grid with maximum wlvl
-        """
+        # Convert netcdf to grid gpkg
+        netcdf_gpkg.run(
+            output_file=self.output_fd.grid_nodes_2d,
+            timesteps_seconds=[T * 3600 for T in self.TIMESTEPS],
+            overwrite=True,
+        )
+
+        # Create depth and wlvl rasters for each timestep.
+        grid_gdf = gpd.read_file(self.output_fd.grid_nodes_2d.path)
+        for T in self.TIMESTEPS:
+            with BaseCalculatorGPKG(
+                dem_path=self.folder.model.schema_base.rasters.dem,
+                grid_gdf=grid_gdf,
+                wlvl_column=f"wlvl_{T}h",
+            ) as raster_calc:
+                raster_calc.run(
+                    output_file=getattr(self.output_fd, f"waterdiepte_T{T}"), mode="MODE_WDEPTH", overwrite=overwrite
+                )
+                raster_calc.run(
+                    output_file=getattr(self.output_fd, f"waterstand_T{T}"), mode="MODE_WLVL", overwrite=overwrite
+                )
 
-        create = hrt.check_create_new_file(output_file=self.grid_path, overwrite=overwrite)
-        if create:
-            # Check required files
-            # if not self.folder.source_data.damo.exists():
-            #     raise Exception(f"{self.folder.source_data.damo} - doesnt exist")
-            # if not self.folder.source_data.panden.exists():
-            #     raise Exception(f"{self.folder.source_data.panden} - doesnt exist")
-
-            grid_gdf = gpd.GeoDataFrame()
-
-            s1_all = self.grid.nodes.subset("2D_open_water").timeseries(indexes=slice(0, -1)).s1
-            vol_all = self.grid.nodes.subset("2D_open_water").timeseries(indexes=slice(0, -1)).vol
-
-            # Find index of max wlvl value in timeseries
-            s1_max_ind = s1_all.argmax(axis=0)
-
-            # * inputs every element from row as a new function argument.
-            grid_gdf["geometry"] = [box(*row) for row in self.grid.nodes.subset("2D_ALL").cell_coords.T]
-            grid_gdf.crs = "EPSG:28992"
-            # nodes_2d["geometry"] = [Point(*row) for row in gr.nodes.subset("2D_ALL").coordinates.T] #centerpoints.
-
-            grid_gdf["id"] = self.grid.cells.subset("2D_open_water").id
-
-            # Retrieve values when wlvl is max
-            grid_gdf["wlvl_max_orig"] = np.round([row[s1_max_ind[enum]] for enum, row in enumerate(s1_all.T)], 5)
-            grid_gdf["vol_netcdf_m3"] = np.round([row[s1_max_ind[enum]] for enum, row in enumerate(vol_all.T)], 5)
-
-            # Percentage of dem in a calculation cell
-            # so we can make a selection of cells on model edge that need to be ignored
-            grid_gdf["dem_area"] = self.grid.cells.subset("2D_open_water").sumax
-            # Percentage dem in calculation cell
-            grid_gdf["dem_perc"] = grid_gdf["dem_area"] / grid_gdf.area * 100
-
-            # Check water surface area in a cell.
-            water_gdf = self._load_water_gdf()
-            if water_gdf is not None:
-                water_gdf["water"] = 1
-                water_cell = gpd.overlay(grid_gdf[["id", "geometry"]], water_gdf[["water", "geometry"]], how="union")
-                # Select only areas with the merged feature.
-                water_cell = water_cell[water_cell["water"] == 1]
-
-                # Calculate sum of area per cell
-                water_cell["water_area"] = water_cell.area
-                water_cell_area = water_cell.groupby("id").agg("sum")
-
-                grid_gdf = pd.merge(grid_gdf, water_cell_area["water_area"], left_on="id", right_on="id", how="left")
-                grid_gdf["water_perc"] = grid_gdf["water_area"] / grid_gdf.area * 100
-            else:
-                grid_gdf["water_perc"] = None
-
-            # Check building area in a cell
-            pand_gdf = self._load_pand_gdf()
-            if pand_gdf is not None:
-                pand_gdf["pand"] = 1
-                pand_cell = gpd.overlay(grid_gdf[["id", "geometry"]], pand_gdf[["pand", "geometry"]], how="union")
-                # Select only areas with the merged feature.
-                pand_cell = pand_cell[pand_cell["pand"] == 1]
-
-                # Calculate sum of area per cell
-                pand_cell["pand_area"] = pand_cell.area
-                pand_cell_area = pand_cell.groupby("id").agg("sum")
-
-                grid_gdf = pd.merge(grid_gdf, pand_cell_area["pand_area"], left_on="id", right_on="id", how="left")
-                grid_gdf["pand_perc"] = grid_gdf["pand_area"] / grid_gdf.area * 100
-            else:
-                grid_gdf["pand_perc"] = None
-
-            # Select cells that need replacing of wlvl
-            grid_gdf["replace_dem"] = grid_gdf["dem_perc"] < replace_dem_below_perc
-            grid_gdf["replace_water"] = grid_gdf["water_perc"] > replace_water_above_perc
-            grid_gdf["replace_pand"] = grid_gdf["pand_perc"] > replace_pand_above_perc
-
-            grid_gdf["replace_all"] = 0
-            grid_gdf.loc[grid_gdf["replace_dem"] == True, "replace_all"] = "dem"
-            grid_gdf.loc[grid_gdf["replace_water"] == True, "replace_all"] = "water"
-            grid_gdf.loc[grid_gdf["replace_pand"] == True, "replace_all"] = "pand"
-
-            # grid_gdf["replace_all"] = grid_gdf["replace_dem"] | grid_gdf["replace_water"] | grid_gdf["replace_pand"]
-
-            grid_gdf = gpd.GeoDataFrame(grid_gdf, geometry="geometry")
-
-            # Save to file
-            grid_gdf.to_file(self.grid_path.base, driver="GPKG")
-
-    def waterlevel_correction(self, output_col="wlvl_max_replaced", overwrite=False):
-        create = hrt.check_create_new_file(output_file=self.grid_corr_path, overwrite=overwrite)
-
-        if create:
-            grid_gdf = self.grid_path.load()
-
-            grid_gdf[output_col] = grid_gdf["wlvl_max_orig"]
-            replace_idx = grid_gdf["replace_all"] != "0"
-            grid_gdf.loc[
-                replace_idx, output_col
-            ] = None  # set values to none so they are not used in calculation of new values.
-
-            for idx, row in grid_gdf.loc[replace_idx].iterrows():
-                # Find neighbour cells
-                neighbours_idx = grid_gdf[grid_gdf.geometry.touches(row.geometry)].index.tolist()
-                neighbours_id = [
-                    grid_gdf.loc[neighbour_idx].id for neighbour_idx in neighbours_idx if idx != neighbour_idx
+    def run_flowline_stats(self):
+        """
+        Deze functie leest alle stroom lijnen in uit het 3di resultaat. Vervolgens wordt gekeken naar het type van de lijn
+        (1D2D of 2D). Vervolgens wordt op drie tijdstappen (het begin van de regen het einde van de regen en het einde van de
+        som) het volgende bepaald:
+            * De waterstand per tijdstap
+            * Het debiet (q) in m3/s per tijdstap
+            * De stroomsnelheid in m/s per tijdstap
+            * De stroomrichting per tijdstap
+        """
+        # Load individual line results
+        flowlines_gdf = self._read_flowline_results()
+        pumplines_gdf = self._read_pumpline_results()
+
+        # combine to one table
+        lines_gdf = pd.concat([flowlines_gdf, pumplines_gdf], ignore_index=True, sort=False)
+        lines_gdf = lines_gdf[lines_gdf.geometry.length != 0]  # Drop weird values with -9999 geometries
+
+        return lines_gdf
+
+    def _read_flowline_results(self):
+        try:
+            coords = hrt.threedi.line_geometries_to_coords(
+                self.grid_result.lines.line_geometries
+            )  # create gdf from node coords
+
+            flowlines_gdf = gpd.GeoDataFrame(geometry=coords, crs=f"EPSG:{DEF_TRGT_CRS}")
+            flowlines_gdf[id_col] = self.grid_result.lines.id
+            flowlines_gdf[spatialite_id_col] = self.grid_result.lines.content_pk
+
+            content_type_list = self.grid_result.lines.content_type.astype("U13")
+            flowlines_gdf[content_type_col] = content_type_list
+
+            flowlines_gdf[kcu_col] = self.grid_result.lines.kcu
+            flowlines_gdf.loc[flowlines_gdf[kcu_col].isin([51, 52]), content_type_col] = one_d_two_d
+            flowlines_gdf.loc[flowlines_gdf[kcu_col].isin([100, 101]), content_type_col] = two_d
+
+            q = self.grid_result.lines.timeseries(
+                indexes=[
+                    self.timestep_df[t_start_rain_col].value,
+                    self.timestep_df[t_end_rain_col].value,
+                    self.timestep_df[t_end_sum_col].value,
                 ]
-                grid_gdf.at[idx, "neighbours"] = str(neighbours_id)
-
-                neighbour_avg_wlvl = np.round(grid_gdf.loc[neighbours_idx][output_col].mean(), 5)
-                grid_gdf.at[idx, output_col] = neighbour_avg_wlvl
-
-            grid_gdf["diff"] = grid_gdf[output_col] - grid_gdf["wlvl_max_orig"]
+            ).q  # waterstand
+            vel = self.grid_result.lines.timeseries(
+                indexes=[
+                    self.timestep_df[t_start_rain_col].value,
+                    self.timestep_df[t_end_rain_col].value,
+                    self.timestep_df[t_end_sum_col].value,
+                ]
+            ).u1
+            q_all = self.grid_result.lines.timeseries(indexes=slice(0, -1)).q
+            vel_all = self.grid_result.lines.timeseries(indexes=slice(0, -1)).u1
+
+            # Write discharge and velocity to columns in dataframe
+            for index, time_str in enumerate(suffixes_list):
+                if time_str == max_sfx:
+                    q_max_ind = abs(q_all).argmax(axis=0)
+                    flowlines_gdf[q_m3_s_col + time_str] = np.round(
+                        [row[q_max_ind[enum]] for enum, row in enumerate(q_all.T)], 5
+                    )
+                else:
+                    flowlines_gdf[q_m3_s_col + time_str] = np.round(q[index], 5)
+
+            for index, time_str in enumerate(suffixes_list):
+                if time_str == max_sfx:
+                    vel_max_ind = abs(vel_all).argmax(axis=0)
+                    flowlines_gdf[vel_m_s_col + time_str] = np.round(
+                        [row[vel_max_ind[enum]] for enum, row in enumerate(vel_all.T)],
+                        5,
+                    )
+                else:
+                    flowlines_gdf[vel_m_s_col + time_str] = np.round(vel[index], 3)
+
+            # Flowlines of 1d2d lines weirdly have flow in different direction.
+            # Therefore we invert this here so arrows are plotted correctly
+            for index, time_str in enumerate(suffixes_list):
+                flowlines_gdf.loc[
+                    flowlines_gdf[content_type_col] == one_d_two_d,
+                    q_m3_s_col + time_str,
+                ] = flowlines_gdf.loc[
+                    flowlines_gdf[content_type_col] == one_d_two_d,
+                    q_m3_s_col + time_str,
+                ].apply(lambda x: x * -1)
+
+            for index, time_str in enumerate(suffixes_list):
+                filt = (
+                    flowlines_gdf[content_type_col] == one_d_two_d,
+                    vel_m_s_col + time_str,
+                )
+
+                flowlines_gdf.loc[filt] = flowlines_gdf.loc[filt].apply(lambda x: x * -1)
+
+            return flowlines_gdf
+        except Exception as e:
+            raise e from None
+
+    def _read_pumpline_results(self):
+        try:
+            coords = [LineString([x[[0, 1]], x[[2, 3]]]) for x in self.grid_result.pumps.node_coordinates.T]
+            pump_gdf = gpd.GeoDataFrame(geometry=coords, crs=f"EPSG:{DEF_TRGT_CRS}")
+
+            pump_gdf[id_col] = self.grid_result.pumps.id
+            pump_gdf[content_type_col] = "pump_line"
+            pump_gdf[pump_capacity_m3_s_col] = self.grid_result.pumps.capacity
+
+            q_m3 = self.grid_result.pumps.timeseries(
+                indexes=[
+                    self.timestep_df[t_start_rain_col].value,
+                    self.timestep_df[t_end_rain_col].value,
+                    self.timestep_df[t_end_sum_col].value,
+                ]
+            ).q_pump  # waterstand
+            q_all_pump = self.grid_result.pumps.timeseries(indexes=slice(0, -1)).q_pump
 
-            # Save to file
-            grid_gdf.to_file(self.grid_corr_path.base, driver="GPKG")
+            for index, time_str in enumerate(suffixes_list):
+                if time_str == max_sfx:
+                    q_max_ind = abs(q_all_pump).argmax(axis=0)
+                    pump_gdf[q_m3_s_col + time_str] = np.round(
+                        [row[q_max_ind[enum]] for enum, row in enumerate(q_all_pump.T)],
+                        5,
+                    )
+                else:
+                    pump_gdf[q_m3_s_col + time_str] = np.round(q_m3[index], 5)
+            return pump_gdf
+        except Exception as e:
+            raise e from None
 
 
+# %%
 if __name__ == "__main__":
-    from hhnk_threedi_tools import Folders
-
-    folder_path = r"E:\02.modellen\23_Katvoed"
-    folder = Folders(folder_path)
+    from pathlib import Path
 
-    threedi_result = folder.threedi_results.one_d_two_d["katvoed #1 piek_ghg_T1000"]
+    TEST_MODEL = Path(__file__).parents[3].joinpath(r"tests/data/model_test/")
+    folder = Folders(TEST_MODEL)
+    self = OneDTwoDTest.from_path(TEST_MODEL)
 
-    self = ThreediGrid(folder=folder, threedi_result=threedi_result)
-    # self = ThreediGrid(threedi_result=threedi_result, waterdeel_path=folder.source_data.damo.path)
+    overwrite = True
 
-    # #Convert netcdf to grid gpkg
-    self.netcdf_to_grid_gpkg()
-
-    # #Replace waterlevel of selected cells with avg of neighbours.
-    # self.waterlevel_correction(output_col="wlvl_max_replaced")
-
-
-# %%
+    output = self.run_wlvl_depth_at_timesteps()
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/migrate.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/migrate.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/model_backup.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/model_backup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/model_splitter.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/model_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# %%
 import datetime
 import os
 import re
 import shutil
 from pathlib import Path
 
 import hhnk_research_tools as hrt
@@ -43,17 +44,15 @@
             self.settings_loaded = True
         else:
             self.settings_df = None
 
         if self.folder.model.settings_default.exists():
             self.settings_default_series = pd.read_excel(
                 self.folder.model.settings_default.base, engine="openpyxl"
-            ).iloc[
-                0
-            ]  # Series, only has one row.
+            ).iloc[0]  # Series, only has one row.
         else:
             self.settings_default_series = None
             self.settings_loaded = False
 
         self.folder.model.set_modelsplitter_paths()
 
         if self.settings_loaded:
@@ -235,17 +234,15 @@
                 df=controlled_weirs_df,
                 layer="v2_cross_section_definition",
                 df_id_col="cross_def_id",
                 db_id_col="id",
                 old_val_col="width",
                 new_val_col="width_new",
             )
-
             database_new.execute_sql_changes(query=query)
-            # hrt.execute_sql_changes(query=query, database=database_path_new)
 
         # execute additional SQL code that is stored in 02_schematisation/model_sql.json.
         if self.folder.model.model_sql.exists():
             model_sql = self.folder.model.model_sql.read_json()
 
             if name in model_sql.keys():
                 for _, query in model_sql[name].items():
@@ -321,24 +318,24 @@
 
 
 # %%
 
 if __name__ == "__main__":
     from hhnk_threedi_tools.core.folders import Folders
 
-    path = r"E:\02.modellen\LangeWeere_NS"
+    path = r"E:\02.modellen\wormer_leggertool"
 
     folder = Folders(path)
-    name = "1d2d_glg"
+    name = "0d1d_test"
 
     self = ModelSchematisations(folder=folder, modelsettings_path=folder.model.settings.path)
     self.create_schematisation(name=name)
-    response = self.create_local_sqlite_revision(commit_message=str(" (local split revision)"))
-    self.upload_schematisation(
-        organisation_uuid="48dac75bef8a42ebbb52e8f89bbdb9f2",
-        name=name,
-        commit_message="testtest",
-        api_key="",
-    )
+    # response = self.create_local_sqlite_revision(commit_message=str(" (local split revision)"))
+    # self.upload_schematisation(
+    #     organisation_uuid="48dac75bef8a42ebbb52e8f89bbdb9f2",
+    #     name=name,
+    #     commit_message="testtest",
+    #     api_key="",
+    # )
 
 
 # %%
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/core/schematisation/upload.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/core/schematisation/upload.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/external/downloader.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/external/downloader.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/external/threedi_calls.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/external/threedi_calls.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/qgis/layer_structure.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/qgis/layer_structure.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/model_settings.xlsx` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/model_settings.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/model_settings_default.xlsx` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/model_settings_default.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/precipitation_frequency.xlsx` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/precipitation_frequency.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif.aux.xml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif.aux.xml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_structure.csv` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_structure.csv`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 test_protocol;['Modelbuilder feedback'];Model feedback naar kijken;"layerid=0|subset=""message"" NOT IN ('Channel segment too short (<5m)','Reference level lowered due to culvert','Reference level lowered due to orifice','culvert ending connection node receives 10m2 storage','weir ending connection node receives 10m2 storage','connection node was removed because it was not connected')";folder.source_data.modelbuilder.path;model_feedback;shp;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";model_feedback_naar_kijken.qml;;;;;;;;;;;;;;;True;;;;;;;;;;;;;
 test_protocol;['Modelbuilder feedback'];Model feedback ernstig;"layerid=0|subset=""level"" NOT IN ('INFO', 'WARNING')";folder.source_data.modelbuilder.path;model_feedback;shp;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";model_feedback_ernstig.qml;;;;;;;;;;;;;;;True;;;;;;;;;;;;;
 test_protocol;['HDB export'];HDB duikers op peilgrens;layername=duikers_op_peilgrens;folder.source_data.path;HDB;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";hdb_duikers_op_peilgrens.qml;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 test_protocol;['HDB export'];HDB stuwen op peilgrens;layername=stuwen_op_peilgrens;folder.source_data.path;HDB;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";hdb_stuwen_op_peilgrens.qml;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 test_protocol;['HDB export'];HDB gemalen op peilgrens;layername=gemalen_op_peilgrens;folder.source_data.path;HDB;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";hdb_gemalen_op_peilgrens.qml;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 test_protocol;['HDB export'];HDB Levee_overstromingsmodel;layername=Levee_overstromingsmodel;folder.source_data.path;HDB;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";hdb_levee_overstromingsmodel.qml;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];Stuw;layername=Stuw;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_stuw.qml;;True;True;True;True;True;;True;True;True;;;;;;;;;;;;;;;;;;
-test_protocol;['DAMO export'];Stuw, automatisch (HDB);layername=Sturing_3Di;folder.source_data.path;HDB;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";HDB_stuw_automatisch.qml;;;;;;;;;;True;;;;;;;;;;;;;;;;;;
+test_protocol;['DAMO export'];Stuw, automatisch (HDB);layername=sturing_kunstwerken;folder.source_data.path;HDB;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";HDB_stuw_automatisch.qml;;;;;;;;;;True;;;;;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];Brug;layername=Brug;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_brug.qml;;;;True;;True;;;;True;;;;;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];Gemaal;layername=Gemaal;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_gemaal.qml;;True;True;True;True;True;;True;True;True;;;;;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];DuikerSifonHevel;layername=DuikerSifonHevel;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_duiker.qml;;True;True;;True;True;;;;True;;;;True;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];Aquaduct;layername=AquaductLijn;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_aquaduct.qml;;;;;;;;;;True;;;;;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];VasteDam;layername=VasteDam;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_vaste_dam.qml;;;;;;;;;;True;;;;;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];Vispassage;layername=Vispassage;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_vispassage.qml;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 test_protocol;['DAMO export'];Sluis;layername=Sluis;folder.source_data.path;DAMO;gpkg;;"os.path.join(qgis_layer_styles_dir, 'test_protocol_v21')";DAMO_sluis.qml;;;True;True;;True;;;;True;;;;;;;;;;;;;;;;;;
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_cross_sections.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_cross_sections.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_flowlines.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_flowlines.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_watergangen.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/bank_levels/stroming_1d2d_watergangen.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/grid/cells.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/grid/cells.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/grid/lines.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/grid/lines.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/grid/nodes.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/grid/nodes.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Landgebruik (v1801c).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Landgebruik (v1801c).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Luchtfoto Actueel Ortho 25cm RGB.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/Luchtfoto Actueel Ortho 25cm RGB.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/brtachtergrondkaartgrijs.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/brtachtergrondkaartgrijs.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast_correctie.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_overlast_correctie.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas_correctie.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/cw_schade_plas_correctie.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/geen_schade.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/geen_schade.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatiediepte.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatiediepte.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0010.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0010.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0100.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T0100.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T1000.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/inundatievlak_T1000.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/maskerkaart.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/maskerkaart.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/peilgebieden.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/peilgebieden.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon_wit.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/polder_polygon_wit.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/ruimtekaart.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/ruimtekaart.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_correctie.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_correctie.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast_correctie.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_overlast_correctie.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas_correctie.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/schade_per_peilgebied_plas_correctie.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/waterlevel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/klimaatsommen/waterlevel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_amount.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_amount.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_dry_category.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/flow_dry_category.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/grid_nodes_2d.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/grid_nodes_2d.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterdepth.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterdepth.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterlevel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/one_d_two_d/waterlevel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_depth.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_depth.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_width.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/channel_width.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/controlled_structs.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/controlled_structs.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_duplicates.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_duplicates.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_no_vertex.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/cross_section_no_vertex.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/dewatering_depth.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/dewatering_depth.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/isolated_channels.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/isolated_channels.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/structs_channel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/structs_channel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/watersurface_area.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/watersurface_area.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/weir_height.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/sqlite_test/weir_height.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_aquaduct.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_aquaduct.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_brug.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_brug.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_duiker.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_duiker.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_gemaal.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_gemaal.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_sluis.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_sluis.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_stuw.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_stuw.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vaste_dam.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vaste_dam.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vispassage.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/DAMO_vispassage.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/HDB_stuw_automatisch.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/HDB_stuw_automatisch.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_lijn.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_lijn.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_punt.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/aquaduct_punt.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bodemhoogte_kunstwerken.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bodemhoogte_kunstwerken.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/boezem.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/boezem.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_niet_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_niet_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_wel_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/bruggen_wel_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/channel_surface_from_profiles.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/channel_surface_from_profiles.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dam.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dam.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_gw_pro.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_gw_pro.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_waterdeel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/damo_waterdeel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_crosssection.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_crosssection.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_output_channel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/datachecker_output_channel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem_hillshade.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/dem_hillshade.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/drooglegging.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/drooglegging.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker,_syphon,_hevel_(lijn).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker,_syphon,_hevel_(lijn).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_bob.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_bob.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_doorstroomafmeting.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_aanname_doorstroomafmeting.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_syphon_hevel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duiker_syphon_hevel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_niet_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_niet_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_wel_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikers_wel_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_lijn.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_lijn.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_punt.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/duikersifonhevel_punt.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/friction.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/friction.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/geisoleerde_watergangen.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/geisoleerde_watergangen.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_niet_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_niet_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_peilafwijking.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_peilafwijking.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_wel_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemaal_wel_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemeten_niet_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gemeten_niet_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gestuurde_kunstwerken.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/gestuurde_kunstwerken.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_kunstwerken.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_kunstwerken.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_watergang_segmenten.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hd_watergang_segmenten.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_duikers_op_peilgrens.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_duikers_op_peilgrens.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_gemalen_op_peilgrens.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_gemalen_op_peilgrens.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_levee_overstromingsmodel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_levee_overstromingsmodel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_stuwen_op_peilgrens.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hdb_stuwen_op_peilgrens.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hydro_deelgebieden_(hdb).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/hydro_deelgebieden_(hdb).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/infiltration.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/infiltration.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/kzk.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/kzk.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/levee_30_cm_boven_max_peil.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/levee_30_cm_boven_max_peil.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/luchtfoto_actueel_ortho_25cm_rgb.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/luchtfoto_actueel_ortho_25cm_rgb.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_lines.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_lines.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_points.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/misfit_points.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ernstig.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ernstig.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_naar_kijken.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_naar_kijken.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ter_info.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/model_feedback_ter_info.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/openstreetmap.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/openstreetmap.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/opmerkingen.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/opmerkingen.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo_huidig).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilafwijkinggebied_(damo_huidig).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebied_aanname_streefpeil.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebied_aanname_streefpeil.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebieden_(datacheck).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebieden_(datacheck).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo_huidig).qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/peilgebiedpraktijk_(damo_huidig).qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/polder_polygon.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/polder_polygon.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ggg.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ggg.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ghg.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_ghg.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_glg.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/storage_glg.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuw_aanname_breedte.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuw_aanname_breedte.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_niet_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_niet_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_wel_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/stuwen_wel_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_boundary_conditions_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_1d_lateral_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_boundary_conditions.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_boundary_conditions.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_lateral.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_2d_lateral.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_aggregation_settings.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_aggregation_settings.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_channel.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_channel.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_connection_nodes.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_connection_nodes.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_definition.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_definition.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_cross_section_location_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_culvert_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_dem_average_area.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_dem_average_area.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_global_settings.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_global_settings.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement_area.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_grid_refinement_area.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_groundwater.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_groundwater.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface_map.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_impervious_surface_map.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_interflow.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_interflow.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_levee.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_levee.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_manhole_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_numerical_settings.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_numerical_settings.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_obstacle.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_obstacle.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_orifice_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pipe_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_point_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_point_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_pumpstation_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_simple_infiltration.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_simple_infiltration.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_map.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_map.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_parameters.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_surface_parameters.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir_view.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_weir_view.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_windshielding.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/v2_windshielding.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_niet_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_niet_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_wel_in_model.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/vaste_dammen_wel_in_model.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_loose.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_loose.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.sld` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergang_channel_nowayout.sld`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.sld` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_breedte.sld`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.sld` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/watergangen_diepte.sld`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.sld` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_primair.sld`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.sld` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen,_secundair,_tertiair.sld`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.sld` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterlopen.sld`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.sld` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/test_protocol_v21/waterpeilen_ahn3_uit_datamining.sld`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__default.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__default.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__detailed.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/debiet_hyd_toets__detailed.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/discharge.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/discharge.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_kunstwerken.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_kunstwerken.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_watergangen.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/hydraulische_toets_watergangen.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_end_rain_min_1.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_end_rain_min_1.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__default.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__default.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__original.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_rain_vs_start_rain__original.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_sum_start_sum.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_end_sum_start_sum.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_start_rain_vs_start_sum.qml` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_layer_styles/zero_d_one_d/waterlvl_start_rain_vs_start_sum.qml`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten.qpt` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten.qpt`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten2.qpt` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten2.qpt`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten_landscape.qpt` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/resources/qgis_print_layouts/wsa_kaarten_landscape.qpt`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Nov  6 13:43:34 2023 UTC, .py size: 20260 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 86ed 4865 244f 0000  a.........He$O..
+00000000: 610d 0d0a 0000 0000 0da4 5c65 754e 0000  a.........\euN..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 006f 0000 0040 0000 0073 3a08 0000 6400  .o...@...s:...d.
+00000020: 006f 0000 0040 0000 0073 1c08 0000 6400  .o...@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000050: 6d08 5a08 0100 6401 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c0b 5400 6401 6405 6c0c  ..d.d.l.T.d.d.l.
 00000070: 5400 6401 6406 6c0d 6d0e 5a0e 0100 6401  T.d.d.l.m.Z...d.
 00000080: 6407 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
 00000090: 6d13 5a13 6d14 5a14 6d15 5a15 0100 6401  m.Z.m.Z.m.Z...d.
@@ -103,877 +103,869 @@
 00000660: 9b00 6415 6537 9b00 643b 652b 9b00 6415  ..d.e7..d;e+..d.
 00000670: 6519 9b00 6437 6534 9b00 643c 652b 9b00  e...d7e4..d<e+..
 00000680: 6415 6519 9b00 641b 6534 9b00 6415 6531  d.e...d.e4..d.e1
 00000690: 9b00 643d 654a 9b00 6415 6558 9b00 643e  ..d=eJ..d.eX..d>
 000006a0: 6548 9b00 643f 9d69 5a59 642a 655a 9b00  eH..d?.iZYd*eZ..
 000006b0: 642b 6519 9b00 642c 655b 9b00 6440 9d07  d+e...d,e[..d@..
 000006c0: 5a5c 6441 6519 9b00 6442 652e 9b00 6443  Z\dAe...dBe...dC
-000006d0: 6537 9b00 6444 651d 9b00 640e 655d 9b00  e7..dDe...d.e]..
-000006e0: 6445 651e 9b00 6446 651f 9b00 6444 651d  dEe...dFe...dDe.
-000006f0: 9b00 640e 655d 9b00 640e 655e 9b00 6445  ..d.e]..d.e^..dE
-00000700: 651e 9b00 6447 655f 9b00 6444 651d 9b00  e...dGe_..dDe...
-00000710: 640e 655d 9b00 640e 655e 9b00 6445 651e  d.e]..d.e^..dEe.
-00000720: 9b00 641a 6560 9b00 6445 651e 9b00 6448  ..d.e`..dEe...dH
-00000730: 6561 9b00 6444 651d 9b00 640e 655d 9b00  ea..dDe...d.e]..
-00000740: 6449 651e 9b00 6446 6562 9b00 6444 651d  dIe...dFeb..dDe.
-00000750: 9b00 640e 655d 9b00 644a 651e 9b00 6446  ..d.e]..dJe...dF
-00000760: 6563 9b00 644b 6520 9b00 640c 6564 9b00  ec..dKe ..d.ed..
-00000770: 644c 6519 9b00 644d 6537 9b00 644e 6520  dLe...dMe7..dNe 
-00000780: 9b00 640c 6565 9b00 644f 6519 9b00 644d  ..d.ee..dOe...dM
-00000790: 652e 9b00 6450 6562 9b00 6451 655f 9b00  e...dPeb..dQe_..
-000007a0: 6452 6563 9b00 6451 6561 9b00 6411 9d4f  dRec..dQea..d..O
-000007b0: 5a66 6453 6454 8400 5a67 6700 6700 6700  ZfdSdT..Zgg.g.g.
-000007c0: 6603 6455 6456 8401 5a68 6700 6601 6457  f.dUdV..Zhg.f.dW
-000007d0: 6458 8401 5a69 6459 645a 8400 5a6a 6700  dX..ZidYdZ..Zjg.
-000007e0: 6601 645b 645c 8401 5a6b 645d 645e 8400  f.d[d\..Zkd]d^..
-000007f0: 5a6c 645f 6460 8400 5a6d 6700 6601 6461  Zld_d`..Zmg.f.da
-00000800: 6462 8401 5a6e 6700 6601 6463 6464 8401  db..Zng.f.dcdd..
-00000810: 5a6f 6465 6466 8400 5a70 6467 6468 8400  Zodedf..Zpdgdh..
-00000820: 5a71 6571 8300 5a72 6700 6601 6469 646a  Zqeq..Zrg.f.didj
-00000830: 8401 5a73 646b 646c 8400 5a74 646d 646e  ..Zsdkdl..Ztdmdn
-00000840: 8400 5a75 6575 8300 5a76 650e 6601 646f  ..Zueu..Zve.f.do
-00000850: 6470 8401 5a77 6577 652b 6578 6702 6471  dp..Zwewe+exg.dq
-00000860: 8d01 5a79 6402 5300 2972 7a91 0a43 7265  ..Zyd.S.)rz..Cre
-00000870: 6174 6564 206f 6e20 4d6f 6e20 4175 6720  ated on Mon Aug 
-00000880: 3136 2031 323a 3034 3a33 3320 3230 3231  16 12:04:33 2021
-00000890: 0a0a 4061 7574 686f 723a 2063 6872 6973  ..@author: chris
-000008a0: 2e6b 6572 6b6c 6161 6e0a 0a41 6c6c 2073  .kerklaan..All s
-000008b0: 716c 6974 6520 7175 6572 6965 7320 6172  qlite queries ar
-000008c0: 6520 7374 6f72 6564 2077 6974 6869 6e20  e stored within 
-000008d0: 7468 6973 2073 6372 6970 742e 2051 7565  this script. Que
-000008e0: 7269 6573 2061 7265 206c 6973 7465 6420  ries are listed 
-000008f0: 7065 7220 7461 626c 652e 0a0a 0ae9 0000  per table.......
-00000900: 0000 4e29 03da 1342 414e 4b5f 4c56 4c53  ..N)...BANK_LVLS
-00000910: 5f4c 4153 545f 4341 4c43 da17 434f 4e54  _LAST_CALC..CONT
-00000920: 525f 5745 4952 5f57 4944 5448 5f42 4143  R_WEIR_WIDTH_BAC
-00000930: 4b55 50da 1547 4c4f 4241 4c5f 5345 5454  KUP..GLOBAL_SETT
-00000940: 494e 4753 5f54 4142 4c45 2901 da12 6e65  INGS_TABLE)...ne
-00000950: 775f 6261 6e6b 5f6c 6576 656c 5f63 6f6c  w_bank_level_col
-00000960: 2901 da01 2a29 01da 0c44 4546 5f54 5247  )...*)...DEF_TRG
-00000970: 545f 4352 5329 06da 1663 6861 6e6e 656c  T_CRS)...channel
-00000980: 735f 6e65 775f 6361 6c63 5f74 7970 65da  s_new_calc_type.
-00000990: 1c67 6c6f 6261 6c5f 7365 7474 696e 6773  .global_settings
-000009a0: 5f6e 6577 5f63 6f6c 5f6e 616d 65da 1468  _new_col_name..h
-000009b0: 7964 7261 756c 6963 5f74 6573 745f 7374  ydraulic_test_st
-000009c0: 6174 65da 166d 616e 686f 6c65 735f 6e65  ate..manholes_ne
-000009d0: 775f 6361 6c63 5f74 7970 65da 116f 6e65  w_calc_type..one
-000009e0: 5f64 5f74 776f 5f64 5f73 7461 7465 da13  _d_two_d_state..
-000009f0: 7765 6972 735f 6e65 775f 7769 6474 685f  weirs_new_width_
-00000a00: 636f 6c29 01da 0b6e 6577 5f72 6566 5f6c  col)...new_ref_l
-00000a10: 766c 7a13 0a20 2020 2053 454c 4543 5420  vlz..    SELECT 
-00000a20: 2a20 4652 4f4d 207a 120a 2020 2020 5748  * FROM z..    WH
-00000a30: 4552 4520 7b7d 0a20 2020 20fa 0c0a 2020  ERE {}.    ...  
-00000a40: 2020 5345 4c45 4354 20fa 0420 6173 207a    SELECT .. as z
-00000a50: 062c 2020 2020 20fa 0128 fa05 2920 6173  .,     ..(..) as
-00000a60: 207a 0a20 2020 2020 4652 4f4d 207a 050a   z.     FROM z..
-00000a70: 2020 2020 fa06 2c0a 2020 2020 fa0a 0a20      ..,.    ... 
-00000a80: 2020 2046 524f 4d20 7a10 0a20 2020 2053     FROM z..    S
-00000a90: 454c 4543 540a 2020 2020 da01 2efa 0f0a  ELECT.    ......
-00000aa0: 2020 2020 4c45 4654 204a 4f49 4e20 fa08      LEFT JOIN ..
-00000ab0: 0a20 2020 204f 4e20 7a04 203d 3d20 7a10  .    ON z. == z.
-00000ac0: 0a20 2020 2053 454c 4543 5420 2020 2020  .    SELECT     
-00000ad0: fa02 2c20 fa03 203d 207a 210a 2020 2020  .., .. = z!.    
-00000ae0: 2020 2020 2020 2020 5345 4c45 4354 200a          SELECT .
-00000af0: 2020 2020 2020 2020 2020 2020 7a04 2041              z. A
-00000b00: 5320 7a0e 2c0a 2020 2020 2020 2020 2020  S z.,.          
-00000b10: 2020 7a12 0a20 2020 2020 2020 2020 2020    z..           
-00000b20: 2046 524f 4d20 7a17 0a20 2020 2020 2020   FROM z..       
-00000b30: 2020 2020 204c 4546 5420 4a4f 494e 207a       LEFT JOIN z
-00000b40: 0420 4f4e 207a 160a 2020 2020 2020 2020  . ON z..        
-00000b50: 2020 2020 4752 4f55 5020 4259 207a 0d0a      GROUP BY z..
-00000b60: 2020 2020 2020 2020 2020 2020 7a0d 6372              z.cr
-00000b70: 6561 7465 2074 6162 6c65 207a 2128 6964  eate table z!(id
-00000b80: 2069 6e74 2050 5249 4d41 5259 204b 4559   int PRIMARY KEY
-00000b90: 2c20 6474 2064 6174 6574 696d 6529 7a17  , dt datetime)z.
-00000ba0: 494e 5345 5254 204f 5220 5245 504c 4143  INSERT OR REPLAC
-00000bb0: 4520 494e 544f 207a 1d0a 5641 4c55 4553  E INTO z..VALUES
-00000bc0: 2831 2c20 6375 7272 656e 745f 7469 6d65  (1, current_time
-00000bd0: 7374 616d 7029 7a2c 5345 4c45 4354 2064  stamp)z,SELECT d
-00000be0: 6174 6574 696d 6528 6474 2c20 276c 6f63  atetime(dt, 'loc
-00000bf0: 616c 7469 6d65 2729 2041 5320 6474 2046  altime') AS dt F
-00000c00: 524f 4d20 7a08 206c 696d 6974 2031 7a08  ROM z. limit 1z.
-00000c10: 0a53 454c 4543 5420 fa02 2c0a 7a06 0a46  .SELECT ..,.z..F
-00000c20: 524f 4d20 da01 0a7a 130a 2020 2020 5345  ROM ...z..    SE
-00000c30: 4c45 4354 202a 2066 726f 6d20 7a07 2057  LECT * from z. W
-00000c40: 4845 5245 207a 1520 696e 2028 0a20 2020  HERE z. in (.   
-00000c50: 2053 454c 4543 540a 2020 2020 fa10 0a20   SELECT.    ... 
-00000c60: 2020 2049 4e4e 4552 204a 4f49 4e20 7a0b     INNER JOIN z.
-00000c70: 0a20 2020 2029 0a20 2020 207a 0e0a 2020  .    ).    z..  
-00000c80: 2020 5345 4c45 4354 2077 2e7a 082c 0a20    SELECT w.z.,. 
-00000c90: 2020 2077 2e7a 1920 6173 2077 0a20 2020     w.z. as w.   
-00000ca0: 2020 2020 2049 4e4e 4552 204a 4f49 4e20       INNER JOIN 
-00000cb0: 7a0e 0a20 2020 2020 2020 204f 4e20 772e  z..        ON w.
-00000cc0: fa13 0a20 2020 2020 2020 204c 4546 5420  ...        LEFT 
-00000cd0: 4a4f 494e 207a 0f0a 2020 2020 2020 2020  JOIN z..        
-00000ce0: 4f4e 2028 772e 7a05 2069 6e20 287a 0f29  ON (w.z. in (z.)
-00000cf0: 0a20 2020 2020 2020 204f 5220 772e 7a0f  .        OR w.z.
-00000d00: 2929 0a20 2020 2020 2020 2041 4e44 20fa  )).        AND .
-00000d10: 0c0a 2020 2020 2020 2020 4f4e 20fa 0b0a  ..        ON ...
-00000d20: 2020 2020 5748 4552 4520 7a04 203d 2027      WHERE z. = '
-00000d30: fa06 270a 2020 2020 fa02 3b0a 7a2f 2020  ..'.    ..;.z/  
-00000d40: 2020 5345 4c45 4354 202a 0a20 2020 2046    SELECT *.    F
-00000d50: 524f 4d20 280a 2020 2020 2020 2020 5345  ROM (.        SE
-00000d60: 4c45 4354 207b 7461 626c 657d 2e7a 332c  LECT {table}.z3,
-00000d70: 0a20 2020 2020 2020 2027 7b74 6162 6c65  .        '{table
-00000d80: 7d27 2061 7320 7461 626c 655f 6e61 6d65  }' as table_name
-00000d90: 2c0a 2020 2020 2020 2020 7b74 6162 6c65  ,.        {table
-00000da0: 7d2e 7a12 2c0a 2020 2020 2020 2020 7b74  }.z.,.        {t
-00000db0: 6162 6c65 7d2e fa0a 2c0a 2020 2020 2020  able}...,.      
-00000dc0: 2020 7a09 287b 7461 626c 657d 2e7a 142c    z.({table}.z.,
-00000dd0: 207b 7072 6f6a 6563 7469 6f6e 7d29 2920   {projection})) 
-00000de0: 6173 207a 182c 2031 292c 207b 7072 6f6a  as z., 1), {proj
-00000df0: 6563 7469 6f6e 7d29 2920 6173 207a 1629  ection})) as z.)
-00000e00: 292c 207b 7072 6f6a 6563 7469 6f6e 7d29  ), {projection})
-00000e10: 2920 6173 207a 1828 636f 6e6e 6563 7469  ) as z.(connecti
-00000e20: 6f6e 5f6e 6f64 6573 5f73 7461 7274 2e7a  on_nodes_start.z
-00000e30: 1628 636f 6e6e 6563 7469 6f6e 5f6e 6f64  .(connection_nod
-00000e40: 6573 5f65 6e64 2e7a 380a 2020 2020 2020  es_end.z8.      
-00000e50: 2020 4652 4f4d 0a20 2020 2020 2020 207b    FROM.        {
-00000e60: 7461 626c 657d 0a20 2020 2020 2020 204c  table}.        L
-00000e70: 4546 5420 4a4f 494e 0a20 2020 2020 2020  EFT JOIN.       
-00000e80: 207a 290a 2020 2020 2020 2020 4f4e 0a20   z).        ON. 
-00000e90: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-00000ea0: 6e5f 6e6f 6465 735f 656e 642e 7a0c 2049  n_nodes_end.z. I
-00000eb0: 5320 7b74 6162 6c65 7d2e 7a1b 0a20 2020  S {table}.z..   
-00000ec0: 2020 2020 204c 4546 5420 4a4f 494e 0a20       LEFT JOIN. 
-00000ed0: 2020 2020 2020 207a 2b0a 2020 2020 2020         z+.      
-00000ee0: 2020 4f4e 0a20 2020 2020 2020 2063 6f6e    ON.        con
-00000ef0: 6e65 6374 696f 6e5f 6e6f 6465 735f 7374  nection_nodes_st
-00000f00: 6172 742e 7a11 0a20 2020 2029 0a20 2020  art.z..    ).   
-00000f10: 2057 4845 5245 207a 0820 4953 204e 4f54   WHERE z. IS NOT
-00000f20: 207a 0420 4f52 2063 0100 0000 0000 0000   z. OR c........
-00000f30: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000f40: 7344 0000 0074 009b 0064 0174 019b 0064  sD...t...d.t...d
-00000f50: 029d 047d 017c 0074 026b 0272 247c 01a0  ...}.|.t.k.r$|..
-00000f60: 0364 03a1 017d 016e 127c 0074 046b 0272  .d...}.n.|.t.k.r
-00000f70: 367c 01a0 0364 04a1 017d 0174 05a0 037c  6|...d...}.t...|
-00000f80: 01a1 017d 027c 0253 0029 054e 7a05 207b  ...}.|.S.).Nz. {
-00000f90: 7d20 27fa 0127 7a02 3d3d 7a02 213d 2906  } '..'z.==z.!=).
-00000fa0: 5a08 6e61 6d65 5f63 6f6c 5a10 7a65 726f  Z.name_colZ.zero
-00000fb0: 5f64 5f6f 6e65 5f64 5f76 616c 720a 0000  _d_one_d_valr...
-00000fc0: 00da 0666 6f72 6d61 7472 0c00 0000 da13  ...formatr......
-00000fd0: 616c 6c5f 676c 6f62 616c 5f73 6574 7469  all_global_setti
-00000fe0: 6e67 7329 035a 0874 6f5f 7374 6174 655a  ngs).Z.to_stateZ
-00000ff0: 0c77 6865 7265 5f63 6c61 7573 65da 0571  .where_clause..q
-00001000: 7565 7279 a900 7227 0000 00fa 4b65 3a5c  uery..r'....Ke:\
-00001010: 6769 7468 7562 5c77 7661 6e67 6572 7765  github\wvangerwe
-00001020: 6e5c 6868 6e6b 2d74 6872 6565 6469 2d74  n\hhnk-threedi-t
-00001030: 6f6f 6c73 5c68 686e 6b5f 7468 7265 6564  ools\hhnk_threed
-00001040: 695f 746f 6f6c 735c 7574 696c 735c 7175  i_tools\utils\qu
-00001050: 6572 6965 732e 7079 da28 6372 6561 7465  eries.py.(create
-00001060: 5f67 6c6f 6261 6c5f 7365 7474 696e 6773  _global_settings
-00001070: 5f66 726f 6d5f 6261 636b 7570 5f71 7565  _from_backup_que
-00001080: 7279 dd00 0000 730e 0000 0000 0110 0108  ry....s.........
-00001090: 010c 0108 010a 010a 0172 2900 0000 6303  .........r)...c.
-000010a0: 0000 0000 0000 0000 0000 0007 0000 000e  ................
-000010b0: 0000 0043 0000 0073 ac00 0000 6401 7400  ...C...s....d.t.
-000010c0: 9b00 6402 7401 9b00 6403 7402 9b00 6404  ..d.t...d.t...d.
-000010d0: 7402 9b00 6405 6406 a003 7404 7405 7c00  t...d.d...t.t.|.
-000010e0: 8302 a101 9b00 6407 9d0b 7d03 6408 7400  ......d...}.d.t.
-000010f0: 9b00 6403 7402 9b00 6409 7402 9b00 6405  ..d.t...d.t...d.
-00001100: 6406 a003 7404 7405 7c00 8302 a101 9b00  d...t.t.|.......
-00001110: 6407 9d09 7d04 6700 7d05 7c01 727e 7c05  d...}.g.}.|.r~|.
-00001120: a006 7c03 a007 6406 a003 7404 7405 7c01  ..|...d...t.t.|.
-00001130: 8302 a101 a101 a101 0100 7c02 729e 7c05  ..........|.r.|.
-00001140: a006 7c04 a007 6406 a003 7404 7405 7c02  ..|...d...t.t.|.
-00001150: 8302 a101 a101 a101 0100 640a a003 7c05  ..........d...|.
-00001160: a101 7d06 7c06 5300 290b 7a74 0a20 2020  ..}.|.S.).zt.   
-00001170: 2041 6464 2072 6f77 7320 6672 6f6d 2062   Add rows from b
-00001180: 6163 6b75 702c 2064 656c 6574 6520 726f  ackup, delete ro
-00001190: 7773 2066 726f 6d20 6d6f 6465 6c0a 2020  ws from model.  
-000011a0: 2020 4f6e 6365 2074 6865 2063 6f72 7265    Once the corre
-000011b0: 6374 2072 6f77 7320 6172 6520 696e 2074  ct rows are in t
-000011c0: 6865 206d 6f64 656c 2c20 7365 7420 6d6f  he model, set mo
-000011d0: 6465 6c20 636f 6e74 726f 6c0a 2020 2020  del control.    
-000011e0: 7a11 0a20 2020 2049 4e53 4552 5420 494e  z..    INSERT IN
-000011f0: 544f 207a 170a 2020 2020 5345 4c45 4354  TO z..    SELECT
-00001200: 202a 0a20 2020 2046 524f 4d20 721f 0000   *.    FROM r...
-00001210: 007a 1120 696e 2028 7b7d 290a 2020 2020  .z. in ({}).    
-00001220: 414e 4420 7a09 204e 4f54 2049 4e20 2872  AND z. NOT IN (r
-00001230: 1800 0000 fa06 290a 2020 2020 7a11 0a20  ......).    z.. 
-00001240: 2020 2044 454c 4554 4520 4652 4f4d 207a     DELETE FROM z
-00001250: 1120 494e 2028 7b7d 290a 2020 2020 414e  . IN ({}).    AN
-00001260: 4420 7221 0000 0029 08da 1567 6c6f 6261  D r!...)...globa
-00001270: 6c5f 7365 7474 696e 6773 5f6c 6179 6572  l_settings_layer
-00001280: 7204 0000 00da 0669 645f 636f 6cda 046a  r......id_col..j
-00001290: 6f69 6eda 036d 6170 da03 7374 72da 0661  oin..map..str..a
-000012a0: 7070 656e 6472 2400 0000 2907 da0c 6578  ppendr$...)...ex
-000012b0: 636c 7564 6564 5f69 6473 5a0a 6964 735f  cluded_idsZ.ids_
-000012c0: 746f 5f61 6464 5a0d 6964 735f 746f 5f64  to_addZ.ids_to_d
-000012d0: 656c 6574 655a 0e61 6464 5f72 6f77 735f  eleteZ.add_rows_
-000012e0: 7175 6572 795a 1164 656c 6574 655f 726f  queryZ.delete_ro
-000012f0: 7773 5f71 7565 7279 da0a 7175 6572 795f  ws_query..query_
-00001300: 6c69 7374 7226 0000 0072 2700 0000 7227  listr&...r'...r'
-00001310: 0000 0072 2800 0000 da28 6372 6561 7465  ...r(....(create
-00001320: 5f67 6c6f 6261 6c5f 7365 7474 696e 6773  _global_settings
-00001330: 5f72 6f77 735f 7570 6461 7465 5f71 7565  _rows_update_que
-00001340: 7279 e700 0000 7336 0000 0000 0502 0102  ry....s6........
-00001350: ff04 0302 fd04 0402 fc04 0502 fb04 050e  ................
-00001360: fb08 0802 0102 ff04 0202 fe04 0302 fd04  ................
-00001370: 030e fd08 0504 0104 011c 0104 011c 010a  ................
-00001380: 0172 3300 0000 6302 0000 0000 0000 0000  .r3...c.........
-00001390: 0000 0003 0000 0009 0000 0043 0000 0073  ...........C...s
-000013a0: 1c00 0000 7400 6a01 7c00 7402 7403 7403  ....t.j.|.t.t.t.
-000013b0: 7404 7405 7c01 6401 8d07 7d02 7c02 5300  t.t.|.d...}.|.S.
-000013c0: a902 4ea9 07da 0264 66da 056c 6179 6572  ..N....df..layer
-000013d0: da09 6466 5f69 645f 636f 6cda 0964 625f  ..df_id_col..db_
-000013e0: 6964 5f63 6f6c da0b 6f6c 645f 7661 6c5f  id_col..old_val_
-000013f0: 636f 6cda 0b6e 6577 5f76 616c 5f63 6f6c  col..new_val_col
-00001400: 7231 0000 0029 06da 0368 7274 da20 7371  r1...)...hrt. sq
-00001410: 6c5f 6372 6561 7465 5f75 7064 6174 655f  l_create_update_
-00001420: 6361 7365 5f73 7461 7465 6d65 6e74 722b  case_statementr+
-00001430: 0000 0072 2c00 0000 5a11 636f 6e74 726f  ...r,...Z.contro
-00001440: 6c5f 6772 6f75 705f 636f 6c72 0900 0000  l_group_colr....
-00001450: 2903 5a1c 676c 6f62 616c 5f73 6574 7469  ).Z.global_setti
-00001460: 6e67 735f 746f 5f75 7064 6174 655f 6466  ngs_to_update_df
-00001470: 7231 0000 0072 2600 0000 7227 0000 0072  r1...r&...r'...r
-00001480: 2700 0000 7228 0000 00da 2d63 6f6e 7374  '...r(....-const
-00001490: 7275 6374 5f67 6c6f 6261 6c5f 7365 7474  ruct_global_sett
-000014a0: 696e 6773 5f63 6f6e 7472 6f6c 5f67 726f  ings_control_gro
-000014b0: 7570 5f71 7565 7279 0201 0000 7314 0000  up_query....s...
-000014c0: 0000 0104 0102 0102 0102 0102 0102 0102  ................
-000014d0: 0102 f906 0972 3e00 0000 6302 0000 0000  .....r>...c.....
-000014e0: 0000 0000 0000 0006 0000 001a 0000 0043  ...............C
-000014f0: 0000 0073 2c01 0000 6401 7d02 7c02 6402  ...s,...d.}.|.d.
-00001500: 7400 9b00 6403 7401 9b00 6404 7402 9b00  t...d.t...d.t...
-00001510: 6404 7403 9b00 6404 7404 9b00 6405 7405  d.t...d.t...d.t.
-00001520: 9b00 6404 7406 9b00 6404 7407 9b00 6404  ..d.t...d.t...d.
-00001530: 7408 9b00 6404 7409 9b00 6404 740a 9b00  t...d.t...d.t...
-00001540: 6404 740b 9b00 6406 9d19 3700 7d02 7c02  d.t...d...7.}.|.
-00001550: 6407 3700 7d02 6700 7d03 7c00 a00c a100  d.7.}.g.}.|.....
-00001560: 4400 5d8e 5c02 7d04 7d05 7c05 7403 1900  D.].\.}.}.|.t...
-00001570: 7c01 7601 726a 7c03 a00d 6408 7c05 7401  |.v.rj|...d.|.t.
-00001580: 1900 9b00 6409 7c05 7402 1900 9b00 640a  ....d.|.t.....d.
-00001590: 7c05 7403 1900 9b00 640b 7c05 7404 1900  |.t.....d.|.t...
-000015a0: 9b00 640a 7c05 7405 1900 9b00 6404 7c05  ..d.|.t.....d.|.
-000015b0: 7406 1900 9b00 6404 7c05 7407 1900 9b00  t.....d.|.t.....
-000015c0: 6404 7c05 7408 1900 9b00 6404 7c05 7409  d.|.t.....d.|.t.
-000015d0: 1900 9b00 6404 7c05 740a 1900 9b00 6404  ....d.|.t.....d.
-000015e0: 7c05 740b 1900 9b00 640c 9d17 a101 0100  |.t.....d.......
-000015f0: 716a 7c03 9001 7304 640d 5300 7c02 640e  qj|...s.d.S.|.d.
-00001600: a00e 7c03 a101 640f 1700 3700 7d02 7c02  ..|...d...7.}.|.
-00001610: 740f 7c00 7c01 8302 3700 7d02 7c02 5300  t.|.|...7.}.|.S.
-00001620: 640d 5300 2910 6173 0100 004d 6161 6b20  d.S.).as...Maak 
-00001630: 7371 6c20 7374 6174 656d 656e 7420 6461  sql statement da
-00001640: 7420 6765 6272 7569 6b74 2077 6f72 6474  t gebruikt wordt
-00001650: 206f 6d20 6d61 6e68 6f6c 6573 2074 6520   om manholes te 
-00001660: 6d61 6b65 6e20 6f70 2064 6520 626f 7665  maken op de bove
-00001670: 6e20 656e 2062 656e 656e 6465 6e73 7472  n en benendenstr
-00001680: 6f6f 6d73 6520 636f 6e6e 6563 7469 6f6e  oomse connection
-00001690: 206e 6f64 6573 0a20 2020 2076 616e 206b   nodes.    van k
-000016a0: 756e 7374 7765 726b 656e 206f 7020 7065  unstwerken op pe
-000016b0: 696c 6772 656e 732e 204f 6d64 6174 2064  ilgrens. Omdat d
-000016c0: 657a 6520 6d61 6e68 6f6c 6573 2069 736f  eze manholes iso
-000016d0: 6c61 7465 6420 7a69 6a6e 2069 7320 6572  lated zijn is er
-000016e0: 2067 6565 6e20 7374 726f 6d69 6e67 206d   geen stroming m
-000016f0: 6565 7220 6f76 6572 2064 6520 7065 696c  eer over de peil
-00001700: 6772 656e 7320 6e6f 6469 672e 0a20 2020  grens nodig..   
-00001710: 204f 6f6b 2077 6f72 6474 2065 656e 2073   Ook wordt een s
-00001720: 746f 7261 6765 2061 7265 6120 746f 6567  torage area toeg
-00001730: 6576 6f65 6764 2061 616e 2064 6520 636f  evoegd aan de co
-00001740: 6e6e 6563 7469 6f6e 206e 6f64 6573 2077  nnection nodes w
-00001750: 6161 7220 6d61 6e68 6f6c 6573 2061 616e  aar manholes aan
-00001760: 2077 6f72 6465 6e20 746f 6567 6576 6f65   worden toegevoe
-00001770: 6764 2061 6c73 2064 6965 206e 6f67 0a20  gd als die nog. 
-00001780: 2020 206e 6965 7420 6765 7370 6563 6966     niet gespecif
-00001790: 6963 6565 7264 2069 730a 2020 2020 da00  iceerd is.    ..
-000017a0: 7a0c 494e 5345 5254 2049 4e54 4f20 7a02  z.INSERT INTO z.
-000017b0: 2028 7218 0000 00fa 012c 7a02 290a 7a07   (r......,z.).z.
-000017c0: 5641 4c55 4553 207a 0228 277a 0427 2c20  VALUES z.('z.', 
-000017d0: 277a 0327 2c20 7a03 2c20 27fa 0129 4e72  'z.', z., '..)Nr
-000017e0: 1a00 0000 fa01 3b29 10da 0d6d 616e 686f  ......;)...manho
-000017f0: 6c65 5f6c 6179 6572 da10 6469 7370 6c61  le_layer..displa
-00001800: 795f 6e61 6d65 5f63 6f6c da08 636f 6465  y_name_col..code
-00001810: 5f63 6f6c da10 636f 6e6e 5f6e 6f64 655f  _col..conn_node_
-00001820: 6964 5f63 6f6c da09 7368 6170 655f 636f  id_col..shape_co
-00001830: 6cda 0977 6964 7468 5f63 6f6c da15 6d61  l..width_col..ma
-00001840: 6e68 6f6c 655f 696e 6469 6361 746f 725f  nhole_indicator_
-00001850: 636f 6cda 1463 616c 6375 6c61 7469 6f6e  col..calculation
-00001860: 5f74 7970 655f 636f 6cda 0f64 7261 696e  _type_col..drain
-00001870: 5f6c 6576 656c 5f63 6f6c da0e 626f 7474  _level_col..bott
-00001880: 6f6d 5f6c 766c 5f63 6f6c da0f 7375 7266  om_lvl_col..surf
-00001890: 6163 655f 6c76 6c5f 636f 6cda 0c7a 6f6f  ace_lvl_col..zoo
-000018a0: 6d5f 6361 745f 636f 6cda 0869 7465 7272  m_cat_col..iterr
-000018b0: 6f77 7372 3000 0000 722d 0000 00da 1e63  owsr0...r-.....c
-000018c0: 7265 6174 655f 7570 6461 7465 5f73 746f  reate_update_sto
-000018d0: 7261 6765 5f61 7265 615f 7371 6c29 06da  rage_area_sql)..
-000018e0: 0f6e 6577 5f6d 616e 686f 6c65 735f 6466  .new_manholes_df
-000018f0: 7231 0000 0072 2600 0000 5a08 7371 6c5f  r1...r&...Z.sql_
-00001900: 626f 6479 da05 696e 6465 78da 0372 6f77  body..index..row
-00001910: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
-00001920: 1963 7265 6174 655f 6e65 775f 6d61 6e68  .create_new_manh
-00001930: 6f6c 6573 5f71 7565 7279 1001 0000 7368  oles_query....sh
-00001940: 0000 0000 0604 0102 0108 0102 ff04 0102  ................
-00001950: ff04 0102 ff04 0102 ff04 0202 fe04 0202  ................
-00001960: fe04 0202 fe04 0202 fe04 0302 fd04 0302  ................
-00001970: fd04 0302 fd06 ff04 0608 0104 0110 010c  ................
-00001980: 0104 012a 0106 ff04 0106 ff04 0106 ff04  ...*............
-00001990: 0106 ff04 0206 fe04 0206 fe04 0206 fe06  ................
-000019a0: ff06 0506 0104 0212 010e 0172 5400 0000  ...........rT...
-000019b0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-000019c0: 000a 0000 0043 0000 0073 4e00 0000 7a1e  .....C...sN...z.
-000019d0: 7400 6a01 7c00 7402 7403 7403 7404 7405  t.j.|.t.t.t.t.t.
-000019e0: 7c01 6401 8d07 7d02 7c02 5700 5300 0400  |.d...}.|.W.S...
-000019f0: 7406 7948 0100 7d03 0100 7a12 7c03 6400  t.yH..}...z.|.d.
-00001a00: 8202 5700 5900 6400 7d03 7e03 6e0a 6400  ..W.Y.d.}.~.n.d.
-00001a10: 7d03 7e03 3000 3000 6400 5300 7234 0000  }.~.0.0.d.S.r4..
-00001a20: 0029 0772 3c00 0000 723d 0000 0072 4300  .).r<...r=...rC.
-00001a30: 0000 722c 0000 0072 4a00 0000 720b 0000  ..r,...rJ...r...
-00001a40: 00da 0945 7863 6570 7469 6f6e 2904 5a15  ...Exception).Z.
-00001a50: 6d61 6e68 6f6c 6573 5f74 6f5f 7570 6461  manholes_to_upda
-00001a60: 7465 5f64 6672 3100 0000 7226 0000 00da  te_dfr1...r&....
-00001a70: 0165 7227 0000 0072 2700 0000 7228 0000  .er'...r'...r(..
-00001a80: 00da 1f63 6f6e 7374 7275 6374 5f6d 616e  ...construct_man
-00001a90: 686f 6c65 735f 7570 6461 7465 5f71 7565  holes_update_que
-00001aa0: 7279 2e01 0000 731a 0000 0000 0102 0104  ry....s.........
-00001ab0: 0102 0102 0102 0102 0102 0102 0102 f906  ................
-00001ac0: 0906 010e 0172 5700 0000 6302 0000 0000  .....rW...c.....
-00001ad0: 0000 0000 0000 0005 0000 0009 0000 0043  ...............C
-00001ae0: 0000 0073 7400 0000 6700 7d02 7c00 7400  ...st...g.}.|.t.
-00001af0: a001 7c00 7402 1900 a101 1900 7d03 7c03  ..|.t.......}.|.
-00001b00: 7c03 7403 1900 a004 7c01 a101 0f00 1900  |.t.....|.......
-00001b10: 7d03 7c03 6a05 7346 6401 6402 8400 7c03  }.|.j.sFd.d...|.
-00001b20: 7403 1900 a006 a100 4400 8301 7d02 6403  t.......D...}.d.
-00001b30: a007 7408 7409 7c02 8302 a101 7d04 6404  ..t.t.|.....}.d.
-00001b40: 740a 9b00 6405 7402 9b00 6406 740b 9b00  t...d.t...d.t...
-00001b50: 6407 7c04 9b00 6408 9d09 5300 2909 4e63  d.|...d...S.).Nc
-00001b60: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001b70: 0300 0000 5300 0000 7310 0000 0067 007c  ....S...s....g.|
-00001b80: 005d 087d 017c 0191 0271 0453 0072 2700  .].}.|...q.S.r'.
-00001b90: 0000 7227 0000 0029 02da 022e 30da 0469  ..r'...)....0..i
-00001ba0: 7465 6d72 2700 0000 7227 0000 0072 2800  temr'...r'...r(.
-00001bb0: 0000 da0a 3c6c 6973 7463 6f6d 703e 4301  ....<listcomp>C.
-00001bc0: 0000 f300 0000 007a 3263 7265 6174 655f  .......z2create_
-00001bd0: 7570 6461 7465 5f73 746f 7261 6765 5f61  update_storage_a
-00001be0: 7265 615f 7371 6c2e 3c6c 6f63 616c 733e  rea_sql.<locals>
-00001bf0: 2e3c 6c69 7374 636f 6d70 3e72 4000 0000  .<listcomp>r@...
-00001c00: 7a0c 0a20 2020 2055 5044 4154 4520 7a09  z..    UPDATE z.
-00001c10: 0a20 2020 2053 4554 207a 0f20 3d20 320a  .    SET z. = 2.
-00001c20: 2020 2020 5748 4552 4520 fa05 2049 4e20      WHERE .. IN 
-00001c30: 2872 2a00 0000 290c da02 6e70 da05 6973  (r*...)...np..is
-00001c40: 6e61 6eda 1073 746f 7261 6765 5f61 7265  nan..storage_are
-00001c50: 615f 636f 6c72 4600 0000 da04 6973 696e  a_colrF.....isin
-00001c60: da05 656d 7074 79da 0674 6f6c 6973 7472  ..empty..tolistr
-00001c70: 2d00 0000 722e 0000 0072 2f00 0000 da16  -...r....r/.....
-00001c80: 636f 6e6e 6563 7469 6f6e 5f6e 6f64 6573  connection_nodes
-00001c90: 5f6c 6179 6572 722c 0000 0029 0572 5100  _layerr,...).rQ.
-00001ca0: 0000 7231 0000 005a 1275 7064 6174 655f  ..r1...Z.update_
-00001cb0: 7374 6f72 6167 655f 6964 735a 1875 7064  storage_idsZ.upd
-00001cc0: 6174 655f 7374 6f72 6167 655f 6172 6561  ate_storage_area
-00001cd0: 5f72 6f77 735a 1e75 7064 6174 655f 7374  _rowsZ.update_st
-00001ce0: 6f72 6167 655f 6172 6561 5f69 6473 5f73  orage_area_ids_s
-00001cf0: 7472 696e 6772 2700 0000 7227 0000 0072  tringr'...r'...r
-00001d00: 2800 0000 7250 0000 003e 0100 0073 1e00  (...rP...>...s..
-00001d10: 0000 0001 0401 1201 1401 0601 1601 1001  ................
-00001d20: 0201 02ff 0402 02fe 0403 02fd 0403 02fd  ................
-00001d30: 7250 0000 0063 0200 0000 0000 0000 0000  rP...c..........
-00001d40: 0000 0400 0000 0a00 0000 4300 0000 734e  ..........C...sN
-00001d50: 0000 007a 1e74 006a 017c 0074 0274 0374  ...z.t.j.|.t.t.t
-00001d60: 0474 0574 067c 0164 018d 077d 027c 0257  .t.t.|.d...}.|.W
-00001d70: 0053 0004 0074 0779 4801 007d 0301 007a  .S...t.yH..}...z
-00001d80: 127c 0364 0282 0257 0059 0064 027d 037e  .|.d...W.Y.d.}.~
-00001d90: 036e 0a64 027d 037e 0330 0030 0064 0253  .n.d.}.~.0.0.d.S
-00001da0: 0029 0361 e701 0000 446f 6f72 2065 656e  .).a....Door een
-00001db0: 2061 6e61 6c79 7365 206f 7020 6465 2072   analyse op de r
-00001dc0: 6573 756c 7461 7465 6e20 7765 7465 6e20  esultaten weten 
-00001dd0: 7765 2077 656c 6b65 2077 6174 6572 6761  we welke waterga
-00001de0: 6e67 656e 2065 656e 2031 6432 6420 7665  ngen een 1d2d ve
-00001df0: 7262 696e 6469 6e67 2068 6562 6265 6e20  rbinding hebben 
-00001e00: 6f76 6572 206c 6576 6565 7320 6865 656e  over levees heen
-00001e10: 2e20 416c 6c65 656e 2076 6f6f 7220 6465  . Alleen voor de
-00001e20: 7a65 0a20 2020 2077 6174 6572 6761 6e67  ze.    watergang
-00001e30: 656e 2077 6f72 6465 6e20 6465 2062 616e  en worden de ban
-00001e40: 6b20 6c65 7665 6c73 2067 656c 696a 6b20  k levels gelijk 
-00001e50: 6765 7a65 7420 6161 6e20 6465 206c 6576  gezet aan de lev
-00001e60: 6565 2068 6f6f 6774 6520 6f6d 2076 726f  ee hoogte om vro
-00001e70: 6567 7469 6a64 6967 6520 7569 7477 6973  egtijdige uitwis
-00001e80: 7365 6c69 6e67 2074 6520 766f 6f72 6b6f  seling te voorko
-00001e90: 6d65 6e2e 2044 6520 7265 7374 2076 616e  men. De rest van
-00001ea0: 2064 650a 2020 2020 6261 6e6b 206c 6576   de.    bank lev
-00001eb0: 656c 7320 6b6f 6d74 206f 7020 7374 7265  els komt op stre
-00001ec0: 6566 7065 696c 2b31 3063 6d20 7465 2073  efpeil+10cm te s
-00001ed0: 7461 616e 2e0a 2020 2020 426f 7665 6e73  taan..    Bovens
-00001ee0: 7461 616e 6465 2067 656c 6474 2061 6c73  taande geldt als
-00001ef0: 2077 6520 6465 2062 616e 6b20 6c65 7665   we de bank leve
-00001f00: 6c73 206f 706e 6965 7577 2062 6572 656b  ls opnieuw berek
-00001f10: 656e 656e 2e20 496e 2061 6c6c 6520 616e  enen. In alle an
-00001f20: 6465 7265 2067 6576 616c 6c65 6e0a 2020  dere gevallen.  
-00001f30: 2020 776f 7264 656e 2077 6161 7264 656e    worden waarden
-00001f40: 2067 6562 7275 696b 7420 7569 7420 6565   gebruikt uit ee
-00001f50: 6e20 6261 636b 7570 206f 6620 6469 6520  n backup of die 
-00001f60: 6861 6e64 6d61 7469 6720 7a69 6a6e 2061  handmatig zijn a
-00001f70: 616e 6765 7061 7374 2064 6f6f 7220 6465  angepast door de
-00001f80: 2067 6562 7275 696b 6572 0a20 2020 2029   gebruiker.    )
-00001f90: 0772 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
-00001fa0: 7239 0000 0072 3b00 0000 723a 0000 0072  r9...r;...r:...r
-00001fb0: 3100 0000 4e29 0872 3c00 0000 723d 0000  1...N).r<...r=..
-00001fc0: 00da 1363 726f 7373 5f73 6563 5f6c 6f63  ...cross_sec_loc
-00001fd0: 5f6c 6179 6572 da0e 615f 6372 6f73 735f  _layer..a_cross_
-00001fe0: 6c6f 635f 6964 722c 0000 0072 0500 0000  loc_idr,...r....
-00001ff0: da0e 6261 6e6b 5f6c 6576 656c 5f63 6f6c  ..bank_level_col
-00002000: 7255 0000 0029 045a 126e 6577 5f62 616e  rU...).Z.new_ban
-00002010: 6b5f 6c65 7665 6c73 5f64 6672 3100 0000  k_levels_dfr1...
-00002020: 7226 0000 0072 5600 0000 7227 0000 0072  r&...rV...r'...r
-00002030: 2700 0000 7228 0000 00da 1f63 7265 6174  '...r(.....creat
-00002040: 655f 6261 6e6b 5f6c 6576 656c 735f 7570  e_bank_levels_up
-00002050: 6461 7465 5f71 7565 7279 4d01 0000 731a  date_queryM...s.
-00002060: 0000 0000 0702 0104 0102 0102 0102 0102  ................
-00002070: 0102 0102 0102 f906 0906 010e 0172 6700  .............rg.
-00002080: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
-00002090: 0000 000a 0000 0043 0000 0073 4e00 0000  .......C...sN...
-000020a0: 7a1e 7400 6a01 7c00 7402 7403 7403 7404  z.t.j.|.t.t.t.t.
-000020b0: 7405 7c01 6401 8d07 7d02 7c02 5700 5300  t.|.d...}.|.W.S.
-000020c0: 0400 7406 7948 0100 7d03 0100 7a12 7c03  ..t.yH..}...z.|.
-000020d0: 6400 8202 5700 5900 6400 7d03 7e03 6e0a  d...W.Y.d.}.~.n.
-000020e0: 6400 7d03 7e03 3000 3000 6400 5300 7234  d.}.~.0.0.d.S.r4
-000020f0: 0000 0029 0772 3c00 0000 723d 0000 00da  ...).r<...r=....
-00002100: 0e63 6861 6e6e 656c 735f 6c61 7965 7272  .channels_layerr
-00002110: 2c00 0000 724a 0000 0072 0800 0000 7255  ,...rJ...r....rU
-00002120: 0000 0029 045a 1563 6861 6e6e 656c 735f  ...).Z.channels_
-00002130: 746f 5f75 7064 6174 655f 6466 7231 0000  to_update_dfr1..
-00002140: 0072 2600 0000 7256 0000 0072 2700 0000  .r&...rV...r'...
-00002150: 7227 0000 0072 2800 0000 da23 636f 6e73  r'...r(....#cons
-00002160: 7472 7563 745f 6368 616e 6e65 6c73 5f75  truct_channels_u
-00002170: 7064 6174 655f 7374 6174 656d 656e 7463  pdate_statementc
-00002180: 0100 0073 1a00 0000 0001 0201 0401 0201  ...s............
-00002190: 0201 0201 0201 0201 0201 02f9 0609 0601  ................
-000021a0: 0e01 7269 0000 0063 0200 0000 0000 0000  ..ri...c........
-000021b0: 0000 0000 0300 0000 0900 0000 4300 0000  ............C...
-000021c0: 731c 0000 0074 006a 017c 0074 0274 0374  s....t.j.|.t.t.t
-000021d0: 0474 0574 067c 0164 018d 077d 027c 0253  .t.t.|.d...}.|.S
-000021e0: 0029 027a 8b0a 2020 2020 4372 6561 7465  .).z..    Create
-000021f0: 7320 7173 6c20 7175 6572 7920 746f 2075  s qsl query to u
-00002200: 7064 6174 6520 7265 6665 7265 6e63 6520  pdate reference 
-00002210: 6c65 7665 6c20 7768 6572 6520 6d69 6e69  level where mini
-00002220: 6d75 6d20 7765 6972 2068 6569 6768 7420  mum weir height 
-00002230: 6973 2062 656c 6f77 0a20 2020 2067 726f  is below.    gro
-00002240: 756e 6420 6c65 7665 6c20 2861 6e79 2064  und level (any d
-00002250: 6573 656c 6563 7465 6420 6964 2773 2061  eselected id's a
-00002260: 7265 2073 6b69 7070 6564 290a 2020 2020  re skipped).    
-00002270: 7235 0000 0029 0772 3c00 0000 723d 0000  r5...).r<...r=..
-00002280: 0072 6400 0000 da13 615f 7765 6972 5f63  .rd.....a_weir_c
-00002290: 726f 7373 5f6c 6f63 5f69 6472 2c00 0000  ross_loc_idr,...
-000022a0: da13 7265 6665 7265 6e63 655f 6c65 7665  ..reference_leve
-000022b0: 6c5f 636f 6c72 0e00 0000 2903 5a12 7772  l_colr....).Z.wr
-000022c0: 6f6e 675f 7072 6f66 696c 6573 5f67 6466  ong_profiles_gdf
-000022d0: 7231 0000 0072 2600 0000 7227 0000 0072  r1...r&...r'...r
-000022e0: 2700 0000 7228 0000 00da 2363 7265 6174  '...r(....#creat
-000022f0: 655f 7570 6461 7465 5f72 6566 6572 656e  e_update_referen
-00002300: 6365 5f6c 6576 656c 5f71 7565 7279 7301  ce_level_querys.
-00002310: 0000 7314 0000 0000 0504 0102 0102 0102  ..s.............
-00002320: 0102 0102 0102 0102 f906 0972 6c00 0000  ...........rl...
-00002330: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-00002340: 0072 0000 0043 0000 0073 9c01 0000 7c00  .r...C...s....|.
-00002350: 6401 6400 8502 1900 7d02 7c00 7400 6b02  d.d.....}.|.t.k.
-00002360: 7228 7c01 6402 6b02 7222 7401 7d03 712c  r(|.d.k.r"t.}.q,
-00002370: 7402 7d03 6e04 7403 7d03 7c01 6402 6b02  t.}.n.t.}.|.d.k.
-00002380: 723a 7404 7d04 6e04 7405 7d04 6403 7c02  r:t.}.n.t.}.d.|.
-00002390: 9b00 6404 7406 9b00 6405 7c00 9b00 6406  ..d.t...d.|...d.
-000023a0: 7407 9b00 6407 7408 9b00 6408 7409 9b00  t...d.t...d.t...
-000023b0: 6406 7407 9b00 6407 740a 9b00 6408 7c00  d.t...d.t...d.|.
-000023c0: 9b00 6406 740b 9b00 6407 740c 9b00 6408  ..d.t...d.t...d.
-000023d0: 7c00 9b00 6406 7c04 9b00 6407 740d 9b00  |...d.|...d.t...
-000023e0: 6405 7c00 9b00 6406 7c03 9b00 6407 740e  d.|...d.|...d.t.
-000023f0: 9b00 6408 740f 9b00 6406 7410 9b00 6407  ..d.t...d.t...d.
-00002400: 7411 9b00 6408 740f 9b00 6406 7407 9b00  t...d.t...d.t...
-00002410: 6407 7412 9b00 6408 7413 9b00 6409 740f  d.t...d.t...d.t.
-00002420: 9b00 6406 7414 9b00 640a 7415 9b00 6406  ..d.t...d.t...d.
-00002430: 7414 9b00 640b 7416 9b00 6405 7417 9b00  t...d.t...d.t...
-00002440: 6409 7418 9b00 6409 740f 9b00 6406 7414  d.t...d.t...d.t.
-00002450: 9b00 640c 7415 9b00 6406 7414 9b00 640d  ..d.t...d.t...d.
-00002460: 7419 9b00 640e 7c00 9b00 640f 7409 9b00  t...d.|...d.t...
-00002470: 6410 7c00 9b00 6406 7c04 9b00 6411 7409  d.|...d.|...d.t.
-00002480: 9b00 6406 7404 9b00 640a 7409 9b00 6406  ..d.t...d.t...d.
-00002490: 7405 9b00 6412 740f 9b00 6410 7409 9b00  t...d.t...d.t...
-000024a0: 6406 7407 9b00 6413 740f 9b00 6406 741a  d.t...d.t...d.t.
-000024b0: 9b00 6414 7415 9b00 6410 7c00 9b00 6406  ..d.t...d.|...d.
-000024c0: 7c04 9b00 6413 7415 9b00 6406 7407 9b00  |...d.t...d.t...
-000024d0: 6415 740d 9b00 640a 7416 9b00 6416 740d  d.t...d.t...d.t.
-000024e0: 9b00 9d72 7d05 7c05 5300 2917 4ee9 0300  ...r}.|.S.).N...
-000024f0: 0000 da05 7374 6172 747a 2d53 454c 4543  ....startz-SELEC
-00002500: 5420 2a0a 2020 2020 4652 4f4d 2028 0a20  T *.    FROM (. 
-00002510: 2020 2020 2020 2053 454c 4543 5420 0a20         SELECT . 
-00002520: 2020 2020 2020 2027 7a05 2720 6173 207a         'z.' as z
-00002530: 0b2c 200a 2020 2020 2020 2020 7215 0000  ., .        r...
-00002540: 0072 1000 0000 7222 0000 0072 1100 0000  .r....r"...r....
-00002550: 7218 0000 0072 1200 0000 7240 0000 00fa  r....r....r@....
-00002560: 0629 2920 6173 207a 0e0a 2020 2020 2020  .)) as z..      
-00002570: 2020 4652 4f4d 207a 140a 2020 2020 2020    FROM z..      
-00002580: 2020 494e 4e45 5220 4a4f 494e 2072 1e00    INNER JOIN r..
-00002590: 0000 725c 0000 007a 1529 0a20 2020 2020  ..r\...z.).     
-000025a0: 2020 2049 4e4e 4552 204a 4f49 4e20 7219     INNER JOIN r.
-000025b0: 0000 0072 1d00 0000 7a12 0a20 2020 2020  ...r....z..     
-000025c0: 2020 2047 524f 5550 2042 5920 7a18 0a20     GROUP BY z.. 
-000025d0: 2020 2020 2020 2029 0a20 2020 2047 524f         ).    GRO
-000025e0: 5550 2042 5920 291b da0d 6375 6c76 6572  UP BY )...culver
-000025f0: 745f 6c61 7965 725a 1469 6e76 6572 745f  t_layerZ.invert_
-00002600: 6c76 6c5f 7374 6172 745f 636f 6c5a 1269  lvl_start_colZ.i
-00002610: 6e76 6572 745f 6c76 6c5f 656e 645f 636f  nvert_lvl_end_co
-00002620: 6c5a 0f63 7265 7374 5f6c 6576 656c 5f63  lZ.crest_level_c
-00002630: 6f6c da16 636f 6e6e 5f6e 6f64 655f 7374  ol..conn_node_st
-00002640: 6172 745f 6964 5f63 6f6c da14 636f 6e6e  art_id_col..conn
-00002650: 5f6e 6f64 655f 656e 645f 6964 5f63 6f6c  _node_end_id_col
-00002660: 5a16 615f 6368 616e 5f62 6564 5f73 7472  Z.a_chan_bed_str
-00002670: 7563 745f 7479 7065 722c 0000 005a 1461  uct_typer,...Z.a
-00002680: 5f63 6861 6e5f 6265 645f 7374 7275 6374  _chan_bed_struct
-00002690: 5f69 6472 6800 0000 5a15 615f 6368 616e  _idrh...Z.a_chan
-000026a0: 5f62 6564 5f63 6861 6e6e 656c 5f69 6472  _bed_channel_idr
-000026b0: 4500 0000 5a16 615f 6368 616e 5f62 6564  E...Z.a_chan_bed
-000026c0: 5f73 7472 7563 745f 636f 6465 5a12 615f  _struct_codeZ.a_
-000026d0: 6368 616e 5f62 6564 5f63 6f6e 6e5f 6964  chan_bed_conn_id
-000026e0: da19 615f 6368 616e 5f62 6564 5f73 7472  ..a_chan_bed_str
-000026f0: 7563 745f 7265 665f 6c76 6c72 6400 0000  uct_ref_lvlrd...
-00002700: 726b 0000 00da 1861 5f63 6861 6e5f 6265  rk.....a_chan_be
-00002710: 645f 6372 6f73 735f 7265 665f 6c76 6c5a  d_cross_ref_lvlZ
-00002720: 1361 5f63 6861 6e5f 6265 645f 6372 6f73  .a_chan_bed_cros
-00002730: 735f 6964 5a0a 665f 6469 7374 616e 6365  s_idZ.f_distance
-00002740: da07 6765 6f5f 636f 6c72 6300 0000 5a1c  ..geo_colrc...Z.
-00002750: 615f 6368 616e 5f62 6564 5f64 6973 745f  a_chan_bed_dist_
-00002760: 6372 6f73 735f 7374 7275 6374 da07 665f  cross_struct..f_
-00002770: 6173 776b 74da 0a66 5f6d 616b 656c 696e  aswkt..f_makelin
-00002780: 65da 0a64 665f 6765 6f5f 636f 6cda 0e63  e..df_geo_col..c
-00002790: 6861 6e6e 656c 5f69 645f 636f 6c29 06da  hannel_id_col)..
-000027a0: 0673 7472 7563 745a 0873 7461 7274 656e  .structZ.starten
-000027b0: 64da 0474 7970 655a 1372 6566 6572 656e  d..typeZ.referen
-000027c0: 6365 5f70 6172 616d 6574 6572 da0c 636f  ce_parameter..co
-000027d0: 6e6e 5f6e 6f64 655f 6964 7226 0000 0072  nn_node_idr&...r
-000027e0: 2700 0000 7227 0000 0072 2800 0000 da23  '...r'...r(....#
-000027f0: 5f5f 636f 6e73 7472 7563 745f 6368 616e  __construct_chan
-00002800: 6e65 6c5f 6265 645f 7175 6572 795f 696e  nel_bed_query_in
-00002810: 6e65 7284 0100 0073 fa00 0000 0002 0c01  ner....s........
-00002820: 0801 0801 0602 0602 0401 0801 0602 0401  ................
-00002830: 0203 02fd 0403 02fd 0404 02fc 0404 02fc  ................
-00002840: 0404 02fc 0405 02fb 0405 02fb 0405 02fb  ................
-00002850: 0406 02fa 0406 02fa 0406 02fa 0407 02f9  ................
-00002860: 0407 02f9 0407 02f9 0408 02f8 0408 02f8  ................
-00002870: 0408 02f8 0409 02f7 0409 02f7 0409 02f7  ................
-00002880: 040a 02f6 040a 02f6 040a 02f6 040b 02f5  ................
-00002890: 040b 02f5 040b 02f5 040b 02f5 040b 02f5  ................
-000028a0: 040b 02f5 040c 02f4 040c 02f4 040c 02f4  ................
-000028b0: 040c 02f4 040c 02f4 040c 02f4 040c 02f4  ................
-000028c0: 040d 02f3 040e 02f2 040f 02f1 040f 02f1  ................
-000028d0: 040f 02f1 040f 02f1 040f 02f1 040f 02f1  ................
-000028e0: 0410 02f0 0411 02ef 0411 02ef 0411 02ef  ................
-000028f0: 0411 02ef 0412 02ee 0413 02ed 0413 02ed  ................
-00002900: 0413 02ed 0413 02ed 0414 02ec 0414 02ec  ................
-00002910: 0416 02ea 0617 727d 0000 0063 0000 0000  ......r}...c....
-00002920: 0000 0000 0000 0000 0100 0000 0d00 0000  ................
-00002930: 4300 0000 7346 0000 0064 0174 0074 0164  C...sF...d.t.t.d
-00002940: 0283 029b 0064 0374 0074 0164 0483 029b  .....d.t.t.d....
-00002950: 0064 0574 0074 0264 0283 029b 0064 0374  .d.t.t.d.....d.t
-00002960: 0074 0264 0483 029b 0064 0674 039b 0064  .t.d.....d.t...d
-00002970: 0774 049b 0064 089d 0d7d 007c 0053 0029  .t...d...}.|.S.)
-00002980: 097a 4c0a 2020 2020 4164 6420 6372 6f73  .zL.    Add cros
-00002990: 7320 7365 6374 696f 6e20 616e 6420 6368  s section and ch
-000029a0: 616e 6e65 6c20 696e 666f 726d 6174 696f  annel informatio
-000029b0: 6e20 746f 2063 6f6e 7472 6f6c 6c65 6420  n to controlled 
-000029c0: 7374 7275 6374 7572 6573 0a20 2020 207a  structures.    z
-000029d0: 1353 454c 4543 5420 2a20 4652 4f4d 2028  .SELECT * FROM (
-000029e0: 2020 2020 726e 0000 007a 0b20 2020 2020      rn...z.     
-000029f0: 554e 494f 4e20 da03 656e 647a 0a20 2020  UNION ..endz.   
-00002a00: 2055 4e49 4f4e 207a 0c29 2020 2020 2057   UNION z.)     W
-00002a10: 4845 5245 207a 0320 3c20 7242 0000 0029  HERE z. < rB...)
-00002a20: 0572 7d00 0000 7270 0000 00da 0d6f 7269  .r}...rp.....ori
-00002a30: 6669 6365 5f6c 6179 6572 7273 0000 0072  fice_layerrs...r
-00002a40: 7400 0000 a901 7226 0000 0072 2700 0000  t.....r&...r'...
-00002a50: 7227 0000 0072 2800 0000 da22 636f 6e73  r'...r(...."cons
-00002a60: 7472 7563 745f 7374 7275 6374 5f63 6861  truct_struct_cha
-00002a70: 6e6e 656c 5f62 6564 5f71 7565 7279 ac01  nnel_bed_query..
-00002a80: 0000 731c 0000 0000 0402 0108 ff04 0208  ..s.............
-00002a90: fe04 0308 fd04 0408 fc04 0502 fb04 0502  ................
-00002aa0: fb08 0672 8100 0000 6302 0000 0000 0000  ...r....c.......
-00002ab0: 0000 0000 0004 0000 000a 0000 0043 0000  .............C..
-00002ac0: 0073 4e00 0000 7a1e 7400 6a01 7c00 7402  .sN...z.t.j.|.t.
-00002ad0: 7403 7404 7405 7406 7c01 6401 8d07 7d02  t.t.t.t.|.d...}.
-00002ae0: 7c02 5700 5300 0400 7407 7948 0100 7d03  |.W.S...t.yH..}.
-00002af0: 0100 7a12 7c03 6400 8202 5700 5900 6400  ..z.|.d...W.Y.d.
-00002b00: 7d03 7e03 6e0a 6400 7d03 7e03 3000 3000  }.~.n.d.}.~.0.0.
-00002b10: 6400 5300 7234 0000 0029 0872 3c00 0000  d.S.r4...).r<...
-00002b20: 723d 0000 00da 1363 726f 7373 5f73 6563  r=.....cross_sec
-00002b30: 5f64 6566 5f6c 6179 6572 da13 615f 7765  _def_layer..a_we
-00002b40: 6972 5f63 726f 7373 5f64 6566 5f69 6472  ir_cross_def_idr
-00002b50: 2c00 0000 7248 0000 0072 0d00 0000 7255  ,...rH...r....rU
-00002b60: 0000 0029 045a 1877 6569 725f 7769 6474  ...).Z.weir_widt
-00002b70: 6873 5f74 6f5f 7570 6461 7465 5f64 6672  hs_to_update_dfr
-00002b80: 3100 0000 7226 0000 0072 5600 0000 7227  1...r&...rV...r'
-00002b90: 0000 0072 2700 0000 7228 0000 00da 2663  ...r'...r(....&c
-00002ba0: 6f6e 7374 7275 6374 5f77 6569 725f 6865  onstruct_weir_he
-00002bb0: 6967 6874 5f75 7064 6174 655f 7374 6174  ight_update_stat
-00002bc0: 656d 656e 74bd 0100 0073 1a00 0000 0001  ement....s......
-00002bd0: 0201 0401 0201 0201 0201 0201 0201 0201  ................
-00002be0: 02f9 0609 0601 0e01 7284 0000 0063 0100  ........r....c..
-00002bf0: 0000 0000 0000 0000 0000 0200 0000 5900  ..............Y.
-00002c00: 0000 4300 0000 7312 0100 0064 0174 009b  ..C...s....d.t..
-00002c10: 0064 0274 019b 0064 0374 029b 0064 0474  .d.t...d.t...d.t
-00002c20: 009b 0064 0274 039b 0064 0474 009b 0064  ...d.t...d.t...d
-00002c30: 0274 049b 0064 0574 009b 0064 0274 059b  .t...d.t...d.t..
-00002c40: 0064 047c 009b 0064 0274 069b 0064 0474  .d.|...d.t...d.t
-00002c50: 079b 0064 0674 089b 0064 0774 099b 0064  ...d.t...d.t...d
-00002c60: 0874 0a9b 0064 0274 099b 0064 0974 0b9b  .t...d.t...d.t..
-00002c70: 0064 0a7c 009b 0064 0b74 009b 0064 0c7c  .d.|...d.t...d.|
-00002c80: 009b 0064 0274 019b 0064 0d74 009b 0064  ...d.t...d.t...d
-00002c90: 0274 059b 0064 0e74 0a9b 0064 0c7c 009b  .t...d.t...d.|..
-00002ca0: 0064 0274 0c9b 0064 0d74 0a9b 0064 0274  .d.t...d.t...d.t
-00002cb0: 019b 0064 0e74 0d9b 0064 0c74 0d9b 0064  ...d.t...d.t...d
-00002cc0: 0274 0e9b 0064 0d74 009b 0064 0274 019b  .t...d.t...d.t..
-00002cd0: 0064 0e74 0f9b 0064 0c74 0f9b 0064 0274  .d.t...d.t...d.t
-00002ce0: 109b 0064 0d74 0d9b 0064 0274 109b 0064  ...d.t...d.t...d
-00002cf0: 0e74 0a9b 0064 0f74 0f9b 0064 0274 119b  .t...d.t...d.t..
-00002d00: 0064 1074 009b 0064 0274 049b 0064 117c  .d.t...d.t...d.|
-00002d10: 009b 0064 129d 597d 017c 0153 0029 134e  ...d..Y}.|.S.).N
-00002d20: 720f 0000 0072 1500 0000 7210 0000 007a  r....r....r....z
-00002d30: 072c 200a 2020 2020 7213 0000 0072 1100  ., .    r....r..
-00002d40: 0000 7a16 2876 325f 636f 6e6e 6563 7469  ..z.(v2_connecti
-00002d50: 6f6e 5f6e 6f64 6573 322e 7240 0000 0072  on_nodes2.r@...r
-00002d60: 6f00 0000 7214 0000 0072 1c00 0000 7217  o...r....r....r.
-00002d70: 0000 0072 1900 0000 7216 0000 007a 2020  ...r....r....z  
-00002d80: 6173 2076 325f 636f 6e6e 6563 7469 6f6e  as v2_connection
-00002d90: 5f6e 6f64 6573 320a 2020 2020 4f4e 207a  _nodes2.    ON z
-00002da0: 2520 3d20 7632 5f63 6f6e 6e65 6374 696f  % = v2_connectio
-00002db0: 6e5f 6e6f 6465 7332 2e69 640a 2020 2020  n_nodes2.id.    
-00002dc0: 5748 4552 4520 7a02 3d27 7220 0000 0029  WHERE z.='r ...)
-00002dd0: 12da 1363 6f6e 7472 6f6c 5f74 6162 6c65  ...control_table
-00002de0: 5f6c 6179 6572 722c 0000 005a 1761 5f63  _layerr,...Z.a_c
-00002df0: 6f6e 7472 5f73 7472 7563 745f 636f 6e74  ontr_struct_cont
-00002e00: 725f 6964 da0a 6163 7469 6f6e 5f63 6f6c  r_id..action_col
-00002e10: da0f 7461 7267 6574 5f74 7970 655f 636f  ..target_type_co
-00002e20: 6cda 0d74 6172 6765 745f 6964 5f63 6f6c  l..target_id_col
-00002e30: 7245 0000 0072 7600 0000 7277 0000 0072  rE...rv...rw...r
-00002e40: 7500 0000 7263 0000 0072 7800 0000 7271  u...rc...rx...rq
-00002e50: 0000 005a 0d63 6f6e 7472 6f6c 5f6c 6179  ...Z.control_lay
-00002e60: 6572 5a0e 636f 6e74 726f 6c5f 6964 5f63  erZ.control_id_c
-00002e70: 6f6c 5a13 636f 6e74 726f 6c5f 6d65 6173  olZ.control_meas
-00002e80: 7572 655f 6d61 705a 146d 6561 7375 7265  ure_mapZ.measure
-00002e90: 5f67 726f 7570 5f69 645f 636f 6c5a 0d6f  _group_id_colZ.o
-00002ea0: 626a 6563 745f 6964 5f63 6f6c 2902 da09  bject_id_col)...
-00002eb0: 7374 7275 6374 7572 6572 2600 0000 7227  structurer&...r'
-00002ec0: 0000 0072 2700 0000 7228 0000 00da 2b63  ...r'...r(....+c
-00002ed0: 6f6e 7374 7275 6374 5f63 6f6e 7472 6f6c  onstruct_control
-00002ee0: 6c65 645f 7374 7275 6374 7572 6573 5f71  led_structures_q
-00002ef0: 7565 7279 5f69 6e6e 6572 ce01 0000 73b4  uery_inner....s.
-00002f00: 0000 0000 0102 0102 ff04 0102 ff04 0102  ................
-00002f10: ff04 0202 fe04 0202 fe04 0302 fd04 0302  ................
-00002f20: fd04 0402 fc04 0402 fc04 0502 fb04 0502  ................
-00002f30: fb04 0602 fa04 0602 fa04 0602 fa04 0602  ................
-00002f40: fa04 0602 fa04 0602 fa04 0702 f904 0802  ................
-00002f50: f804 0902 f704 0902 f704 0902 f704 0902  ................
-00002f60: f704 0a02 f604 0b02 f504 0b02 f504 0b02  ................
-00002f70: f504 0b02 f504 0c02 f404 0d02 f304 0d02  ................
-00002f80: f304 0d02 f304 0d02 f304 0e02 f204 0f02  ................
-00002f90: f104 0f02 f104 0f02 f104 0f02 f104 1002  ................
-00002fa0: f004 1102 ef04 1102 ef04 1202 ee04 1202  ................
-00002fb0: ee04 1202 ee08 1472 8a00 0000 6300 0000  .......r....c...
-00002fc0: 0000 0000 0000 0000 0001 0000 0007 0000  ................
-00002fd0: 0043 0000 0073 2800 0000 6401 7400 7401  .C...s(...d.t.t.
-00002fe0: 8301 9b00 6402 7400 7402 8301 9b00 6402  ....d.t.t.....d.
-00002ff0: 7400 7403 8301 9b00 6403 9d07 7d00 7c00  t.t.....d...}.|.
-00003000: 5300 2904 4e7a 1453 454c 4543 5420 2a20  S.).Nz.SELECT * 
-00003010: 4652 4f4d 2028 0a20 2020 207a 0b0a 2020  FROM (.    z..  
-00003020: 2020 554e 494f 4e20 7241 0000 0029 0472    UNION rA...).r
-00003030: 8a00 0000 da0a 7765 6972 5f6c 6179 6572  ......weir_layer
-00003040: 7270 0000 0072 7f00 0000 7280 0000 0072  rp...r....r....r
-00003050: 2700 0000 7227 0000 0072 2800 0000 da25  '...r'...r(....%
-00003060: 636f 6e73 7472 7563 745f 636f 6e74 726f  construct_contro
-00003070: 6c6c 6564 5f73 7472 7563 7475 7265 735f  lled_structures_
-00003080: 7175 6572 79e6 0100 0073 1000 0000 0001  query....s......
-00003090: 0201 06ff 0402 06fe 0403 06fd 0804 728c  ..............r.
-000030a0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000030b0: 0500 0000 0700 0000 4300 0000 7330 0000  ........C...s0..
-000030c0: 0067 007d 027c 0044 005d 187d 037c 02a0  .g.}.|.D.].}.|..
-000030d0: 0074 016a 027c 037c 0164 018d 02a1 0101  .t.j.|.|.d......
-000030e0: 0071 0864 02a0 037c 02a1 017d 047c 0453  .q.d...|...}.|.S
-000030f0: 0029 034e 2902 da05 7461 626c 65da 0a70  .).N)...table..p
-00003100: 726f 6a65 6374 696f 6e7a 0b0a 554e 494f  rojectionz..UNIO
-00003110: 4e20 414c 4c0a 2904 7230 0000 00da 1967  N ALL.).r0.....g
-00003120: 656f 6d65 7472 795f 6368 6563 6b5f 7175  eometry_check_qu
-00003130: 6572 795f 6261 7365 7224 0000 0072 2d00  ery_baser$...r-.
-00003140: 0000 2905 da0b 7461 626c 655f 6e61 6d65  ..)...table_name
-00003150: 735a 0764 7374 5f63 7273 5a0b 7175 6572  sZ.dst_crsZ.quer
-00003160: 6965 735f 6c73 7472 8d00 0000 7226 0000  ies_lstr....r&..
-00003170: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
-00003180: da18 636f 6e73 7472 7563 745f 6765 6f6d  ..construct_geom
-00003190: 6574 7279 5f71 7565 7279 f101 0000 730a  etry_query....s.
-000031a0: 0000 0000 0104 0108 0116 010a 0172 9100  .............r..
-000031b0: 0000 2901 7290 0000 0029 7ada 075f 5f64  ..).r....)z..__d
-000031c0: 6f63 5f5f da13 6868 6e6b 5f72 6573 6561  oc__..hhnk_resea
-000031d0: 7263 685f 746f 6f6c 7372 3c00 0000 da05  rch_toolsr<.....
-000031e0: 6e75 6d70 7972 5d00 0000 5a30 6868 6e6b  numpyr]...Z0hhnk
-000031f0: 5f74 6872 6565 6469 5f74 6f6f 6c73 2e76  _threedi_tools.v
-00003200: 6172 6961 626c 6573 2e62 6163 6b75 7073  ariables.backups
-00003210: 5f74 6162 6c65 5f6e 616d 6573 7202 0000  _table_namesr...
-00003220: 0072 0300 0000 7204 0000 00da 2868 686e  .r....r.....(hhn
-00003230: 6b5f 7468 7265 6564 695f 746f 6f6c 732e  k_threedi_tools.
-00003240: 7661 7269 6162 6c65 732e 6261 6e6b 5f6c  variables.bank_l
-00003250: 6576 656c 7372 0500 0000 da2d 6868 6e6b  evelsr.....-hhnk
+000006d0: 6537 9b00 6444 651d 9b00 6445 651e 9b00  e7..dDe...dEe...
+000006e0: 640f 651f 9b00 6444 651d 9b00 640e 655d  d.e...dDe...d.e]
+000006f0: 9b00 6445 651e 9b00 6446 655e 9b00 6444  ..dEe...dFe^..dD
+00000700: 651d 9b00 640e 655d 9b00 6445 651e 9b00  e...d.e]..dEe...
+00000710: 641a 655f 9b00 6445 651e 9b00 6447 6560  d.e_..dEe...dGe`
+00000720: 9b00 6444 651d 9b00 6448 651e 9b00 640f  ..dDe...dHe...d.
+00000730: 6561 9b00 6444 651d 9b00 6449 651e 9b00  ea..dDe...dIe...
+00000740: 640f 6562 9b00 644a 6520 9b00 640c 6563  d.eb..dJe ..d.ec
+00000750: 9b00 644b 6519 9b00 644c 6537 9b00 644d  ..dKe...dLe7..dM
+00000760: 6520 9b00 640c 6564 9b00 644e 6519 9b00  e ..d.ed..dNe...
+00000770: 644c 652e 9b00 644f 6561 9b00 6450 655e  dLe...dOea..dPe^
+00000780: 9b00 6451 6562 9b00 6450 6560 9b00 6411  ..dQeb..dPe`..d.
+00000790: 9d45 5a65 6452 6453 8400 5a66 6700 6700  .EZedRdS..Zfg.g.
+000007a0: 6700 6603 6454 6455 8401 5a67 6700 6601  g.f.dTdU..Zgg.f.
+000007b0: 6456 6457 8401 5a68 6458 6459 8400 5a69  dVdW..ZhdXdY..Zi
+000007c0: 6700 6601 645a 645b 8401 5a6a 645c 645d  g.f.dZd[..Zjd\d]
+000007d0: 8400 5a6b 645e 645f 8400 5a6c 6700 6601  ..Zkd^d_..Zlg.f.
+000007e0: 6460 6461 8401 5a6d 6700 6601 6462 6463  d`da..Zmg.f.dbdc
+000007f0: 8401 5a6e 6464 6465 8400 5a6f 6466 6467  ..Znddde..Zodfdg
+00000800: 8400 5a70 6570 8300 5a71 6700 6601 6468  ..Zpep..Zqg.f.dh
+00000810: 6469 8401 5a72 646a 646b 8400 5a73 646c  di..Zrdjdk..Zsdl
+00000820: 646d 8400 5a74 6574 8300 5a75 650e 6601  dm..Ztet..Zue.f.
+00000830: 646e 646f 8401 5a76 6576 652b 6577 6702  dndo..Zveve+ewg.
+00000840: 6470 8d01 5a78 6402 5300 2971 7a91 0a43  dp..Zxd.S.)qz..C
+00000850: 7265 6174 6564 206f 6e20 4d6f 6e20 4175  reated on Mon Au
+00000860: 6720 3136 2031 323a 3034 3a33 3320 3230  g 16 12:04:33 20
+00000870: 3231 0a0a 4061 7574 686f 723a 2063 6872  21..@author: chr
+00000880: 6973 2e6b 6572 6b6c 6161 6e0a 0a41 6c6c  is.kerklaan..All
+00000890: 2073 716c 6974 6520 7175 6572 6965 7320   sqlite queries 
+000008a0: 6172 6520 7374 6f72 6564 2077 6974 6869  are stored withi
+000008b0: 6e20 7468 6973 2073 6372 6970 742e 2051  n this script. Q
+000008c0: 7565 7269 6573 2061 7265 206c 6973 7465  ueries are liste
+000008d0: 6420 7065 7220 7461 626c 652e 0a0a 0ae9  d per table.....
+000008e0: 0000 0000 4e29 03da 1342 414e 4b5f 4c56  ....N)...BANK_LV
+000008f0: 4c53 5f4c 4153 545f 4341 4c43 da17 434f  LS_LAST_CALC..CO
+00000900: 4e54 525f 5745 4952 5f57 4944 5448 5f42  NTR_WEIR_WIDTH_B
+00000910: 4143 4b55 50da 1547 4c4f 4241 4c5f 5345  ACKUP..GLOBAL_SE
+00000920: 5454 494e 4753 5f54 4142 4c45 2901 da12  TTINGS_TABLE)...
+00000930: 6e65 775f 6261 6e6b 5f6c 6576 656c 5f63  new_bank_level_c
+00000940: 6f6c 2901 da01 2a29 01da 0c44 4546 5f54  ol)...*)...DEF_T
+00000950: 5247 545f 4352 5329 06da 1663 6861 6e6e  RGT_CRS)...chann
+00000960: 656c 735f 6e65 775f 6361 6c63 5f74 7970  els_new_calc_typ
+00000970: 65da 1c67 6c6f 6261 6c5f 7365 7474 696e  e..global_settin
+00000980: 6773 5f6e 6577 5f63 6f6c 5f6e 616d 65da  gs_new_col_name.
+00000990: 1468 7964 7261 756c 6963 5f74 6573 745f  .hydraulic_test_
+000009a0: 7374 6174 65da 166d 616e 686f 6c65 735f  state..manholes_
+000009b0: 6e65 775f 6361 6c63 5f74 7970 65da 116f  new_calc_type..o
+000009c0: 6e65 5f64 5f74 776f 5f64 5f73 7461 7465  ne_d_two_d_state
+000009d0: da13 7765 6972 735f 6e65 775f 7769 6474  ..weirs_new_widt
+000009e0: 685f 636f 6c29 01da 0b6e 6577 5f72 6566  h_col)...new_ref
+000009f0: 5f6c 766c 7a13 0a20 2020 2053 454c 4543  _lvlz..    SELEC
+00000a00: 5420 2a20 4652 4f4d 207a 120a 2020 2020  T * FROM z..    
+00000a10: 5748 4552 4520 7b7d 0a20 2020 20fa 0c0a  WHERE {}.    ...
+00000a20: 2020 2020 5345 4c45 4354 20fa 0420 6173      SELECT .. as
+00000a30: 207a 062c 2020 2020 20fa 0128 fa05 2920   z.,     ..(..) 
+00000a40: 6173 207a 0a20 2020 2020 4652 4f4d 207a  as z.     FROM z
+00000a50: 050a 2020 2020 fa06 2c0a 2020 2020 fa0a  ..    ..,.    ..
+00000a60: 0a20 2020 2046 524f 4d20 7a10 0a20 2020  .    FROM z..   
+00000a70: 2053 454c 4543 540a 2020 2020 da01 2efa   SELECT.    ....
+00000a80: 0f0a 2020 2020 4c45 4654 204a 4f49 4e20  ..    LEFT JOIN 
+00000a90: fa08 0a20 2020 204f 4e20 7a04 203d 3d20  ...    ON z. == 
+00000aa0: 7a10 0a20 2020 2053 454c 4543 5420 2020  z..    SELECT   
+00000ab0: 2020 fa02 2c20 fa03 203d 207a 210a 2020    .., .. = z!.  
+00000ac0: 2020 2020 2020 2020 2020 5345 4c45 4354            SELECT
+00000ad0: 200a 2020 2020 2020 2020 2020 2020 7a04   .            z.
+00000ae0: 2041 5320 7a0e 2c0a 2020 2020 2020 2020   AS z.,.        
+00000af0: 2020 2020 7a12 0a20 2020 2020 2020 2020      z..         
+00000b00: 2020 2046 524f 4d20 7a17 0a20 2020 2020     FROM z..     
+00000b10: 2020 2020 2020 204c 4546 5420 4a4f 494e         LEFT JOIN
+00000b20: 207a 0420 4f4e 207a 160a 2020 2020 2020   z. ON z..      
+00000b30: 2020 2020 2020 4752 4f55 5020 4259 207a        GROUP BY z
+00000b40: 0d0a 2020 2020 2020 2020 2020 2020 7a0d  ..            z.
+00000b50: 6372 6561 7465 2074 6162 6c65 207a 2128  create table z!(
+00000b60: 6964 2069 6e74 2050 5249 4d41 5259 204b  id int PRIMARY K
+00000b70: 4559 2c20 6474 2064 6174 6574 696d 6529  EY, dt datetime)
+00000b80: 7a17 494e 5345 5254 204f 5220 5245 504c  z.INSERT OR REPL
+00000b90: 4143 4520 494e 544f 207a 1d0a 5641 4c55  ACE INTO z..VALU
+00000ba0: 4553 2831 2c20 6375 7272 656e 745f 7469  ES(1, current_ti
+00000bb0: 6d65 7374 616d 7029 7a2c 5345 4c45 4354  mestamp)z,SELECT
+00000bc0: 2064 6174 6574 696d 6528 6474 2c20 276c   datetime(dt, 'l
+00000bd0: 6f63 616c 7469 6d65 2729 2041 5320 6474  ocaltime') AS dt
+00000be0: 2046 524f 4d20 7a08 206c 696d 6974 2031   FROM z. limit 1
+00000bf0: 7a08 0a53 454c 4543 5420 fa02 2c0a 7a06  z..SELECT ..,.z.
+00000c00: 0a46 524f 4d20 da01 0a7a 130a 2020 2020  .FROM ...z..    
+00000c10: 5345 4c45 4354 202a 2066 726f 6d20 7a07  SELECT * from z.
+00000c20: 2057 4845 5245 207a 1520 696e 2028 0a20   WHERE z. in (. 
+00000c30: 2020 2053 454c 4543 540a 2020 2020 fa10     SELECT.    ..
+00000c40: 0a20 2020 2049 4e4e 4552 204a 4f49 4e20  .    INNER JOIN 
+00000c50: 7a0b 0a20 2020 2029 0a20 2020 207a 0e0a  z..    ).    z..
+00000c60: 2020 2020 5345 4c45 4354 2077 2e7a 082c      SELECT w.z.,
+00000c70: 0a20 2020 2077 2e7a 1920 6173 2077 0a20  .    w.z. as w. 
+00000c80: 2020 2020 2020 2049 4e4e 4552 204a 4f49         INNER JOI
+00000c90: 4e20 7a0e 0a20 2020 2020 2020 204f 4e20  N z..        ON 
+00000ca0: 772e fa13 0a20 2020 2020 2020 204c 4546  w....        LEF
+00000cb0: 5420 4a4f 494e 207a 0f0a 2020 2020 2020  T JOIN z..      
+00000cc0: 2020 4f4e 2028 772e 7a05 2069 6e20 287a    ON (w.z. in (z
+00000cd0: 0f29 0a20 2020 2020 2020 204f 5220 772e  .).        OR w.
+00000ce0: 7a0f 2929 0a20 2020 2020 2020 2041 4e44  z.)).        AND
+00000cf0: 20fa 0c0a 2020 2020 2020 2020 4f4e 20fa   ...        ON .
+00000d00: 0b0a 2020 2020 5748 4552 4520 7a04 203d  ..    WHERE z. =
+00000d10: 2027 fa06 270a 2020 2020 fa02 3b0a 7a2f   '..'.    ..;.z/
+00000d20: 2020 2020 5345 4c45 4354 202a 0a20 2020      SELECT *.   
+00000d30: 2046 524f 4d20 280a 2020 2020 2020 2020   FROM (.        
+00000d40: 5345 4c45 4354 207b 7461 626c 657d 2e7a  SELECT {table}.z
+00000d50: 332c 0a20 2020 2020 2020 2027 7b74 6162  3,.        '{tab
+00000d60: 6c65 7d27 2061 7320 7461 626c 655f 6e61  le}' as table_na
+00000d70: 6d65 2c0a 2020 2020 2020 2020 7b74 6162  me,.        {tab
+00000d80: 6c65 7d2e 7a12 2c0a 2020 2020 2020 2020  le}.z.,.        
+00000d90: 7b74 6162 6c65 7d2e fa0a 2c0a 2020 2020  {table}...,.    
+00000da0: 2020 2020 7a09 287b 7461 626c 657d 2e7a      z.({table}.z
+00000db0: 092c 2031 2929 2061 7320 7a07 2929 2920  ., 1)) as z.))) 
+00000dc0: 6173 207a 1828 636f 6e6e 6563 7469 6f6e  as z.(connection
+00000dd0: 5f6e 6f64 6573 5f73 7461 7274 2e7a 1628  _nodes_start.z.(
+00000de0: 636f 6e6e 6563 7469 6f6e 5f6e 6f64 6573  connection_nodes
+00000df0: 5f65 6e64 2e7a 380a 2020 2020 2020 2020  _end.z8.        
+00000e00: 4652 4f4d 0a20 2020 2020 2020 207b 7461  FROM.        {ta
+00000e10: 626c 657d 0a20 2020 2020 2020 204c 4546  ble}.        LEF
+00000e20: 5420 4a4f 494e 0a20 2020 2020 2020 207a  T JOIN.        z
+00000e30: 290a 2020 2020 2020 2020 4f4e 0a20 2020  ).        ON.   
+00000e40: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
+00000e50: 6e6f 6465 735f 656e 642e 7a0c 2049 5320  nodes_end.z. IS 
+00000e60: 7b74 6162 6c65 7d2e 7a1b 0a20 2020 2020  {table}.z..     
+00000e70: 2020 204c 4546 5420 4a4f 494e 0a20 2020     LEFT JOIN.   
+00000e80: 2020 2020 207a 2b0a 2020 2020 2020 2020       z+.        
+00000e90: 4f4e 0a20 2020 2020 2020 2063 6f6e 6e65  ON.        conne
+00000ea0: 6374 696f 6e5f 6e6f 6465 735f 7374 6172  ction_nodes_star
+00000eb0: 742e 7a11 0a20 2020 2029 0a20 2020 2057  t.z..    ).    W
+00000ec0: 4845 5245 207a 0820 4953 204e 4f54 207a  HERE z. IS NOT z
+00000ed0: 0420 4f52 2063 0100 0000 0000 0000 0000  . OR c..........
+00000ee0: 0000 0300 0000 0400 0000 4300 0000 7344  ..........C...sD
+00000ef0: 0000 0074 009b 0064 0174 019b 0064 029d  ...t...d.t...d..
+00000f00: 047d 017c 0074 026b 0272 247c 01a0 0364  .}.|.t.k.r$|...d
+00000f10: 03a1 017d 016e 127c 0074 046b 0272 367c  ...}.n.|.t.k.r6|
+00000f20: 01a0 0364 04a1 017d 0174 05a0 037c 01a1  ...d...}.t...|..
+00000f30: 017d 027c 0253 0029 054e 7a05 207b 7d20  .}.|.S.).Nz. {} 
+00000f40: 27fa 0127 7a02 3d3d 7a02 213d 2906 5a08  '..'z.==z.!=).Z.
+00000f50: 6e61 6d65 5f63 6f6c 5a10 7a65 726f 5f64  name_colZ.zero_d
+00000f60: 5f6f 6e65 5f64 5f76 616c 720a 0000 00da  _one_d_valr.....
+00000f70: 0666 6f72 6d61 7472 0c00 0000 da13 616c  .formatr......al
+00000f80: 6c5f 676c 6f62 616c 5f73 6574 7469 6e67  l_global_setting
+00000f90: 7329 035a 0874 6f5f 7374 6174 655a 0c77  s).Z.to_stateZ.w
+00000fa0: 6865 7265 5f63 6c61 7573 65da 0571 7565  here_clause..que
+00000fb0: 7279 a900 7227 0000 00fa 4b65 3a5c 6769  ry..r'....Ke:\gi
+00000fc0: 7468 7562 5c77 7661 6e67 6572 7765 6e5c  thub\wvangerwen\
+00000fd0: 6868 6e6b 2d74 6872 6565 6469 2d74 6f6f  hhnk-threedi-too
+00000fe0: 6c73 5c68 686e 6b5f 7468 7265 6564 695f  ls\hhnk_threedi_
+00000ff0: 746f 6f6c 735c 7574 696c 735c 7175 6572  tools\utils\quer
+00001000: 6965 732e 7079 da28 6372 6561 7465 5f67  ies.py.(create_g
+00001010: 6c6f 6261 6c5f 7365 7474 696e 6773 5f66  lobal_settings_f
+00001020: 726f 6d5f 6261 636b 7570 5f71 7565 7279  rom_backup_query
+00001030: dd00 0000 730e 0000 0000 0110 0108 010c  ....s...........
+00001040: 0108 010a 010a 0172 2900 0000 6303 0000  .......r)...c...
+00001050: 0000 0000 0000 0000 0007 0000 000e 0000  ................
+00001060: 0043 0000 0073 ac00 0000 6401 7400 9b00  .C...s....d.t...
+00001070: 6402 7401 9b00 6403 7402 9b00 6404 7402  d.t...d.t...d.t.
+00001080: 9b00 6405 6406 a003 7404 7405 7c00 8302  ..d.d...t.t.|...
+00001090: a101 9b00 6407 9d0b 7d03 6408 7400 9b00  ....d...}.d.t...
+000010a0: 6403 7402 9b00 6409 7402 9b00 6405 6406  d.t...d.t...d.d.
+000010b0: a003 7404 7405 7c00 8302 a101 9b00 6407  ..t.t.|.......d.
+000010c0: 9d09 7d04 6700 7d05 7c01 727e 7c05 a006  ..}.g.}.|.r~|...
+000010d0: 7c03 a007 6406 a003 7404 7405 7c01 8302  |...d...t.t.|...
+000010e0: a101 a101 a101 0100 7c02 729e 7c05 a006  ........|.r.|...
+000010f0: 7c04 a007 6406 a003 7404 7405 7c02 8302  |...d...t.t.|...
+00001100: a101 a101 a101 0100 640a a003 7c05 a101  ........d...|...
+00001110: 7d06 7c06 5300 290b 7a74 0a20 2020 2041  }.|.S.).zt.    A
+00001120: 6464 2072 6f77 7320 6672 6f6d 2062 6163  dd rows from bac
+00001130: 6b75 702c 2064 656c 6574 6520 726f 7773  kup, delete rows
+00001140: 2066 726f 6d20 6d6f 6465 6c0a 2020 2020   from model.    
+00001150: 4f6e 6365 2074 6865 2063 6f72 7265 6374  Once the correct
+00001160: 2072 6f77 7320 6172 6520 696e 2074 6865   rows are in the
+00001170: 206d 6f64 656c 2c20 7365 7420 6d6f 6465   model, set mode
+00001180: 6c20 636f 6e74 726f 6c0a 2020 2020 7a11  l control.    z.
+00001190: 0a20 2020 2049 4e53 4552 5420 494e 544f  .    INSERT INTO
+000011a0: 207a 170a 2020 2020 5345 4c45 4354 202a   z..    SELECT *
+000011b0: 0a20 2020 2046 524f 4d20 721f 0000 007a  .    FROM r....z
+000011c0: 1120 696e 2028 7b7d 290a 2020 2020 414e  . in ({}).    AN
+000011d0: 4420 7a09 204e 4f54 2049 4e20 2872 1800  D z. NOT IN (r..
+000011e0: 0000 fa06 290a 2020 2020 7a11 0a20 2020  ....).    z..   
+000011f0: 2044 454c 4554 4520 4652 4f4d 207a 1120   DELETE FROM z. 
+00001200: 494e 2028 7b7d 290a 2020 2020 414e 4420  IN ({}).    AND 
+00001210: 7221 0000 0029 08da 1567 6c6f 6261 6c5f  r!...)...global_
+00001220: 7365 7474 696e 6773 5f6c 6179 6572 7204  settings_layerr.
+00001230: 0000 00da 0669 645f 636f 6cda 046a 6f69  .....id_col..joi
+00001240: 6eda 036d 6170 da03 7374 72da 0661 7070  n..map..str..app
+00001250: 656e 6472 2400 0000 2907 da0c 6578 636c  endr$...)...excl
+00001260: 7564 6564 5f69 6473 5a0a 6964 735f 746f  uded_idsZ.ids_to
+00001270: 5f61 6464 5a0d 6964 735f 746f 5f64 656c  _addZ.ids_to_del
+00001280: 6574 655a 0e61 6464 5f72 6f77 735f 7175  eteZ.add_rows_qu
+00001290: 6572 795a 1164 656c 6574 655f 726f 7773  eryZ.delete_rows
+000012a0: 5f71 7565 7279 da0a 7175 6572 795f 6c69  _query..query_li
+000012b0: 7374 7226 0000 0072 2700 0000 7227 0000  str&...r'...r'..
+000012c0: 0072 2800 0000 da28 6372 6561 7465 5f67  .r(....(create_g
+000012d0: 6c6f 6261 6c5f 7365 7474 696e 6773 5f72  lobal_settings_r
+000012e0: 6f77 735f 7570 6461 7465 5f71 7565 7279  ows_update_query
+000012f0: e700 0000 7336 0000 0000 0502 0102 ff04  ....s6..........
+00001300: 0302 fd04 0402 fc04 0502 fb04 050e fb08  ................
+00001310: 0802 0102 ff04 0202 fe04 0302 fd04 030e  ................
+00001320: fd08 0504 0104 011c 0104 011c 010a 0172  ...............r
+00001330: 3300 0000 6302 0000 0000 0000 0000 0000  3...c...........
+00001340: 0003 0000 0009 0000 0043 0000 0073 1c00  .........C...s..
+00001350: 0000 7400 6a01 7c00 7402 7403 7403 7404  ..t.j.|.t.t.t.t.
+00001360: 7405 7c01 6401 8d07 7d02 7c02 5300 a902  t.|.d...}.|.S...
+00001370: 4ea9 07da 0264 66da 056c 6179 6572 da09  N....df..layer..
+00001380: 6466 5f69 645f 636f 6cda 0964 625f 6964  df_id_col..db_id
+00001390: 5f63 6f6c da0b 6f6c 645f 7661 6c5f 636f  _col..old_val_co
+000013a0: 6cda 0b6e 6577 5f76 616c 5f63 6f6c 7231  l..new_val_colr1
+000013b0: 0000 0029 06da 0368 7274 da20 7371 6c5f  ...)...hrt. sql_
+000013c0: 6372 6561 7465 5f75 7064 6174 655f 6361  create_update_ca
+000013d0: 7365 5f73 7461 7465 6d65 6e74 722b 0000  se_statementr+..
+000013e0: 0072 2c00 0000 5a11 636f 6e74 726f 6c5f  .r,...Z.control_
+000013f0: 6772 6f75 705f 636f 6c72 0900 0000 2903  group_colr....).
+00001400: 5a1c 676c 6f62 616c 5f73 6574 7469 6e67  Z.global_setting
+00001410: 735f 746f 5f75 7064 6174 655f 6466 7231  s_to_update_dfr1
+00001420: 0000 0072 2600 0000 7227 0000 0072 2700  ...r&...r'...r'.
+00001430: 0000 7228 0000 00da 2d63 6f6e 7374 7275  ..r(....-constru
+00001440: 6374 5f67 6c6f 6261 6c5f 7365 7474 696e  ct_global_settin
+00001450: 6773 5f63 6f6e 7472 6f6c 5f67 726f 7570  gs_control_group
+00001460: 5f71 7565 7279 0201 0000 7314 0000 0000  _query....s.....
+00001470: 0104 0102 0102 0102 0102 0102 0102 0102  ................
+00001480: f906 0972 3e00 0000 6302 0000 0000 0000  ...r>...c.......
+00001490: 0000 0000 0006 0000 001a 0000 0043 0000  .............C..
+000014a0: 0073 2c01 0000 6401 7d02 7c02 6402 7400  .s,...d.}.|.d.t.
+000014b0: 9b00 6403 7401 9b00 6404 7402 9b00 6404  ..d.t...d.t...d.
+000014c0: 7403 9b00 6404 7404 9b00 6405 7405 9b00  t...d.t...d.t...
+000014d0: 6404 7406 9b00 6404 7407 9b00 6404 7408  d.t...d.t...d.t.
+000014e0: 9b00 6404 7409 9b00 6404 740a 9b00 6404  ..d.t...d.t...d.
+000014f0: 740b 9b00 6406 9d19 3700 7d02 7c02 6407  t...d...7.}.|.d.
+00001500: 3700 7d02 6700 7d03 7c00 a00c a100 4400  7.}.g.}.|.....D.
+00001510: 5d8e 5c02 7d04 7d05 7c05 7403 1900 7c01  ].\.}.}.|.t...|.
+00001520: 7601 726a 7c03 a00d 6408 7c05 7401 1900  v.rj|...d.|.t...
+00001530: 9b00 6409 7c05 7402 1900 9b00 640a 7c05  ..d.|.t.....d.|.
+00001540: 7403 1900 9b00 640b 7c05 7404 1900 9b00  t.....d.|.t.....
+00001550: 640a 7c05 7405 1900 9b00 6404 7c05 7406  d.|.t.....d.|.t.
+00001560: 1900 9b00 6404 7c05 7407 1900 9b00 6404  ....d.|.t.....d.
+00001570: 7c05 7408 1900 9b00 6404 7c05 7409 1900  |.t.....d.|.t...
+00001580: 9b00 6404 7c05 740a 1900 9b00 6404 7c05  ..d.|.t.....d.|.
+00001590: 740b 1900 9b00 640c 9d17 a101 0100 716a  t.....d.......qj
+000015a0: 7c03 9001 7304 640d 5300 7c02 640e a00e  |...s.d.S.|.d...
+000015b0: 7c03 a101 640f 1700 3700 7d02 7c02 740f  |...d...7.}.|.t.
+000015c0: 7c00 7c01 8302 3700 7d02 7c02 5300 640d  |.|...7.}.|.S.d.
+000015d0: 5300 2910 6173 0100 004d 6161 6b20 7371  S.).as...Maak sq
+000015e0: 6c20 7374 6174 656d 656e 7420 6461 7420  l statement dat 
+000015f0: 6765 6272 7569 6b74 2077 6f72 6474 206f  gebruikt wordt o
+00001600: 6d20 6d61 6e68 6f6c 6573 2074 6520 6d61  m manholes te ma
+00001610: 6b65 6e20 6f70 2064 6520 626f 7665 6e20  ken op de boven 
+00001620: 656e 2062 656e 656e 6465 6e73 7472 6f6f  en benendenstroo
+00001630: 6d73 6520 636f 6e6e 6563 7469 6f6e 206e  mse connection n
+00001640: 6f64 6573 0a20 2020 2076 616e 206b 756e  odes.    van kun
+00001650: 7374 7765 726b 656e 206f 7020 7065 696c  stwerken op peil
+00001660: 6772 656e 732e 204f 6d64 6174 2064 657a  grens. Omdat dez
+00001670: 6520 6d61 6e68 6f6c 6573 2069 736f 6c61  e manholes isola
+00001680: 7465 6420 7a69 6a6e 2069 7320 6572 2067  ted zijn is er g
+00001690: 6565 6e20 7374 726f 6d69 6e67 206d 6565  een stroming mee
+000016a0: 7220 6f76 6572 2064 6520 7065 696c 6772  r over de peilgr
+000016b0: 656e 7320 6e6f 6469 672e 0a20 2020 204f  ens nodig..    O
+000016c0: 6f6b 2077 6f72 6474 2065 656e 2073 746f  ok wordt een sto
+000016d0: 7261 6765 2061 7265 6120 746f 6567 6576  rage area toegev
+000016e0: 6f65 6764 2061 616e 2064 6520 636f 6e6e  oegd aan de conn
+000016f0: 6563 7469 6f6e 206e 6f64 6573 2077 6161  ection nodes waa
+00001700: 7220 6d61 6e68 6f6c 6573 2061 616e 2077  r manholes aan w
+00001710: 6f72 6465 6e20 746f 6567 6576 6f65 6764  orden toegevoegd
+00001720: 2061 6c73 2064 6965 206e 6f67 0a20 2020   als die nog.   
+00001730: 206e 6965 7420 6765 7370 6563 6966 6963   niet gespecific
+00001740: 6565 7264 2069 730a 2020 2020 da00 7a0c  eerd is.    ..z.
+00001750: 494e 5345 5254 2049 4e54 4f20 7a02 2028  INSERT INTO z. (
+00001760: 7218 0000 00fa 012c 7a02 290a 7a07 5641  r......,z.).z.VA
+00001770: 4c55 4553 207a 0228 277a 0427 2c20 277a  LUES z.('z.', 'z
+00001780: 0327 2c20 7a03 2c20 27fa 0129 4e72 1a00  .', z., '..)Nr..
+00001790: 0000 fa01 3b29 10da 0d6d 616e 686f 6c65  ....;)...manhole
+000017a0: 5f6c 6179 6572 da10 6469 7370 6c61 795f  _layer..display_
+000017b0: 6e61 6d65 5f63 6f6c da08 636f 6465 5f63  name_col..code_c
+000017c0: 6f6c da10 636f 6e6e 5f6e 6f64 655f 6964  ol..conn_node_id
+000017d0: 5f63 6f6c da09 7368 6170 655f 636f 6cda  _col..shape_col.
+000017e0: 0977 6964 7468 5f63 6f6c da15 6d61 6e68  .width_col..manh
+000017f0: 6f6c 655f 696e 6469 6361 746f 725f 636f  ole_indicator_co
+00001800: 6cda 1463 616c 6375 6c61 7469 6f6e 5f74  l..calculation_t
+00001810: 7970 655f 636f 6cda 0f64 7261 696e 5f6c  ype_col..drain_l
+00001820: 6576 656c 5f63 6f6c da0e 626f 7474 6f6d  evel_col..bottom
+00001830: 5f6c 766c 5f63 6f6c da0f 7375 7266 6163  _lvl_col..surfac
+00001840: 655f 6c76 6c5f 636f 6cda 0c7a 6f6f 6d5f  e_lvl_col..zoom_
+00001850: 6361 745f 636f 6cda 0869 7465 7272 6f77  cat_col..iterrow
+00001860: 7372 3000 0000 722d 0000 00da 1e63 7265  sr0...r-.....cre
+00001870: 6174 655f 7570 6461 7465 5f73 746f 7261  ate_update_stora
+00001880: 6765 5f61 7265 615f 7371 6c29 06da 0f6e  ge_area_sql)...n
+00001890: 6577 5f6d 616e 686f 6c65 735f 6466 7231  ew_manholes_dfr1
+000018a0: 0000 0072 2600 0000 5a08 7371 6c5f 626f  ...r&...Z.sql_bo
+000018b0: 6479 da05 696e 6465 78da 0372 6f77 7227  dy..index..rowr'
+000018c0: 0000 0072 2700 0000 7228 0000 00da 1963  ...r'...r(.....c
+000018d0: 7265 6174 655f 6e65 775f 6d61 6e68 6f6c  reate_new_manhol
+000018e0: 6573 5f71 7565 7279 1001 0000 7368 0000  es_query....sh..
+000018f0: 0000 0604 0102 0108 0102 ff04 0102 ff04  ................
+00001900: 0102 ff04 0102 ff04 0202 fe04 0202 fe04  ................
+00001910: 0202 fe04 0202 fe04 0302 fd04 0302 fd04  ................
+00001920: 0302 fd06 ff04 0608 0104 0110 010c 0104  ................
+00001930: 012a 0106 ff04 0106 ff04 0106 ff04 0106  .*..............
+00001940: ff04 0206 fe04 0206 fe04 0206 fe06 ff06  ................
+00001950: 0506 0104 0212 010e 0172 5400 0000 6302  .........rT...c.
+00001960: 0000 0000 0000 0000 0000 0004 0000 000a  ................
+00001970: 0000 0043 0000 0073 4e00 0000 7a1e 7400  ...C...sN...z.t.
+00001980: 6a01 7c00 7402 7403 7403 7404 7405 7c01  j.|.t.t.t.t.t.|.
+00001990: 6401 8d07 7d02 7c02 5700 5300 0400 7406  d...}.|.W.S...t.
+000019a0: 7948 0100 7d03 0100 7a12 7c03 6400 8202  yH..}...z.|.d...
+000019b0: 5700 5900 6400 7d03 7e03 6e0a 6400 7d03  W.Y.d.}.~.n.d.}.
+000019c0: 7e03 3000 3000 6400 5300 7234 0000 0029  ~.0.0.d.S.r4...)
+000019d0: 0772 3c00 0000 723d 0000 0072 4300 0000  .r<...r=...rC...
+000019e0: 722c 0000 0072 4a00 0000 720b 0000 00da  r,...rJ...r.....
+000019f0: 0945 7863 6570 7469 6f6e 2904 5a15 6d61  .Exception).Z.ma
+00001a00: 6e68 6f6c 6573 5f74 6f5f 7570 6461 7465  nholes_to_update
+00001a10: 5f64 6672 3100 0000 7226 0000 00da 0165  _dfr1...r&.....e
+00001a20: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
+00001a30: 1f63 6f6e 7374 7275 6374 5f6d 616e 686f  .construct_manho
+00001a40: 6c65 735f 7570 6461 7465 5f71 7565 7279  les_update_query
+00001a50: 2e01 0000 731a 0000 0000 0102 0104 0102  ....s...........
+00001a60: 0102 0102 0102 0102 0102 0102 f906 0906  ................
+00001a70: 010e 0172 5700 0000 6302 0000 0000 0000  ...rW...c.......
+00001a80: 0000 0000 0005 0000 0009 0000 0043 0000  .............C..
+00001a90: 0073 7400 0000 6700 7d02 7c00 7400 a001  .st...g.}.|.t...
+00001aa0: 7c00 7402 1900 a101 1900 7d03 7c03 7c03  |.t.......}.|.|.
+00001ab0: 7403 1900 a004 7c01 a101 0f00 1900 7d03  t.....|.......}.
+00001ac0: 7c03 6a05 7346 6401 6402 8400 7c03 7403  |.j.sFd.d...|.t.
+00001ad0: 1900 a006 a100 4400 8301 7d02 6403 a007  ......D...}.d...
+00001ae0: 7408 7409 7c02 8302 a101 7d04 6404 740a  t.t.|.....}.d.t.
+00001af0: 9b00 6405 7402 9b00 6406 740b 9b00 6407  ..d.t...d.t...d.
+00001b00: 7c04 9b00 6408 9d09 5300 2909 4e63 0100  |...d...S.).Nc..
+00001b10: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001b20: 0000 5300 0000 7310 0000 0067 007c 005d  ..S...s....g.|.]
+00001b30: 087d 017c 0191 0271 0453 0072 2700 0000  .}.|...q.S.r'...
+00001b40: 7227 0000 0029 02da 022e 30da 0469 7465  r'...)....0..ite
+00001b50: 6d72 2700 0000 7227 0000 0072 2800 0000  mr'...r'...r(...
+00001b60: da0a 3c6c 6973 7463 6f6d 703e 4301 0000  ..<listcomp>C...
+00001b70: f300 0000 007a 3263 7265 6174 655f 7570  .....z2create_up
+00001b80: 6461 7465 5f73 746f 7261 6765 5f61 7265  date_storage_are
+00001b90: 615f 7371 6c2e 3c6c 6f63 616c 733e 2e3c  a_sql.<locals>.<
+00001ba0: 6c69 7374 636f 6d70 3e72 4000 0000 7a0c  listcomp>r@...z.
+00001bb0: 0a20 2020 2055 5044 4154 4520 7a09 0a20  .    UPDATE z.. 
+00001bc0: 2020 2053 4554 207a 0f20 3d20 320a 2020     SET z. = 2.  
+00001bd0: 2020 5748 4552 4520 fa05 2049 4e20 2872    WHERE .. IN (r
+00001be0: 2a00 0000 290c da02 6e70 da05 6973 6e61  *...)...np..isna
+00001bf0: 6eda 1073 746f 7261 6765 5f61 7265 615f  n..storage_area_
+00001c00: 636f 6c72 4600 0000 da04 6973 696e da05  colrF.....isin..
+00001c10: 656d 7074 79da 0674 6f6c 6973 7472 2d00  empty..tolistr-.
+00001c20: 0000 722e 0000 0072 2f00 0000 da16 636f  ..r....r/.....co
+00001c30: 6e6e 6563 7469 6f6e 5f6e 6f64 6573 5f6c  nnection_nodes_l
+00001c40: 6179 6572 722c 0000 0029 0572 5100 0000  ayerr,...).rQ...
+00001c50: 7231 0000 005a 1275 7064 6174 655f 7374  r1...Z.update_st
+00001c60: 6f72 6167 655f 6964 735a 1875 7064 6174  orage_idsZ.updat
+00001c70: 655f 7374 6f72 6167 655f 6172 6561 5f72  e_storage_area_r
+00001c80: 6f77 735a 1e75 7064 6174 655f 7374 6f72  owsZ.update_stor
+00001c90: 6167 655f 6172 6561 5f69 6473 5f73 7472  age_area_ids_str
+00001ca0: 696e 6772 2700 0000 7227 0000 0072 2800  ingr'...r'...r(.
+00001cb0: 0000 7250 0000 003e 0100 0073 1e00 0000  ..rP...>...s....
+00001cc0: 0001 0401 1201 1401 0601 1601 1001 0201  ................
+00001cd0: 02ff 0402 02fe 0403 02fd 0403 02fd 7250  ..............rP
+00001ce0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001cf0: 0400 0000 0a00 0000 4300 0000 734e 0000  ........C...sN..
+00001d00: 007a 1e74 006a 017c 0074 0274 0374 0474  .z.t.j.|.t.t.t.t
+00001d10: 0574 067c 0164 018d 077d 027c 0257 0053  .t.|.d...}.|.W.S
+00001d20: 0004 0074 0779 4801 007d 0301 007a 127c  ...t.yH..}...z.|
+00001d30: 0364 0282 0257 0059 0064 027d 037e 036e  .d...W.Y.d.}.~.n
+00001d40: 0a64 027d 037e 0330 0030 0064 0253 0029  .d.}.~.0.0.d.S.)
+00001d50: 0361 e701 0000 446f 6f72 2065 656e 2061  .a....Door een a
+00001d60: 6e61 6c79 7365 206f 7020 6465 2072 6573  nalyse op de res
+00001d70: 756c 7461 7465 6e20 7765 7465 6e20 7765  ultaten weten we
+00001d80: 2077 656c 6b65 2077 6174 6572 6761 6e67   welke watergang
+00001d90: 656e 2065 656e 2031 6432 6420 7665 7262  en een 1d2d verb
+00001da0: 696e 6469 6e67 2068 6562 6265 6e20 6f76  inding hebben ov
+00001db0: 6572 206c 6576 6565 7320 6865 656e 2e20  er levees heen. 
+00001dc0: 416c 6c65 656e 2076 6f6f 7220 6465 7a65  Alleen voor deze
+00001dd0: 0a20 2020 2077 6174 6572 6761 6e67 656e  .    watergangen
+00001de0: 2077 6f72 6465 6e20 6465 2062 616e 6b20   worden de bank 
+00001df0: 6c65 7665 6c73 2067 656c 696a 6b20 6765  levels gelijk ge
+00001e00: 7a65 7420 6161 6e20 6465 206c 6576 6565  zet aan de levee
+00001e10: 2068 6f6f 6774 6520 6f6d 2076 726f 6567   hoogte om vroeg
+00001e20: 7469 6a64 6967 6520 7569 7477 6973 7365  tijdige uitwisse
+00001e30: 6c69 6e67 2074 6520 766f 6f72 6b6f 6d65  ling te voorkome
+00001e40: 6e2e 2044 6520 7265 7374 2076 616e 2064  n. De rest van d
+00001e50: 650a 2020 2020 6261 6e6b 206c 6576 656c  e.    bank level
+00001e60: 7320 6b6f 6d74 206f 7020 7374 7265 6566  s komt op streef
+00001e70: 7065 696c 2b31 3063 6d20 7465 2073 7461  peil+10cm te sta
+00001e80: 616e 2e0a 2020 2020 426f 7665 6e73 7461  an..    Bovensta
+00001e90: 616e 6465 2067 656c 6474 2061 6c73 2077  ande geldt als w
+00001ea0: 6520 6465 2062 616e 6b20 6c65 7665 6c73  e de bank levels
+00001eb0: 206f 706e 6965 7577 2062 6572 656b 656e   opnieuw bereken
+00001ec0: 656e 2e20 496e 2061 6c6c 6520 616e 6465  en. In alle ande
+00001ed0: 7265 2067 6576 616c 6c65 6e0a 2020 2020  re gevallen.    
+00001ee0: 776f 7264 656e 2077 6161 7264 656e 2067  worden waarden g
+00001ef0: 6562 7275 696b 7420 7569 7420 6565 6e20  ebruikt uit een 
+00001f00: 6261 636b 7570 206f 6620 6469 6520 6861  backup of die ha
+00001f10: 6e64 6d61 7469 6720 7a69 6a6e 2061 616e  ndmatig zijn aan
+00001f20: 6765 7061 7374 2064 6f6f 7220 6465 2067  gepast door de g
+00001f30: 6562 7275 696b 6572 0a20 2020 2029 0772  ebruiker.    ).r
+00001f40: 3600 0000 7237 0000 0072 3800 0000 7239  6...r7...r8...r9
+00001f50: 0000 0072 3b00 0000 723a 0000 0072 3100  ...r;...r:...r1.
+00001f60: 0000 4e29 0872 3c00 0000 723d 0000 00da  ..N).r<...r=....
+00001f70: 1363 726f 7373 5f73 6563 5f6c 6f63 5f6c  .cross_sec_loc_l
+00001f80: 6179 6572 da0e 615f 6372 6f73 735f 6c6f  ayer..a_cross_lo
+00001f90: 635f 6964 722c 0000 0072 0500 0000 da0e  c_idr,...r......
+00001fa0: 6261 6e6b 5f6c 6576 656c 5f63 6f6c 7255  bank_level_colrU
+00001fb0: 0000 0029 045a 126e 6577 5f62 616e 6b5f  ...).Z.new_bank_
+00001fc0: 6c65 7665 6c73 5f64 6672 3100 0000 7226  levels_dfr1...r&
+00001fd0: 0000 0072 5600 0000 7227 0000 0072 2700  ...rV...r'...r'.
+00001fe0: 0000 7228 0000 00da 1f63 7265 6174 655f  ..r(.....create_
+00001ff0: 6261 6e6b 5f6c 6576 656c 735f 7570 6461  bank_levels_upda
+00002000: 7465 5f71 7565 7279 4d01 0000 731a 0000  te_queryM...s...
+00002010: 0000 0702 0104 0102 0102 0102 0102 0102  ................
+00002020: 0102 0102 f906 0906 010e 0172 6700 0000  ...........rg...
+00002030: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00002040: 000a 0000 0043 0000 0073 4e00 0000 7a1e  .....C...sN...z.
+00002050: 7400 6a01 7c00 7402 7403 7403 7404 7405  t.j.|.t.t.t.t.t.
+00002060: 7c01 6401 8d07 7d02 7c02 5700 5300 0400  |.d...}.|.W.S...
+00002070: 7406 7948 0100 7d03 0100 7a12 7c03 6400  t.yH..}...z.|.d.
+00002080: 8202 5700 5900 6400 7d03 7e03 6e0a 6400  ..W.Y.d.}.~.n.d.
+00002090: 7d03 7e03 3000 3000 6400 5300 7234 0000  }.~.0.0.d.S.r4..
+000020a0: 0029 0772 3c00 0000 723d 0000 00da 0e63  .).r<...r=.....c
+000020b0: 6861 6e6e 656c 735f 6c61 7965 7272 2c00  hannels_layerr,.
+000020c0: 0000 724a 0000 0072 0800 0000 7255 0000  ..rJ...r....rU..
+000020d0: 0029 045a 1563 6861 6e6e 656c 735f 746f  .).Z.channels_to
+000020e0: 5f75 7064 6174 655f 6466 7231 0000 0072  _update_dfr1...r
+000020f0: 2600 0000 7256 0000 0072 2700 0000 7227  &...rV...r'...r'
+00002100: 0000 0072 2800 0000 da23 636f 6e73 7472  ...r(....#constr
+00002110: 7563 745f 6368 616e 6e65 6c73 5f75 7064  uct_channels_upd
+00002120: 6174 655f 7374 6174 656d 656e 7463 0100  ate_statementc..
+00002130: 0073 1a00 0000 0001 0201 0401 0201 0201  .s..............
+00002140: 0201 0201 0201 0201 02f9 0609 0601 0e01  ................
+00002150: 7269 0000 0063 0200 0000 0000 0000 0000  ri...c..........
+00002160: 0000 0300 0000 0900 0000 4300 0000 731c  ..........C...s.
+00002170: 0000 0074 006a 017c 0074 0274 0374 0474  ...t.j.|.t.t.t.t
+00002180: 0574 067c 0164 018d 077d 027c 0253 0029  .t.|.d...}.|.S.)
+00002190: 027a 8b0a 2020 2020 4372 6561 7465 7320  .z..    Creates 
+000021a0: 7173 6c20 7175 6572 7920 746f 2075 7064  qsl query to upd
+000021b0: 6174 6520 7265 6665 7265 6e63 6520 6c65  ate reference le
+000021c0: 7665 6c20 7768 6572 6520 6d69 6e69 6d75  vel where minimu
+000021d0: 6d20 7765 6972 2068 6569 6768 7420 6973  m weir height is
+000021e0: 2062 656c 6f77 0a20 2020 2067 726f 756e   below.    groun
+000021f0: 6420 6c65 7665 6c20 2861 6e79 2064 6573  d level (any des
+00002200: 656c 6563 7465 6420 6964 2773 2061 7265  elected id's are
+00002210: 2073 6b69 7070 6564 290a 2020 2020 7235   skipped).    r5
+00002220: 0000 0029 0772 3c00 0000 723d 0000 0072  ...).r<...r=...r
+00002230: 6400 0000 da13 615f 7765 6972 5f63 726f  d.....a_weir_cro
+00002240: 7373 5f6c 6f63 5f69 6472 2c00 0000 da13  ss_loc_idr,.....
+00002250: 7265 6665 7265 6e63 655f 6c65 7665 6c5f  reference_level_
+00002260: 636f 6c72 0e00 0000 2903 5a12 7772 6f6e  colr....).Z.wron
+00002270: 675f 7072 6f66 696c 6573 5f67 6466 7231  g_profiles_gdfr1
+00002280: 0000 0072 2600 0000 7227 0000 0072 2700  ...r&...r'...r'.
+00002290: 0000 7228 0000 00da 2363 7265 6174 655f  ..r(....#create_
+000022a0: 7570 6461 7465 5f72 6566 6572 656e 6365  update_reference
+000022b0: 5f6c 6576 656c 5f71 7565 7279 7301 0000  _level_querys...
+000022c0: 7314 0000 0000 0504 0102 0102 0102 0102  s...............
+000022d0: 0102 0102 0102 f906 0972 6c00 0000 6302  .........rl...c.
+000022e0: 0000 0000 0000 0000 0000 0006 0000 0072  ...............r
+000022f0: 0000 0043 0000 0073 9c01 0000 7c00 6401  ...C...s....|.d.
+00002300: 6400 8502 1900 7d02 7c00 7400 6b02 7228  d.....}.|.t.k.r(
+00002310: 7c01 6402 6b02 7222 7401 7d03 712c 7402  |.d.k.r"t.}.q,t.
+00002320: 7d03 6e04 7403 7d03 7c01 6402 6b02 723a  }.n.t.}.|.d.k.r:
+00002330: 7404 7d04 6e04 7405 7d04 6403 7c02 9b00  t.}.n.t.}.d.|...
+00002340: 6404 7406 9b00 6405 7c00 9b00 6406 7407  d.t...d.|...d.t.
+00002350: 9b00 6407 7408 9b00 6408 7409 9b00 6406  ..d.t...d.t...d.
+00002360: 7407 9b00 6407 740a 9b00 6408 7c00 9b00  t...d.t...d.|...
+00002370: 6406 740b 9b00 6407 740c 9b00 6408 7c00  d.t...d.t...d.|.
+00002380: 9b00 6406 7c04 9b00 6407 740d 9b00 6405  ..d.|...d.t...d.
+00002390: 7c00 9b00 6406 7c03 9b00 6407 740e 9b00  |...d.|...d.t...
+000023a0: 6408 740f 9b00 6406 7410 9b00 6407 7411  d.t...d.t...d.t.
+000023b0: 9b00 6408 740f 9b00 6406 7407 9b00 6407  ..d.t...d.t...d.
+000023c0: 7412 9b00 6408 7413 9b00 6409 740f 9b00  t...d.t...d.t...
+000023d0: 6406 7414 9b00 640a 7415 9b00 6406 7414  d.t...d.t...d.t.
+000023e0: 9b00 640b 7416 9b00 6405 7417 9b00 6409  ..d.t...d.t...d.
+000023f0: 7418 9b00 6409 740f 9b00 6406 7414 9b00  t...d.t...d.t...
+00002400: 640c 7415 9b00 6406 7414 9b00 640d 7419  d.t...d.t...d.t.
+00002410: 9b00 640e 7c00 9b00 640f 7409 9b00 6410  ..d.|...d.t...d.
+00002420: 7c00 9b00 6406 7c04 9b00 6411 7409 9b00  |...d.|...d.t...
+00002430: 6406 7404 9b00 640a 7409 9b00 6406 7405  d.t...d.t...d.t.
+00002440: 9b00 6412 740f 9b00 6410 7409 9b00 6406  ..d.t...d.t...d.
+00002450: 7407 9b00 6413 740f 9b00 6406 741a 9b00  t...d.t...d.t...
+00002460: 6414 7415 9b00 6410 7c00 9b00 6406 7c04  d.t...d.|...d.|.
+00002470: 9b00 6413 7415 9b00 6406 7407 9b00 6415  ..d.t...d.t...d.
+00002480: 740d 9b00 640a 7416 9b00 6416 740d 9b00  t...d.t...d.t...
+00002490: 9d72 7d05 7c05 5300 2917 4ee9 0300 0000  .r}.|.S.).N.....
+000024a0: da05 7374 6172 747a 2d53 454c 4543 5420  ..startz-SELECT 
+000024b0: 2a0a 2020 2020 4652 4f4d 2028 0a20 2020  *.    FROM (.   
+000024c0: 2020 2020 2053 454c 4543 5420 0a20 2020       SELECT .   
+000024d0: 2020 2020 2027 7a05 2720 6173 207a 0b2c       'z.' as z.,
+000024e0: 200a 2020 2020 2020 2020 7215 0000 0072   .        r....r
+000024f0: 1000 0000 7222 0000 0072 1100 0000 7218  ....r"...r....r.
+00002500: 0000 0072 1200 0000 7240 0000 00fa 0629  ...r....r@.....)
+00002510: 2920 6173 207a 0e0a 2020 2020 2020 2020  ) as z..        
+00002520: 4652 4f4d 207a 140a 2020 2020 2020 2020  FROM z..        
+00002530: 494e 4e45 5220 4a4f 494e 2072 1e00 0000  INNER JOIN r....
+00002540: 725c 0000 007a 1529 0a20 2020 2020 2020  r\...z.).       
+00002550: 2049 4e4e 4552 204a 4f49 4e20 7219 0000   INNER JOIN r...
+00002560: 0072 1d00 0000 7a12 0a20 2020 2020 2020  .r....z..       
+00002570: 2047 524f 5550 2042 5920 7a18 0a20 2020   GROUP BY z..   
+00002580: 2020 2020 2029 0a20 2020 2047 524f 5550       ).    GROUP
+00002590: 2042 5920 291b da0d 6375 6c76 6572 745f   BY )...culvert_
+000025a0: 6c61 7965 725a 1469 6e76 6572 745f 6c76  layerZ.invert_lv
+000025b0: 6c5f 7374 6172 745f 636f 6c5a 1269 6e76  l_start_colZ.inv
+000025c0: 6572 745f 6c76 6c5f 656e 645f 636f 6c5a  ert_lvl_end_colZ
+000025d0: 0f63 7265 7374 5f6c 6576 656c 5f63 6f6c  .crest_level_col
+000025e0: da16 636f 6e6e 5f6e 6f64 655f 7374 6172  ..conn_node_star
+000025f0: 745f 6964 5f63 6f6c da14 636f 6e6e 5f6e  t_id_col..conn_n
+00002600: 6f64 655f 656e 645f 6964 5f63 6f6c 5a16  ode_end_id_colZ.
+00002610: 615f 6368 616e 5f62 6564 5f73 7472 7563  a_chan_bed_struc
+00002620: 745f 7479 7065 722c 0000 005a 1461 5f63  t_typer,...Z.a_c
+00002630: 6861 6e5f 6265 645f 7374 7275 6374 5f69  han_bed_struct_i
+00002640: 6472 6800 0000 5a15 615f 6368 616e 5f62  drh...Z.a_chan_b
+00002650: 6564 5f63 6861 6e6e 656c 5f69 6472 4500  ed_channel_idrE.
+00002660: 0000 5a16 615f 6368 616e 5f62 6564 5f73  ..Z.a_chan_bed_s
+00002670: 7472 7563 745f 636f 6465 5a12 615f 6368  truct_codeZ.a_ch
+00002680: 616e 5f62 6564 5f63 6f6e 6e5f 6964 da19  an_bed_conn_id..
+00002690: 615f 6368 616e 5f62 6564 5f73 7472 7563  a_chan_bed_struc
+000026a0: 745f 7265 665f 6c76 6c72 6400 0000 726b  t_ref_lvlrd...rk
+000026b0: 0000 00da 1861 5f63 6861 6e5f 6265 645f  .....a_chan_bed_
+000026c0: 6372 6f73 735f 7265 665f 6c76 6c5a 1361  cross_ref_lvlZ.a
+000026d0: 5f63 6861 6e5f 6265 645f 6372 6f73 735f  _chan_bed_cross_
+000026e0: 6964 5a0a 665f 6469 7374 616e 6365 da07  idZ.f_distance..
+000026f0: 6765 6f5f 636f 6c72 6300 0000 5a1c 615f  geo_colrc...Z.a_
+00002700: 6368 616e 5f62 6564 5f64 6973 745f 6372  chan_bed_dist_cr
+00002710: 6f73 735f 7374 7275 6374 da07 665f 6173  oss_struct..f_as
+00002720: 776b 74da 0a66 5f6d 616b 656c 696e 65da  wkt..f_makeline.
+00002730: 0a64 665f 6765 6f5f 636f 6cda 0e63 6861  .df_geo_col..cha
+00002740: 6e6e 656c 5f69 645f 636f 6c29 06da 0673  nnel_id_col)...s
+00002750: 7472 7563 745a 0873 7461 7274 656e 64da  tructZ.startend.
+00002760: 0474 7970 655a 1372 6566 6572 656e 6365  .typeZ.reference
+00002770: 5f70 6172 616d 6574 6572 da0c 636f 6e6e  _parameter..conn
+00002780: 5f6e 6f64 655f 6964 7226 0000 0072 2700  _node_idr&...r'.
+00002790: 0000 7227 0000 0072 2800 0000 da23 5f5f  ..r'...r(....#__
+000027a0: 636f 6e73 7472 7563 745f 6368 616e 6e65  construct_channe
+000027b0: 6c5f 6265 645f 7175 6572 795f 696e 6e65  l_bed_query_inne
+000027c0: 7284 0100 0073 fa00 0000 0002 0c01 0801  r....s..........
+000027d0: 0801 0602 0602 0401 0801 0602 0401 0203  ................
+000027e0: 02fd 0403 02fd 0404 02fc 0404 02fc 0404  ................
+000027f0: 02fc 0405 02fb 0405 02fb 0405 02fb 0406  ................
+00002800: 02fa 0406 02fa 0406 02fa 0407 02f9 0407  ................
+00002810: 02f9 0407 02f9 0408 02f8 0408 02f8 0408  ................
+00002820: 02f8 0409 02f7 0409 02f7 0409 02f7 040a  ................
+00002830: 02f6 040a 02f6 040a 02f6 040b 02f5 040b  ................
+00002840: 02f5 040b 02f5 040b 02f5 040b 02f5 040b  ................
+00002850: 02f5 040c 02f4 040c 02f4 040c 02f4 040c  ................
+00002860: 02f4 040c 02f4 040c 02f4 040c 02f4 040d  ................
+00002870: 02f3 040e 02f2 040f 02f1 040f 02f1 040f  ................
+00002880: 02f1 040f 02f1 040f 02f1 040f 02f1 0410  ................
+00002890: 02f0 0411 02ef 0411 02ef 0411 02ef 0411  ................
+000028a0: 02ef 0412 02ee 0413 02ed 0413 02ed 0413  ................
+000028b0: 02ed 0413 02ed 0414 02ec 0414 02ec 0416  ................
+000028c0: 02ea 0617 727d 0000 0063 0000 0000 0000  ....r}...c......
+000028d0: 0000 0000 0000 0100 0000 0d00 0000 4300  ..............C.
+000028e0: 0000 7346 0000 0064 0174 0074 0164 0283  ..sF...d.t.t.d..
+000028f0: 029b 0064 0374 0074 0164 0483 029b 0064  ...d.t.t.d.....d
+00002900: 0574 0074 0264 0283 029b 0064 0374 0074  .t.t.d.....d.t.t
+00002910: 0264 0483 029b 0064 0674 039b 0064 0774  .d.....d.t...d.t
+00002920: 049b 0064 089d 0d7d 007c 0053 0029 097a  ...d...}.|.S.).z
+00002930: 4c0a 2020 2020 4164 6420 6372 6f73 7320  L.    Add cross 
+00002940: 7365 6374 696f 6e20 616e 6420 6368 616e  section and chan
+00002950: 6e65 6c20 696e 666f 726d 6174 696f 6e20  nel information 
+00002960: 746f 2063 6f6e 7472 6f6c 6c65 6420 7374  to controlled st
+00002970: 7275 6374 7572 6573 0a20 2020 207a 1353  ructures.    z.S
+00002980: 454c 4543 5420 2a20 4652 4f4d 2028 2020  ELECT * FROM (  
+00002990: 2020 726e 0000 007a 0b20 2020 2020 554e    rn...z.     UN
+000029a0: 494f 4e20 da03 656e 647a 0a20 2020 2055  ION ..endz.    U
+000029b0: 4e49 4f4e 207a 0c29 2020 2020 2057 4845  NION z.)     WHE
+000029c0: 5245 207a 0320 3c20 7242 0000 0029 0572  RE z. < rB...).r
+000029d0: 7d00 0000 7270 0000 00da 0d6f 7269 6669  }...rp.....orifi
+000029e0: 6365 5f6c 6179 6572 7273 0000 0072 7400  ce_layerrs...rt.
+000029f0: 0000 a901 7226 0000 0072 2700 0000 7227  ....r&...r'...r'
+00002a00: 0000 0072 2800 0000 da22 636f 6e73 7472  ...r(...."constr
+00002a10: 7563 745f 7374 7275 6374 5f63 6861 6e6e  uct_struct_chann
+00002a20: 656c 5f62 6564 5f71 7565 7279 ac01 0000  el_bed_query....
+00002a30: 731c 0000 0000 0402 0108 ff04 0208 fe04  s...............
+00002a40: 0308 fd04 0408 fc04 0502 fb04 0502 fb08  ................
+00002a50: 0672 8100 0000 6302 0000 0000 0000 0000  .r....c.........
+00002a60: 0000 0004 0000 000a 0000 0043 0000 0073  ...........C...s
+00002a70: 4e00 0000 7a1e 7400 6a01 7c00 7402 7403  N...z.t.j.|.t.t.
+00002a80: 7404 7405 7406 7c01 6401 8d07 7d02 7c02  t.t.t.|.d...}.|.
+00002a90: 5700 5300 0400 7407 7948 0100 7d03 0100  W.S...t.yH..}...
+00002aa0: 7a12 7c03 6400 8202 5700 5900 6400 7d03  z.|.d...W.Y.d.}.
+00002ab0: 7e03 6e0a 6400 7d03 7e03 3000 3000 6400  ~.n.d.}.~.0.0.d.
+00002ac0: 5300 7234 0000 0029 0872 3c00 0000 723d  S.r4...).r<...r=
+00002ad0: 0000 00da 1363 726f 7373 5f73 6563 5f64  .....cross_sec_d
+00002ae0: 6566 5f6c 6179 6572 da13 615f 7765 6972  ef_layer..a_weir
+00002af0: 5f63 726f 7373 5f64 6566 5f69 6472 2c00  _cross_def_idr,.
+00002b00: 0000 7248 0000 0072 0d00 0000 7255 0000  ..rH...r....rU..
+00002b10: 0029 045a 1877 6569 725f 7769 6474 6873  .).Z.weir_widths
+00002b20: 5f74 6f5f 7570 6461 7465 5f64 6672 3100  _to_update_dfr1.
+00002b30: 0000 7226 0000 0072 5600 0000 7227 0000  ..r&...rV...r'..
+00002b40: 0072 2700 0000 7228 0000 00da 2663 6f6e  .r'...r(....&con
+00002b50: 7374 7275 6374 5f77 6569 725f 6865 6967  struct_weir_heig
+00002b60: 6874 5f75 7064 6174 655f 7374 6174 656d  ht_update_statem
+00002b70: 656e 74bd 0100 0073 1a00 0000 0001 0201  ent....s........
+00002b80: 0401 0201 0201 0201 0201 0201 0201 02f9  ................
+00002b90: 0609 0601 0e01 7284 0000 0063 0100 0000  ......r....c....
+00002ba0: 0000 0000 0000 0000 0200 0000 5900 0000  ............Y...
+00002bb0: 4300 0000 7312 0100 0064 0174 009b 0064  C...s....d.t...d
+00002bc0: 0274 019b 0064 0374 029b 0064 0474 009b  .t...d.t...d.t..
+00002bd0: 0064 0274 039b 0064 0474 009b 0064 0274  .d.t...d.t...d.t
+00002be0: 049b 0064 0574 009b 0064 0274 059b 0064  ...d.t...d.t...d
+00002bf0: 047c 009b 0064 0274 069b 0064 0474 079b  .|...d.t...d.t..
+00002c00: 0064 0674 089b 0064 0774 099b 0064 0874  .d.t...d.t...d.t
+00002c10: 0a9b 0064 0274 099b 0064 0974 0b9b 0064  ...d.t...d.t...d
+00002c20: 0a7c 009b 0064 0b74 009b 0064 0c7c 009b  .|...d.t...d.|..
+00002c30: 0064 0274 019b 0064 0d74 009b 0064 0274  .d.t...d.t...d.t
+00002c40: 059b 0064 0e74 0a9b 0064 0c7c 009b 0064  ...d.t...d.|...d
+00002c50: 0274 0c9b 0064 0d74 0a9b 0064 0274 019b  .t...d.t...d.t..
+00002c60: 0064 0e74 0d9b 0064 0c74 0d9b 0064 0274  .d.t...d.t...d.t
+00002c70: 0e9b 0064 0d74 009b 0064 0274 019b 0064  ...d.t...d.t...d
+00002c80: 0e74 0f9b 0064 0c74 0f9b 0064 0274 109b  .t...d.t...d.t..
+00002c90: 0064 0d74 0d9b 0064 0274 109b 0064 0e74  .d.t...d.t...d.t
+00002ca0: 0a9b 0064 0f74 0f9b 0064 0274 119b 0064  ...d.t...d.t...d
+00002cb0: 1074 009b 0064 0274 049b 0064 117c 009b  .t...d.t...d.|..
+00002cc0: 0064 129d 597d 017c 0153 0029 134e 720f  .d..Y}.|.S.).Nr.
+00002cd0: 0000 0072 1500 0000 7210 0000 007a 072c  ...r....r....z.,
+00002ce0: 200a 2020 2020 7213 0000 0072 1100 0000   .    r....r....
+00002cf0: 7a16 2876 325f 636f 6e6e 6563 7469 6f6e  z.(v2_connection
+00002d00: 5f6e 6f64 6573 322e 7240 0000 0072 6f00  _nodes2.r@...ro.
+00002d10: 0000 7214 0000 0072 1c00 0000 7217 0000  ..r....r....r...
+00002d20: 0072 1900 0000 7216 0000 007a 2020 6173  .r....r....z  as
+00002d30: 2076 325f 636f 6e6e 6563 7469 6f6e 5f6e   v2_connection_n
+00002d40: 6f64 6573 320a 2020 2020 4f4e 207a 2520  odes2.    ON z% 
+00002d50: 3d20 7632 5f63 6f6e 6e65 6374 696f 6e5f  = v2_connection_
+00002d60: 6e6f 6465 7332 2e69 640a 2020 2020 5748  nodes2.id.    WH
+00002d70: 4552 4520 7a02 3d27 7220 0000 0029 12da  ERE z.='r ...)..
+00002d80: 1363 6f6e 7472 6f6c 5f74 6162 6c65 5f6c  .control_table_l
+00002d90: 6179 6572 722c 0000 005a 1761 5f63 6f6e  ayerr,...Z.a_con
+00002da0: 7472 5f73 7472 7563 745f 636f 6e74 725f  tr_struct_contr_
+00002db0: 6964 da0a 6163 7469 6f6e 5f63 6f6c da0f  id..action_col..
+00002dc0: 7461 7267 6574 5f74 7970 655f 636f 6cda  target_type_col.
+00002dd0: 0d74 6172 6765 745f 6964 5f63 6f6c 7245  .target_id_colrE
+00002de0: 0000 0072 7600 0000 7277 0000 0072 7500  ...rv...rw...ru.
+00002df0: 0000 7263 0000 0072 7800 0000 7271 0000  ..rc...rx...rq..
+00002e00: 005a 0d63 6f6e 7472 6f6c 5f6c 6179 6572  .Z.control_layer
+00002e10: 5a0e 636f 6e74 726f 6c5f 6964 5f63 6f6c  Z.control_id_col
+00002e20: 5a13 636f 6e74 726f 6c5f 6d65 6173 7572  Z.control_measur
+00002e30: 655f 6d61 705a 146d 6561 7375 7265 5f67  e_mapZ.measure_g
+00002e40: 726f 7570 5f69 645f 636f 6c5a 0d6f 626a  roup_id_colZ.obj
+00002e50: 6563 745f 6964 5f63 6f6c 2902 da09 7374  ect_id_col)...st
+00002e60: 7275 6374 7572 6572 2600 0000 7227 0000  ructurer&...r'..
+00002e70: 0072 2700 0000 7228 0000 00da 2b63 6f6e  .r'...r(....+con
+00002e80: 7374 7275 6374 5f63 6f6e 7472 6f6c 6c65  struct_controlle
+00002e90: 645f 7374 7275 6374 7572 6573 5f71 7565  d_structures_que
+00002ea0: 7279 5f69 6e6e 6572 ce01 0000 73b4 0000  ry_inner....s...
+00002eb0: 0000 0102 0102 ff04 0102 ff04 0102 ff04  ................
+00002ec0: 0202 fe04 0202 fe04 0302 fd04 0302 fd04  ................
+00002ed0: 0402 fc04 0402 fc04 0502 fb04 0502 fb04  ................
+00002ee0: 0602 fa04 0602 fa04 0602 fa04 0602 fa04  ................
+00002ef0: 0602 fa04 0602 fa04 0702 f904 0802 f804  ................
+00002f00: 0902 f704 0902 f704 0902 f704 0902 f704  ................
+00002f10: 0a02 f604 0b02 f504 0b02 f504 0b02 f504  ................
+00002f20: 0b02 f504 0c02 f404 0d02 f304 0d02 f304  ................
+00002f30: 0d02 f304 0d02 f304 0e02 f204 0f02 f104  ................
+00002f40: 0f02 f104 0f02 f104 0f02 f104 1002 f004  ................
+00002f50: 1102 ef04 1102 ef04 1202 ee04 1202 ee04  ................
+00002f60: 1202 ee08 1472 8a00 0000 6300 0000 0000  .....r....c.....
+00002f70: 0000 0000 0000 0001 0000 0007 0000 0043  ...............C
+00002f80: 0000 0073 2800 0000 6401 7400 7401 8301  ...s(...d.t.t...
+00002f90: 9b00 6402 7400 7402 8301 9b00 6402 7400  ..d.t.t.....d.t.
+00002fa0: 7403 8301 9b00 6403 9d07 7d00 7c00 5300  t.....d...}.|.S.
+00002fb0: 2904 4e7a 1453 454c 4543 5420 2a20 4652  ).Nz.SELECT * FR
+00002fc0: 4f4d 2028 0a20 2020 207a 0b0a 2020 2020  OM (.    z..    
+00002fd0: 554e 494f 4e20 7241 0000 0029 0472 8a00  UNION rA...).r..
+00002fe0: 0000 da0a 7765 6972 5f6c 6179 6572 7270  ....weir_layerrp
+00002ff0: 0000 0072 7f00 0000 7280 0000 0072 2700  ...r....r....r'.
+00003000: 0000 7227 0000 0072 2800 0000 da25 636f  ..r'...r(....%co
+00003010: 6e73 7472 7563 745f 636f 6e74 726f 6c6c  nstruct_controll
+00003020: 6564 5f73 7472 7563 7475 7265 735f 7175  ed_structures_qu
+00003030: 6572 79e6 0100 0073 1000 0000 0001 0201  ery....s........
+00003040: 06ff 0402 06fe 0403 06fd 0804 728c 0000  ............r...
+00003050: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
+00003060: 0000 0600 0000 4300 0000 732e 0000 0067  ......C...s....g
+00003070: 007d 027c 0044 005d 167d 037c 02a0 0074  .}.|.D.].}.|...t
+00003080: 016a 027c 0364 018d 01a1 0101 0071 0864  .j.|.d.......q.d
+00003090: 02a0 037c 02a1 017d 047c 0453 0029 034e  ...|...}.|.S.).N
+000030a0: 2901 da05 7461 626c 657a 0b0a 554e 494f  )...tablez..UNIO
+000030b0: 4e20 414c 4c0a 2904 7230 0000 00da 1967  N ALL.).r0.....g
+000030c0: 656f 6d65 7472 795f 6368 6563 6b5f 7175  eometry_check_qu
+000030d0: 6572 795f 6261 7365 7224 0000 0072 2d00  ery_baser$...r-.
+000030e0: 0000 2905 da0b 7461 626c 655f 6e61 6d65  ..)...table_name
+000030f0: 735a 0764 7374 5f63 7273 5a0b 7175 6572  sZ.dst_crsZ.quer
+00003100: 6965 735f 6c73 7472 8d00 0000 7226 0000  ies_lstr....r&..
+00003110: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
+00003120: da18 636f 6e73 7472 7563 745f 6765 6f6d  ..construct_geom
+00003130: 6574 7279 5f71 7565 7279 f101 0000 730a  etry_query....s.
+00003140: 0000 0000 0104 0108 0114 010a 0172 9000  .............r..
+00003150: 0000 2901 728f 0000 0029 79da 075f 5f64  ..).r....)y..__d
+00003160: 6f63 5f5f da13 6868 6e6b 5f72 6573 6561  oc__..hhnk_resea
+00003170: 7263 685f 746f 6f6c 7372 3c00 0000 da05  rch_toolsr<.....
+00003180: 6e75 6d70 7972 5d00 0000 5a30 6868 6e6b  numpyr]...Z0hhnk
+00003190: 5f74 6872 6565 6469 5f74 6f6f 6c73 2e76  _threedi_tools.v
+000031a0: 6172 6961 626c 6573 2e62 6163 6b75 7073  ariables.backups
+000031b0: 5f74 6162 6c65 5f6e 616d 6573 7202 0000  _table_namesr...
+000031c0: 0072 0300 0000 7204 0000 00da 2868 686e  .r....r.....(hhn
+000031d0: 6b5f 7468 7265 6564 695f 746f 6f6c 732e  k_threedi_tools.
+000031e0: 7661 7269 6162 6c65 732e 6261 6e6b 5f6c  variables.bank_l
+000031f0: 6576 656c 7372 0500 0000 da2d 6868 6e6b  evelsr.....-hhnk
+00003200: 5f74 6872 6565 6469 5f74 6f6f 6c73 2e76  _threedi_tools.v
+00003210: 6172 6961 626c 6573 2e64 6174 6162 6173  ariables.databas
+00003220: 655f 616c 6961 7365 73da 2f68 686e 6b5f  e_aliases./hhnk_
+00003230: 7468 7265 6564 695f 746f 6f6c 732e 7661  threedi_tools.va
+00003240: 7269 6162 6c65 732e 6461 7461 6261 7365  riables.database
+00003250: 5f76 6172 6961 626c 6573 da2e 6868 6e6b  _variables..hhnk
 00003260: 5f74 6872 6565 6469 5f74 6f6f 6c73 2e76  _threedi_tools.v
-00003270: 6172 6961 626c 6573 2e64 6174 6162 6173  ariables.databas
-00003280: 655f 616c 6961 7365 73da 2f68 686e 6b5f  e_aliases./hhnk_
-00003290: 7468 7265 6564 695f 746f 6f6c 732e 7661  threedi_tools.va
-000032a0: 7269 6162 6c65 732e 6461 7461 6261 7365  riables.database
-000032b0: 5f76 6172 6961 626c 6573 da2e 6868 6e6b  _variables..hhnk
-000032c0: 5f74 6872 6565 6469 5f74 6f6f 6c73 2e76  _threedi_tools.v
-000032d0: 6172 6961 626c 6573 2e64 6566 6175 6c74  ariables.default
-000032e0: 5f76 6172 6961 626c 6573 7207 0000 005a  _variablesr....Z
-000032f0: 2868 686e 6b5f 7468 7265 6564 695f 746f  (hhnk_threedi_to
-00003300: 6f6c 732e 7661 7269 6162 6c65 732e 6d6f  ols.variables.mo
-00003310: 6465 6c5f 7374 6174 6572 0800 0000 7209  del_stater....r.
-00003320: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-00003330: 0000 720d 0000 005a 2268 686e 6b5f 7468  ..r....Z"hhnk_th
-00003340: 7265 6564 695f 746f 6f6c 732e 7661 7269  reedi_tools.vari
-00003350: 6162 6c65 732e 7765 6972 7372 0e00 0000  ables.weirsr....
-00003360: 7225 0000 0072 2c00 0000 da0e 615f 636f  r%...r,.....a_co
-00003370: 6e6e 5f6e 6f64 655f 6964 da16 696e 6974  nn_node_id..init
-00003380: 6961 6c5f 7761 7465 726c 6576 656c 5f63  ial_waterlevel_c
-00003390: 6f6c 725f 0000 0072 7600 0000 7275 0000  olr_...rv...ru..
-000033a0: 0072 7800 0000 7263 0000 00da 1063 6f6e  .rx...rc.....con
-000033b0: 6e5f 6e6f 6465 735f 7175 6572 795a 1361  n_nodes_queryZ.a
-000033c0: 5f77 6174 6572 7375 7266 5f63 6f6e 6e5f  _watersurf_conn_
-000033d0: 6964 5a1c 7761 7465 7273 7572 6661 6365  idZ.watersurface
-000033e0: 5f63 6f6e 6e5f 6e6f 6465 5f71 7565 7279  _conn_node_query
-000033f0: 7243 0000 00da 0861 5f6d 616e 5f69 6472  rC.....a_man_idr
-00003400: 4600 0000 da0d 615f 6d61 6e5f 636f 6e6e  F.....a_man_conn
-00003410: 5f69 6472 4500 0000 724b 0000 00da 0e6d  _idrE...rK.....m
-00003420: 616e 686f 6c65 735f 7175 6572 7972 6800  anholes_queryrh.
-00003430: 0000 da09 615f 6368 616e 5f69 645a 0c61  ....a_chan_idZ.a
-00003440: 5f63 6f6e 6e5f 6e6f 6465 7372 7100 0000  _conn_nodesrq...
-00003450: da0e 6368 616e 6e65 6c73 5f71 7565 7279  ..channels_query
-00003460: 7265 0000 0072 7900 0000 726b 0000 0072  re...ry...rk...r
-00003470: 6600 0000 7264 0000 00da 1c63 726f 7373  f...rd.....cross
-00003480: 5f73 6563 7469 6f6e 5f6c 6f63 6174 696f  _section_locatio
-00003490: 6e5f 7175 6572 795a 0b61 5f63 6861 6e5f  n_queryZ.a_chan_
-000034a0: 636f 6465 7272 0000 005a 0e61 5f63 6861  coderr...Z.a_cha
-000034b0: 6e5f 6e6f 6465 5f69 6472 4e00 0000 5a0a  n_node_idrN...Z.
-000034c0: 615f 7a6f 6f6d 5f63 6174 5a12 615f 6372  a_zoom_catZ.a_cr
-000034d0: 6f73 735f 7365 635f 6c6f 635f 6964 5a14  oss_sec_loc_idZ.
-000034e0: 615f 6372 6f73 735f 7365 635f 6c6f 635f  a_cross_sec_loc_
-000034f0: 636f 6465 5a0a 6465 665f 6964 5f63 6f6c  codeZ.def_id_col
-00003500: 7282 0000 005a 1261 5f63 726f 7373 5f73  r....Z.a_cross_s
-00003510: 6563 5f64 6566 5f69 6472 4800 0000 5a0a  ec_def_idrH...Z.
-00003520: 6865 6967 6874 5f63 6f6c 5a13 7072 6f66  height_colZ.prof
-00003530: 696c 6573 5f75 7365 645f 7175 6572 795a  iles_used_queryZ
-00003540: 1f62 616e 6b5f 6c76 6c73 5f73 6f75 7263  .bank_lvls_sourc
-00003550: 655f 6372 6561 7469 6f6e 5f71 7565 7279  e_creation_query
-00003560: 5a1d 6261 6e6b 5f6c 766c 735f 736f 7572  Z.bank_lvls_sour
-00003570: 6365 5f75 7064 6174 655f 7175 6572 795a  ce_update_queryZ
-00003580: 1662 616e 6b5f 6c76 6c73 5f6c 6173 745f  .bank_lvls_last_
-00003590: 6368 616e 6765 6472 4a00 0000 5a17 6973  changedrJ...Z.is
-000035a0: 6f6c 6174 6564 5f63 6861 6e6e 656c 735f  olated_channels_
-000035b0: 7175 6572 7972 8b00 0000 5a10 6372 6f73  queryr....Z.cros
-000035c0: 735f 6465 665f 6964 5f63 6f6c 7285 0000  s_def_id_colr...
-000035d0: 0072 8800 0000 5a17 7765 6972 5f77 6964  .r....Z.weir_wid
-000035e0: 7468 5f62 6163 6b75 705f 7175 6572 7972  th_backup_queryr
-000035f0: 8300 0000 5a0b 615f 7765 6972 5f63 6f64  ....Z.a_weir_cod
-00003600: 655a 0961 5f77 6569 725f 6964 5a1d 7765  eZ.a_weir_idZ.we
-00003610: 6972 5f77 6964 7468 735f 6672 6f6d 5f62  ir_widths_from_b
-00003620: 6163 6b75 705f 7175 6572 795a 2063 6f6e  ackup_queryZ con
-00003630: 7472 6f6c 6c65 645f 7765 6972 735f 7365  trolled_weirs_se
-00003640: 6c65 6374 696f 6e5f 7175 6572 795a 1961  lection_queryZ.a
-00003650: 5f77 6569 725f 636f 6e6e 5f6e 6f64 655f  _weir_conn_node_
-00003660: 7374 6172 745f 6964 5a17 615f 7765 6972  start_idZ.a_weir
-00003670: 5f63 6f6e 6e5f 6e6f 6465 5f65 6e64 5f69  _conn_node_end_i
-00003680: 6472 8600 0000 5a19 615f 7765 6972 5f63  dr....Z.a_weir_c
-00003690: 6861 6e5f 636f 6e6e 5f73 7461 7274 5f69  han_conn_start_i
-000036a0: 645a 1761 5f77 6569 725f 6368 616e 5f63  dZ.a_weir_chan_c
-000036b0: 6f6e 6e5f 656e 645f 6964 726a 0000 0072  onn_end_idrj...r
-000036c0: 8700 0000 5a11 7765 6972 5f68 6569 6768  ....Z.weir_heigh
-000036d0: 745f 7175 6572 795a 0861 7265 615f 636f  t_queryZ.area_co
-000036e0: 6c5a 1869 6d70 6572 7669 6f75 735f 7375  lZ.impervious_su
-000036f0: 7266 6163 655f 6c61 7965 725a 1869 6d70  rface_layerZ.imp
-00003700: 6572 7669 6f75 735f 7375 7266 6163 655f  ervious_surface_
-00003710: 7175 6572 795a 0b66 5f74 7261 6e73 666f  queryZ.f_transfo
-00003720: 726d 5a08 665f 706f 696e 746e 5a11 615f  rmZ.f_pointnZ.a_
-00003730: 6765 6f5f 7374 6172 745f 636f 6f72 645a  geo_start_coordZ
-00003740: 0b66 5f6e 756d 706f 696e 7473 5a0f 615f  .f_numpointsZ.a_
-00003750: 6765 6f5f 656e 645f 636f 6f72 645a 1061  geo_end_coordZ.a
-00003760: 5f67 656f 5f73 7461 7274 5f6e 6f64 655a  _geo_start_nodeZ
-00003770: 0e61 5f67 656f 5f65 6e64 5f6e 6f64 655a  .a_geo_end_nodeZ
-00003780: 1461 5f67 656f 5f63 6f6e 6e5f 6e6f 6465  .a_geo_conn_node
-00003790: 735f 656e 645a 1661 5f67 656f 5f63 6f6e  s_endZ.a_geo_con
-000037a0: 6e5f 6e6f 6465 735f 7374 6172 7472 8f00  n_nodes_startr..
-000037b0: 0000 7229 0000 0072 3300 0000 723e 0000  ..r)...r3...r>..
-000037c0: 0072 5400 0000 7257 0000 0072 5000 0000  .rT...rW...rP...
-000037d0: 7267 0000 0072 6900 0000 726c 0000 0072  rg...ri...rl...r
-000037e0: 7d00 0000 7281 0000 005a 1873 7472 7563  }...r....Z.struc
-000037f0: 745f 6368 616e 6e65 6c5f 6265 645f 7175  t_channel_bed_qu
-00003800: 6572 7972 8400 0000 728a 0000 0072 8c00  eryr....r....r..
-00003810: 0000 5a1b 636f 6e74 726f 6c6c 6564 5f73  ..Z.controlled_s
-00003820: 7472 7563 7475 7265 735f 7175 6572 7972  tructures_queryr
-00003830: 9100 0000 7270 0000 005a 1467 656f 6d65  ....rp...Z.geome
-00003840: 7472 795f 6368 6563 6b5f 7175 6572 7972  try_check_queryr
-00003850: 2700 0000 7227 0000 0072 2700 0000 7228  '...r'...r'...r(
-00003860: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
-00003870: 0073 b804 0000 040a 0801 0802 1405 0c03  .s..............
-00003880: 0804 0801 0c01 2008 0c04 0201 02ff 0806  ...... .........
-00003890: 0201 02ff 0401 02ff 0402 02fe 0403 02fd  ................
-000038a0: 0404 02fc 0404 02fc 0404 02fc 0405 02fb  ................
-000038b0: 0808 0201 02ff 0401 02ff 0402 02fe 0403  ................
-000038c0: 02fd 0404 02fc 0404 02fc 0404 02fc 0405  ................
-000038d0: 02fb 0809 0202 02fe 0402 02fe 0402 02fe  ................
-000038e0: 0403 02fd 0403 02fd 0403 02fd 0404 02fc  ................
-000038f0: 0404 02fc 0405 02fb 0405 02fb 0406 02fa  ................
-00003900: 0406 02fa 0407 02f9 0407 02f9 0408 02f8  ................
-00003910: 0408 02f8 0408 02f8 0408 02f8 0409 02f7  ................
-00003920: 040a 02f6 040b 02f5 040b 02f5 040b 02f5  ................
-00003930: 040b 02f5 080f 0202 02fe 0402 02fe 0402  ................
-00003940: 02fe 0403 02fd 0403 02fd 0403 02fd 0403  ................
-00003950: 02fd 0403 02fd 0403 02fd 0404 02fc 0405  ................
-00003960: 02fb 0405 02fb 0406 02fa 0406 02fa 0406  ................
-00003970: 02fa 0406 02fa 0809 0202 02fe 0402 02fe  ................
-00003980: 0403 02fd 0404 02fc 0405 02fb 0405 02fb  ................
-00003990: 0405 02fb 0405 02fb 0406 02fa 0808 0202  ................
-000039a0: 02fe 0402 02fe 0402 02fe 0403 02fd 0403  ................
-000039b0: 02fd 0403 02fd 0404 02fc 0404 02fc 0404  ................
-000039c0: 02fc 0405 02fb 0405 02fb 0405 02fb 0406  ................
-000039d0: 02fa 0406 02fa 0406 02fa 0406 02fa 0407  ................
-000039e0: 02f9 0407 02f9 0407 02f9 0408 02f8 0408  ................
-000039f0: 02f8 0408 02f8 0409 02f7 0409 02f7 040a  ................
-00003a00: 02f6 040a 02f6 040b 02f5 040b 02f5 040c  ................
-00003a10: 02f4 040c 02f4 040c 02f4 040d 02f3 040d  ................
-00003a20: 02f3 040e 02f2 040e 02f2 040f 02f1 040f  ................
-00003a30: 02f1 0410 02f0 0411 02ef 0411 02ef 0411  ................
-00003a40: 02ef 0411 02ef 0411 02ef 0412 02ee 0412  ................
-00003a50: 02ee 0412 02ee 0412 02ee 0412 02ee 0413  ................
-00003a60: 02ed 0413 02ed 0413 02ed 0413 02ed 0413  ................
-00003a70: 02ed 0414 02ec 0414 02ec 0816 0c01 0c01  ................
-00003a80: 0c02 0201 02ff 0402 02fe 0403 02fd 0403  ................
-00003a90: 02fd 0403 02fd 0404 02fc 0808 0201 02ff  ................
-00003aa0: 0401 02ff 0403 02fd 0403 02fd 0404 02fc  ................
-00003ab0: 0405 02fb 0405 02fb 0405 02fb 0405 02fb  ................
-00003ac0: 0405 02fb 0406 02fa 0406 02fa 0406 02fa  ................
-00003ad0: 0406 02fa 0406 02fa 0809 0202 02fe 0402  ................
-00003ae0: 02fe 0402 02fe 0403 02fd 0403 02fd 0403  ................
-00003af0: 02fd 0404 02fc 0404 02fc 0404 02fc 0405  ................
-00003b00: 02fb 0405 02fb 0406 02fa 0407 02f9 0407  ................
-00003b10: 02f9 0407 02f9 0407 02f9 0407 02f9 0408  ................
-00003b20: 02f8 0408 02f8 0408 02f8 0408 02f8 0408  ................
-00003b30: 02f8 080a 0202 02fe 0402 02fe 0402 02fe  ................
-00003b40: 0403 02fd 0403 02fd 0403 02fd 0404 02fc  ................
-00003b50: 0404 02fc 0404 02fc 0405 02fb 0405 02fb  ................
-00003b60: 0406 02fa 0407 02f9 0407 02f9 0407 02f9  ................
-00003b70: 0407 02f9 0407 02f9 0408 02f8 0408 02f8  ................
-00003b80: 0408 02f8 0408 02f8 0408 02f8 080b 0201  ................
-00003b90: 02ff 0401 02ff 0402 02fe 0402 02fe 0403  ................
-00003ba0: 02fd 0403 02fd 0404 02fc 0404 02fc 0405  ................
-00003bb0: 02fb 0405 02fb 0405 02fb 0406 02fa 0406  ................
-00003bc0: 02fa 0406 02fa 0407 02f9 0407 02f9 0407  ................
-00003bd0: 02f9 0408 02f8 0408 02f8 0409 02f7 0409  ................
-00003be0: 02f7 0409 02f7 040a 02f6 040a 02f6 040a  ................
-00003bf0: 02f6 040a 02f6 040b 02f5 040c 02f4 040d  ................
-00003c00: 02f3 040d 02f3 040d 02f3 040e 02f2 040f  ................
-00003c10: 02f1 040f 02f1 040f 02f1 040f 02f1 040f  ................
-00003c20: 02f1 0410 02f0 0410 02f0 0410 02f0 0410  ................
-00003c30: 02f0 0410 02f0 0411 02ef 0411 02ef 0412  ................
-00003c40: 02ee 0413 02ed 0413 02ed 0413 02ed 0413  ................
-00003c50: 02ed 0414 02ec 0414 02ec 0414 02ec 081a  ................
-00003c60: 0201 02ff 0402 02fe 0403 02fd 0806 0203  ................
-00003c70: 02fd 0405 02fb 0406 02fa 0407 02f9 0407  ................
-00003c80: 02f9 0407 02f9 0407 02f9 0408 02f8 0408  ................
-00003c90: 02f8 0408 02f8 0408 02f8 0408 02f8 0409  ................
-00003ca0: 02f7 0409 02f7 0409 02f7 0409 02f7 0409  ................
-00003cb0: 02f7 0409 02f7 0409 02f7 040a 02f6 040a  ................
-00003cc0: 02f6 040a 02f6 040a 02f6 040b 02f5 040b  ................
-00003cd0: 02f5 040b 02f5 040b 02f5 040f 02f1 040f  ................
-00003ce0: 02f1 0411 02ef 0411 02ef 0413 02ed 0413  ................
-00003cf0: 02ed 0415 02eb 0415 02eb 0417 02e9 0417  ................
-00003d00: 02e9 0417 02e9 0417 02e9 081d 080a 101b  ................
-00003d10: 0c0e 081e 0c10 080f 0816 0c10 0c11 0828  ...............(
-00003d20: 080d 0604 0c11 0818 0808 0603 0c08       ..............
+00003270: 6172 6961 626c 6573 2e64 6566 6175 6c74  ariables.default
+00003280: 5f76 6172 6961 626c 6573 7207 0000 005a  _variablesr....Z
+00003290: 2868 686e 6b5f 7468 7265 6564 695f 746f  (hhnk_threedi_to
+000032a0: 6f6c 732e 7661 7269 6162 6c65 732e 6d6f  ols.variables.mo
+000032b0: 6465 6c5f 7374 6174 6572 0800 0000 7209  del_stater....r.
+000032c0: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+000032d0: 0000 720d 0000 005a 2268 686e 6b5f 7468  ..r....Z"hhnk_th
+000032e0: 7265 6564 695f 746f 6f6c 732e 7661 7269  reedi_tools.vari
+000032f0: 6162 6c65 732e 7765 6972 7372 0e00 0000  ables.weirsr....
+00003300: 7225 0000 0072 2c00 0000 da0e 615f 636f  r%...r,.....a_co
+00003310: 6e6e 5f6e 6f64 655f 6964 da16 696e 6974  nn_node_id..init
+00003320: 6961 6c5f 7761 7465 726c 6576 656c 5f63  ial_waterlevel_c
+00003330: 6f6c 725f 0000 0072 7600 0000 7275 0000  olr_...rv...ru..
+00003340: 0072 7800 0000 7263 0000 00da 1063 6f6e  .rx...rc.....con
+00003350: 6e5f 6e6f 6465 735f 7175 6572 795a 1361  n_nodes_queryZ.a
+00003360: 5f77 6174 6572 7375 7266 5f63 6f6e 6e5f  _watersurf_conn_
+00003370: 6964 5a1c 7761 7465 7273 7572 6661 6365  idZ.watersurface
+00003380: 5f63 6f6e 6e5f 6e6f 6465 5f71 7565 7279  _conn_node_query
+00003390: 7243 0000 00da 0861 5f6d 616e 5f69 6472  rC.....a_man_idr
+000033a0: 4600 0000 da0d 615f 6d61 6e5f 636f 6e6e  F.....a_man_conn
+000033b0: 5f69 6472 4500 0000 724b 0000 00da 0e6d  _idrE...rK.....m
+000033c0: 616e 686f 6c65 735f 7175 6572 7972 6800  anholes_queryrh.
+000033d0: 0000 da09 615f 6368 616e 5f69 645a 0c61  ....a_chan_idZ.a
+000033e0: 5f63 6f6e 6e5f 6e6f 6465 7372 7100 0000  _conn_nodesrq...
+000033f0: da0e 6368 616e 6e65 6c73 5f71 7565 7279  ..channels_query
+00003400: 7265 0000 0072 7900 0000 726b 0000 0072  re...ry...rk...r
+00003410: 6600 0000 7264 0000 00da 1c63 726f 7373  f...rd.....cross
+00003420: 5f73 6563 7469 6f6e 5f6c 6f63 6174 696f  _section_locatio
+00003430: 6e5f 7175 6572 795a 0b61 5f63 6861 6e5f  n_queryZ.a_chan_
+00003440: 636f 6465 7272 0000 005a 0e61 5f63 6861  coderr...Z.a_cha
+00003450: 6e5f 6e6f 6465 5f69 6472 4e00 0000 5a0a  n_node_idrN...Z.
+00003460: 615f 7a6f 6f6d 5f63 6174 5a12 615f 6372  a_zoom_catZ.a_cr
+00003470: 6f73 735f 7365 635f 6c6f 635f 6964 5a14  oss_sec_loc_idZ.
+00003480: 615f 6372 6f73 735f 7365 635f 6c6f 635f  a_cross_sec_loc_
+00003490: 636f 6465 5a0a 6465 665f 6964 5f63 6f6c  codeZ.def_id_col
+000034a0: 7282 0000 005a 1261 5f63 726f 7373 5f73  r....Z.a_cross_s
+000034b0: 6563 5f64 6566 5f69 6472 4800 0000 5a0a  ec_def_idrH...Z.
+000034c0: 6865 6967 6874 5f63 6f6c 5a13 7072 6f66  height_colZ.prof
+000034d0: 696c 6573 5f75 7365 645f 7175 6572 795a  iles_used_queryZ
+000034e0: 1f62 616e 6b5f 6c76 6c73 5f73 6f75 7263  .bank_lvls_sourc
+000034f0: 655f 6372 6561 7469 6f6e 5f71 7565 7279  e_creation_query
+00003500: 5a1d 6261 6e6b 5f6c 766c 735f 736f 7572  Z.bank_lvls_sour
+00003510: 6365 5f75 7064 6174 655f 7175 6572 795a  ce_update_queryZ
+00003520: 1662 616e 6b5f 6c76 6c73 5f6c 6173 745f  .bank_lvls_last_
+00003530: 6368 616e 6765 6472 4a00 0000 5a17 6973  changedrJ...Z.is
+00003540: 6f6c 6174 6564 5f63 6861 6e6e 656c 735f  olated_channels_
+00003550: 7175 6572 7972 8b00 0000 5a10 6372 6f73  queryr....Z.cros
+00003560: 735f 6465 665f 6964 5f63 6f6c 7285 0000  s_def_id_colr...
+00003570: 0072 8800 0000 5a17 7765 6972 5f77 6964  .r....Z.weir_wid
+00003580: 7468 5f62 6163 6b75 705f 7175 6572 7972  th_backup_queryr
+00003590: 8300 0000 5a0b 615f 7765 6972 5f63 6f64  ....Z.a_weir_cod
+000035a0: 655a 0961 5f77 6569 725f 6964 5a1d 7765  eZ.a_weir_idZ.we
+000035b0: 6972 5f77 6964 7468 735f 6672 6f6d 5f62  ir_widths_from_b
+000035c0: 6163 6b75 705f 7175 6572 795a 2063 6f6e  ackup_queryZ con
+000035d0: 7472 6f6c 6c65 645f 7765 6972 735f 7365  trolled_weirs_se
+000035e0: 6c65 6374 696f 6e5f 7175 6572 795a 1961  lection_queryZ.a
+000035f0: 5f77 6569 725f 636f 6e6e 5f6e 6f64 655f  _weir_conn_node_
+00003600: 7374 6172 745f 6964 5a17 615f 7765 6972  start_idZ.a_weir
+00003610: 5f63 6f6e 6e5f 6e6f 6465 5f65 6e64 5f69  _conn_node_end_i
+00003620: 6472 8600 0000 5a19 615f 7765 6972 5f63  dr....Z.a_weir_c
+00003630: 6861 6e5f 636f 6e6e 5f73 7461 7274 5f69  han_conn_start_i
+00003640: 645a 1761 5f77 6569 725f 6368 616e 5f63  dZ.a_weir_chan_c
+00003650: 6f6e 6e5f 656e 645f 6964 726a 0000 0072  onn_end_idrj...r
+00003660: 8700 0000 5a11 7765 6972 5f68 6569 6768  ....Z.weir_heigh
+00003670: 745f 7175 6572 795a 0861 7265 615f 636f  t_queryZ.area_co
+00003680: 6c5a 1869 6d70 6572 7669 6f75 735f 7375  lZ.impervious_su
+00003690: 7266 6163 655f 6c61 7965 725a 1869 6d70  rface_layerZ.imp
+000036a0: 6572 7669 6f75 735f 7375 7266 6163 655f  ervious_surface_
+000036b0: 7175 6572 795a 0866 5f70 6f69 6e74 6e5a  queryZ.f_pointnZ
+000036c0: 1161 5f67 656f 5f73 7461 7274 5f63 6f6f  .a_geo_start_coo
+000036d0: 7264 5a0b 665f 6e75 6d70 6f69 6e74 735a  rdZ.f_numpointsZ
+000036e0: 0f61 5f67 656f 5f65 6e64 5f63 6f6f 7264  .a_geo_end_coord
+000036f0: 5a10 615f 6765 6f5f 7374 6172 745f 6e6f  Z.a_geo_start_no
+00003700: 6465 5a0e 615f 6765 6f5f 656e 645f 6e6f  deZ.a_geo_end_no
+00003710: 6465 5a14 615f 6765 6f5f 636f 6e6e 5f6e  deZ.a_geo_conn_n
+00003720: 6f64 6573 5f65 6e64 5a16 615f 6765 6f5f  odes_endZ.a_geo_
+00003730: 636f 6e6e 5f6e 6f64 6573 5f73 7461 7274  conn_nodes_start
+00003740: 728e 0000 0072 2900 0000 7233 0000 0072  r....r)...r3...r
+00003750: 3e00 0000 7254 0000 0072 5700 0000 7250  >...rT...rW...rP
+00003760: 0000 0072 6700 0000 7269 0000 0072 6c00  ...rg...ri...rl.
+00003770: 0000 727d 0000 0072 8100 0000 5a18 7374  ..r}...r....Z.st
+00003780: 7275 6374 5f63 6861 6e6e 656c 5f62 6564  ruct_channel_bed
+00003790: 5f71 7565 7279 7284 0000 0072 8a00 0000  _queryr....r....
+000037a0: 728c 0000 005a 1b63 6f6e 7472 6f6c 6c65  r....Z.controlle
+000037b0: 645f 7374 7275 6374 7572 6573 5f71 7565  d_structures_que
+000037c0: 7279 7290 0000 0072 7000 0000 5a14 6765  ryr....rp...Z.ge
+000037d0: 6f6d 6574 7279 5f63 6865 636b 5f71 7565  ometry_check_que
+000037e0: 7279 7227 0000 0072 2700 0000 7227 0000  ryr'...r'...r'..
+000037f0: 0072 2800 0000 da08 3c6d 6f64 756c 653e  .r(.....<module>
+00003800: 0200 0000 73a4 0400 0004 0a08 0108 0214  ....s...........
+00003810: 050c 0308 0408 010c 0120 080c 0402 0102  ......... ......
+00003820: ff08 0602 0102 ff04 0102 ff04 0202 fe04  ................
+00003830: 0302 fd04 0402 fc04 0402 fc04 0402 fc04  ................
+00003840: 0502 fb08 0802 0102 ff04 0102 ff04 0202  ................
+00003850: fe04 0302 fd04 0402 fc04 0402 fc04 0402  ................
+00003860: fc04 0502 fb08 0902 0202 fe04 0202 fe04  ................
+00003870: 0202 fe04 0302 fd04 0302 fd04 0302 fd04  ................
+00003880: 0402 fc04 0402 fc04 0502 fb04 0502 fb04  ................
+00003890: 0602 fa04 0602 fa04 0702 f904 0702 f904  ................
+000038a0: 0802 f804 0802 f804 0802 f804 0802 f804  ................
+000038b0: 0902 f704 0a02 f604 0b02 f504 0b02 f504  ................
+000038c0: 0b02 f504 0b02 f508 0f02 0202 fe04 0202  ................
+000038d0: fe04 0202 fe04 0302 fd04 0302 fd04 0302  ................
+000038e0: fd04 0302 fd04 0302 fd04 0302 fd04 0402  ................
+000038f0: fc04 0502 fb04 0502 fb04 0602 fa04 0602  ................
+00003900: fa04 0602 fa04 0602 fa08 0902 0202 fe04  ................
+00003910: 0202 fe04 0302 fd04 0402 fc04 0502 fb04  ................
+00003920: 0502 fb04 0502 fb04 0502 fb04 0602 fa08  ................
+00003930: 0802 0202 fe04 0202 fe04 0202 fe04 0302  ................
+00003940: fd04 0302 fd04 0302 fd04 0402 fc04 0402  ................
+00003950: fc04 0402 fc04 0502 fb04 0502 fb04 0502  ................
+00003960: fb04 0602 fa04 0602 fa04 0602 fa04 0602  ................
+00003970: fa04 0702 f904 0702 f904 0702 f904 0802  ................
+00003980: f804 0802 f804 0802 f804 0902 f704 0902  ................
+00003990: f704 0a02 f604 0a02 f604 0b02 f504 0b02  ................
+000039a0: f504 0c02 f404 0c02 f404 0c02 f404 0d02  ................
+000039b0: f304 0d02 f304 0e02 f204 0e02 f204 0f02  ................
+000039c0: f104 0f02 f104 1002 f004 1102 ef04 1102  ................
+000039d0: ef04 1102 ef04 1102 ef04 1102 ef04 1202  ................
+000039e0: ee04 1202 ee04 1202 ee04 1202 ee04 1202  ................
+000039f0: ee04 1302 ed04 1302 ed04 1302 ed04 1302  ................
+00003a00: ed04 1302 ed04 1402 ec04 1402 ec08 160c  ................
+00003a10: 010c 010c 0202 0102 ff04 0202 fe04 0302  ................
+00003a20: fd04 0302 fd04 0302 fd04 0402 fc08 0802  ................
+00003a30: 0102 ff04 0102 ff04 0302 fd04 0302 fd04  ................
+00003a40: 0402 fc04 0502 fb04 0502 fb04 0502 fb04  ................
+00003a50: 0502 fb04 0502 fb04 0602 fa04 0602 fa04  ................
+00003a60: 0602 fa04 0602 fa04 0602 fa08 0902 0202  ................
+00003a70: fe04 0202 fe04 0202 fe04 0302 fd04 0302  ................
+00003a80: fd04 0302 fd04 0402 fc04 0402 fc04 0402  ................
+00003a90: fc04 0502 fb04 0502 fb04 0602 fa04 0702  ................
+00003aa0: f904 0702 f904 0702 f904 0702 f904 0702  ................
+00003ab0: f904 0802 f804 0802 f804 0802 f804 0802  ................
+00003ac0: f804 0802 f808 0a02 0202 fe04 0202 fe04  ................
+00003ad0: 0202 fe04 0302 fd04 0302 fd04 0302 fd04  ................
+00003ae0: 0402 fc04 0402 fc04 0402 fc04 0502 fb04  ................
+00003af0: 0502 fb04 0602 fa04 0702 f904 0702 f904  ................
+00003b00: 0702 f904 0702 f904 0702 f904 0802 f804  ................
+00003b10: 0802 f804 0802 f804 0802 f804 0802 f808  ................
+00003b20: 0b02 0102 ff04 0102 ff04 0202 fe04 0202  ................
+00003b30: fe04 0302 fd04 0302 fd04 0402 fc04 0402  ................
+00003b40: fc04 0502 fb04 0502 fb04 0502 fb04 0602  ................
+00003b50: fa04 0602 fa04 0602 fa04 0702 f904 0702  ................
+00003b60: f904 0702 f904 0802 f804 0802 f804 0902  ................
+00003b70: f704 0902 f704 0902 f704 0a02 f604 0a02  ................
+00003b80: f604 0a02 f604 0a02 f604 0b02 f504 0c02  ................
+00003b90: f404 0d02 f304 0d02 f304 0d02 f304 0e02  ................
+00003ba0: f204 0f02 f104 0f02 f104 0f02 f104 0f02  ................
+00003bb0: f104 0f02 f104 1002 f004 1002 f004 1002  ................
+00003bc0: f004 1002 f004 1002 f004 1102 ef04 1102  ................
+00003bd0: ef04 1202 ee04 1302 ed04 1302 ed04 1302  ................
+00003be0: ed04 1302 ed04 1402 ec04 1402 ec04 1402  ................
+00003bf0: ec08 1a02 0102 ff04 0202 fe04 0302 fd08  ................
+00003c00: 0602 0302 fd04 0502 fb04 0602 fa04 0702  ................
+00003c10: f904 0702 f904 0702 f904 0802 f804 0802  ................
+00003c20: f804 0802 f804 0802 f804 0902 f704 0902  ................
+00003c30: f704 0902 f704 0902 f704 0902 f704 0902  ................
+00003c40: f704 0a02 f604 0a02 f604 0a02 f604 0b02  ................
+00003c50: f504 0b02 f504 0b02 f504 0f02 f104 0f02  ................
+00003c60: f104 1102 ef04 1102 ef04 1302 ed04 1302  ................
+00003c70: ed04 1502 eb04 1502 eb04 1702 e904 1702  ................
+00003c80: e904 1702 e904 1702 e908 1d08 0a10 1b0c  ................
+00003c90: 0e08 1e0c 1008 0f08 160c 100c 1108 2808  ..............(.
+00003ca0: 0d06 040c 1108 1808 0806 030c 08         .............
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Nov  6 13:43:31 2023 UTC, .py size: 25162 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 83ed 4865 4a62 0000  a.........HeJb..
+00000000: 610d 0d0a 0000 0000 3ac5 3066 4e62 0000  a.......:.0fNb..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 002a 0000 0040 0000 0073 3e08 0000 6400  .*...@...s>...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
@@ -37,15 +37,15 @@
 00000240: 9b00 6439 6505 9b00 9d03 6512 6507 a105  ..d9e.....e.e...
 00000250: 6545 6435 6544 6436 6437 6437 6438 8d03  eEd5eDd6d7d7d8..
 00000260: 1700 642e 8d01 a04a 6546 6523 652b 8302  ..d....JeFe#e+..
 00000270: 6523 6523 9b00 6439 6512 9b00 9d03 6522  e#e#..d9e.....e"
 00000280: 6524 a105 6545 6435 6544 6436 6437 6437  e$..eEd5eDd6d7d7
 00000290: 6438 8d03 1700 642e 8d01 a04a 6546 6515  d8....d....JeFe.
 000002a0: 652c 8302 6515 6515 9b00 6439 6512 9b00  e,..e.e...d9e...
-000002b0: 9d03 6513 6514 a105 6545 6422 6544 643a  ..e.e...eEd"eDd:
+000002b0: 9d03 6512 6514 a105 6545 6422 6544 643a  ..e.e...eEd"eDd:
 000002c0: 6437 6437 6544 6436 6437 6437 643b 8d03  d7d7eDd6d7d7d;..
 000002d0: 643c 8d04 1700 642e 8d01 a04a 6546 6507  d<....d....JeFe.
 000002e0: 652d 8302 6507 6507 9b00 6439 6512 9b00  e-..e.e...d9e...
 000002f0: 9d03 6515 9b00 6439 6505 9b00 9d03 6515  ..e...d9e.....e.
 00000300: 6515 9b00 6439 6513 9b00 9d03 6514 9b00  e...d9e.....e...
 00000310: 6439 6512 9b00 9d03 6514 a108 6545 643d  d9e.....e...eEd=
 00000320: 6422 643e 6901 643f 8d02 a04a 6546 6503  d"d>i.d?...JeFe.
@@ -182,604 +182,605 @@
 00000b50: 2073 6563 7469 6f6e 2064 6566 696e 6974   section definit
 00000b60: 696f 6e20 6865 6967 6874 206e 6f74 2075  ion height not u
 00000b70: 7365 6420 666f 7220 7368 6170 6520 7479  sed for shape ty
 00000b80: 7065 2031 7a41 4552 524f 523a 206d 756c  pe 1zAERROR: mul
 00000b90: 7469 706c 6520 6865 6967 6874 2061 6e64  tiple height and
 00000ba0: 2077 6964 7468 2065 6e74 7269 6573 206d   width entries m
 00000bb0: 7573 7420 6861 7665 2074 6865 2073 616d  ust have the sam
-00000bc0: 6520 636f 756e 747a 3145 5252 4f52 3a20  e countz1ERROR: 
-00000bd0: 696d 7065 7276 696f 7573 2073 7572 6661  impervious surfa
-00000be0: 6365 2069 7320 6e6f 7420 696e 206d 6170  ce is not in map
-00000bf0: 7069 6e67 2074 6162 6c65 7a39 4552 524f  ping tablez9ERRO
-00000c00: 523a 2069 6d70 6572 7669 6f75 7320 7375  R: impervious su
-00000c10: 7266 6163 6520 6d61 7020 7265 6665 7273  rface map refers
-00000c20: 2074 6f20 6e6f 6e2d 6578 6973 7465 6e74   to non-existent
-00000c30: 206e 6f64 657a 2645 5252 4f52 3a20 7375   nodez&ERROR: su
-00000c40: 7266 6163 6520 6973 206e 6f74 2069 6e20  rface is not in 
-00000c50: 6d61 7070 696e 6720 7461 626c 657a 4045  mapping tablez@E
-00000c60: 5252 4f52 3a20 696d 7065 7276 696f 7573  RROR: impervious
-00000c70: 2073 7572 6661 6365 206d 6170 2069 7320   surface map is 
-00000c80: 6e6f 7420 696e 2069 6d70 6572 7669 6f75  not in imperviou
-00000c90: 7320 7375 7266 6163 6520 6c61 7965 727a  s surface layerz
-00000ca0: 3145 5252 4f52 3a20 636f 6e6e 6563 7469  1ERROR: connecti
-00000cb0: 6f6e 206e 6f64 6520 7769 7468 6f75 7420  on node without 
-00000cc0: 696d 7065 7276 696f 7573 2073 7572 6661  impervious surfa
-00000cd0: 6365 7a2d 4552 524f 523a 2063 6861 6e6e  cez-ERROR: chann
-00000ce0: 656c 2077 6974 686f 7574 2063 726f 7373  el without cross
-00000cf0: 2073 6563 7469 6f6e 206c 6f63 6174 696f   section locatio
-00000d00: 6e7a 3045 5252 4f52 3a20 6372 6f73 7320  nz0ERROR: cross 
-00000d10: 7365 6374 696f 6e20 6c6f 6361 7469 6f6e  section location
-00000d20: 2077 6974 686f 7574 2064 6566 696e 6974   without definit
-00000d30: 696f 6e7a 2f45 5252 4f52 3a20 6375 6c76  ionz/ERROR: culv
-00000d40: 6572 7420 7769 7468 6f75 7420 6372 6f73  ert without cros
-00000d50: 7320 7365 6374 696f 6e20 6465 6669 6e69  s section defini
-00000d60: 7469 6f6e 7a2c 4552 524f 523a 2077 6569  tionz,ERROR: wei
-00000d70: 7220 7769 7468 6f75 7420 6372 6f73 7320  r without cross 
-00000d80: 7365 6374 696f 6e20 6465 6669 6e69 7469  section definiti
-00000d90: 6f6e 7a2f 4552 524f 523a 206f 7269 6669  onz/ERROR: orifi
-00000da0: 6365 2077 6974 686f 7574 2063 726f 7373  ce without cross
-00000db0: 2073 6563 7469 6f6e 2064 6566 696e 6974   section definit
-00000dc0: 696f 6e7a 2645 5252 4f52 3a20 6d61 6e68  ionz&ERROR: manh
-00000dd0: 6f6c 6520 7769 7468 6f75 7420 636f 6e6e  ole without conn
-00000de0: 6563 7469 6f6e 206e 6f64 657a 2c57 4152  ection nodez,WAR
-00000df0: 4e49 4e47 3a20 3164 2062 6f75 6e64 6172  NING: 1d boundar
-00000e00: 7920 7769 7468 6f75 7420 636f 6e6e 6563  y without connec
-00000e10: 7469 6f6e 206e 6f64 657a 3545 5252 4f52  tion nodez5ERROR
-00000e20: 3a20 6372 6f73 7320 7365 6374 696f 6e20  : cross section 
-00000e30: 6c6f 6361 7469 6f6e 2077 6974 686f 7574  location without
-00000e40: 2072 6566 6572 656e 6365 206c 6576 656c   reference level
-00000e50: 7a33 5741 524e 494e 473a 2063 6f6e 6e65  z3WARNING: conne
-00000e60: 6374 696f 6e20 6e6f 6465 2077 6974 686f  ction node witho
-00000e70: 7574 2069 6e69 7469 616c 2077 6174 6572  ut initial water
-00000e80: 6c65 7665 6c7a 1e45 5252 4f52 3a20 6e6f  levelz.ERROR: no
-00000e90: 6465 2077 6974 686f 7574 2063 6f6e 6e65  de without conne
-00000ea0: 6374 696f 6e7a 4557 4152 4e49 4e47 3a20  ctionzEWARNING: 
-00000eb0: 7374 6172 7420 6c65 7665 6c20 666f 7220  start level for 
-00000ec0: 7075 6d70 2073 7461 7469 6f6e 206e 6f74  pump station not
-00000ed0: 2063 6c6f 7365 2074 6f20 696e 6974 6961   close to initia
-00000ee0: 6c20 7761 7465 726c 6576 656c 7a24 4552  l waterlevelz$ER
-00000ef0: 524f 523a 2073 6861 7065 206f 7220 7769  ROR: shape or wi
-00000f00: 6474 6820 6973 206e 6f74 2064 6566 696e  dth is not defin
-00000f10: 6564 7a37 4552 524f 523a 2070 756d 7073  edz7ERROR: pumps
-00000f20: 7461 7469 6f6e 2066 726f 6d20 616e 6420  tation from and 
-00000f30: 746f 2074 6865 2073 616d 6520 636f 6e6e  to the same conn
-00000f40: 6563 7469 6f6e 206e 6f64 657a 3045 5252  ection nodez0ERR
-00000f50: 4f52 3a20 7765 6972 2066 726f 6d20 616e  OR: weir from an
-00000f60: 6420 746f 2074 6865 2073 616d 6520 636f  d to the same co
-00000f70: 6e6e 6563 7469 6f6e 206e 6f64 657a 3345  nnection nodez3E
-00000f80: 5252 4f52 3a20 6f72 6966 6963 6520 6672  RROR: orifice fr
-00000f90: 6f6d 2061 6e64 2074 6f20 7468 6520 7361  om and to the sa
-00000fa0: 6d65 2063 6f6e 6e65 6374 696f 6e20 6e6f  me connection no
-00000fb0: 6465 7a33 4552 524f 523a 2063 756c 7665  dez3ERROR: culve
-00000fc0: 7274 2066 726f 6d20 616e 6420 746f 2074  rt from and to t
-00000fd0: 6865 2073 616d 6520 636f 6e6e 6563 7469  he same connecti
-00000fe0: 6f6e 206e 6f64 657a 5827 5741 524e 494e  on nodezX'WARNIN
-00000ff0: 473a 2073 7461 7274 206c 6576 656c 2027  G: start level '
-00001000: 207c 7c20 7b7d 207c 7c20 2720 6e6f 7420   || {} || ' not 
-00001010: 636c 6f73 6520 746f 2069 6e69 7469 616c  close to initial
-00001020: 2077 6174 6572 6c65 7665 6c20 2720 7c7c   waterlevel ' ||
-00001030: 207b 7d20 7c7c 2027 2c20 2720 7c7c 207b   {} || ', ' || {
-00001040: 7d7a 5727 5741 524e 494e 473a 2069 6e69  }zW'WARNING: ini
-00001050: 7469 616c 2077 6174 6572 206c 6576 656c  tial water level
-00001060: 2061 7420 7374 6172 7420 616e 6420 656e   at start and en
-00001070: 6420 6e6f 6465 2061 7265 206e 6f74 2065  d node are not e
-00001080: 7175 616c 2027 207c 7c20 7b7d 207c 7c20  qual ' || {} || 
-00001090: 272c 2027 207c 7c20 7b7d 7a50 2757 4152  ', ' || {}zP'WAR
-000010a0: 4e49 4e47 3a20 496e 6974 6961 6c20 7761  NING: Initial wa
-000010b0: 7465 726c 6576 656c 2061 7420 7374 6172  terlevel at star
-000010c0: 7420 656e 2065 6e64 206e 6f64 6520 6e6f  t en end node no
-000010d0: 7420 6571 7561 6c27 207c 7c20 7b7d 207c  t equal' || {} |
-000010e0: 7c20 272c 2027 207c 7c20 7b7d 7a32 4552  | ', ' || {}z2ER
-000010f0: 524f 523a 2070 6572 6365 6e74 6167 6520  ROR: percentage 
-00001100: 3d20 3130 3020 616e 6420 7368 6f75 6c64  = 100 and should
-00001110: 2062 6520 3134 2e34 206f 7220 3131 2e35   be 14.4 or 11.5
-00001120: 7a44 4552 524f 523a 2061 6374 696f 6e5f  zDERROR: action_
-00001130: 7461 626c 6520 6861 7320 6d6f 7265 2074  table has more t
-00001140: 6861 6e20 3130 3030 2063 6861 7261 6374  han 1000 charact
-00001150: 6572 7320 286d 6f64 656c 2077 696c 6c20  ers (model will 
-00001160: 6372 6173 6829 464e 6304 0000 0000 0000  crash)FNc.......
-00001170: 0000 0000 0005 0000 0003 0000 0043 0000  .............C..
-00001180: 0073 4000 0000 6401 7c00 1700 6402 1700  .s@...d.|...d...
-00001190: 7d04 7c01 7218 7c04 6403 3700 7d04 7c02  }.|.r.|.d.7.}.|.
-000011a0: 7224 7c04 6404 3700 7d04 7c03 7234 7c04  r$|.d.7.}.|.r4|.
-000011b0: 6405 7c03 1700 3700 7d04 7c04 6406 3700  d.|...7.}.|.d.7.
-000011c0: 7d04 7c04 5300 2907 61c6 0100 000a 2020  }.|.S.).a.....  
-000011d0: 2020 2020 2020 636f 6e73 7472 5f69 6e5f        constr_in_
-000011e0: 636c 6175 7365 280a 2020 2020 2020 2020  clause(.        
-000011f0: 2020 2020 696e 6e6f 7469 6e20 2873 7472      innotin (str
-00001200: 696e 673a 2065 6974 6865 7220 2749 4e27  ing: either 'IN'
-00001210: 206f 7220 274e 4f54 2049 4e27 290a 2020   or 'NOT IN').  
-00001220: 2020 2020 2020 2020 2020 7365 6c20 2d3e            sel ->
-00001230: 2046 616c 7365 2028 626f 6f6c 3a20 6164   False (bool: ad
-00001240: 6420 2753 454c 4543 5420 7b7d 2720 6c69  d 'SELECT {}' li
-00001250: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00001260: 6672 6d20 2d3e 2046 616c 7365 2028 626f  frm -> False (bo
-00001270: 6f6c 3a20 6164 6420 2746 524f 4d20 7b7d  ol: add 'FROM {}
-00001280: 2720 6c69 6e65 290a 2020 2020 2020 2020  ' line).        
-00001290: 2020 2020 7768 6572 6520 2d3e 2046 616c      where -> Fal
-000012a0: 7365 2028 626f 6f6c 3a20 6164 6420 2757  se (bool: add 'W
-000012b0: 4845 5245 207b 7d27 206c 696e 6529 0a20  HERE {}' line). 
-000012c0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-000012d0: 2020 436f 6e73 7472 7563 7473 2061 2049    Constructs a I
-000012e0: 4e20 6f72 204e 4f54 2049 4e20 7365 6c65  N or NOT IN sele
-000012f0: 6374 696f 6e20 636c 6175 7365 2e0a 2020  ction clause..  
-00001300: 2020 4578 3a0a 2020 2020 2020 2020 494e    Ex:.        IN
-00001310: 0a20 2020 2020 2020 2028 5345 4c45 4354  .        (SELECT
-00001320: 207b 7d0a 2020 2020 2020 2020 4652 4f4d   {}.        FROM
-00001330: 207b 7d0a 2020 2020 2020 2020 5748 4552   {}.        WHER
-00001340: 4520 7b7d 290a 0a20 2020 2057 6869 6368  E {})..    Which
-00001350: 2063 616e 2074 6865 6e20 6265 2066 6f72   can then be for
-00001360: 6d61 7474 6564 2074 6f20 696e 7365 7274  matted to insert
-00001370: 2074 6162 6c65 206e 616d 6573 2061 6e64   table names and
-00001380: 2063 6f6e 6469 7469 6f6e 2065 7463 0a20   condition etc. 
-00001390: 2020 20da 0120 7a02 280a 7a0a 5345 4c45     .. z.(.z.SELE
-000013a0: 4354 207b 7d0a 7a08 4652 4f4d 207b 7d0a  CT {}.z.FROM {}.
-000013b0: 7a08 5748 4552 4520 7b7d fa01 29a9 0029  z.WHERE {}..)..)
-000013c0: 05da 0769 6e6e 6f74 696e da03 7365 6cda  ...innotin..sel.
-000013d0: 0366 726d da05 7768 6572 65da 0372 6573  .frm..where..res
-000013e0: 722a 0000 0072 2a00 0000 fa5a 653a 5c67  r*...r*....Ze:\g
-000013f0: 6974 6875 625c 7776 616e 6765 7277 656e  ithub\wvangerwen
-00001400: 5c68 686e 6b2d 7468 7265 6564 692d 746f  \hhnk-threedi-to
-00001410: 6f6c 735c 6868 6e6b 5f74 6872 6565 6469  ols\hhnk_threedi
-00001420: 5f74 6f6f 6c73 5c75 7469 6c73 5c71 7565  _tools\utils\que
-00001430: 7269 6573 5f67 656e 6572 616c 5f63 6865  ries_general_che
-00001440: 636b 732e 7079 da10 636f 6e73 7472 5f69  cks.py..constr_i
-00001450: 6e5f 636c 6175 7365 5200 0000 7312 0000  n_clauseR...s...
-00001460: 0000 120c 0104 0108 0104 0108 0104 010c  ................
-00001470: 0108 0172 3100 0000 7a02 7b7d 6305 0000  ...r1...z.{}c...
-00001480: 0000 0000 0000 0000 0007 0000 0005 0000  ................
-00001490: 0043 0000 0073 9000 0000 6401 7d05 7c00  .C...s....d.}.|.
-000014a0: 7218 7c05 6402 7c00 1700 6403 1700 3700  r.|.d.|...d...7.
-000014b0: 7d05 7c01 722c 7c05 6404 7c01 1700 6403  }.|.r,|.d.|...d.
-000014c0: 1700 3700 7d05 7c03 4400 5d20 7d06 7c05  ..7.}.|.D.] }.|.
-000014d0: 6405 7c06 1700 6406 1700 7c03 7c06 1900  d.|...d...|.|...
-000014e0: 1700 6403 1700 3700 7d05 7130 7c04 4400  ..d...7.}.q0|.D.
-000014f0: 5d20 7d06 7c05 6407 7c06 1700 6406 1700  ] }.|.d.|...d...
-00001500: 7c04 7c06 1900 1700 6403 1700 3700 7d05  |.|.....d...7.}.
-00001510: 7156 7c02 728c 7c05 6408 7c02 1700 6403  qV|.r.|.d.|...d.
-00001520: 1700 3700 7d05 7c05 5300 2909 61aa 0200  ..7.}.|.S.).a...
-00001530: 000a 2020 2020 436f 6e73 7472 7563 7473  ..    Constructs
-00001540: 2073 656c 6563 7420 2f20 6672 6f6d 202f   select / from /
-00001550: 2077 6865 7265 2071 7565 7279 2077 6974   where query wit
-00001560: 6820 706f 7373 6962 6c65 206a 6f69 6e20  h possible join 
-00001570: 636c 6175 7365 7320 2869 6e6e 6572 206f  clauses (inner o
-00001580: 7220 6c65 6674 206a 6f69 6e29 0a0a 2020  r left join)..  
-00001590: 2020 2020 2020 636f 6e73 7472 7563 745f        construct_
-000015a0: 7365 6c5f 6672 6f6d 5f77 6865 7265 5f71  sel_from_where_q
-000015b0: 7565 7279 280a 2020 2020 2020 2020 2020  uery(.          
-000015c0: 2020 2020 2020 7365 6c20 2d3e 2027 7b7d        sel -> '{}
-000015d0: 2720 2873 7472 696e 672c 2077 6861 7465  ' (string, whate
-000015e0: 7665 7220 636f 6d65 7320 6166 7465 7220  ver comes after 
-000015f0: 2753 454c 4543 5420 2720 6b65 7977 6f72  'SELECT ' keywor
-00001600: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-00001610: 2020 2066 726f 6d20 2d3e 2027 7b7d 2720     from -> '{}' 
-00001620: 2873 7472 696e 672c 2077 6861 7465 7665  (string, whateve
-00001630: 7220 636f 6d65 7320 6166 7465 7220 2746  r comes after 'F
-00001640: 524f 4d20 2720 6b65 7977 6f72 6429 0a20  ROM ' keyword). 
-00001650: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00001660: 6865 7265 202d 3e20 277b 7d27 2028 7374  here -> '{}' (st
-00001670: 7269 6e67 2c20 7768 6174 6576 6572 2063  ring, whatever c
-00001680: 6f6d 6573 2061 6674 6572 2027 5748 4552  omes after 'WHER
-00001690: 4520 2720 6b65 7977 6f72 6429 0a20 2020  E ' keyword).   
-000016a0: 2020 2020 2020 2020 2020 2020 206c 6566               lef
-000016b0: 745f 6a6f 696e 202d 3e20 7b7d 2028 6469  t_join -> {} (di
-000016c0: 6374 696f 6e61 7279 2c20 7265 7475 726e  ctionary, return
-000016d0: 6564 2061 7320 274c 4546 5420 4a4f 494e  ed as 'LEFT JOIN
-000016e0: 207b 6b65 797d 204f 4e20 7b76 616c 7565   {key} ON {value
-000016f0: 7d20 666f 7220 6576 6572 7920 656e 7472  } for every entr
-00001700: 7920 696e 2064 6963 7429 0a20 2020 2020  y in dict).     
-00001710: 2020 2020 2020 2020 2020 2069 6e6e 6572             inner
-00001720: 5f6a 6f69 6e20 2d3e 207b 7d20 2864 6963  _join -> {} (dic
-00001730: 7469 6f6e 6172 792c 2072 6574 7572 6e65  tionary, returne
-00001740: 6420 6173 2027 494e 4e45 5220 4a4f 494e  d as 'INNER JOIN
-00001750: 207b 6b65 797d 204f 4e20 7b76 616c 7565   {key} ON {value
-00001760: 7d20 666f 7220 6576 6572 7920 656e 7472  } for every entr
-00001770: 7920 696e 2064 6963 7429 0a20 2020 2020  y in dict).     
-00001780: 2020 2020 2020 2029 0a0a 2020 2020 5265         )..    Re
-00001790: 7475 726e 7320 6569 7468 6572 2066 756c  turns either ful
-000017a0: 6c20 7175 6572 7920 6f72 2074 656d 706c  l query or templ
-000017b0: 6174 6520 746f 2066 6f72 6d61 7420 6c61  ate to format la
-000017c0: 7465 7220 6465 7065 6e64 696e 6720 6f6e  ter depending on
-000017d0: 2069 6e70 7574 0a20 2020 20da 007a 0753   input.    ..z.S
-000017e0: 454c 4543 5420 da01 0a7a 0546 524f 4d20  ELECT ...z.FROM 
-000017f0: 7a0a 4c45 4654 204a 4f49 4e20 7a04 0a4f  z.LEFT JOIN z..O
-00001800: 4e20 7a0b 494e 4e45 5220 4a4f 494e 207a  N z.INNER JOIN z
-00001810: 0657 4845 5245 2072 2a00 0000 2907 722c  .WHERE r*...).r,
-00001820: 0000 0072 2d00 0000 722e 0000 00da 096c  ...r-...r......l
-00001830: 6566 745f 6a6f 696e da0a 696e 6e65 725f  eft_join..inner_
-00001840: 6a6f 696e 722f 0000 00da 036b 6579 722a  joinr/.....keyr*
-00001850: 0000 0072 2a00 0000 7230 0000 00da 1e63  ...r*...r0.....c
-00001860: 6f6e 7374 7275 6374 5f73 656c 5f66 726f  onstruct_sel_fro
-00001870: 6d5f 7768 6572 655f 7175 6572 796f 0000  m_where_queryo..
-00001880: 0073 1800 0000 000e 0401 0401 1001 0401  .s..............
-00001890: 1001 0801 1e01 0801 1e01 0401 1001 7237  ..............r7
-000018a0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000018b0: 0300 0000 0900 0000 4300 0000 7322 0000  ........C...s"..
-000018c0: 0064 017c 009b 0064 027c 009b 0064 0374  .d.|...d.|...d.t
-000018d0: 009b 0064 047c 019b 0064 059d 097d 027c  ...d.|...d...}.|
-000018e0: 0253 0029 064e fa01 27fa 1127 2061 7320  .S.).N..'..' as 
-000018f0: 7461 626c 655f 6e61 6d65 2c0a da01 2e7a  table_name,....z
-00001900: 0920 6173 2069 642c 0a27 7a0a 2720 6173  . as id,.'z.' as
-00001910: 2065 7272 6f72 a901 7213 0000 00a9 03da   error..r.......
-00001920: 0574 6162 6c65 da03 6d73 6772 2f00 0000  .table..msgr/...
-00001930: 722a 0000 0072 2a00 0000 7230 0000 00da  r*...r*...r0....
-00001940: 1463 6f6e 7374 7275 6374 5f71 7565 7279  .construct_query
-00001950: 5f68 6561 648b 0000 0073 0400 0000 0001  _head....s......
-00001960: 1e01 723f 0000 0063 0200 0000 0000 0000  ..r?...c........
-00001970: 0000 0000 0300 0000 0900 0000 4300 0000  ............C...
-00001980: 7322 0000 0064 017c 009b 0064 027c 009b  s"...d.|...d.|..
-00001990: 0064 0374 009b 0064 047c 019b 0064 059d  .d.t...d.|...d..
-000019a0: 097d 027c 0253 0029 064e 7238 0000 0072  .}.|.S.).Nr8...r
-000019b0: 3900 0000 723a 0000 007a 0820 6173 2069  9...r:...z. as i
-000019c0: 642c 0a7a 0920 6173 2065 7272 6f72 723b  d,.z. as errorr;
-000019d0: 0000 0072 3c00 0000 722a 0000 0072 2a00  ...r<...r*...r*.
-000019e0: 0000 7230 0000 00da 1e63 6f6e 7374 7275  ..r0.....constru
-000019f0: 6374 5f71 7565 7279 5f68 6561 645f 6e6f  ct_query_head_no
-00001a00: 5f71 756f 7465 7390 0000 0073 0400 0000  _quotes....s....
-00001a10: 0001 1e01 7240 0000 0063 0000 0000 0000  ....r@...c......
-00001a20: 0000 0000 0000 0600 0000 0800 0000 4300  ..............C.
-00001a30: 0000 7380 0000 0064 017d 0074 0074 0174  ..s....d.}.t.t.t
-00001a40: 0274 0374 0474 0567 067d 0174 067c 0183  .t.t.t.g.}.t.|..
-00001a50: 017d 0274 077c 0183 0144 005d 565c 027d  .}.t.|...D.]V\.}
-00001a60: 037d 0474 0874 0966 0244 005d 447d 057c  .}.t.t.f.D.]D}.|
-00001a70: 0074 0a64 0264 038d 01a0 0b7c 057c 047c  .t.d.d.....|.|.|
-00001a80: 05a1 0337 007d 007c 037c 0264 0418 0075  ...7.}.|.|.d...u
-00001a90: 0173 707c 037c 0264 0418 0075 0072 347c  .sp|.|.d...u.r4|
-00001aa0: 0574 0875 0072 347c 0064 0537 007d 0071  .t.u.r4|.d.7.}.q
-00001ab0: 3471 247c 0053 0029 064e 7232 0000 007a  4q$|.S.).Nr2...z
-00001ac0: 0e7b 7d20 4953 204e 4f54 204e 554c 4ca9  .{} IS NOT NULL.
-00001ad0: 0172 2e00 0000 e901 0000 00fa 0a55 4e49  .r...........UNI
-00001ae0: 4f4e 2041 4c4c 0a29 0c72 1f00 0000 7204  ON ALL.).r....r.
-00001af0: 0000 0072 0e00 0000 721e 0000 0072 2600  ...r....r....r&.
-00001b00: 0000 721c 0000 00da 036c 656e da09 656e  ..r......len..en
-00001b10: 756d 6572 6174 6572 0700 0000 7205 0000  umerater....r...
-00001b20: 0072 3700 0000 da06 666f 726d 6174 2906  .r7.....format).
-00001b30: da05 7175 6572 79da 066c 6179 6572 73da  ..query..layers.
-00001b40: 066c 656e 6774 68da 0169 da05 6c61 7965  .length..i..laye
-00001b50: 72da 046e 6f64 6572 2a00 0000 722a 0000  r..noder*...r*..
-00001b60: 0072 3000 0000 da24 636f 6e73 7472 5f63  .r0....$constr_c
-00001b70: 6f6e 6e5f 6e6f 6465 735f 7769 7468 6f75  onn_nodes_withou
-00001b80: 745f 636f 6e6e 5f71 7565 7279 9500 0000  t_conn_query....
-00001b90: 731e 0000 0000 0104 0202 0102 0102 0102  s...............
-00001ba0: 0102 0102 fa04 0808 0110 010c 0118 0120  ............... 
-00001bb0: 010c 0172 4d00 0000 6300 0000 0000 0000  ...rM...c.......
-00001bc0: 0000 0000 0006 0000 000a 0000 0043 0000  .............C..
-00001bd0: 0073 a400 0000 6401 7d00 7400 7401 7402  .s....d.}.t.t.t.
-00001be0: 7403 6704 7d01 7404 7c01 8301 7d02 7405  t.g.}.t.|...}.t.
-00001bf0: 7c01 8301 4400 5d7e 5c02 7d03 7d04 7c04  |...D.]~\.}.}.|.
-00001c00: 7400 6b02 7236 7406 7d05 6e20 7c04 7401  t.k.r6t.}.n |.t.
-00001c10: 6b02 7244 7407 7d05 6e12 7c04 7402 6b02  k.rDt.}.n.|.t.k.
-00001c20: 7252 7408 7d05 6e04 7409 7d05 7c00 740a  rRt.}.n.t.}.|.t.
-00001c30: 6402 6403 8d01 a00b 740c 7c04 7c05 8302  d.d.....t.|.|...
-00001c40: 7c04 7c04 9b00 6404 740d 9b00 9d03 7c04  |.|...d.t.....|.
-00001c50: 9b00 6404 740e 9b00 9d03 a104 3700 7d00  ..d.t.......7.}.
-00001c60: 7c03 7c02 6405 1800 7501 7220 7c00 6406  |.|.d...u.r |.d.
-00001c70: 3700 7d00 7120 7c00 5300 2907 4e72 3200  7.}.q |.S.).Nr2.
-00001c80: 0000 fa07 7b7d 203d 207b 7d72 4100 0000  ....{} = {}rA...
-00001c90: 723a 0000 0072 4200 0000 7243 0000 0029  r:...rB...rC...)
-00001ca0: 0f72 1f00 0000 7226 0000 0072 1c00 0000  .r....r&...r....
-00001cb0: 720e 0000 0072 4400 0000 7245 0000 00da  r....rD...rE....
-00001cc0: 1a6d 7367 5f70 756d 705f 7374 6174 696f  .msg_pump_statio
-00001cd0: 6e5f 7361 6d65 5f6e 6f64 65da 126d 7367  n_same_node..msg
-00001ce0: 5f77 6569 725f 7361 6d65 5f6e 6f64 65da  _weir_same_node.
-00001cf0: 156d 7367 5f6f 7269 6669 6365 5f73 616d  .msg_orifice_sam
-00001d00: 655f 6e6f 6465 da15 6d73 675f 6375 6c76  e_node..msg_culv
-00001d10: 6572 745f 7361 6d65 5f6e 6f64 6572 3700  ert_same_noder7.
-00001d20: 0000 7246 0000 0072 3f00 0000 7207 0000  ..rF...r?...r...
-00001d30: 0072 0500 0000 2906 7247 0000 0072 4800  .r....).rG...rH.
-00001d40: 0000 7249 0000 0072 4a00 0000 724b 0000  ..rI...rJ...rK..
-00001d50: 0072 3e00 0000 722a 0000 0072 2a00 0000  .r>...r*...r*...
-00001d60: 7230 0000 00da 1e63 6f6e 7374 725f 6672  r0.....constr_fr
-00001d70: 6f6d 5f74 6f5f 7361 6d65 5f6e 6f64 655f  om_to_same_node_
-00001d80: 7175 6572 79a8 0000 0073 2800 0000 0001  query....s(.....
-00001d90: 0401 0c01 0801 1001 0801 0601 0801 0601  ................
-00001da0: 0801 0602 0401 0c01 0801 0201 0c01 0cfc  ................
-00001db0: 0606 0c01 0a01 7253 0000 007a 197b 7d20  ......rS...z.{} 
-00001dc0: 4953 204e 4f54 204e 554c 4c20 414e 4420  IS NOT NULL AND 
-00001dd0: 7b7d 203d 2031 7241 0000 0072 3800 0000  {} = 1rA...r8...
-00001de0: 7a12 7b7d 202d 207b 7d20 3c3e 207b 7d20  z.{} - {} <> {} 
-00001df0: 2d20 7b7d 7a08 6c65 6e67 7468 2827 7a02  - {}z.length('z.
-00001e00: 2729 7a10 6c65 6e67 7468 2872 6570 6c61  ')z.length(repla
-00001e10: 6365 2827 7a0c 272c 2027 2027 2c20 2727  ce('z.', ' ', ''
-00001e20: 2929 7a03 7b7d 207a 064e 4f54 2049 4e54  ))z.{} z.NOT INT
-00001e30: 2903 722b 0000 0072 2c00 0000 722d 0000  ).r+...r,...r-..
-00001e40: 0072 3a00 0000 da02 494e 2902 722c 0000  .r:.....IN).r,..
-00001e50: 0072 2d00 0000 2903 722c 0000 0072 2d00  .r-...).r,...r-.
-00001e60: 0000 722e 0000 007a 0a7b 7d20 4953 204e  ..r....z.{} IS N
-00001e70: 554c 4c72 4e00 0000 2902 722e 0000 0072  ULLrN...).r....r
-00001e80: 3400 0000 7a0b 7b7d 204e 4f54 2049 4e20  4...z.{} NOT IN 
-00001e90: 2872 2900 0000 7a13 6162 7328 7b7d 202d  (r)...z.abs({} -
-00001ea0: 207b 7d29 203e 2030 2e30 357a 237b 7d20   {}) > 0.05z#{} 
-00001eb0: 4953 204e 554c 4c20 4f52 207b 7d20 4953  IS NULL OR {} IS
-00001ec0: 204e 554c 4c20 4f52 207b 7d20 3d20 2727   NULL OR {} = ''
-00001ed0: 2902 7a0b 7b7d 2061 7320 636f 6e6e 317a  ).z.{} as conn1z
-00001ee0: 0b7b 7d20 6173 2063 6f6e 6e32 7a38 6162  .{} as conn2z8ab
-00001ef0: 7328 7b7d 202d 207b 7d29 203e 2030 2e30  s({} - {}) > 0.0
-00001f00: 3520 414e 4420 6162 7328 7b7d 202d 207b  5 AND abs({} - {
-00001f10: 7d29 203e 2030 2e30 3520 414e 4420 7b7d  }) > 0.05 AND {}
-00001f20: 2021 3d20 3135 2902 7234 0000 0072 2e00   != 15).r4...r..
-00001f30: 0000 7a06 636f 6e6e 312e 7a06 636f 6e6e  ..z.conn1.z.conn
-00001f40: 322e 7a08 7b7d 2021 3d20 7b7d 7a35 7b7d  2.z.{} != {}z5{}
-00001f50: 2021 3d20 7b7d 2041 4e44 207b 7d20 213d   != {} AND {} !=
-00001f60: 2030 2041 4e44 207b 7d20 213d 2030 2041   0 AND {} != 0 A
-00001f70: 4e44 207b 7d20 3c20 6d61 7828 7b7d 2c20  ND {} < max({}, 
-00001f80: 7b7d 297a 3e7b 7d20 213d 207b 7d20 414e  {})z>{} != {} AN
-00001f90: 4420 7b7d 2021 3d20 3020 414e 4420 7b7d  D {} != 0 AND {}
-00001fa0: 2021 3d20 3020 414e 4420 6d61 7828 7b7d   != 0 AND max({}
-00001fb0: 2c20 7b7d 2920 3c20 6d61 7828 7b7d 2c20  , {}) < max({}, 
-00001fc0: 7b7d 297a 087b 7d20 3d20 3130 307a 116c  {})z.{} = 100z.l
-00001fd0: 656e 6774 6828 7b7d 2920 3e20 3130 3030  ength({}) > 1000
-00001fe0: 291a da19 6865 6967 6874 5f6e 6f74 5f75  )...height_not_u
-00001ff0: 7365 645f 666f 725f 7368 6170 65da 226d  sed_for_shape."m
-00002000: 756c 7469 706c 655f 6865 6967 6874 735f  ultiple_heights_
-00002010: 7769 6474 6873 5f73 616d 655f 636f 756e  widths_same_coun
-00002020: 74da 2169 6d70 6572 7669 6f75 735f 7375  t.!impervious_su
-00002030: 7266 6163 655f 6e6f 745f 696e 5f6d 6170  rface_not_in_map
-00002040: 7069 6e67 da2e 696d 7065 7276 696f 7573  ping..impervious
-00002050: 5f73 7572 6661 6365 5f6d 6170 5f72 6566  _surface_map_ref
-00002060: 6572 735f 746f 5f69 6e76 5f63 6f6e 6e5f  ers_to_inv_conn_
-00002070: 6e6f 6465 da1c 7375 7266 6163 655f 6e6f  node..surface_no
-00002080: 745f 696e 5f6d 6170 7069 6e67 5f74 6162  t_in_mapping_tab
-00002090: 6c65 da2d 696d 7065 7276 696f 7573 5f73  le.-impervious_s
-000020a0: 7572 6661 6365 5f6d 6170 5f72 6566 6572  urface_map_refer
-000020b0: 735f 746f 5f69 6e76 5f69 6d70 5f73 7572  s_to_inv_imp_sur
-000020c0: 66da 1d63 6f6e 6e5f 6e6f 6465 5f77 6974  f..conn_node_wit
-000020d0: 686f 7574 5f69 6d70 5f73 7572 6661 6365  hout_imp_surface
-000020e0: da19 6368 616e 6e65 6c5f 7769 7468 6f75  ..channel_withou
-000020f0: 745f 6372 6f73 735f 6c6f 63da 2963 726f  t_cross_loc.)cro
-00002100: 7373 5f73 6563 7469 6f6e 5f6c 6f63 6174  ss_section_locat
-00002110: 696f 6e5f 7769 7468 6f75 745f 6465 6669  ion_without_defi
-00002120: 6e69 7469 6f6e da20 6375 6c76 6572 745f  nition. culvert_
-00002130: 7769 7468 6f75 745f 6372 6f73 735f 6465  without_cross_de
-00002140: 6669 6e69 7469 6f6e da1d 7765 6972 5f77  finition..weir_w
-00002150: 6974 686f 7574 5f63 726f 7373 5f64 6566  ithout_cross_def
-00002160: 696e 6974 696f 6eda 206f 7269 6669 6365  inition. orifice
-00002170: 5f77 6974 686f 7574 5f63 726f 7373 5f64  _without_cross_d
-00002180: 6566 696e 6974 696f 6eda 196d 616e 686f  efinition..manho
-00002190: 6c65 5f77 6974 686f 7574 5f63 6f6e 6e5f  le_without_conn_
-000021a0: 6e6f 6465 da20 6f6e 655f 645f 626f 756e  node. one_d_boun
-000021b0: 6461 7279 5f77 6974 686f 7574 5f63 6f6e  dary_without_con
-000021c0: 6e5f 6e6f 6465 da1d 6372 6f73 735f 7365  n_node..cross_se
-000021d0: 635f 6c6f 635f 7769 7468 6f75 745f 7265  c_loc_without_re
-000021e0: 665f 6c76 6cda 2063 6f6e 6e5f 6e6f 6465  f_lvl. conn_node
-000021f0: 5f77 6974 686f 7574 5f69 6e69 745f 7761  _without_init_wa
-00002200: 7465 725f 6c76 6cda 1663 6f6e 6e5f 6e6f  ter_lvl..conn_no
-00002210: 6465 5f77 6974 686f 7574 5f63 6f6e 6eda  de_without_conn.
-00002220: 2473 7461 7274 5f6c 766c 5f6e 6f74 5f63  $start_lvl_not_c
-00002230: 6c6f 7365 5f74 6f5f 696e 6974 5f77 6174  lose_to_init_wat
-00002240: 6572 6c76 6cda 1875 6e64 6566 696e 6564  erlvl..undefined
-00002250: 5f73 6861 7065 5f6f 725f 7769 6474 68da  _shape_or_width.
-00002260: 1166 726f 6d5f 746f 5f73 616d 655f 6e6f  .from_to_same_no
-00002270: 6465 da29 7765 6972 5f73 7461 7274 5f6c  de.)weir_start_l
-00002280: 766c 5f6e 6f74 5f63 6c6f 7365 5f74 6f5f  vl_not_close_to_
-00002290: 696e 6974 5f77 6174 6572 6c76 6cda 2763  init_waterlvl.'c
-000022a0: 6861 6e6e 656c 5f73 7472 745f 656e 645f  hannel_strt_end_
-000022b0: 6e6f 745f 7361 6d65 5f69 6e69 745f 7761  not_same_init_wa
-000022c0: 7465 726c 766c da27 6f72 6966 6963 655f  terlvl.'orifice_
-000022d0: 7374 7274 5f65 6e64 5f6e 6f74 5f73 616d  strt_end_not_sam
-000022e0: 655f 696e 6974 5f77 6174 6572 6c76 6cda  e_init_waterlvl.
-000022f0: 2763 756c 7665 7274 5f73 7472 745f 656e  'culvert_strt_en
-00002300: 645f 6e6f 745f 7361 6d65 5f69 6e69 745f  d_not_same_init_
-00002310: 7761 7465 726c 766c da10 696d 705f 7375  waterlvl..imp_su
-00002320: 7266 6163 655f 7065 7263 da17 6163 7469  rface_perc..acti
-00002330: 6f6e 5f74 6162 6c65 5f63 6861 725f 636f  on_table_char_co
-00002340: 756e 7463 0000 0000 0000 0000 0000 0000  untc............
-00002350: 0000 0000 0300 0000 4000 0000 7324 0000  ........@...s$..
-00002360: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
-00002370: 0384 005a 0465 0564 0464 0584 0083 015a  ...Z.e.d.d.....Z
-00002380: 0664 0653 0029 07da 0a4d 6f64 656c 4368  .d.S.)...ModelCh
-00002390: 6563 6b7a 550a 2020 2020 486f 6c64 7320  eckzU.    Holds 
-000023a0: 616c 6c20 7465 7374 7320 7468 6174 2061  all tests that a
-000023b0: 7265 2070 6172 7420 6f66 2074 6865 2067  re part of the g
-000023c0: 656e 6572 616c 206d 6f64 656c 2063 6865  eneral model che
-000023d0: 636b 7320 666f 7220 6561 7369 6572 2061  cks for easier a
-000023e0: 6363 6573 730a 2020 2020 6301 0000 0000  ccess.    c.....
-000023f0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00002400: 0000 0073 0801 0000 7400 6401 1900 7c00  ...s....t.d...|.
-00002410: 5f01 7400 6402 1900 7c00 5f02 7400 6403  _.t.d...|._.t.d.
-00002420: 1900 7c00 5f03 7400 6404 1900 7c00 5f04  ..|._.t.d...|._.
-00002430: 7400 6405 1900 7c00 5f05 7400 6406 1900  t.d...|._.t.d...
-00002440: 7c00 5f06 7400 6407 1900 7c00 5f07 7400  |._.t.d...|._.t.
-00002450: 6408 1900 7c00 5f08 7400 6409 1900 7c00  d...|._.t.d...|.
-00002460: 5f09 7400 640a 1900 7c00 5f0a 7400 640b  _.t.d...|._.t.d.
-00002470: 1900 7c00 5f0b 7400 640c 1900 7c00 5f0c  ..|._.t.d...|._.
-00002480: 7400 640d 1900 7c00 5f0d 7400 640e 1900  t.d...|._.t.d...
-00002490: 7c00 5f0e 7400 640f 1900 7c00 5f0f 7400  |._.t.d...|._.t.
-000024a0: 6410 1900 7c00 5f10 7400 6411 1900 7c00  d...|._.t.d...|.
-000024b0: 5f11 7400 6412 1900 7c00 5f12 7400 6413  _.t.d...|._.t.d.
-000024c0: 1900 7c00 5f13 7400 6414 1900 7c00 5f14  ..|._.t.d...|._.
-000024d0: 7400 6415 1900 7c00 5f15 7400 6416 1900  t.d...|._.t.d...
-000024e0: 7c00 5f16 7400 6417 1900 7c00 5f17 7400  |._.t.d...|._.t.
-000024f0: 6418 1900 7c00 5f18 7400 6419 1900 7c00  d...|._.t.d...|.
-00002500: 5f19 7400 641a 1900 7c00 5f1a 6400 5300  _.t.d...|._.d.S.
-00002510: 291b 4e72 5500 0000 7256 0000 0072 5700  ).NrU...rV...rW.
-00002520: 0000 7258 0000 0072 5900 0000 725a 0000  ..rX...rY...rZ..
-00002530: 0072 5b00 0000 725c 0000 0072 5d00 0000  .r[...r\...r]...
-00002540: 725e 0000 0072 5f00 0000 7260 0000 0072  r^...r_...r`...r
-00002550: 6100 0000 7262 0000 0072 6300 0000 7264  a...rb...rc...rd
-00002560: 0000 0072 6500 0000 7266 0000 0072 6700  ...re...rf...rg.
-00002570: 0000 7268 0000 0072 6900 0000 726a 0000  ..rh...ri...rj..
-00002580: 0072 6b00 0000 726c 0000 0072 6d00 0000  .rk...rl...rm...
-00002590: 726e 0000 0029 1bda 0c6d 6f64 656c 5f63  rn...)...model_c
-000025a0: 6865 636b 7372 5500 0000 5a1d 6d75 6c74  hecksrU...Z.mult
-000025b0: 6970 6c65 5f68 6569 6768 7473 5f77 6964  iple_heights_wid
-000025c0: 7468 735f 636f 756e 7472 5700 0000 7258  ths_countrW...rX
-000025d0: 0000 005a 1673 7572 6661 6365 5f6e 6f74  ...Z.surface_not
-000025e0: 5f69 6e5f 6d61 7070 696e 675a 2169 6d70  _in_mappingZ!imp
-000025f0: 6572 7669 6f75 735f 6d61 705f 6e6f 745f  ervious_map_not_
-00002600: 696e 5f69 6d70 5f73 7572 6661 6365 725b  in_imp_surfacer[
-00002610: 0000 005a 2663 6861 6e6e 656c 5f77 6974  ...Z&channel_wit
-00002620: 686f 7574 5f63 726f 7373 5f73 6563 7469  hout_cross_secti
-00002630: 6f6e 5f6c 6f63 6174 696f 6e5a 2463 726f  on_locationZ$cro
-00002640: 7373 5f73 6563 7469 6f6e 5f6c 6f63 5f77  ss_section_loc_w
-00002650: 6974 686f 7574 5f64 6566 696e 6974 696f  ithout_definitio
-00002660: 6e5a 2863 756c 7665 7274 5f77 6974 686f  nZ(culvert_witho
-00002670: 7574 5f63 726f 7373 5f73 6563 7469 6f6e  ut_cross_section
-00002680: 5f64 6566 696e 6974 696f 6e5a 2577 6569  _definitionZ%wei
-00002690: 725f 7769 7468 6f75 745f 6372 6f73 735f  r_without_cross_
-000026a0: 7365 6374 696f 6e5f 6465 6669 6e69 7469  section_definiti
-000026b0: 6f6e 5a28 6f72 6966 6963 655f 7769 7468  onZ(orifice_with
-000026c0: 6f75 745f 6372 6f73 735f 7365 6374 696f  out_cross_sectio
-000026d0: 6e5f 6465 6669 6e69 7469 6f6e 7261 0000  n_definitionra..
-000026e0: 0072 6200 0000 7263 0000 0072 6400 0000  .rb...rc...rd...
-000026f0: 7265 0000 005a 2173 7461 7274 5f6c 766c  re...Z!start_lvl
-00002700: 5f6e 6f74 5f63 6c6f 7365 5f69 6e69 745f  _not_close_init_
-00002710: 7761 7465 726c 766c 5a18 7368 6170 655f  waterlvlZ.shape_
-00002720: 6f72 5f77 6964 7468 5f75 6e64 6566 696e  or_width_undefin
-00002730: 6564 7268 0000 0072 6900 0000 726a 0000  edrh...ri...rj..
-00002740: 0072 6b00 0000 726c 0000 005a 1769 6d70  .rk...rl...Z.imp
-00002750: 6572 7669 6f75 735f 7375 7266 6163 655f  ervious_surface_
-00002760: 7065 7263 5a1b 6163 7469 6f6e 5f74 6162  percZ.action_tab
-00002770: 6c65 5f74 6f6f 5f6d 616e 795f 6368 6172  le_too_many_char
-00002780: 7329 01da 0473 656c 6672 2a00 0000 722a  s)...selfr*...r*
-00002790: 0000 0072 3000 0000 da08 5f5f 696e 6974  ...r0.....__init
-000027a0: 5f5f fa01 0000 7338 0000 0000 010a 010a  __....s8........
-000027b0: 010a 0102 0102 ff06 030a 010a 010a 010a  ................
-000027c0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00000bc0: 6520 636f 756e 747a 3357 4152 4e49 4e47  e countz3WARNING
+00000bd0: 3a20 696d 7065 7276 696f 7573 2073 7572  : impervious sur
+00000be0: 6661 6365 2069 7320 6e6f 7420 696e 206d  face is not in m
+00000bf0: 6170 7069 6e67 2074 6162 6c65 7a39 4552  apping tablez9ER
+00000c00: 524f 523a 2069 6d70 6572 7669 6f75 7320  ROR: impervious 
+00000c10: 7375 7266 6163 6520 6d61 7020 7265 6665  surface map refe
+00000c20: 7273 2074 6f20 6e6f 6e2d 6578 6973 7465  rs to non-existe
+00000c30: 6e74 206e 6f64 657a 2857 4152 4e49 4e47  nt nodez(WARNING
+00000c40: 3a20 7375 7266 6163 6520 6973 206e 6f74  : surface is not
+00000c50: 2069 6e20 6d61 7070 696e 6720 7461 626c   in mapping tabl
+00000c60: 657a 4257 4152 4e49 4e47 3a20 696d 7065  ezBWARNING: impe
+00000c70: 7276 696f 7573 2073 7572 6661 6365 206d  rvious surface m
+00000c80: 6170 2069 7320 6e6f 7420 696e 2069 6d70  ap is not in imp
+00000c90: 6572 7669 6f75 7320 7375 7266 6163 6520  ervious surface 
+00000ca0: 6c61 7965 727a 3357 4152 4e49 4e47 3a20  layerz3WARNING: 
+00000cb0: 636f 6e6e 6563 7469 6f6e 206e 6f64 6520  connection node 
+00000cc0: 7769 7468 6f75 7420 696d 7065 7276 696f  without impervio
+00000cd0: 7573 2073 7572 6661 6365 7a2d 4552 524f  us surfacez-ERRO
+00000ce0: 523a 2063 6861 6e6e 656c 2077 6974 686f  R: channel witho
+00000cf0: 7574 2063 726f 7373 2073 6563 7469 6f6e  ut cross section
+00000d00: 206c 6f63 6174 696f 6e7a 3045 5252 4f52   locationz0ERROR
+00000d10: 3a20 6372 6f73 7320 7365 6374 696f 6e20  : cross section 
+00000d20: 6c6f 6361 7469 6f6e 2077 6974 686f 7574  location without
+00000d30: 2064 6566 696e 6974 696f 6e7a 2f45 5252   definitionz/ERR
+00000d40: 4f52 3a20 6375 6c76 6572 7420 7769 7468  OR: culvert with
+00000d50: 6f75 7420 6372 6f73 7320 7365 6374 696f  out cross sectio
+00000d60: 6e20 6465 6669 6e69 7469 6f6e 7a2c 4552  n definitionz,ER
+00000d70: 524f 523a 2077 6569 7220 7769 7468 6f75  ROR: weir withou
+00000d80: 7420 6372 6f73 7320 7365 6374 696f 6e20  t cross section 
+00000d90: 6465 6669 6e69 7469 6f6e 7a2f 4552 524f  definitionz/ERRO
+00000da0: 523a 206f 7269 6669 6365 2077 6974 686f  R: orifice witho
+00000db0: 7574 2063 726f 7373 2073 6563 7469 6f6e  ut cross section
+00000dc0: 2064 6566 696e 6974 696f 6e7a 2645 5252   definitionz&ERR
+00000dd0: 4f52 3a20 6d61 6e68 6f6c 6520 7769 7468  OR: manhole with
+00000de0: 6f75 7420 636f 6e6e 6563 7469 6f6e 206e  out connection n
+00000df0: 6f64 657a 2c57 4152 4e49 4e47 3a20 3164  odez,WARNING: 1d
+00000e00: 2062 6f75 6e64 6172 7920 7769 7468 6f75   boundary withou
+00000e10: 7420 636f 6e6e 6563 7469 6f6e 206e 6f64  t connection nod
+00000e20: 657a 3545 5252 4f52 3a20 6372 6f73 7320  ez5ERROR: cross 
+00000e30: 7365 6374 696f 6e20 6c6f 6361 7469 6f6e  section location
+00000e40: 2077 6974 686f 7574 2072 6566 6572 656e   without referen
+00000e50: 6365 206c 6576 656c 7a33 5741 524e 494e  ce levelz3WARNIN
+00000e60: 473a 2063 6f6e 6e65 6374 696f 6e20 6e6f  G: connection no
+00000e70: 6465 2077 6974 686f 7574 2069 6e69 7469  de without initi
+00000e80: 616c 2077 6174 6572 6c65 7665 6c7a 1e45  al waterlevelz.E
+00000e90: 5252 4f52 3a20 6e6f 6465 2077 6974 686f  RROR: node witho
+00000ea0: 7574 2063 6f6e 6e65 6374 696f 6e7a 4557  ut connectionzEW
+00000eb0: 4152 4e49 4e47 3a20 7374 6172 7420 6c65  ARNING: start le
+00000ec0: 7665 6c20 666f 7220 7075 6d70 2073 7461  vel for pump sta
+00000ed0: 7469 6f6e 206e 6f74 2063 6c6f 7365 2074  tion not close t
+00000ee0: 6f20 696e 6974 6961 6c20 7761 7465 726c  o initial waterl
+00000ef0: 6576 656c 7a24 4552 524f 523a 2073 6861  evelz$ERROR: sha
+00000f00: 7065 206f 7220 7769 6474 6820 6973 206e  pe or width is n
+00000f10: 6f74 2064 6566 696e 6564 7a37 4552 524f  ot definedz7ERRO
+00000f20: 523a 2070 756d 7073 7461 7469 6f6e 2066  R: pumpstation f
+00000f30: 726f 6d20 616e 6420 746f 2074 6865 2073  rom and to the s
+00000f40: 616d 6520 636f 6e6e 6563 7469 6f6e 206e  ame connection n
+00000f50: 6f64 657a 3045 5252 4f52 3a20 7765 6972  odez0ERROR: weir
+00000f60: 2066 726f 6d20 616e 6420 746f 2074 6865   from and to the
+00000f70: 2073 616d 6520 636f 6e6e 6563 7469 6f6e   same connection
+00000f80: 206e 6f64 657a 3345 5252 4f52 3a20 6f72   nodez3ERROR: or
+00000f90: 6966 6963 6520 6672 6f6d 2061 6e64 2074  ifice from and t
+00000fa0: 6f20 7468 6520 7361 6d65 2063 6f6e 6e65  o the same conne
+00000fb0: 6374 696f 6e20 6e6f 6465 7a33 4552 524f  ction nodez3ERRO
+00000fc0: 523a 2063 756c 7665 7274 2066 726f 6d20  R: culvert from 
+00000fd0: 616e 6420 746f 2074 6865 2073 616d 6520  and to the same 
+00000fe0: 636f 6e6e 6563 7469 6f6e 206e 6f64 657a  connection nodez
+00000ff0: 5827 5741 524e 494e 473a 2073 7461 7274  X'WARNING: start
+00001000: 206c 6576 656c 2027 207c 7c20 7b7d 207c   level ' || {} |
+00001010: 7c20 2720 6e6f 7420 636c 6f73 6520 746f  | ' not close to
+00001020: 2069 6e69 7469 616c 2077 6174 6572 6c65   initial waterle
+00001030: 7665 6c20 2720 7c7c 207b 7d20 7c7c 2027  vel ' || {} || '
+00001040: 2c20 2720 7c7c 207b 7d7a 5727 5741 524e  , ' || {}zW'WARN
+00001050: 494e 473a 2069 6e69 7469 616c 2077 6174  ING: initial wat
+00001060: 6572 206c 6576 656c 2061 7420 7374 6172  er level at star
+00001070: 7420 616e 6420 656e 6420 6e6f 6465 2061  t and end node a
+00001080: 7265 206e 6f74 2065 7175 616c 2027 207c  re not equal ' |
+00001090: 7c20 7b7d 207c 7c20 272c 2027 207c 7c20  | {} || ', ' || 
+000010a0: 7b7d 7a50 2757 4152 4e49 4e47 3a20 496e  {}zP'WARNING: In
+000010b0: 6974 6961 6c20 7761 7465 726c 6576 656c  itial waterlevel
+000010c0: 2061 7420 7374 6172 7420 656e 2065 6e64   at start en end
+000010d0: 206e 6f64 6520 6e6f 7420 6571 7561 6c27   node not equal'
+000010e0: 207c 7c20 7b7d 207c 7c20 272c 2027 207c   || {} || ', ' |
+000010f0: 7c20 7b7d 7a34 5741 524e 494e 473a 2070  | {}z4WARNING: p
+00001100: 6572 6365 6e74 6167 6520 3d20 3130 3020  ercentage = 100 
+00001110: 616e 6420 7368 6f75 6c64 2062 6520 3134  and should be 14
+00001120: 2e34 206f 7220 3131 2e35 7a44 4552 524f  .4 or 11.5zDERRO
+00001130: 523a 2061 6374 696f 6e5f 7461 626c 6520  R: action_table 
+00001140: 6861 7320 6d6f 7265 2074 6861 6e20 3130  has more than 10
+00001150: 3030 2063 6861 7261 6374 6572 7320 286d  00 characters (m
+00001160: 6f64 656c 2077 696c 6c20 6372 6173 6829  odel will crash)
+00001170: 464e 6304 0000 0000 0000 0000 0000 0005  FNc.............
+00001180: 0000 0003 0000 0043 0000 0073 4000 0000  .......C...s@...
+00001190: 6401 7c00 1700 6402 1700 7d04 7c01 7218  d.|...d...}.|.r.
+000011a0: 7c04 6403 3700 7d04 7c02 7224 7c04 6404  |.d.7.}.|.r$|.d.
+000011b0: 3700 7d04 7c03 7234 7c04 6405 7c03 1700  7.}.|.r4|.d.|...
+000011c0: 3700 7d04 7c04 6406 3700 7d04 7c04 5300  7.}.|.d.7.}.|.S.
+000011d0: 2907 61c6 0100 000a 2020 2020 2020 2020  ).a.....        
+000011e0: 636f 6e73 7472 5f69 6e5f 636c 6175 7365  constr_in_clause
+000011f0: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
+00001200: 6e6f 7469 6e20 2873 7472 696e 673a 2065  notin (string: e
+00001210: 6974 6865 7220 2749 4e27 206f 7220 274e  ither 'IN' or 'N
+00001220: 4f54 2049 4e27 290a 2020 2020 2020 2020  OT IN').        
+00001230: 2020 2020 7365 6c20 2d3e 2046 616c 7365      sel -> False
+00001240: 2028 626f 6f6c 3a20 6164 6420 2753 454c   (bool: add 'SEL
+00001250: 4543 5420 7b7d 2720 6c69 6e65 290a 2020  ECT {}' line).  
+00001260: 2020 2020 2020 2020 2020 6672 6d20 2d3e            frm ->
+00001270: 2046 616c 7365 2028 626f 6f6c 3a20 6164   False (bool: ad
+00001280: 6420 2746 524f 4d20 7b7d 2720 6c69 6e65  d 'FROM {}' line
+00001290: 290a 2020 2020 2020 2020 2020 2020 7768  ).            wh
+000012a0: 6572 6520 2d3e 2046 616c 7365 2028 626f  ere -> False (bo
+000012b0: 6f6c 3a20 6164 6420 2757 4845 5245 207b  ol: add 'WHERE {
+000012c0: 7d27 206c 696e 6529 0a20 2020 2020 2020  }' line).       
+000012d0: 2020 2020 2029 0a0a 2020 2020 436f 6e73       )..    Cons
+000012e0: 7472 7563 7473 2061 2049 4e20 6f72 204e  tructs a IN or N
+000012f0: 4f54 2049 4e20 7365 6c65 6374 696f 6e20  OT IN selection 
+00001300: 636c 6175 7365 2e0a 2020 2020 4578 3a0a  clause..    Ex:.
+00001310: 2020 2020 2020 2020 494e 0a20 2020 2020          IN.     
+00001320: 2020 2028 5345 4c45 4354 207b 7d0a 2020     (SELECT {}.  
+00001330: 2020 2020 2020 4652 4f4d 207b 7d0a 2020        FROM {}.  
+00001340: 2020 2020 2020 5748 4552 4520 7b7d 290a        WHERE {}).
+00001350: 0a20 2020 2057 6869 6368 2063 616e 2074  .    Which can t
+00001360: 6865 6e20 6265 2066 6f72 6d61 7474 6564  hen be formatted
+00001370: 2074 6f20 696e 7365 7274 2074 6162 6c65   to insert table
+00001380: 206e 616d 6573 2061 6e64 2063 6f6e 6469   names and condi
+00001390: 7469 6f6e 2065 7463 0a20 2020 20da 0120  tion etc.    .. 
+000013a0: 7a02 280a 7a0a 5345 4c45 4354 207b 7d0a  z.(.z.SELECT {}.
+000013b0: 7a08 4652 4f4d 207b 7d0a 7a08 5748 4552  z.FROM {}.z.WHER
+000013c0: 4520 7b7d fa01 29a9 0029 05da 0769 6e6e  E {}..)..)...inn
+000013d0: 6f74 696e da03 7365 6cda 0366 726d da05  otin..sel..frm..
+000013e0: 7768 6572 65da 0372 6573 722a 0000 0072  where..resr*...r
+000013f0: 2a00 0000 fa5a 643a 5c67 6974 6875 625c  *....Zd:\github\
+00001400: 7776 616e 6765 7277 656e 5c68 686e 6b2d  wvangerwen\hhnk-
+00001410: 7468 7265 6564 692d 746f 6f6c 735c 6868  threedi-tools\hh
+00001420: 6e6b 5f74 6872 6565 6469 5f74 6f6f 6c73  nk_threedi_tools
+00001430: 5c75 7469 6c73 5c71 7565 7269 6573 5f67  \utils\queries_g
+00001440: 656e 6572 616c 5f63 6865 636b 732e 7079  eneral_checks.py
+00001450: da10 636f 6e73 7472 5f69 6e5f 636c 6175  ..constr_in_clau
+00001460: 7365 5200 0000 7312 0000 0000 120c 0104  seR...s.........
+00001470: 0108 0104 0108 0104 010c 0108 0172 3100  .............r1.
+00001480: 0000 7a02 7b7d 6305 0000 0000 0000 0000  ..z.{}c.........
+00001490: 0000 0007 0000 0005 0000 0043 0000 0073  ...........C...s
+000014a0: 9000 0000 6401 7d05 7c00 7218 7c05 6402  ....d.}.|.r.|.d.
+000014b0: 7c00 1700 6403 1700 3700 7d05 7c01 722c  |...d...7.}.|.r,
+000014c0: 7c05 6404 7c01 1700 6403 1700 3700 7d05  |.d.|...d...7.}.
+000014d0: 7c03 4400 5d20 7d06 7c05 6405 7c06 1700  |.D.] }.|.d.|...
+000014e0: 6406 1700 7c03 7c06 1900 1700 6403 1700  d...|.|.....d...
+000014f0: 3700 7d05 7130 7c04 4400 5d20 7d06 7c05  7.}.q0|.D.] }.|.
+00001500: 6407 7c06 1700 6406 1700 7c04 7c06 1900  d.|...d...|.|...
+00001510: 1700 6403 1700 3700 7d05 7156 7c02 728c  ..d...7.}.qV|.r.
+00001520: 7c05 6408 7c02 1700 6403 1700 3700 7d05  |.d.|...d...7.}.
+00001530: 7c05 5300 2909 61aa 0200 000a 2020 2020  |.S.).a.....    
+00001540: 436f 6e73 7472 7563 7473 2073 656c 6563  Constructs selec
+00001550: 7420 2f20 6672 6f6d 202f 2077 6865 7265  t / from / where
+00001560: 2071 7565 7279 2077 6974 6820 706f 7373   query with poss
+00001570: 6962 6c65 206a 6f69 6e20 636c 6175 7365  ible join clause
+00001580: 7320 2869 6e6e 6572 206f 7220 6c65 6674  s (inner or left
+00001590: 206a 6f69 6e29 0a0a 2020 2020 2020 2020   join)..        
+000015a0: 636f 6e73 7472 7563 745f 7365 6c5f 6672  construct_sel_fr
+000015b0: 6f6d 5f77 6865 7265 5f71 7565 7279 280a  om_where_query(.
+000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015d0: 7365 6c20 2d3e 2027 7b7d 2720 2873 7472  sel -> '{}' (str
+000015e0: 696e 672c 2077 6861 7465 7665 7220 636f  ing, whatever co
+000015f0: 6d65 7320 6166 7465 7220 2753 454c 4543  mes after 'SELEC
+00001600: 5420 2720 6b65 7977 6f72 6429 0a20 2020  T ' keyword).   
+00001610: 2020 2020 2020 2020 2020 2020 2066 726f               fro
+00001620: 6d20 2d3e 2027 7b7d 2720 2873 7472 696e  m -> '{}' (strin
+00001630: 672c 2077 6861 7465 7665 7220 636f 6d65  g, whatever come
+00001640: 7320 6166 7465 7220 2746 524f 4d20 2720  s after 'FROM ' 
+00001650: 6b65 7977 6f72 6429 0a20 2020 2020 2020  keyword).       
+00001660: 2020 2020 2020 2020 2077 6865 7265 202d           where -
+00001670: 3e20 277b 7d27 2028 7374 7269 6e67 2c20  > '{}' (string, 
+00001680: 7768 6174 6576 6572 2063 6f6d 6573 2061  whatever comes a
+00001690: 6674 6572 2027 5748 4552 4520 2720 6b65  fter 'WHERE ' ke
+000016a0: 7977 6f72 6429 0a20 2020 2020 2020 2020  yword).         
+000016b0: 2020 2020 2020 206c 6566 745f 6a6f 696e         left_join
+000016c0: 202d 3e20 7b7d 2028 6469 6374 696f 6e61   -> {} (dictiona
+000016d0: 7279 2c20 7265 7475 726e 6564 2061 7320  ry, returned as 
+000016e0: 274c 4546 5420 4a4f 494e 207b 6b65 797d  'LEFT JOIN {key}
+000016f0: 204f 4e20 7b76 616c 7565 7d20 666f 7220   ON {value} for 
+00001700: 6576 6572 7920 656e 7472 7920 696e 2064  every entry in d
+00001710: 6963 7429 0a20 2020 2020 2020 2020 2020  ict).           
+00001720: 2020 2020 2069 6e6e 6572 5f6a 6f69 6e20       inner_join 
+00001730: 2d3e 207b 7d20 2864 6963 7469 6f6e 6172  -> {} (dictionar
+00001740: 792c 2072 6574 7572 6e65 6420 6173 2027  y, returned as '
+00001750: 494e 4e45 5220 4a4f 494e 207b 6b65 797d  INNER JOIN {key}
+00001760: 204f 4e20 7b76 616c 7565 7d20 666f 7220   ON {value} for 
+00001770: 6576 6572 7920 656e 7472 7920 696e 2064  every entry in d
+00001780: 6963 7429 0a20 2020 2020 2020 2020 2020  ict).           
+00001790: 2029 0a0a 2020 2020 5265 7475 726e 7320   )..    Returns 
+000017a0: 6569 7468 6572 2066 756c 6c20 7175 6572  either full quer
+000017b0: 7920 6f72 2074 656d 706c 6174 6520 746f  y or template to
+000017c0: 2066 6f72 6d61 7420 6c61 7465 7220 6465   format later de
+000017d0: 7065 6e64 696e 6720 6f6e 2069 6e70 7574  pending on input
+000017e0: 0a20 2020 20da 007a 0753 454c 4543 5420  .    ..z.SELECT 
+000017f0: da01 0a7a 0546 524f 4d20 7a0a 4c45 4654  ...z.FROM z.LEFT
+00001800: 204a 4f49 4e20 7a04 0a4f 4e20 7a0b 494e   JOIN z..ON z.IN
+00001810: 4e45 5220 4a4f 494e 207a 0657 4845 5245  NER JOIN z.WHERE
+00001820: 2072 2a00 0000 2907 722c 0000 0072 2d00   r*...).r,...r-.
+00001830: 0000 722e 0000 00da 096c 6566 745f 6a6f  ..r......left_jo
+00001840: 696e da0a 696e 6e65 725f 6a6f 696e 722f  in..inner_joinr/
+00001850: 0000 00da 036b 6579 722a 0000 0072 2a00  .....keyr*...r*.
+00001860: 0000 7230 0000 00da 1e63 6f6e 7374 7275  ..r0.....constru
+00001870: 6374 5f73 656c 5f66 726f 6d5f 7768 6572  ct_sel_from_wher
+00001880: 655f 7175 6572 796f 0000 0073 1800 0000  e_queryo...s....
+00001890: 000e 0401 0401 1001 0401 1001 0801 1e01  ................
+000018a0: 0801 1e01 0401 1001 7237 0000 0063 0200  ........r7...c..
+000018b0: 0000 0000 0000 0000 0000 0300 0000 0900  ................
+000018c0: 0000 4300 0000 7322 0000 0064 017c 009b  ..C...s"...d.|..
+000018d0: 0064 027c 009b 0064 0374 009b 0064 047c  .d.|...d.t...d.|
+000018e0: 019b 0064 059d 097d 027c 0253 0029 064e  ...d...}.|.S.).N
+000018f0: fa01 27fa 1127 2061 7320 7461 626c 655f  ..'..' as table_
+00001900: 6e61 6d65 2c0a da01 2e7a 0920 6173 2069  name,....z. as i
+00001910: 642c 0a27 7a0a 2720 6173 2065 7272 6f72  d,.'z.' as error
+00001920: a901 7213 0000 00a9 03da 0574 6162 6c65  ..r........table
+00001930: da03 6d73 6772 2f00 0000 722a 0000 0072  ..msgr/...r*...r
+00001940: 2a00 0000 7230 0000 00da 1463 6f6e 7374  *...r0.....const
+00001950: 7275 6374 5f71 7565 7279 5f68 6561 648b  ruct_query_head.
+00001960: 0000 0073 0400 0000 0001 1e01 723f 0000  ...s........r?..
+00001970: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+00001980: 0000 0900 0000 4300 0000 7322 0000 0064  ......C...s"...d
+00001990: 017c 009b 0064 027c 009b 0064 0374 009b  .|...d.|...d.t..
+000019a0: 0064 047c 019b 0064 059d 097d 027c 0253  .d.|...d...}.|.S
+000019b0: 0029 064e 7238 0000 0072 3900 0000 723a  .).Nr8...r9...r:
+000019c0: 0000 007a 0820 6173 2069 642c 0a7a 0920  ...z. as id,.z. 
+000019d0: 6173 2065 7272 6f72 723b 0000 0072 3c00  as errorr;...r<.
+000019e0: 0000 722a 0000 0072 2a00 0000 7230 0000  ..r*...r*...r0..
+000019f0: 00da 1e63 6f6e 7374 7275 6374 5f71 7565  ...construct_que
+00001a00: 7279 5f68 6561 645f 6e6f 5f71 756f 7465  ry_head_no_quote
+00001a10: 7390 0000 0073 0400 0000 0001 1e01 7240  s....s........r@
+00001a20: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001a30: 0600 0000 0800 0000 4300 0000 7380 0000  ........C...s...
+00001a40: 0064 017d 0074 0074 0174 0274 0374 0474  .d.}.t.t.t.t.t.t
+00001a50: 0567 067d 0174 067c 0183 017d 0274 077c  .g.}.t.|...}.t.|
+00001a60: 0183 0144 005d 565c 027d 037d 0474 0874  ...D.]V\.}.}.t.t
+00001a70: 0966 0244 005d 447d 057c 0074 0a64 0264  .f.D.]D}.|.t.d.d
+00001a80: 038d 01a0 0b7c 057c 047c 05a1 0337 007d  .....|.|.|...7.}
+00001a90: 007c 037c 0264 0418 0075 0173 707c 037c  .|.|.d...u.sp|.|
+00001aa0: 0264 0418 0075 0072 347c 0574 0875 0072  .d...u.r4|.t.u.r
+00001ab0: 347c 0064 0537 007d 0071 3471 247c 0053  4|.d.7.}.q4q$|.S
+00001ac0: 0029 064e 7232 0000 007a 0e7b 7d20 4953  .).Nr2...z.{} IS
+00001ad0: 204e 4f54 204e 554c 4ca9 0172 2e00 0000   NOT NULL..r....
+00001ae0: e901 0000 00fa 0a55 4e49 4f4e 2041 4c4c  .......UNION ALL
+00001af0: 0a29 0c72 1f00 0000 7204 0000 0072 0e00  .).r....r....r..
+00001b00: 0000 721e 0000 0072 2600 0000 721c 0000  ..r....r&...r...
+00001b10: 00da 036c 656e da09 656e 756d 6572 6174  ...len..enumerat
+00001b20: 6572 0700 0000 7205 0000 0072 3700 0000  er....r....r7...
+00001b30: da06 666f 726d 6174 2906 da05 7175 6572  ..format)...quer
+00001b40: 79da 066c 6179 6572 73da 066c 656e 6774  y..layers..lengt
+00001b50: 68da 0169 da05 6c61 7965 72da 046e 6f64  h..i..layer..nod
+00001b60: 6572 2a00 0000 722a 0000 0072 3000 0000  er*...r*...r0...
+00001b70: da24 636f 6e73 7472 5f63 6f6e 6e5f 6e6f  .$constr_conn_no
+00001b80: 6465 735f 7769 7468 6f75 745f 636f 6e6e  des_without_conn
+00001b90: 5f71 7565 7279 9500 0000 731e 0000 0000  _query....s.....
+00001ba0: 0104 0202 0102 0102 0102 0102 0102 fa04  ................
+00001bb0: 0808 0110 010c 0118 0120 010c 0172 4d00  ......... ...rM.
+00001bc0: 0000 6300 0000 0000 0000 0000 0000 0006  ..c.............
+00001bd0: 0000 000a 0000 0043 0000 0073 a400 0000  .......C...s....
+00001be0: 6401 7d00 7400 7401 7402 7403 6704 7d01  d.}.t.t.t.t.g.}.
+00001bf0: 7404 7c01 8301 7d02 7405 7c01 8301 4400  t.|...}.t.|...D.
+00001c00: 5d7e 5c02 7d03 7d04 7c04 7400 6b02 7236  ]~\.}.}.|.t.k.r6
+00001c10: 7406 7d05 6e20 7c04 7401 6b02 7244 7407  t.}.n |.t.k.rDt.
+00001c20: 7d05 6e12 7c04 7402 6b02 7252 7408 7d05  }.n.|.t.k.rRt.}.
+00001c30: 6e04 7409 7d05 7c00 740a 6402 6403 8d01  n.t.}.|.t.d.d...
+00001c40: a00b 740c 7c04 7c05 8302 7c04 7c04 9b00  ..t.|.|...|.|...
+00001c50: 6404 740d 9b00 9d03 7c04 9b00 6404 740e  d.t.....|...d.t.
+00001c60: 9b00 9d03 a104 3700 7d00 7c03 7c02 6405  ......7.}.|.|.d.
+00001c70: 1800 7501 7220 7c00 6406 3700 7d00 7120  ..u.r |.d.7.}.q 
+00001c80: 7c00 5300 2907 4e72 3200 0000 fa07 7b7d  |.S.).Nr2.....{}
+00001c90: 203d 207b 7d72 4100 0000 723a 0000 0072   = {}rA...r:...r
+00001ca0: 4200 0000 7243 0000 0029 0f72 1f00 0000  B...rC...).r....
+00001cb0: 7226 0000 0072 1c00 0000 720e 0000 0072  r&...r....r....r
+00001cc0: 4400 0000 7245 0000 00da 1a6d 7367 5f70  D...rE.....msg_p
+00001cd0: 756d 705f 7374 6174 696f 6e5f 7361 6d65  ump_station_same
+00001ce0: 5f6e 6f64 65da 126d 7367 5f77 6569 725f  _node..msg_weir_
+00001cf0: 7361 6d65 5f6e 6f64 65da 156d 7367 5f6f  same_node..msg_o
+00001d00: 7269 6669 6365 5f73 616d 655f 6e6f 6465  rifice_same_node
+00001d10: da15 6d73 675f 6375 6c76 6572 745f 7361  ..msg_culvert_sa
+00001d20: 6d65 5f6e 6f64 6572 3700 0000 7246 0000  me_noder7...rF..
+00001d30: 0072 3f00 0000 7207 0000 0072 0500 0000  .r?...r....r....
+00001d40: 2906 7247 0000 0072 4800 0000 7249 0000  ).rG...rH...rI..
+00001d50: 0072 4a00 0000 724b 0000 0072 3e00 0000  .rJ...rK...r>...
+00001d60: 722a 0000 0072 2a00 0000 7230 0000 00da  r*...r*...r0....
+00001d70: 1e63 6f6e 7374 725f 6672 6f6d 5f74 6f5f  .constr_from_to_
+00001d80: 7361 6d65 5f6e 6f64 655f 7175 6572 79a8  same_node_query.
+00001d90: 0000 0073 2800 0000 0001 0401 0c01 0801  ...s(...........
+00001da0: 1001 0801 0601 0801 0601 0801 0602 0401  ................
+00001db0: 0c01 0801 0201 0c01 0cfc 0606 0c01 0a01  ................
+00001dc0: 7253 0000 007a 197b 7d20 4953 204e 4f54  rS...z.{} IS NOT
+00001dd0: 204e 554c 4c20 414e 4420 7b7d 203d 2031   NULL AND {} = 1
+00001de0: 7241 0000 0072 3800 0000 7a12 7b7d 202d  rA...r8...z.{} -
+00001df0: 207b 7d20 3c3e 207b 7d20 2d20 7b7d 7a08   {} <> {} - {}z.
+00001e00: 6c65 6e67 7468 2827 7a02 2729 7a10 6c65  length('z.')z.le
+00001e10: 6e67 7468 2872 6570 6c61 6365 2827 7a0c  ngth(replace('z.
+00001e20: 272c 2027 2027 2c20 2727 2929 7a03 7b7d  ', ' ', ''))z.{}
+00001e30: 207a 064e 4f54 2049 4e54 2903 722b 0000   z.NOT INT).r+..
+00001e40: 0072 2c00 0000 722d 0000 0072 3a00 0000  .r,...r-...r:...
+00001e50: da02 494e 2902 722c 0000 0072 2d00 0000  ..IN).r,...r-...
+00001e60: 2903 722c 0000 0072 2d00 0000 722e 0000  ).r,...r-...r...
+00001e70: 007a 0a7b 7d20 4953 204e 554c 4c72 4e00  .z.{} IS NULLrN.
+00001e80: 0000 2902 722e 0000 0072 3400 0000 7a0b  ..).r....r4...z.
+00001e90: 7b7d 204e 4f54 2049 4e20 2872 2900 0000  {} NOT IN (r)...
+00001ea0: 7a13 6162 7328 7b7d 202d 207b 7d29 203e  z.abs({} - {}) >
+00001eb0: 2030 2e30 357a 237b 7d20 4953 204e 554c   0.05z#{} IS NUL
+00001ec0: 4c20 4f52 207b 7d20 4953 204e 554c 4c20  L OR {} IS NULL 
+00001ed0: 4f52 207b 7d20 3d20 2727 2902 7a0b 7b7d  OR {} = '').z.{}
+00001ee0: 2061 7320 636f 6e6e 317a 0b7b 7d20 6173   as conn1z.{} as
+00001ef0: 2063 6f6e 6e32 7a38 6162 7328 7b7d 202d   conn2z8abs({} -
+00001f00: 207b 7d29 203e 2030 2e30 3520 414e 4420   {}) > 0.05 AND 
+00001f10: 6162 7328 7b7d 202d 207b 7d29 203e 2030  abs({} - {}) > 0
+00001f20: 2e30 3520 414e 4420 7b7d 2021 3d20 3135  .05 AND {} != 15
+00001f30: 2902 7234 0000 0072 2e00 0000 7a06 636f  ).r4...r....z.co
+00001f40: 6e6e 312e 7a06 636f 6e6e 322e 7a08 7b7d  nn1.z.conn2.z.{}
+00001f50: 2021 3d20 7b7d 7a35 7b7d 2021 3d20 7b7d   != {}z5{} != {}
+00001f60: 2041 4e44 207b 7d20 213d 2030 2041 4e44   AND {} != 0 AND
+00001f70: 207b 7d20 213d 2030 2041 4e44 207b 7d20   {} != 0 AND {} 
+00001f80: 3c20 6d61 7828 7b7d 2c20 7b7d 297a 3e7b  < max({}, {})z>{
+00001f90: 7d20 213d 207b 7d20 414e 4420 7b7d 2021  } != {} AND {} !
+00001fa0: 3d20 3020 414e 4420 7b7d 2021 3d20 3020  = 0 AND {} != 0 
+00001fb0: 414e 4420 6d61 7828 7b7d 2c20 7b7d 2920  AND max({}, {}) 
+00001fc0: 3c20 6d61 7828 7b7d 2c20 7b7d 297a 087b  < max({}, {})z.{
+00001fd0: 7d20 3d20 3130 307a 116c 656e 6774 6828  } = 100z.length(
+00001fe0: 7b7d 2920 3e20 3130 3030 291a da19 6865  {}) > 1000)...he
+00001ff0: 6967 6874 5f6e 6f74 5f75 7365 645f 666f  ight_not_used_fo
+00002000: 725f 7368 6170 65da 226d 756c 7469 706c  r_shape."multipl
+00002010: 655f 6865 6967 6874 735f 7769 6474 6873  e_heights_widths
+00002020: 5f73 616d 655f 636f 756e 74da 2169 6d70  _same_count.!imp
+00002030: 6572 7669 6f75 735f 7375 7266 6163 655f  ervious_surface_
+00002040: 6e6f 745f 696e 5f6d 6170 7069 6e67 da2e  not_in_mapping..
+00002050: 696d 7065 7276 696f 7573 5f73 7572 6661  impervious_surfa
+00002060: 6365 5f6d 6170 5f72 6566 6572 735f 746f  ce_map_refers_to
+00002070: 5f69 6e76 5f63 6f6e 6e5f 6e6f 6465 da1c  _inv_conn_node..
+00002080: 7375 7266 6163 655f 6e6f 745f 696e 5f6d  surface_not_in_m
+00002090: 6170 7069 6e67 5f74 6162 6c65 da2d 696d  apping_table.-im
+000020a0: 7065 7276 696f 7573 5f73 7572 6661 6365  pervious_surface
+000020b0: 5f6d 6170 5f72 6566 6572 735f 746f 5f69  _map_refers_to_i
+000020c0: 6e76 5f69 6d70 5f73 7572 66da 1d63 6f6e  nv_imp_surf..con
+000020d0: 6e5f 6e6f 6465 5f77 6974 686f 7574 5f69  n_node_without_i
+000020e0: 6d70 5f73 7572 6661 6365 da19 6368 616e  mp_surface..chan
+000020f0: 6e65 6c5f 7769 7468 6f75 745f 6372 6f73  nel_without_cros
+00002100: 735f 6c6f 63da 2963 726f 7373 5f73 6563  s_loc.)cross_sec
+00002110: 7469 6f6e 5f6c 6f63 6174 696f 6e5f 7769  tion_location_wi
+00002120: 7468 6f75 745f 6465 6669 6e69 7469 6f6e  thout_definition
+00002130: da20 6375 6c76 6572 745f 7769 7468 6f75  . culvert_withou
+00002140: 745f 6372 6f73 735f 6465 6669 6e69 7469  t_cross_definiti
+00002150: 6f6e da1d 7765 6972 5f77 6974 686f 7574  on..weir_without
+00002160: 5f63 726f 7373 5f64 6566 696e 6974 696f  _cross_definitio
+00002170: 6eda 206f 7269 6669 6365 5f77 6974 686f  n. orifice_witho
+00002180: 7574 5f63 726f 7373 5f64 6566 696e 6974  ut_cross_definit
+00002190: 696f 6eda 196d 616e 686f 6c65 5f77 6974  ion..manhole_wit
+000021a0: 686f 7574 5f63 6f6e 6e5f 6e6f 6465 da20  hout_conn_node. 
+000021b0: 6f6e 655f 645f 626f 756e 6461 7279 5f77  one_d_boundary_w
+000021c0: 6974 686f 7574 5f63 6f6e 6e5f 6e6f 6465  ithout_conn_node
+000021d0: da1d 6372 6f73 735f 7365 635f 6c6f 635f  ..cross_sec_loc_
+000021e0: 7769 7468 6f75 745f 7265 665f 6c76 6cda  without_ref_lvl.
+000021f0: 2063 6f6e 6e5f 6e6f 6465 5f77 6974 686f   conn_node_witho
+00002200: 7574 5f69 6e69 745f 7761 7465 725f 6c76  ut_init_water_lv
+00002210: 6cda 1663 6f6e 6e5f 6e6f 6465 5f77 6974  l..conn_node_wit
+00002220: 686f 7574 5f63 6f6e 6eda 2473 7461 7274  hout_conn.$start
+00002230: 5f6c 766c 5f6e 6f74 5f63 6c6f 7365 5f74  _lvl_not_close_t
+00002240: 6f5f 696e 6974 5f77 6174 6572 6c76 6cda  o_init_waterlvl.
+00002250: 1875 6e64 6566 696e 6564 5f73 6861 7065  .undefined_shape
+00002260: 5f6f 725f 7769 6474 68da 1166 726f 6d5f  _or_width..from_
+00002270: 746f 5f73 616d 655f 6e6f 6465 da29 7765  to_same_node.)we
+00002280: 6972 5f73 7461 7274 5f6c 766c 5f6e 6f74  ir_start_lvl_not
+00002290: 5f63 6c6f 7365 5f74 6f5f 696e 6974 5f77  _close_to_init_w
+000022a0: 6174 6572 6c76 6cda 2763 6861 6e6e 656c  aterlvl.'channel
+000022b0: 5f73 7472 745f 656e 645f 6e6f 745f 7361  _strt_end_not_sa
+000022c0: 6d65 5f69 6e69 745f 7761 7465 726c 766c  me_init_waterlvl
+000022d0: da27 6f72 6966 6963 655f 7374 7274 5f65  .'orifice_strt_e
+000022e0: 6e64 5f6e 6f74 5f73 616d 655f 696e 6974  nd_not_same_init
+000022f0: 5f77 6174 6572 6c76 6cda 2763 756c 7665  _waterlvl.'culve
+00002300: 7274 5f73 7472 745f 656e 645f 6e6f 745f  rt_strt_end_not_
+00002310: 7361 6d65 5f69 6e69 745f 7761 7465 726c  same_init_waterl
+00002320: 766c da10 696d 705f 7375 7266 6163 655f  vl..imp_surface_
+00002330: 7065 7263 da17 6163 7469 6f6e 5f74 6162  perc..action_tab
+00002340: 6c65 5f63 6861 725f 636f 756e 7463 0000  le_char_countc..
+00002350: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00002360: 0000 4000 0000 7324 0000 0065 005a 0164  ..@...s$...e.Z.d
+00002370: 005a 0264 015a 0364 0264 0384 005a 0465  .Z.d.Z.d.d...Z.e
+00002380: 0564 0464 0584 0083 015a 0664 0653 0029  .d.d.....Z.d.S.)
+00002390: 07da 0a4d 6f64 656c 4368 6563 6b7a 550a  ...ModelCheckzU.
+000023a0: 2020 2020 486f 6c64 7320 616c 6c20 7465      Holds all te
+000023b0: 7374 7320 7468 6174 2061 7265 2070 6172  sts that are par
+000023c0: 7420 6f66 2074 6865 2067 656e 6572 616c  t of the general
+000023d0: 206d 6f64 656c 2063 6865 636b 7320 666f   model checks fo
+000023e0: 7220 6561 7369 6572 2061 6363 6573 730a  r easier access.
+000023f0: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+00002400: 0001 0000 0002 0000 0043 0000 0073 0801  .........C...s..
+00002410: 0000 7400 6401 1900 7c00 5f01 7400 6402  ..t.d...|._.t.d.
+00002420: 1900 7c00 5f02 7400 6403 1900 7c00 5f03  ..|._.t.d...|._.
+00002430: 7400 6404 1900 7c00 5f04 7400 6405 1900  t.d...|._.t.d...
+00002440: 7c00 5f05 7400 6406 1900 7c00 5f06 7400  |._.t.d...|._.t.
+00002450: 6407 1900 7c00 5f07 7400 6408 1900 7c00  d...|._.t.d...|.
+00002460: 5f08 7400 6409 1900 7c00 5f09 7400 640a  _.t.d...|._.t.d.
+00002470: 1900 7c00 5f0a 7400 640b 1900 7c00 5f0b  ..|._.t.d...|._.
+00002480: 7400 640c 1900 7c00 5f0c 7400 640d 1900  t.d...|._.t.d...
+00002490: 7c00 5f0d 7400 640e 1900 7c00 5f0e 7400  |._.t.d...|._.t.
+000024a0: 640f 1900 7c00 5f0f 7400 6410 1900 7c00  d...|._.t.d...|.
+000024b0: 5f10 7400 6411 1900 7c00 5f11 7400 6412  _.t.d...|._.t.d.
+000024c0: 1900 7c00 5f12 7400 6413 1900 7c00 5f13  ..|._.t.d...|._.
+000024d0: 7400 6414 1900 7c00 5f14 7400 6415 1900  t.d...|._.t.d...
+000024e0: 7c00 5f15 7400 6416 1900 7c00 5f16 7400  |._.t.d...|._.t.
+000024f0: 6417 1900 7c00 5f17 7400 6418 1900 7c00  d...|._.t.d...|.
+00002500: 5f18 7400 6419 1900 7c00 5f19 7400 641a  _.t.d...|._.t.d.
+00002510: 1900 7c00 5f1a 6400 5300 291b 4e72 5500  ..|._.d.S.).NrU.
+00002520: 0000 7256 0000 0072 5700 0000 7258 0000  ..rV...rW...rX..
+00002530: 0072 5900 0000 725a 0000 0072 5b00 0000  .rY...rZ...r[...
+00002540: 725c 0000 0072 5d00 0000 725e 0000 0072  r\...r]...r^...r
+00002550: 5f00 0000 7260 0000 0072 6100 0000 7262  _...r`...ra...rb
+00002560: 0000 0072 6300 0000 7264 0000 0072 6500  ...rc...rd...re.
+00002570: 0000 7266 0000 0072 6700 0000 7268 0000  ..rf...rg...rh..
+00002580: 0072 6900 0000 726a 0000 0072 6b00 0000  .ri...rj...rk...
+00002590: 726c 0000 0072 6d00 0000 726e 0000 0029  rl...rm...rn...)
+000025a0: 1bda 0c6d 6f64 656c 5f63 6865 636b 7372  ...model_checksr
+000025b0: 5500 0000 5a1d 6d75 6c74 6970 6c65 5f68  U...Z.multiple_h
+000025c0: 6569 6768 7473 5f77 6964 7468 735f 636f  eights_widths_co
+000025d0: 756e 7472 5700 0000 7258 0000 005a 1673  untrW...rX...Z.s
+000025e0: 7572 6661 6365 5f6e 6f74 5f69 6e5f 6d61  urface_not_in_ma
+000025f0: 7070 696e 675a 2169 6d70 6572 7669 6f75  ppingZ!imperviou
+00002600: 735f 6d61 705f 6e6f 745f 696e 5f69 6d70  s_map_not_in_imp
+00002610: 5f73 7572 6661 6365 725b 0000 005a 2663  _surfacer[...Z&c
+00002620: 6861 6e6e 656c 5f77 6974 686f 7574 5f63  hannel_without_c
+00002630: 726f 7373 5f73 6563 7469 6f6e 5f6c 6f63  ross_section_loc
+00002640: 6174 696f 6e5a 2463 726f 7373 5f73 6563  ationZ$cross_sec
+00002650: 7469 6f6e 5f6c 6f63 5f77 6974 686f 7574  tion_loc_without
+00002660: 5f64 6566 696e 6974 696f 6e5a 2863 756c  _definitionZ(cul
+00002670: 7665 7274 5f77 6974 686f 7574 5f63 726f  vert_without_cro
+00002680: 7373 5f73 6563 7469 6f6e 5f64 6566 696e  ss_section_defin
+00002690: 6974 696f 6e5a 2577 6569 725f 7769 7468  itionZ%weir_with
+000026a0: 6f75 745f 6372 6f73 735f 7365 6374 696f  out_cross_sectio
+000026b0: 6e5f 6465 6669 6e69 7469 6f6e 5a28 6f72  n_definitionZ(or
+000026c0: 6966 6963 655f 7769 7468 6f75 745f 6372  ifice_without_cr
+000026d0: 6f73 735f 7365 6374 696f 6e5f 6465 6669  oss_section_defi
+000026e0: 6e69 7469 6f6e 7261 0000 0072 6200 0000  nitionra...rb...
+000026f0: 7263 0000 0072 6400 0000 7265 0000 005a  rc...rd...re...Z
+00002700: 2173 7461 7274 5f6c 766c 5f6e 6f74 5f63  !start_lvl_not_c
+00002710: 6c6f 7365 5f69 6e69 745f 7761 7465 726c  lose_init_waterl
+00002720: 766c 5a18 7368 6170 655f 6f72 5f77 6964  vlZ.shape_or_wid
+00002730: 7468 5f75 6e64 6566 696e 6564 7268 0000  th_undefinedrh..
+00002740: 0072 6900 0000 726a 0000 0072 6b00 0000  .ri...rj...rk...
+00002750: 726c 0000 005a 1769 6d70 6572 7669 6f75  rl...Z.imperviou
+00002760: 735f 7375 7266 6163 655f 7065 7263 5a1b  s_surface_percZ.
+00002770: 6163 7469 6f6e 5f74 6162 6c65 5f74 6f6f  action_table_too
+00002780: 5f6d 616e 795f 6368 6172 7329 01da 0473  _many_chars)...s
+00002790: 656c 6672 2a00 0000 722a 0000 0072 3000  elfr*...r*...r0.
+000027a0: 0000 da08 5f5f 696e 6974 5f5f fa01 0000  ....__init__....
+000027b0: 7338 0000 0000 010a 010a 010a 0102 0102  s8..............
+000027c0: ff06 030a 010a 010a 010a 010a 010a 010a  ................
 000027d0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000027e0: 010a 017a 134d 6f64 656c 4368 6563 6b2e  ...z.ModelCheck.
-000027f0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00002800: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00002810: 0073 2200 0000 6401 6402 8400 7400 7c00  .s"...d.d...t.|.
-00002820: 8300 8301 a001 a100 4400 8301 7d01 6403  ........D...}.d.
-00002830: a002 7c01 a101 5300 2904 7a30 4765 7420  ..|...S.).z0Get 
-00002840: 6120 616c 6c20 7661 7269 6162 6c65 7320  a all variables 
-00002850: 6173 2071 7565 7279 2074 6f20 6578 6563  as query to exec
-00002860: 7574 6520 6f6e 206d 6f64 656c 6301 0000  ute on modelc...
-00002870: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00002880: 0053 0000 0073 1000 0000 6700 7c00 5d08  .S...s....g.|.].
-00002890: 7d01 7c01 9102 7104 5300 722a 0000 0072  }.|...q.S.r*...r
-000028a0: 2a00 0000 2902 da02 2e30 da04 6974 656d  *...)....0..item
-000028b0: 722a 0000 0072 2a00 0000 7230 0000 00da  r*...r*...r0....
-000028c0: 0a3c 6c69 7374 636f 6d70 3e1b 0200 00f3  .<listcomp>.....
-000028d0: 0000 0000 7a28 4d6f 6465 6c43 6865 636b  ....z(ModelCheck
-000028e0: 2e67 6574 5f71 7565 7279 2e3c 6c6f 6361  .get_query.<loca
-000028f0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7243  ls>.<listcomp>rC
-00002900: 0000 0029 03da 0476 6172 73da 0676 616c  ...)...vars..val
-00002910: 7565 73da 046a 6f69 6e29 02da 0363 6c73  ues..join)...cls
-00002920: da0b 7175 6572 6965 735f 6c73 7472 2a00  ..queries_lstr*.
-00002930: 0000 722a 0000 0072 3000 0000 da09 6765  ..r*...r0.....ge
-00002940: 745f 7175 6572 7918 0200 0073 0400 0000  t_query....s....
-00002950: 0003 1801 7a14 4d6f 6465 6c43 6865 636b  ....z.ModelCheck
-00002960: 2e67 6574 5f71 7565 7279 4e29 07da 085f  .get_queryN)..._
-00002970: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00002980: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00002990: 5fda 075f 5f64 6f63 5f5f 7272 0000 00da  _..__doc__rr....
-000029a0: 0b63 6c61 7373 6d65 7468 6f64 727c 0000  .classmethodr|..
-000029b0: 0072 2a00 0000 722a 0000 0072 2a00 0000  .r*...r*...r*...
-000029c0: 7230 0000 0072 6f00 0000 f501 0000 7308  r0...ro.......s.
-000029d0: 0000 0008 0104 0408 1e02 0172 6f00 0000  ...........ro...
-000029e0: 2903 4646 4e29 4dda 2f68 686e 6b5f 7468  ).FFN)M./hhnk_th
-000029f0: 7265 6564 695f 746f 6f6c 732e 7661 7269  reedi_tools.vari
-00002a00: 6162 6c65 732e 6461 7461 6261 7365 5f76  ables.database_v
-00002a10: 6172 6961 626c 6573 7202 0000 0072 0300  ariablesr....r..
-00002a20: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00002a30: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00002a40: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00002a50: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00002a60: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00002a70: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00002a80: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-00002a90: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-00002aa0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-00002ab0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
-00002ac0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
-00002ad0: 0072 2700 0000 5a1d 6d73 675f 6865 6967  .r'...Z.msg_heig
-00002ae0: 6874 5f6e 6f74 5f75 7365 645f 666f 725f  ht_not_used_for_
-00002af0: 7368 6170 655a 176d 7367 5f75 6e65 7665  shapeZ.msg_uneve
-00002b00: 6e5f 7769 6474 685f 6865 6967 6874 5a19  n_width_heightZ.
-00002b10: 6d73 675f 696d 7065 7276 696f 7573 5f6e  msg_impervious_n
-00002b20: 6f74 5f69 6e5f 6d61 705a 216d 7367 5f69  ot_in_mapZ!msg_i
-00002b30: 6d70 6572 7669 6f75 735f 6d61 705f 7265  mpervious_map_re
-00002b40: 6665 7273 5f74 6f5f 6e6f 6e65 5a1a 6d73  fers_to_noneZ.ms
-00002b50: 675f 7375 7266 6163 655f 6e6f 745f 696e  g_surface_not_in
-00002b60: 5f6d 6170 7069 6e67 5a2c 6d73 675f 696d  _mappingZ,msg_im
-00002b70: 7065 7276 696f 7573 5f73 7572 6661 6365  pervious_surface
-00002b80: 5f6d 6170 5f6e 6f74 5f69 6e5f 696d 7065  _map_not_in_impe
-00002b90: 7276 696f 7573 5a21 6d73 675f 636f 6e6e  rviousZ!msg_conn
-00002ba0: 5f6e 6f64 655f 7769 7468 6f75 745f 696d  _node_without_im
-00002bb0: 705f 7375 7266 6163 655a 1d6d 7367 5f63  p_surfaceZ.msg_c
-00002bc0: 6861 6e6e 656c 5f77 6974 686f 7574 5f63  hannel_without_c
-00002bd0: 726f 7373 5f6c 6f63 5a1d 6d73 675f 6372  ross_locZ.msg_cr
-00002be0: 6f73 735f 7365 635f 6c6f 635f 7769 7468  oss_sec_loc_with
-00002bf0: 6f75 745f 6465 665a 176d 7367 5f63 756c  out_defZ.msg_cul
-00002c00: 7665 7274 5f77 6974 686f 7574 5f64 6566  vert_without_def
-00002c10: 5a14 6d73 675f 7765 6972 5f77 6974 686f  Z.msg_weir_witho
-00002c20: 7574 5f64 6566 5a17 6d73 675f 6f72 6966  ut_defZ.msg_orif
-00002c30: 6963 655f 7769 7468 6f75 745f 6465 665a  ice_without_defZ
-00002c40: 1d6d 7367 5f6d 616e 686f 6c65 5f77 6974  .msg_manhole_wit
-00002c50: 686f 7574 5f63 6f6e 6e5f 6e6f 6465 5a24  hout_conn_nodeZ$
-00002c60: 6d73 675f 6f6e 655f 645f 626f 756e 6461  msg_one_d_bounda
-00002c70: 7279 5f63 6f6e 645f 7769 7468 6f75 745f  ry_cond_without_
-00002c80: 636f 6e6e 5a21 6d73 675f 6372 6f73 735f  connZ!msg_cross_
-00002c90: 7365 635f 6c6f 635f 7769 7468 6f75 745f  sec_loc_without_
-00002ca0: 7265 665f 6c76 6c5a 246d 7367 5f63 6f6e  ref_lvlZ$msg_con
-00002cb0: 6e5f 6e6f 6465 5f77 6974 686f 7574 5f69  n_node_without_i
-00002cc0: 6e69 745f 7761 7465 725f 6c76 6c5a 1a6d  nit_water_lvlZ.m
-00002cd0: 7367 5f63 6f6e 6e5f 6e6f 6465 5f77 6974  sg_conn_node_wit
-00002ce0: 686f 7574 5f63 6f6e 6e5a 246d 7367 5f73  hout_connZ$msg_s
-00002cf0: 7472 745f 6c76 6c5f 6e6f 745f 636c 6f73  trt_lvl_not_clos
-00002d00: 655f 696e 6974 5f77 6174 6572 6c76 6c5a  e_init_waterlvlZ
-00002d10: 1c6d 7367 5f75 6e64 6566 696e 6564 5f73  .msg_undefined_s
-00002d20: 6861 7065 5f6f 725f 7769 6474 6872 4f00  hape_or_widthrO.
-00002d30: 0000 7250 0000 0072 5100 0000 7252 0000  ..rP...rQ...rR..
-00002d40: 005a 2d6d 7367 5f77 6569 725f 7374 6172  .Z-msg_weir_star
-00002d50: 745f 6c76 6c5f 6e6f 745f 636c 6f73 655f  t_lvl_not_close_
-00002d60: 746f 5f69 6e69 745f 7761 7465 726c 766c  to_init_waterlvl
-00002d70: 5a2b 6d73 675f 6368 616e 6e65 6c5f 7374  Z+msg_channel_st
-00002d80: 7274 5f65 6e64 5f6e 6f74 5f73 616d 655f  rt_end_not_same_
-00002d90: 696e 6974 5f77 6174 6572 6c76 6c5a 2b6d  init_waterlvlZ+m
-00002da0: 7367 5f6f 7269 6669 6365 5f73 7472 745f  sg_orifice_strt_
-00002db0: 656e 645f 6e6f 745f 7361 6d65 5f69 6e69  end_not_same_ini
-00002dc0: 745f 7761 7465 726c 766c 5a2b 6d73 675f  t_waterlvlZ+msg_
-00002dd0: 6375 6c76 6572 745f 7374 7274 5f65 6e64  culvert_strt_end
-00002de0: 5f6e 6f74 5f73 616d 655f 696e 6974 5f77  _not_same_init_w
-00002df0: 6174 6572 6c76 6c5a 146d 7367 5f69 6d70  aterlvlZ.msg_imp
-00002e00: 5f73 7572 6661 6365 5f70 6572 635a 206d  _surface_percZ m
-00002e10: 7367 5f63 6f6e 7472 6f6c 5f74 6162 6c65  sg_control_table
-00002e20: 5f74 6f6f 5f6d 616e 795f 6368 6172 7372  _too_many_charsr
-00002e30: 3100 0000 7237 0000 0072 3f00 0000 7240  1...r7...r?...r@
-00002e40: 0000 0072 4d00 0000 7253 0000 0072 4600  ...rM...rS...rF.
-00002e50: 0000 7270 0000 0072 6f00 0000 722a 0000  ..rp...ro...r*..
-00002e60: 0072 2a00 0000 722a 0000 0072 3000 0000  .r*...r*...r0...
-00002e70: da08 3c6d 6f64 756c 653e 0100 0000 738a  ..<module>....s.
-00002e80: 0200 00a0 2a04 0104 0104 0104 0104 0104  ....*...........
+000027e0: 010a 010a 010a 010a 010a 010a 017a 134d  .............z.M
+000027f0: 6f64 656c 4368 6563 6b2e 5f5f 696e 6974  odelCheck.__init
+00002800: 5f5f 6301 0000 0000 0000 0000 0000 0002  __c.............
+00002810: 0000 0003 0000 0043 0000 0073 2200 0000  .......C...s"...
+00002820: 6401 6402 8400 7400 7c00 8300 8301 a001  d.d...t.|.......
+00002830: a100 4400 8301 7d01 6403 a002 7c01 a101  ..D...}.d...|...
+00002840: 5300 2904 7a30 4765 7420 6120 616c 6c20  S.).z0Get a all 
+00002850: 7661 7269 6162 6c65 7320 6173 2071 7565  variables as que
+00002860: 7279 2074 6f20 6578 6563 7574 6520 6f6e  ry to execute on
+00002870: 206d 6f64 656c 6301 0000 0000 0000 0000   modelc.........
+00002880: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00002890: 1000 0000 6700 7c00 5d08 7d01 7c01 9102  ....g.|.].}.|...
+000028a0: 7104 5300 722a 0000 0072 2a00 0000 2902  q.S.r*...r*...).
+000028b0: da02 2e30 da04 6974 656d 722a 0000 0072  ...0..itemr*...r
+000028c0: 2a00 0000 7230 0000 00da 0a3c 6c69 7374  *...r0.....<list
+000028d0: 636f 6d70 3e1b 0200 00f3 0000 0000 7a28  comp>.........z(
+000028e0: 4d6f 6465 6c43 6865 636b 2e67 6574 5f71  ModelCheck.get_q
+000028f0: 7565 7279 2e3c 6c6f 6361 6c73 3e2e 3c6c  uery.<locals>.<l
+00002900: 6973 7463 6f6d 703e 7243 0000 0029 03da  istcomp>rC...)..
+00002910: 0476 6172 73da 0676 616c 7565 73da 046a  .vars..values..j
+00002920: 6f69 6e29 02da 0363 6c73 da0b 7175 6572  oin)...cls..quer
+00002930: 6965 735f 6c73 7472 2a00 0000 722a 0000  ies_lstr*...r*..
+00002940: 0072 3000 0000 da09 6765 745f 7175 6572  .r0.....get_quer
+00002950: 7918 0200 0073 0400 0000 0003 1801 7a14  y....s........z.
+00002960: 4d6f 6465 6c43 6865 636b 2e67 6574 5f71  ModelCheck.get_q
+00002970: 7565 7279 4e29 07da 085f 5f6e 616d 655f  ueryN)...__name_
+00002980: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00002990: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+000029a0: 6f63 5f5f 7272 0000 00da 0b63 6c61 7373  oc__rr.....class
+000029b0: 6d65 7468 6f64 727c 0000 0072 2a00 0000  methodr|...r*...
+000029c0: 722a 0000 0072 2a00 0000 7230 0000 0072  r*...r*...r0...r
+000029d0: 6f00 0000 f501 0000 7308 0000 0008 0104  o.......s.......
+000029e0: 0408 1e02 0172 6f00 0000 2903 4646 4e29  .....ro...).FFN)
+000029f0: 4dda 2f68 686e 6b5f 7468 7265 6564 695f  M./hhnk_threedi_
+00002a00: 746f 6f6c 732e 7661 7269 6162 6c65 732e  tools.variables.
+00002a10: 6461 7461 6261 7365 5f76 6172 6961 626c  database_variabl
+00002a20: 6573 7202 0000 0072 0300 0000 7204 0000  esr....r....r...
+00002a30: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+00002a40: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00002a50: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
+00002a60: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00002a70: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00002a80: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00002a90: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00002aa0: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+00002ab0: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+00002ac0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+00002ad0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+00002ae0: 5a1d 6d73 675f 6865 6967 6874 5f6e 6f74  Z.msg_height_not
+00002af0: 5f75 7365 645f 666f 725f 7368 6170 655a  _used_for_shapeZ
+00002b00: 176d 7367 5f75 6e65 7665 6e5f 7769 6474  .msg_uneven_widt
+00002b10: 685f 6865 6967 6874 5a19 6d73 675f 696d  h_heightZ.msg_im
+00002b20: 7065 7276 696f 7573 5f6e 6f74 5f69 6e5f  pervious_not_in_
+00002b30: 6d61 705a 216d 7367 5f69 6d70 6572 7669  mapZ!msg_impervi
+00002b40: 6f75 735f 6d61 705f 7265 6665 7273 5f74  ous_map_refers_t
+00002b50: 6f5f 6e6f 6e65 5a1a 6d73 675f 7375 7266  o_noneZ.msg_surf
+00002b60: 6163 655f 6e6f 745f 696e 5f6d 6170 7069  ace_not_in_mappi
+00002b70: 6e67 5a2c 6d73 675f 696d 7065 7276 696f  ngZ,msg_impervio
+00002b80: 7573 5f73 7572 6661 6365 5f6d 6170 5f6e  us_surface_map_n
+00002b90: 6f74 5f69 6e5f 696d 7065 7276 696f 7573  ot_in_impervious
+00002ba0: 5a21 6d73 675f 636f 6e6e 5f6e 6f64 655f  Z!msg_conn_node_
+00002bb0: 7769 7468 6f75 745f 696d 705f 7375 7266  without_imp_surf
+00002bc0: 6163 655a 1d6d 7367 5f63 6861 6e6e 656c  aceZ.msg_channel
+00002bd0: 5f77 6974 686f 7574 5f63 726f 7373 5f6c  _without_cross_l
+00002be0: 6f63 5a1d 6d73 675f 6372 6f73 735f 7365  ocZ.msg_cross_se
+00002bf0: 635f 6c6f 635f 7769 7468 6f75 745f 6465  c_loc_without_de
+00002c00: 665a 176d 7367 5f63 756c 7665 7274 5f77  fZ.msg_culvert_w
+00002c10: 6974 686f 7574 5f64 6566 5a14 6d73 675f  ithout_defZ.msg_
+00002c20: 7765 6972 5f77 6974 686f 7574 5f64 6566  weir_without_def
+00002c30: 5a17 6d73 675f 6f72 6966 6963 655f 7769  Z.msg_orifice_wi
+00002c40: 7468 6f75 745f 6465 665a 1d6d 7367 5f6d  thout_defZ.msg_m
+00002c50: 616e 686f 6c65 5f77 6974 686f 7574 5f63  anhole_without_c
+00002c60: 6f6e 6e5f 6e6f 6465 5a24 6d73 675f 6f6e  onn_nodeZ$msg_on
+00002c70: 655f 645f 626f 756e 6461 7279 5f63 6f6e  e_d_boundary_con
+00002c80: 645f 7769 7468 6f75 745f 636f 6e6e 5a21  d_without_connZ!
+00002c90: 6d73 675f 6372 6f73 735f 7365 635f 6c6f  msg_cross_sec_lo
+00002ca0: 635f 7769 7468 6f75 745f 7265 665f 6c76  c_without_ref_lv
+00002cb0: 6c5a 246d 7367 5f63 6f6e 6e5f 6e6f 6465  lZ$msg_conn_node
+00002cc0: 5f77 6974 686f 7574 5f69 6e69 745f 7761  _without_init_wa
+00002cd0: 7465 725f 6c76 6c5a 1a6d 7367 5f63 6f6e  ter_lvlZ.msg_con
+00002ce0: 6e5f 6e6f 6465 5f77 6974 686f 7574 5f63  n_node_without_c
+00002cf0: 6f6e 6e5a 246d 7367 5f73 7472 745f 6c76  onnZ$msg_strt_lv
+00002d00: 6c5f 6e6f 745f 636c 6f73 655f 696e 6974  l_not_close_init
+00002d10: 5f77 6174 6572 6c76 6c5a 1c6d 7367 5f75  _waterlvlZ.msg_u
+00002d20: 6e64 6566 696e 6564 5f73 6861 7065 5f6f  ndefined_shape_o
+00002d30: 725f 7769 6474 6872 4f00 0000 7250 0000  r_widthrO...rP..
+00002d40: 0072 5100 0000 7252 0000 005a 2d6d 7367  .rQ...rR...Z-msg
+00002d50: 5f77 6569 725f 7374 6172 745f 6c76 6c5f  _weir_start_lvl_
+00002d60: 6e6f 745f 636c 6f73 655f 746f 5f69 6e69  not_close_to_ini
+00002d70: 745f 7761 7465 726c 766c 5a2b 6d73 675f  t_waterlvlZ+msg_
+00002d80: 6368 616e 6e65 6c5f 7374 7274 5f65 6e64  channel_strt_end
+00002d90: 5f6e 6f74 5f73 616d 655f 696e 6974 5f77  _not_same_init_w
+00002da0: 6174 6572 6c76 6c5a 2b6d 7367 5f6f 7269  aterlvlZ+msg_ori
+00002db0: 6669 6365 5f73 7472 745f 656e 645f 6e6f  fice_strt_end_no
+00002dc0: 745f 7361 6d65 5f69 6e69 745f 7761 7465  t_same_init_wate
+00002dd0: 726c 766c 5a2b 6d73 675f 6375 6c76 6572  rlvlZ+msg_culver
+00002de0: 745f 7374 7274 5f65 6e64 5f6e 6f74 5f73  t_strt_end_not_s
+00002df0: 616d 655f 696e 6974 5f77 6174 6572 6c76  ame_init_waterlv
+00002e00: 6c5a 146d 7367 5f69 6d70 5f73 7572 6661  lZ.msg_imp_surfa
+00002e10: 6365 5f70 6572 635a 206d 7367 5f63 6f6e  ce_percZ msg_con
+00002e20: 7472 6f6c 5f74 6162 6c65 5f74 6f6f 5f6d  trol_table_too_m
+00002e30: 616e 795f 6368 6172 7372 3100 0000 7237  any_charsr1...r7
+00002e40: 0000 0072 3f00 0000 7240 0000 0072 4d00  ...r?...r@...rM.
+00002e50: 0000 7253 0000 0072 4600 0000 7270 0000  ..rS...rF...rp..
+00002e60: 0072 6f00 0000 722a 0000 0072 2a00 0000  .ro...r*...r*...
+00002e70: 722a 0000 0072 3000 0000 da08 3c6d 6f64  r*...r0.....<mod
+00002e80: 756c 653e 0100 0000 738a 0200 00a0 2a04  ule>....s.....*.
 00002e90: 0104 0104 0104 0104 0104 0104 0104 0104  ................
 00002ea0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00002eb0: 0104 0202 ff02 0402 ff02 0402 ff02 0402  ................
-00002ec0: ff02 0304 0104 030a 1d14 1c08 0508 0508  ................
-00002ed0: 1308 1a0a 0108 0102 010a 010a fc02 070a  ................
-00002ee0: 0108 0102 010a 010a 010a 010a fa02 0902  ................
-00002ef0: 0110 ff06 0308 0102 010c 0102 0102 f902  ................
-00002f00: 0a02 0110 ff06 0308 0102 010c 0102 0102  ................
-00002f10: f902 0a02 0110 ff06 0308 0102 010c 0102  ................
-00002f20: 0102 f902 0a02 0110 ff06 0308 0102 010c  ................
-00002f30: 0102 0102 f902 0a02 0102 0102 0102 0102  ................
-00002f40: 0102 010c fc04 ff02 ff06 0908 0102 010c  ................
-00002f50: 010c 0102 010c 010c 0102 f002 1302 0108  ................
-00002f60: ff06 0308 0102 0102 010c 010c 010c f802  ................
-00002f70: 0b02 0108 ff06 0308 0102 0102 010c 010c  ................
-00002f80: 010c f802 0b02 0108 ff06 0308 0102 0102  ................
-00002f90: 010c 010c 010c f802 0b02 0108 ff06 0308  ................
-00002fa0: 0102 0102 010c 010c 010c f802 0b02 0108  ................
-00002fb0: ff06 0308 0102 0102 010c 010c 010c f802  ................
-00002fc0: 0b02 0108 ff06 0308 0102 0102 010c 010c  ................
-00002fd0: 010c f802 0b02 0108 ff06 0308 0102 0102  ................
-00002fe0: 010c 010c 010c f802 0b0a 0108 0102 0102  ................
-00002ff0: fd02 060a 0108 0102 0102 fd02 0602 010c  ................
-00003000: ff06 0308 0102 010c fb02 0802 0108 ff06  ................
-00003010: 0308 0102 0102 010c 010c 010c 010c f702  ................
-00003020: 0c0a 0108 0102 0102 0102 0102 fb02 0804  ................
-00003030: 0202 0108 0102 fe06 0402 0102 0104 010c  ................
-00003040: 0108 0108 fd02 fe02 0802 0102 010c 0108  ................
-00003050: 0102 010c 0108 0108 010c 0108 010c 010c  ................
-00003060: e902 1a02 010a ff06 0302 0102 0104 0110  ................
-00003070: ff02 fe02 0602 0102 010c 0108 0102 010c  ................
-00003080: 0108 0108 0108 ef02 1402 0108 0102 fe06  ................
-00003090: 0402 0102 0104 0110 ff02 fe02 0602 0102  ................
-000030a0: 010c 0108 0102 010c 0108 0108 0108 010c  ................
-000030b0: 010c 010c 0108 0108 e902 1a02 0108 0102  ................
-000030c0: fe06 0402 0102 0104 0110 ff02 fe02 0602  ................
-000030d0: 0102 010c 0108 0102 010c 0108 0108 0108  ................
-000030e0: 010c 010c 010c 010c 0108 0108 e802 1b0a  ................
-000030f0: 0108 0102 010c fd02 060a 0108 0102 010c  ................
-00003100: fd02 8000 8000 d306 7f00 7f00 37         ............7
+00002eb0: 0104 0104 0104 0104 0104 0104 0202 ff02  ................
+00002ec0: 0402 ff02 0402 ff02 0402 ff02 0304 0104  ................
+00002ed0: 030a 1d14 1c08 0508 0508 1308 1a0a 0108  ................
+00002ee0: 0102 010a 010a fc02 070a 0108 0102 010a  ................
+00002ef0: 010a 010a 010a fa02 0902 0110 ff06 0308  ................
+00002f00: 0102 010c 0102 0102 f902 0a02 0110 ff06  ................
+00002f10: 0308 0102 010c 0102 0102 f902 0a02 0110  ................
+00002f20: ff06 0308 0102 010c 0102 0102 f902 0a02  ................
+00002f30: 0110 ff06 0308 0102 010c 0102 0102 f902  ................
+00002f40: 0a02 0102 0102 0102 0102 0102 010c fc04  ................
+00002f50: ff02 ff06 0908 0102 010c 010c 0102 010c  ................
+00002f60: 010c 0102 f002 1302 0108 ff06 0308 0102  ................
+00002f70: 0102 010c 010c 010c f802 0b02 0108 ff06  ................
+00002f80: 0308 0102 0102 010c 010c 010c f802 0b02  ................
+00002f90: 0108 ff06 0308 0102 0102 010c 010c 010c  ................
+00002fa0: f802 0b02 0108 ff06 0308 0102 0102 010c  ................
+00002fb0: 010c 010c f802 0b02 0108 ff06 0308 0102  ................
+00002fc0: 0102 010c 010c 010c f802 0b02 0108 ff06  ................
+00002fd0: 0308 0102 0102 010c 010c 010c f802 0b02  ................
+00002fe0: 0108 ff06 0308 0102 0102 010c 010c 010c  ................
+00002ff0: f802 0b0a 0108 0102 0102 fd02 060a 0108  ................
+00003000: 0102 0102 fd02 0602 010c ff06 0308 0102  ................
+00003010: 010c fb02 0802 0108 ff06 0308 0102 0102  ................
+00003020: 010c 010c 010c 010c f702 0c0a 0108 0102  ................
+00003030: 0102 0102 0102 fb02 0804 0202 0108 0102  ................
+00003040: fe06 0402 0102 0104 010c 0108 0108 fd02  ................
+00003050: fe02 0802 0102 010c 0108 0102 010c 0108  ................
+00003060: 0108 010c 0108 010c 010c e902 1a02 010a  ................
+00003070: ff06 0302 0102 0104 0110 ff02 fe02 0602  ................
+00003080: 0102 010c 0108 0102 010c 0108 0108 0108  ................
+00003090: ef02 1402 0108 0102 fe06 0402 0102 0104  ................
+000030a0: 0110 ff02 fe02 0602 0102 010c 0108 0102  ................
+000030b0: 010c 0108 0108 0108 010c 010c 010c 0108  ................
+000030c0: 0108 e902 1a02 0108 0102 fe06 0402 0102  ................
+000030d0: 0104 0110 ff02 fe02 0602 0102 010c 0108  ................
+000030e0: 0102 010c 0108 0108 0108 010c 010c 010c  ................
+000030f0: 010c 0108 0108 e802 1b0a 0108 0102 010c  ................
+00003100: fd02 060a 0108 0102 010c fd02 8000 8000  ................
+00003110: d306 7f00 7f00 37                        ......7
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980978260869565%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '# Add qgis plugin deps to syspath and load "*

 * *            "notebook_data\\n'), (2, '\\n'), (17, 'self.w.model.schema_name_widget.value = "*

 * *            "self.vars.folder.name  # default name\\n'), (19, 'display(self.tab)')], delete: [18, "*

 * *            '16, 0]}}}'}*

```diff
@@ -24,33 +24,34 @@
                     "end_time": "2021-10-15T22:52:50.428346Z",
                     "start_time": "2021-10-15T22:52:46.818054Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "#Add qgis plugin deps to syspath and load notebook_data\n",
+                "# Add qgis plugin deps to syspath and load notebook_data\n",
                 "from notebook_setup import setup_notebook\n",
+                "\n",
                 "notebook_data = setup_notebook()\n",
                 "\n",
                 "\n",
                 "# ipython imports\n",
                 "import ipywidgets as widgets\n",
                 "from IPython.display import display, HTML\n",
                 "\n",
                 "display(HTML(\"<style>.container {width:90% !important;}</style>\"))\n",
                 "%matplotlib inline\n",
                 "\n",
                 "\n",
                 "from hhnk_threedi_tools.core.api.calculation_gui_class import StartCalculationGui\n",
                 "\n",
                 "self = StartCalculationGui(data=notebook_data)\n",
-                "self.w.model.schema_name_widget.value = self.vars.folder.name #default name\n",
+                "self.w.model.schema_name_widget.value = self.vars.folder.name  # default name\n",
                 "\n",
-                "display(self.tab) "
+                "display(self.tab)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993262653898769%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '# Add qgis plugin deps to syspath and load "*

 * *            "notebook_data\\n'), (2, '\\n')], delete: [0]}}, 4: {'source': {insert: [(39, '        "*

 * *            'dl.download_waterdepth_raster(uuid, "EPSG:28992", resolution, time, '*

 * *            "pathname=wdepth_path[index])')], delete: [41, 40, 39]}}}"}*

```diff
@@ -18,16 +18,17 @@
                 "ExecuteTime": {
                     "end_time": "2021-10-18T07:27:41.321541Z",
                     "start_time": "2021-10-18T07:27:41.025441Z"
                 }
             },
             "outputs": [],
             "source": [
-                "#Add qgis plugin deps to syspath and load notebook_data\n",
+                "# Add qgis plugin deps to syspath and load notebook_data\n",
                 "from notebook_setup import setup_notebook\n",
+                "\n",
                 "notebook_data = setup_notebook()\n",
                 "\n",
                 "from IPython.display import display, HTML\n",
                 "\n",
                 "display(HTML(\"<style>.container {width:90% !important;}</style>\"))\n",
                 "%matplotlib inline\n",
                 "\n",
@@ -111,17 +112,15 @@
                 "    time_path = time.replace(\"-\", \"_\")\n",
                 "    time_path = time_path.replace(\":\", \"_\")\n",
                 "\n",
                 "    wdepth_path += [os.path.join(output_folder, \"wdepth_\" + time_path + \".tif\")]\n",
                 "    wdepth_path[index]\n",
                 "    if not os.path.exists(wdepth_path[index]):\n",
                 "        print(\"Preparing download: {}\".format(time_path))\n",
-                "        dl.download_waterdepth_raster(\n",
-                "            uuid, \"EPSG:28992\", resolution, time, pathname=wdepth_path[index]\n",
-                "        )"
+                "        dl.download_waterdepth_raster(uuid, \"EPSG:28992\", resolution, time, pathname=wdepth_path[index])"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984261718056806%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '\\n'), (31, 'folder = "*

 * *            'Folders(notebook_data["polder_folder"])\\n\'), (34, \'# '*

 * *            'folder=Folders(r"E:\\\\02.modellen\\\\model_test_v2")\')], delete: [33, 30]}}, 3: '*

 * *            "{'source': {insert: [(41, 'precip_zones_raster = "*

 * *            'hrt.get_pkg_resource_path(package_resource=htt.resources, '*

 * *            'name="precipitation_zones_hhnk.tif")\\n\'), (46, \'freqs_xlsx = '*

 * *            'hrt.get_pkg_resource_path(package_resource=htt.r […]*

```diff
@@ -19,14 +19,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "166eb613",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from notebook_setup import setup_notebook\n",
+                "\n",
                 "notebook_data = setup_notebook()\n",
                 "\n",
                 "import os\n",
                 "import geopandas as gpd\n",
                 "import pandas as pd\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
@@ -48,18 +49,18 @@
                 "import hhnk_threedi_tools.core.climate_scenarios.schadekaart as schadekaart\n",
                 "import hhnk_threedi_tools.core.climate_scenarios.peilgebieden as peilgebieden\n",
                 "from hhnk_threedi_tools.core.climate_scenarios.schadekaart_peilgebieden import maak_schade_polygon\n",
                 "from hhnk_threedi_tools.core.climate_scenarios.maskerkaart_raster import rasterize_maskerkaart\n",
                 "from hhnk_threedi_tools.core.climate_scenarios.klimaatsommen_prep import KlimaatsommenPrep\n",
                 "\n",
                 "# Folders inladen\n",
-                "folder = Folders(notebook_data['polder_folder'])\n",
+                "folder = Folders(notebook_data[\"polder_folder\"])\n",
                 "\n",
                 "# Of handmatig;\n",
-                "# folder=Folders(r\"E:\\02.modellen\\model_test_v2\")\n"
+                "# folder=Folders(r\"E:\\02.modellen\\model_test_v2\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "8ec3f357",
             "metadata": {},
@@ -111,27 +112,25 @@
                 "#     dem_path_dropdown.options = [folder.model.schema_base.rasters.dem.name]\n",
                 "# # Batch folder selection\n",
                 "\n",
                 "\n",
                 "# Display precipitation zones\n",
                 "polder_shape = folder.source_data.polder_polygon.load()\n",
                 "\n",
-                "precip_zones_raster = hrt.get_pkg_resource_path(package_resource=htt.resources, \n",
-                "                      name=\"precipitation_zones_hhnk.tif\")\n",
+                "precip_zones_raster = hrt.get_pkg_resource_path(package_resource=htt.resources, name=\"precipitation_zones_hhnk.tif\")\n",
                 "precip_zones_raster = hrt.Raster(precip_zones_raster)\n",
                 "neerslag_array = precip_zones_raster.get_array(band_count=3)\n",
                 "\n",
                 "\n",
-                "freqs_xlsx = hrt.get_pkg_resource_path(package_resource=htt.resources, \n",
-                "                      name=\"precipitation_frequency.xlsx\")\n",
+                "freqs_xlsx = hrt.get_pkg_resource_path(package_resource=htt.resources, name=\"precipitation_frequency.xlsx\")\n",
                 "freqs = pd.read_excel(freqs_xlsx, engine=\"openpyxl\")\n",
                 "\n",
                 "fig, ax = plt.subplots(figsize=(8, 8))\n",
                 "ax.imshow(neerslag_array, extent=precip_zones_raster.metadata.bounds)\n",
-                "polder_shape.plot(ax=ax, color='red')\n",
+                "polder_shape.plot(ax=ax, color=\"red\")\n",
                 "\n",
                 "\n",
                 "precipitation_zone_box = widgets.Select(\n",
                 "    options=[\"hevig\", \"debilt\"],\n",
                 "    rows=2,\n",
                 "    disabled=False,\n",
                 "    value=None,\n",
@@ -173,23 +172,17 @@
                 "if dem.metadata.pixel_width != 0.5:\n",
                 "    new_dem_path = batch_fd.downloads.full_path(f\"{dem.stem}_05m.tif\")\n",
                 "    dem = hrt.Raster(new_dem_path)\n",
                 "\n",
                 "\n",
                 "df = pd.DataFrame(batch_fd.downloads.names, columns=[\"dl_name\"])\n",
                 "for dl_name in batch_fd.downloads.names:\n",
-                "    df.loc[df[\"dl_name\"] == dl_name, \"wlvl_max\"] = getattr(\n",
-                "        batch_fd.downloads, dl_name\n",
-                "    ).wlvl_max.base\n",
-                "    df.loc[df[\"dl_name\"] == dl_name, \"depth_max\"] = getattr(\n",
-                "        batch_fd.downloads, dl_name\n",
-                "    ).depth_max.base\n",
-                "    df.loc[df[\"dl_name\"] == dl_name, \"damage_total\"] = getattr(\n",
-                "        batch_fd.downloads, dl_name\n",
-                "    ).damage_total.base\n",
+                "    df.loc[df[\"dl_name\"] == dl_name, \"wlvl_max\"] = getattr(batch_fd.downloads, dl_name).wlvl_max.base\n",
+                "    df.loc[df[\"dl_name\"] == dl_name, \"depth_max\"] = getattr(batch_fd.downloads, dl_name).depth_max.base\n",
+                "    df.loc[df[\"dl_name\"] == dl_name, \"damage_total\"] = getattr(batch_fd.downloads, dl_name).damage_total.base\n",
                 "\n",
                 "\n",
                 "## %%\n",
                 "\n",
                 "freqs = freqs[[\"dl_name\", \"freq_{}_jaar\".format(precipitation_zone_box.value)]]\n",
                 "freqs.rename(\n",
                 "    {\"freq_{}_jaar\".format(precipitation_zone_box.value): \"freq_jaar\"},\n",
@@ -199,27 +192,23 @@
                 "\n",
                 "df_freqs = df.merge(freqs, on=\"dl_name\")\n",
                 "\n",
                 "## %% Aanmaken of laden peilgebieden polygon\n",
                 "if not folder.source_data.peilgebieden.peilgebieden.exists():\n",
                 "    fixeddrainage = folder.source_data.datachecker.load(\"fixeddrainagelevelarea\")\n",
                 "\n",
-                "    #Als het vastloopt:\n",
+                "    # Als het vastloopt:\n",
                 "    # fixeddrainage.pop(\"created\")\n",
                 "    # fixeddrainage.pop(\"end\")\n",
                 "    # fixeddrainage.pop(\"start\")\n",
                 "\n",
                 "    fixeddrainage.to_file(folder.source_data.peilgebieden.peilgebieden.base)\n",
-                "    print(\n",
-                "        f\"Peilgebieden shapefile aangemaakt: {folder.source_data.peilgebieden.peilgebieden.name}\"\n",
-                "    )\n",
+                "    print(f\"Peilgebieden shapefile aangemaakt: {folder.source_data.peilgebieden.peilgebieden.name}\")\n",
                 "else:\n",
-                "    print(\n",
-                "        f\"Peilgebieden shapefile gevonden: {folder.source_data.peilgebieden.peilgebieden.name}\"\n",
-                "    )"
+                "    print(f\"Peilgebieden shapefile gevonden: {folder.source_data.peilgebieden.peilgebieden.name}\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "27929cd1",
             "metadata": {},
@@ -230,26 +219,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c5740d69",
             "metadata": {},
             "outputs": [],
             "source": [
-                "klimaatsommenrep = KlimaatsommenPrep(folder=folder,\n",
+                "klimaatsommenrep = KlimaatsommenPrep(\n",
+                "    folder=folder,\n",
                 "    batch_name=batch_fd.name,\n",
-                "    cfg_file = 'cfg_lizard.cfg',\n",
-                "    landuse_file = r\"\\\\corp.hhnk.nl\\data\\Hydrologen_data\\Data\\01.basisgegevens\\rasters\\landgebruik\\landuse2019_tiles\\combined_rasters.vrt\",\n",
-                "    verify=True\n",
+                "    cfg_file=\"cfg_lizard.cfg\",\n",
+                "    landuse_file=r\"\\\\corp.hhnk.nl\\data\\Hydrologen_data\\Data\\01.basisgegevens\\rasters\\landgebruik\\landuse2019_tiles\\combined_rasters.vrt\",\n",
+                "    # landuse_file = folder.model.schema_base.rasters.landuse,\n",
+                "    min_block_size=2**13,\n",
+                "    verify=True,\n",
                 ")\n",
                 "\n",
-                "klimaatsommenrep.run(gridgpkg=True, \n",
-                "                    depth=True, \n",
-                "                    dmg=True, \n",
-                "                    wlvl=False, \n",
-                "                    overwrite=False)"
+                "klimaatsommenrep.run(gridgpkg=True, depth=True, dmg=True, wlvl=False, overwrite=False)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "08fb3fe5",
             "metadata": {},
@@ -300,18 +288,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "10233872",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for raster_type, raster_name in zip(\n",
-                "    [\"depth_max\", \"damage_total\"], \n",
-                "    [\"diepte\", \"schade\"]\n",
-                "):\n",
+                "for raster_type, raster_name in zip([\"depth_max\", \"damage_total\"], [\"diepte\", \"schade\"]):\n",
                 "    peilgebieden.rasterize_peilgebieden(\n",
                 "        input_raster=hrt.Raster(df.iloc[0][raster_type]),\n",
                 "        output_file=getattr(batch_fd.output.temp, f\"peilgebieden_{raster_name}\"),\n",
                 "        input_peilgebieden=folder.source_data.peilgebieden.peilgebieden,\n",
                 "        output_peilgebieden=batch_fd.output.temp.peilgebieden,\n",
                 "        mask_file=batch_fd.output.maskerkaart,\n",
                 "        overwrite=False,\n",
@@ -361,26 +346,25 @@
             "outputs": [],
             "source": [
                 "diepte_rasters = df_freqs[\"depth_max\"].values\n",
                 "frequenties = df_freqs[\"freq_jaar\"].values\n",
                 "\n",
                 "\n",
                 "for T in [10, 100, 1000]:\n",
-                "\n",
                 "    output_file = getattr(batch_fd.output, f\"depth_T{T}_totaal\")\n",
                 "\n",
                 "    # Voor de gegeven herhalingstijd, interpoleer de rasters.\n",
                 "    main_interpolate_rasters(\n",
                 "        T=T,\n",
                 "        output_file=output_file,\n",
                 "        rasters=diepte_rasters,\n",
                 "        frequenties=frequenties,\n",
                 "        output_nodata=-9999.00,\n",
                 "        dem_raster=dem,\n",
-                "        min_value = 0,\n",
+                "        min_value=0,\n",
                 "        extra_nodata_value=0,\n",
                 "    )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -529,30 +513,25 @@
                 "\n",
                 "\n",
                 "# Bereken totale schade per peilgebied voor de twee gemaskerde schaderasters.\n",
                 "for mask_type, mask_name in zip([\"plas\", \"overlast\"], [\"mv\", \"ws\"]):\n",
                 "    schade_raster = getattr(batch_fd.output, f\"cw_schade_{mask_type}\")\n",
                 "\n",
                 "    # Calculate sum per region\n",
-                "    accum = schade_raster.sum_labels(\n",
-                "        labels_raster=labels_raster, labels_index=labels_index\n",
-                "    )\n",
+                "    accum = schade_raster.sum_labels(labels_raster=labels_raster, labels_index=labels_index)\n",
                 "\n",
                 "    schade_gdf[f\"cw_{mask_name}\"] = accum\n",
                 "\n",
                 "schade_gdf[\"cw_tot\"] = schade_gdf[\"cw_ws\"] + schade_gdf[\"cw_mv\"]\n",
                 "\n",
                 "# schade_gdf = schade_gdf.loc[schade_gdf['cw_tot'] > 0.0]\n",
                 "\n",
                 "\n",
                 "schade_per_polder = (\n",
-                "    schade_gdf[[\"name\", \"cw_tot\", \"cw_ws\", \"cw_mv\"]]\n",
-                "    .groupby(\"name\")\n",
-                "    .sum()\n",
-                "    .sort_values(by=\"cw_ws\", ascending=False)\n",
+                "    schade_gdf[[\"name\", \"cw_tot\", \"cw_ws\", \"cw_mv\"]].groupby(\"name\").sum().sort_values(by=\"cw_ws\", ascending=False)\n",
                 ")\n",
                 "\n",
                 "# Opslaan naar shapefile en csv\n",
                 "schade_gdf.to_file(output_file.base)\n",
                 "schade_per_polder.to_csv(batch_fd.output.schade_polder.base)"
             ]
         },
@@ -572,18 +551,18 @@
             "execution_count": null,
             "id": "967b561e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "raster = hrt.Raster(str(batch_fd.output.cw_schade_plas))\n",
                 "\n",
-                "dv = 0.04 #discontovoet [%]\n",
-                "n = 50 #investeringstermijn [jaren]\n",
+                "dv = 0.04  # discontovoet [%]\n",
+                "n = 50  # investeringstermijn [jaren]\n",
                 "cw_factor = (1 - (1 - dv) ** n) / dv\n",
-                "pixel_factor = raster.metadata['pixel_width']**2/0.25 #niet nodig als resolutie goed staat\n"
+                "pixel_factor = raster.metadata[\"pixel_width\"] ** 2 / 0.25  # niet nodig als resolutie goed staat"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "686564bc",
             "metadata": {},
@@ -594,24 +573,26 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "eeadf8f1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "maskerkaart2 = gpd.read_file(str(folder.source_data.peilgebieden.geen_schade)) #load maskerkaart (geen_schade.shp)\n",
+                "maskerkaart2 = gpd.read_file(str(folder.source_data.peilgebieden.geen_schade))  # load maskerkaart (geen_schade.shp)\n",
+                "\n",
+                "maskerkaart_union = maskerkaart2.buffer(0.1).unary_union.buffer(-0.1)  # make one geometry from gdf.\n",
                 "\n",
-                "maskerkaart_union = maskerkaart2.buffer(0.1).unary_union.buffer(-0.1) #make one geometry from gdf.\n",
-                "    \n",
-                "#Rasterize polygon\n",
+                "# Rasterize polygon\n",
                 "maskerkaart_union = gpd.GeoDataFrame(geometry=[maskerkaart_union])\n",
-                "#Voeg kolom toe aan gdf, deze waarden worden in het raster gezet.\n",
-                "maskerkaart_union['val']=1\n",
+                "# Voeg kolom toe aan gdf, deze waarden worden in het raster gezet.\n",
+                "maskerkaart_union[\"val\"] = 1\n",
                 "\n",
-                "mask = hrt.gdf_to_raster(maskerkaart_union, value_field='val', raster_out='', nodata=0, metadata=damage_meta, epsg=28992, driver='MEM')\n",
+                "mask = hrt.gdf_to_raster(\n",
+                "    maskerkaart_union, value_field=\"val\", raster_out=\"\", nodata=0, metadata=damage_meta, epsg=28992, driver=\"MEM\"\n",
+                ")\n",
                 "mask = mask > 0"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "25547551",
@@ -629,22 +610,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "118b227a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "schade_raster_corr_file={\"plas\": str(batch_fd.output.cw_schade_plas_corr),\n",
-                "                        \"overlast\": str(batch_fd.output.cw_schade_overlast_corr)}\n",
-                "schades, schade_per_polder = maak_schade_polygon(peilgebieden_file=folder.source_data.peilgebieden.peilgebieden, \n",
-                "                                                 schade_raster_file=schade_raster_corr_file, \n",
-                "                                                 pixel_factor=pixel_factor, \n",
-                "                                                 output_schade_file=str(batch_fd.output.schade_peilgebied_corr), \n",
-                "                                                 output_polder_file=str(batch_fd.output.schade_polder_corr))\n",
-                "\n"
+                "schade_raster_corr_file = {\n",
+                "    \"plas\": str(batch_fd.output.cw_schade_plas_corr),\n",
+                "    \"overlast\": str(batch_fd.output.cw_schade_overlast_corr),\n",
+                "}\n",
+                "schades, schade_per_polder = maak_schade_polygon(\n",
+                "    peilgebieden_file=folder.source_data.peilgebieden.peilgebieden,\n",
+                "    schade_raster_file=schade_raster_corr_file,\n",
+                "    pixel_factor=pixel_factor,\n",
+                "    output_schade_file=str(batch_fd.output.schade_peilgebied_corr),\n",
+                "    output_polder_file=str(batch_fd.output.schade_polder_corr),\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "e7e7bea5",
             "metadata": {},
@@ -670,15 +654,15 @@
                 "    main_interpolate_rasters(\n",
                 "        T=T,\n",
                 "        output_file=output_file,\n",
                 "        rasters=wlvl_rasters,\n",
                 "        frequenties=frequenties,\n",
                 "        output_nodata=-9999.00,\n",
                 "        dem_raster=dem,\n",
-                "        min_value = None,\n",
+                "        min_value=None,\n",
                 "        extra_nodata_value=0,\n",
                 "    )"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953044188689969%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '# Add qgis plugin deps to syspath and load "*

 * *            "notebook_data\\n'), (2, '\\n'), (6, 'import xarray\\n'), (7, '\\n'), (13, 'import "*

 * *            "hhnk_threedi_tools as htt\\n'), (17, '# User input\\n'), (19, 'scenario = "*

 * *            '"katvoed #1 piek_ghg_T1000"  # mapnaam\\n\'), (27, \'threedi_result = '*

 * *            "folder.threedi_results.one_d_two_d[scenario]')], delete: [25, 17, 15, 11, 5, 0]}}, 3: "*

 * *            "{'source': {insert: [(0, '# Select resu […]*

```diff
@@ -24,40 +24,42 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cb23f2c3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#Add qgis plugin deps to syspath and load notebook_data\n",
+                "# Add qgis plugin deps to syspath and load notebook_data\n",
                 "from notebook_setup import setup_notebook\n",
+                "\n",
                 "notebook_data = setup_notebook()\n",
                 "\n",
                 "\n",
-                "import xarray \n",
+                "import xarray\n",
+                "\n",
                 "# import threedi_raster_edits as tre\n",
                 "from hhnk_threedi_tools import Folders\n",
                 "import hhnk_research_tools as hrt\n",
                 "import geopandas as gpd\n",
                 "\n",
-                "from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import ThreediGrid\n",
+                "import hhnk_threedi_tools as htt\n",
                 "from hhnk_threedi_tools.core.result_rasters.calculate_raster import BaseCalculatorGPKG\n",
                 "\n",
                 "\n",
-                "#User input\n",
+                "# User input\n",
                 "folder_path = r\"E:\\02.modellen\\model_test_v2\"\n",
-                "scenario = \"katvoed #1 piek_ghg_T1000\" #mapnaam\n",
+                "scenario = \"katvoed #1 piek_ghg_T1000\"  # mapnaam\n",
                 "\n",
                 "\n",
                 "folder = Folders(folder_path)\n",
                 "\n",
                 "dem_path = folder.model.schema_base.rasters.dem.base\n",
                 "# dem_path = r'E:\\\\02.modellen\\\\23_Katvoed\\\\02_schematisation\\\\00_basis\\\\rasters/dem_katvoed_ahn3.tif'\n",
                 "\n",
-                "threedi_result = folder.threedi_results.one_d_two_d[scenario]\n"
+                "threedi_result = folder.threedi_results.one_d_two_d[scenario]"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "d5ad226c",
             "metadata": {},
@@ -68,22 +70,22 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "091d3215",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#Select result\n",
-                "threedigrid = ThreediGrid(folder=folder, threedi_result=threedi_result)\n",
+                "# Select result\n",
+                "netcdf_gpkg = htt.NetcdfToGPKG.from_folder(\n",
+                "    folder=folder,\n",
+                "    threedi_result=threedi_result,\n",
+                ")\n",
                 "\n",
-                "#Convert netcdf to grid gpkg\n",
-                "threedigrid.netcdf_to_grid_gpkg()\n",
-                "\n",
-                "#Replace waterlevel of selected cells with avg of neighbours.\n",
-                "threedigrid.waterlevel_correction(output_col=\"wlvl_max_replaced\")"
+                "# Convert netcdf to grid gpkg\n",
+                "netcdf_gpkg.run()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "c7b68276",
             "metadata": {},
@@ -94,56 +96,46 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6c094ec3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "OVERWRITE=False\n",
+                "OVERWRITE = False\n",
                 "\n",
-                "grid_gdf = threedi_result.full_path(\"grid_corr.gpkg\").load()\n"
+                "grid_gdf = threedi_result.full_path(\"grid_wlvl.gpkg\").load()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0fc0e6a4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "calculator_kwargs = {\"dem_path\":dem_path,\n",
-                "                        \"grid_gdf\":grid_gdf, \n",
-                "                        \"wlvl_column\":\"wlvl_max_replaced\"}\n",
+                "calculator_kwargs = {\"dem_path\": dem_path, \"grid_gdf\": grid_gdf, \"wlvl_column\": \"wlvl_max_replaced\"}\n",
                 "\n",
-                "#Init calculator\n",
+                "# Init calculator\n",
                 "with BaseCalculatorGPKG(**calculator_kwargs) as self:\n",
-                "    self.run(output_file=threedi_result.full_path(\"wlvl_corr.tif\"),  \n",
-                "                mode=\"MODE_WLVL\",\n",
-                "                overwrite=OVERWRITE)\n",
-                "    self.run(output_file=threedi_result.full_path(\"wdepth_corr.tif\"),  \n",
-                "                mode=\"MODE_WDEPTH\",\n",
-                "                overwrite=OVERWRITE)\n",
+                "    self.run(output_file=threedi_result.full_path(\"wlvl_corr.tif\"), mode=\"MODE_WLVL\", overwrite=OVERWRITE)\n",
+                "    self.run(output_file=threedi_result.full_path(\"wdepth_corr.tif\"), mode=\"MODE_WDEPTH\", overwrite=OVERWRITE)\n",
                 "    print(\"Done.\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "09fe6053",
             "metadata": {},
             "outputs": [],
             "source": [
-                "calculator_kwargs = {\"dem_path\":dem_path,\n",
-                "                        \"grid_gdf\":grid_gdf, \n",
-                "                        \"wlvl_column\":\"wlvl_max_orig\"}\n",
+                "calculator_kwargs = {\"dem_path\": dem_path, \"grid_gdf\": grid_gdf, \"wlvl_column\": \"wlvl_max_orig\"}\n",
                 "\n",
                 "with BaseCalculatorGPKG(**calculator_kwargs) as self:\n",
-                "    self.run(output_file=threedi_result.full_path(\"wdepth_orig.tif\"),  \n",
-                "                mode=\"MODE_WDEPTH\",\n",
-                "                overwrite=OVERWRITE)"
+                "    self.run(output_file=threedi_result.full_path(\"wdepth_orig.tif\"), mode=\"MODE_WDEPTH\", overwrite=OVERWRITE)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "7d6d51f7",
             "metadata": {},
@@ -157,40 +149,40 @@
             "id": "2fc5875b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Schadeschatter heeft wat extra voorbereiding nodig.\n",
                 "from pathlib import Path\n",
                 "\n",
-                "#Variables\n",
-                "cfg_file = hrt.get_pkg_resource_path(package_resource=hrt.waterschadeschatter.resources, \n",
-                "                                name=\"cfg_lizard.cfg\")\n",
+                "# Variables\n",
+                "cfg_file = hrt.get_pkg_resource_path(package_resource=hrt.waterschadeschatter.resources, name=\"cfg_lizard.cfg\")\n",
                 "landuse_file = r\"E:\\01.basisgegevens\\rasters\\landgebruik\\landuse2019_3di_tiles\\landuse2019_3di_tiles.vrt\"\n",
                 "\n",
                 "depth_file = threedi_result.full_path(\"wdepth_corr.tif\")\n",
                 "output_file = threedi_result.full_path(\"damage_corr_lizard.tif\")\n",
                 "\n",
                 "\n",
-                "wss_settings = {'inundation_period': 48, #uren\n",
-                "                'herstelperiode':'10 dagen',\n",
-                "                'maand':'sep',\n",
-                "                'cfg_file':cfg_file,\n",
-                "                'dmg_type':'gem'}\n",
-                "\n",
-                "#Calculation\n",
-                "self = hrt.Waterschadeschatter(depth_file=depth_file.path, \n",
-                "                        landuse_file=landuse_file.path, \n",
-                "                        wss_settings=wss_settings)\n",
+                "wss_settings = {\n",
+                "    \"inundation_period\": 48,  # uren\n",
+                "    \"herstelperiode\": \"10 dagen\",\n",
+                "    \"maand\": \"sep\",\n",
+                "    \"cfg_file\": cfg_file,\n",
+                "    \"dmg_type\": \"gem\",\n",
+                "}\n",
+                "\n",
+                "# Calculation\n",
+                "self = hrt.Waterschadeschatter(depth_file=depth_file.path, landuse_file=landuse_file.path, wss_settings=wss_settings)\n",
                 "\n",
                 "# Berkenen schaderaster\n",
-                "self.run(output_raster=hrt.Raster(output_file), \n",
-                "            calculation_type=\"sum\", \n",
-                "            verbose=False, \n",
-                "            overwrite=False,\n",
-                "            )"
+                "self.run(\n",
+                "    output_raster=hrt.Raster(output_file),\n",
+                "    calculation_type=\"sum\",\n",
+                "    verbose=False,\n",
+                "    overwrite=False,\n",
+                ")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.5 64-bit",
             "language": "python",
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/net.cpython-39.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/net.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Nov  6 13:38:06 2023 UTC, .py size: 7322 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3eec 4865 9a1c 0000  a.......>.He....
+00000000: 610d 0d0a 0000 0000 27a1 2f66 c21c 0000  a.......'./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6402 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 5a08 6401 6403 6c03 6d09 5a09 0100 6404  Z.d.d.l.m.Z...d.
@@ -31,53 +31,53 @@
 000001e0: 6405 6406 8400 5a05 6407 5300 2908 da08  d.d...Z.d.S.)...
 000001f0: 5465 6d70 436f 7079 6302 0000 0000 0000  TempCopyc.......
 00000200: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000210: 0073 0e00 0000 7400 7c01 8301 7c00 5f01  .s....t.|...|._.
 00000220: 6400 5300 a901 4e29 0272 0300 0000 da0d  d.S...N).r......
 00000230: 6f72 6967 696e 616c 5f70 6174 6829 02da  original_path)..
 00000240: 0473 656c 6672 0700 0000 a900 7209 0000  .selfr......r...
-00000250: 00fa 5165 3a5c 6769 7468 7562 5c77 7661  ..Qe:\github\wva
+00000250: 00fa 5164 3a5c 6769 7468 7562 5c77 7661  ..Qd:\github\wva
 00000260: 6e67 6572 7765 6e5c 6868 6e6b 2d74 6872  ngerwen\hhnk-thr
 00000270: 6565 6469 2d74 6f6f 6c73 5c68 686e 6b5f  eedi-tools\hhnk_
 00000280: 7468 7265 6564 695f 746f 6f6c 735c 7574  threedi_tools\ut
 00000290: 696c 735c 6e6f 7465 626f 6f6b 735c 7275  ils\notebooks\ru
-000002a0: 6e2e 7079 da08 5f5f 696e 6974 5f5f 1c00  n.py..__init__..
+000002a0: 6e2e 7079 da08 5f5f 696e 6974 5f5f 1e00  n.py..__init__..
 000002b0: 0000 7302 0000 0000 017a 1154 656d 7043  ..s......z.TempC
 000002c0: 6f70 792e 5f5f 696e 6974 5f5f 6301 0000  opy.__init__c...
 000002d0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
 000002e0: 0043 0000 0073 3600 0000 7400 a001 a100  .C...s6...t.....
 000002f0: 7d01 7c00 6a02 6a03 7d02 7404 6a05 a006  }.|.j.j.}.t.j...
 00000300: 7c01 7c02 a102 7c00 5f05 7407 a008 7c00  |.|...|._.t...|.
 00000310: 6a02 7c00 6a05 a102 0100 7c00 6a05 5300  j.|.j.....|.j.S.
 00000320: 7206 0000 0029 09da 0874 656d 7066 696c  r....)...tempfil
 00000330: 65da 0a67 6574 7465 6d70 6469 7272 0700  e..gettempdirr..
 00000340: 0000 da04 6e61 6d65 da02 6f73 da04 7061  ....name..os..pa
 00000350: 7468 da04 6a6f 696e da06 7368 7574 696c  th..join..shutil
 00000360: da05 636f 7079 3229 0372 0800 0000 da08  ..copy2).r......
 00000370: 7465 6d70 5f64 6972 da09 6261 7365 5f70  temp_dir..base_p
 00000380: 6174 6872 0900 0000 7209 0000 0072 0a00  athr....r....r..
-00000390: 0000 da09 5f5f 656e 7465 725f 5f1f 0000  ....__enter__...
+00000390: 0000 da09 5f5f 656e 7465 725f 5f21 0000  ....__enter__!..
 000003a0: 0073 0a00 0000 0001 0801 0801 1001 1001  .s..............
 000003b0: 7a12 5465 6d70 436f 7079 2e5f 5f65 6e74  z.TempCopy.__ent
 000003c0: 6572 5f5f 6304 0000 0000 0000 0000 0000  er__c...........
 000003d0: 0004 0000 0003 0000 0043 0000 0073 1000  .........C...s..
 000003e0: 0000 7400 a001 7c00 6a02 a101 0100 6400  ..t...|.j.....d.
 000003f0: 5300 7206 0000 0029 0372 0f00 0000 da06  S.r....).r......
 00000400: 7265 6d6f 7665 7210 0000 0029 0472 0800  remover....).r..
 00000410: 0000 da08 6578 635f 7479 7065 da07 6578  ....exc_type..ex
 00000420: 635f 7661 6cda 0665 7863 5f74 6272 0900  c_val..exc_tbr..
 00000430: 0000 7209 0000 0072 0a00 0000 da08 5f5f  ..r....r......__
-00000440: 6578 6974 5f5f 2600 0000 7302 0000 0000  exit__&...s.....
+00000440: 6578 6974 5f5f 2800 0000 7302 0000 0000  exit__(...s.....
 00000450: 017a 1154 656d 7043 6f70 792e 5f5f 6578  .z.TempCopy.__ex
 00000460: 6974 5f5f 4e29 06da 085f 5f6e 616d 655f  it__N)...__name_
 00000470: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000480: 5f71 7561 6c6e 616d 655f 5f72 0b00 0000  _qualname__r....
 00000490: 7216 0000 0072 1b00 0000 7209 0000 0072  r....r....r....r
 000004a0: 0900 0000 7209 0000 0072 0a00 0000 7205  ....r....r....r.
-000004b0: 0000 001b 0000 0073 0600 0000 0801 0803  .......s........
+000004b0: 0000 001d 0000 0073 0600 0000 0801 0803  .......s........
 000004c0: 0807 7205 0000 0063 0200 0000 0000 0000  ..r....c........
 000004d0: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
 000004e0: 736c 0000 0074 006a 017c 0064 0164 028d  sl...t.j.|.d.d..
 000004f0: 0201 0074 00a0 027c 01a1 0144 005d 4e7d  ...t...|...D.]N}
 00000500: 0274 037c 0283 0101 007c 02a0 0464 03a1  .t.|.....|...d..
 00000510: 0172 3464 017d 036e 127c 0264 046b 0272  .r4d.}.n.|.d.k.r
 00000520: 4264 017d 036e 0464 057d 037c 0372 1874  Bd.}.n.d.}.|.r.t
@@ -89,41 +89,41 @@
 00000580: 2907 720f 0000 00da 086d 616b 6564 6972  ).r......makedir
 00000590: 73da 076c 6973 7464 6972 da05 7072 696e  s..listdir..prin
 000005a0: 74da 0865 6e64 7377 6974 6872 1200 0000  t..endswithr....
 000005b0: 7213 0000 0029 045a 076e 6577 5f64 6972  r....).Z.new_dir
 000005c0: 5a0c 6f72 6967 696e 616c 5f64 6972 da04  Z.original_dir..
 000005d0: 6669 6c65 da04 636f 6e74 7209 0000 0072  file..contr....r
 000005e0: 0900 0000 720a 0000 00da 0e63 6f70 795f  ....r......copy_
-000005f0: 6e6f 7465 626f 6f6b 732a 0000 0073 1400  notebooks*...s..
+000005f0: 6e6f 7465 626f 6f6b 732c 0000 0073 1400  notebooks,...s..
 00000600: 0000 0001 0e02 0e01 0801 0a01 0601 0801  ................
 00000610: 0602 0402 0401 7227 0000 0063 0200 0000  ......r'...c....
 00000620: 0000 0000 0000 0000 0300 0000 0800 0000  ................
 00000630: 4300 0000 733e 0000 0074 007c 0064 0117  C...s>...t.|.d..
 00000640: 0064 0283 028f 1c7d 0274 01a0 027c 017c  .d.....}.t...|.|
 00000650: 02a1 0201 0057 0064 0004 0004 0083 0301  .....W.d........
 00000660: 006e 1031 0073 3030 0001 0001 0001 0059  .n.1.s00.......Y
 00000670: 0001 0064 0053 0029 034e fa13 2f6e 6f74  ...d.S.).N../not
 00000680: 6562 6f6f 6b5f 6461 7461 2e6a 736f 6eda  ebook_data.json.
 00000690: 0177 2903 da04 6f70 656e da04 6a73 6f6e  .w)...open..json
 000006a0: da04 6475 6d70 2903 da09 6469 7265 6374  ..dump)...direct
 000006b0: 6f72 79da 0464 6174 61da 0166 7209 0000  ory..data..fr...
 000006c0: 0072 0900 0000 720a 0000 00da 1377 7269  .r....r......wri
 000006d0: 7465 5f6e 6f74 6562 6f6f 6b5f 6a73 6f6e  te_notebook_json
-000006e0: 3a00 0000 7304 0000 0000 0110 0172 3000  :...s........r0.
+000006e0: 3c00 0000 7304 0000 0000 0110 0172 3000  <...s........r0.
 000006f0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
 00000700: 0000 0008 0000 0043 0000 0073 3a00 0000  .......C...s:...
 00000710: 7400 7c00 6401 1700 8301 8f1a 7d01 7401  t.|.d.......}.t.
 00000720: a002 7c01 a101 5700 0200 6400 0400 0400  ..|...W...d.....
 00000730: 8303 0100 5300 3100 732c 3000 0100 0100  ....S.1.s,0.....
 00000740: 0100 5900 0100 6400 5300 2902 4e72 2800  ..Y...d.S.).Nr(.
 00000750: 0000 2903 722a 0000 0072 2b00 0000 da04  ..).r*...r+.....
 00000760: 6c6f 6164 2902 722d 0000 0072 2f00 0000  load).r-...r/...
 00000770: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
 00000780: 1272 6561 645f 6e6f 7465 626f 6f6b 5f6a  .read_notebook_j
-00000790: 736f 6e3f 0000 0073 0400 0000 0001 0e01  son?...s........
+00000790: 736f 6e41 0000 0073 0400 0000 0001 0e01  sonA...s........
 000007a0: 7232 0000 0063 0000 0000 0000 0000 0000  r2...c..........
 000007b0: 0000 0600 0000 0400 0000 4300 0000 73ba  ..........C...s.
 000007c0: 0000 0064 017d 0074 006a 017d 0174 026a  ...d.}.t.j.}.t.j
 000007d0: 03a0 047c 01a1 015c 027d 027d 0364 027c  ...|...\.}.}.d.|
 000007e0: 0376 0072 587c 03a0 05a1 0064 0376 0072  .v.rX|.....d.v.r
 000007f0: 347c 017d 006e 0c74 0664 047c 0116 0083  4|.}.n.t.d.|....
 00000800: 0182 0174 026a 03a0 077c 00a1 0173 504a  ...t.j...|...sPJ
@@ -149,15 +149,15 @@
 00000940: 626c 6520 7265 6665 7273 2074 6f20 7468  ble refers to th
 00000950: 650a 2020 2020 5167 6973 2073 7461 7274  e.    Qgis start
 00000960: 2d75 7020 7363 7269 7074 2e0a 2020 2020  -up script..    
 00000970: 4eda 0670 7974 686f 6e29 027a 0a70 7974  N..python).z.pyt
 00000980: 686f 6e2e 6578 657a 0b70 7974 686f 6e33  hon.exez.python3
 00000990: 2e65 7865 7a27 556e 6578 7065 6374 6564  .exez'Unexpected
 000009a0: 2076 616c 7565 2066 6f72 2073 7973 2e65   value for sys.e
-000009b0: 7865 6375 7461 626c 653a 2025 735a 0471  xecutable: %sZ.q
+000009b0: 7865 6375 7461 626c 653a 2025 73da 0471  xecutable: %s..q
 000009c0: 6769 7372 0100 0000 7a0b 7079 335f 656e  gisr....z.py3_en
 000009d0: 762e 6261 747a 0c2f 7079 335f 656e 762e  v.batz./py3_env.
 000009e0: 6261 747a 1370 7974 686f 6e2d 7167 6973  batz.python-qgis
 000009f0: 2d6c 7472 2e62 6174 7a14 2f70 7974 686f  -ltr.batz./pytho
 00000a00: 6e2d 7167 6973 2d6c 7472 2e62 6174 7a2a  n-qgis-ltr.batz*
 00000a10: 636f 756c 6420 6e6f 7420 6669 6e64 2071  could not find q
 00000a20: 6769 732d 7079 7468 6f6e 2062 6174 2066  gis-python bat f
@@ -165,50 +165,50 @@
 00000a40: 73da 0a65 7865 6375 7461 626c 6572 0f00  s..executabler..
 00000a50: 0000 7210 0000 00da 0573 706c 6974 da05  ..r......split..
 00000a60: 6c6f 7765 72da 1045 6e76 6972 6f6e 6d65  lower..Environme
 00000a70: 6e74 4572 726f 72da 0665 7869 7374 73da  ntError..exists.
 00000a80: 0373 7472 da07 7061 7468 6c69 6272 0300  .str..pathlibr..
 00000a90: 0000 da07 7061 7265 6e74 7372 2200 0000  ....parentsr"...
 00000aa0: 2906 da0b 696e 7465 7270 7265 7465 7272  )...interpreterr
-00000ab0: 3500 0000 722d 0000 00da 0866 696c 656e  5...r-.....filen
+00000ab0: 3600 0000 722d 0000 00da 0866 696c 656e  6...r-.....filen
 00000ac0: 616d 655a 0b6d 6169 6e5f 666f 6c64 6572  ameZ.main_folder
 00000ad0: 5a0c 666f 6c64 6572 5f66 696c 6573 7209  Z.folder_filesr.
 00000ae0: 0000 0072 0900 0000 720a 0000 00da 175f  ...r....r......_
 00000af0: 6765 745f 7079 7468 6f6e 5f69 6e74 6572  get_python_inter
-00000b00: 7072 6574 6572 4400 0000 7326 0000 0000  preterD...s&....
+00000b00: 7072 6574 6572 4600 0000 7326 0000 0000  preterF...s&....
 00000b10: 0704 0106 0110 0108 010c 0106 020c 0110  ................
 00000b20: 0108 0208 0214 010a 0208 0108 0208 0108  ................
-00000b30: 0204 010c 0272 3f00 0000 6300 0000 0000  .....r?...c.....
+00000b30: 0204 010c 0272 4000 0000 6300 0000 0000  .....r@...c.....
 00000b40: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
 00000b50: 0000 0073 3000 0000 7400 a001 a100 a002  ...s0...t.......
 00000b60: 6401 6402 a102 7d00 7403 6a04 a005 7c00  d.d...}.t.j...|.
 00000b70: 6403 1700 a101 7228 7c00 6403 1700 5300  d.....r(|.d...S.
 00000b80: 6400 5300 6400 5300 2904 4efa 0d73 6974  d.S.d.S.).N..sit
 00000b90: 652d 7061 636b 6167 6573 da07 5363 7269  e-packages..Scri
 00000ba0: 7074 737a 102f 6a75 7079 7465 722d 6c61  ptsz./jupyter-la
 00000bb0: 622e 6578 65a9 06da 0473 6974 65da 1367  b.exe....site..g
 00000bc0: 6574 7573 6572 7369 7465 7061 636b 6167  etusersitepackag
 00000bd0: 6573 da07 7265 706c 6163 6572 0f00 0000  es..replacer....
-00000be0: 7210 0000 0072 3900 0000 a901 7210 0000  r....r9.....r...
+00000be0: 7210 0000 0072 3a00 0000 a901 7210 0000  r....r:.....r...
 00000bf0: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
 00000c00: da1c 7573 6572 5f69 6e73 7461 6c6c 6564  ..user_installed
-00000c10: 5f6e 6f74 6562 6f6f 6b5f 7061 7468 6700  _notebook_pathg.
+00000c10: 5f6e 6f74 6562 6f6f 6b5f 7061 7468 6900  _notebook_pathi.
 00000c20: 0000 7308 0000 0000 0110 0110 0108 0272  ..s............r
-00000c30: 4700 0000 6300 0000 0000 0000 0000 0000  G...c...........
+00000c30: 4800 0000 6300 0000 0000 0000 0000 0000  H...c...........
 00000c40: 0001 0000 0004 0000 0043 0000 0073 3000  .........C...s0.
 00000c50: 0000 7400 a001 a100 a002 6401 6402 a102  ..t.......d.d...
 00000c60: 7d00 7403 6a04 a005 7c00 6403 1700 a101  }.t.j...|.d.....
 00000c70: 7228 7c00 6403 1700 5300 6400 5300 6400  r(|.d...S.d.S.d.
-00000c80: 5300 2904 4e72 4000 0000 7241 0000 007a  S.).Nr@...rA...z
-00000c90: 0c2f 6970 7974 686f 6e2e 6578 6572 4200  ./ipython.exerB.
-00000ca0: 0000 7246 0000 0072 0900 0000 7209 0000  ..rF...r....r...
+00000c80: 5300 2904 4e72 4100 0000 7242 0000 007a  S.).NrA...rB...z
+00000c90: 0c2f 6970 7974 686f 6e2e 6578 6572 4300  ./ipython.exerC.
+00000ca0: 0000 7247 0000 0072 0900 0000 7209 0000  ..rG...r....r...
 00000cb0: 0072 0a00 0000 da1b 7573 6572 5f69 6e73  .r......user_ins
 00000cc0: 7461 6c6c 6564 5f69 7079 7468 6f6e 5f70  talled_ipython_p
-00000cd0: 6174 686f 0000 0073 0800 0000 0001 1001  atho...s........
-00000ce0: 1001 0802 7248 0000 00da 056f 7367 656f  ....rH.....osgeo
+00000cd0: 6174 6871 0000 0073 0800 0000 0001 1001  athq...s........
+00000ce0: 1001 0802 7249 0000 00da 056f 7367 656f  ....rI.....osgeo
 00000cf0: 4663 0200 0000 0000 0000 0000 0000 0500  Fc..............
 00000d00: 0000 0300 0000 4300 0000 733c 0000 0074  ......C...s<...t
 00000d10: 0083 005c 027d 027d 037c 0064 016b 0272  ...\.}.}.|.d.k.r
 00000d20: 1e7c 0364 0264 0367 037d 046e 1a7c 0172  .|.d.d.g.}.n.|.r
 00000d30: 2e7c 0374 0183 0067 027d 046e 0a7c 0374  .|.t...g.}.n.|.t
 00000d40: 0283 0067 027d 047c 0453 0029 047a a969  ...g.}.|.S.).z.i
 00000d50: 6620 6a75 7079 7465 7220 6973 2069 6e73  f jupyter is ins
@@ -217,25 +217,25 @@
 00000d80: 6966 206a 7570 7974 6572 2069 7320 696e  if jupyter is in
 00000d90: 7374 616c 6c65 6420 696e 2074 6865 2075  stalled in the u
 00000da0: 7365 7220 6469 7220 2770 6970 2069 6e73  ser dir 'pip ins
 00000db0: 7461 6c6c 206a 7570 7974 6572 202d 2d75  tall jupyter --u
 00000dc0: 7365 7227 0a20 2020 2075 7365 2027 7573  ser'.    use 'us
 00000dd0: 6572 272e 0a0a 2020 2020 2775 7365 7227  er'...    'user'
 00000de0: 2075 7365 7320 616e 2065 7865 6374 7561   uses an exectua
-00000df0: 626c 650a 2020 2020 7249 0000 007a 022d  ble.    rI...z.-
+00000df0: 626c 650a 2020 2020 724a 0000 007a 022d  ble.    rJ...z.-
 00000e00: 6d7a 0b6a 7570 7974 6572 2d6c 6162 2903  mz.jupyter-lab).
-00000e10: 723f 0000 0072 4800 0000 7247 0000 0029  r?...rH...rG...)
+00000e10: 7240 0000 0072 4900 0000 7248 0000 0029  r@...rI...rH...)
 00000e20: 05da 086c 6f63 6174 696f 6eda 0769 7079  ...location..ipy
-00000e30: 7468 6f6e da06 7379 7374 656d 5a12 7079  thon..systemZ.py
+00000e30: 7468 6f6e da06 7379 7374 656d da12 7079  thon..system..py
 00000e40: 7468 6f6e 5f69 6e74 6572 7072 6574 6572  thon_interpreter
 00000e50: da07 636f 6d6d 616e 6472 0900 0000 7209  ..commandr....r.
 00000e60: 0000 0072 0a00 0000 da10 6e6f 7465 626f  ...r......notebo
-00000e70: 6f6b 5f63 6f6d 6d61 6e64 7700 0000 730e  ok_commandw...s.
+00000e70: 6f6b 5f63 6f6d 6d61 6e64 7900 0000 730e  ok_commandy...s.
 00000e80: 0000 0000 070a 0108 010c 0704 010c 020a  ................
-00000e90: 0172 4e00 0000 da03 7275 6e63 0400 0000  .rN.....runc....
+00000e90: 0172 5000 0000 da03 7275 6e63 0400 0000  .rP.....runc....
 00000ea0: 0000 0000 0000 0000 0800 0000 0a00 0000  ................
 00000eb0: 4300 0000 7300 0100 0064 0164 0284 0074  C...s....d.d...t
 00000ec0: 006a 01a0 0264 03a1 01a0 0374 006a 04a1  .j...d.....t.j..
 00000ed0: 0144 0083 017d 047c 0344 005d 367d 0574  .D...}.|.D.]6}.t
 00000ee0: 057c 0583 017d 057c 057c 0476 0172 227c  .|...}.|.|.v.r"|
 00000ef0: 05a0 06a1 009b 0074 006a 049b 0074 006a  .......t.j...t.j
 00000f00: 0164 0319 009b 009d 0374 006a 0164 033c  .d.......t.j.d.<
@@ -266,63 +266,63 @@
 00001090: 2770 6f70 656e 2720 6f72 2027 7275 6e27  'popen' or 'run'
 000010a0: 290a 2020 2020 6301 0000 0000 0000 0000  ).    c.........
 000010b0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
 000010c0: 1400 0000 6700 7c00 5d0c 7d01 7400 7c01  ....g.|.].}.t.|.
 000010d0: 8301 9102 7104 5300 7209 0000 0072 0200  ....q.S.r....r..
 000010e0: 0000 2902 da02 2e30 da01 6972 0900 0000  ..)....0..ir....
 000010f0: 7209 0000 0072 0a00 0000 da0a 3c6c 6973  r....r......<lis
-00001100: 7463 6f6d 703e 9700 0000 f300 0000 007a  tcomp>.........z
+00001100: 7463 6f6d 703e 9900 0000 f300 0000 007a  tcomp>.........z
 00001110: 1f6f 7065 6e5f 7365 7276 6572 2e3c 6c6f  .open_server.<lo
 00001120: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
 00001130: da04 5041 5448 7a06 7061 7468 203a da05  ..PATHz.path :..
 00001140: 706f 7065 6e54 4e29 07da 0573 6865 6c6c  popenTN)...shell
 00001150: da12 756e 6976 6572 7361 6c5f 6e65 776c  ..universal_newl
 00001160: 696e 6573 da05 7374 6469 6eda 0673 7464  ines..stdin..std
 00001170: 6f75 74da 0673 7464 6572 72da 0963 6c6f  out..stderr..clo
 00001180: 7365 5f66 6473 da0d 6372 6561 7469 6f6e  se_fds..creation
 00001190: 666c 6167 737a 1d53 7461 7274 6564 2070  flagsz.Started p
 000011a0: 726f 6365 7373 696e 6720 7769 7468 2070  rocessing with p
 000011b0: 6964 3a20 7a0d 2061 6e64 2063 6f6d 6d61  id: z. and comma
-000011c0: 6e64 2072 4f00 0000 2903 da05 7374 6172  nd rO...)...star
-000011d0: 74da 0363 6d64 7a02 2f4b a901 7256 0000  t..cmdz./K..rV..
+000011c0: 6e64 2072 5100 0000 2903 da05 7374 6172  nd rQ...)...star
+000011d0: 74da 0363 6d64 7a02 2f4b a901 7258 0000  t..cmdz./K..rX..
 000011e0: 007a 2053 7461 7274 6564 2070 726f 6365  .z Started proce
 000011f0: 7373 696e 6720 7769 7468 2063 6f6d 6d61  ssing with comma
 00001200: 6e64 2029 1072 0f00 0000 da07 656e 7669  nd ).r......envi
-00001210: 726f 6eda 0367 6574 7236 0000 00da 0770  ron..getr6.....p
+00001210: 726f 6eda 0367 6574 7237 0000 00da 0770  ron..getr7.....p
 00001220: 6174 6873 6570 7203 0000 00da 0861 735f  athsepr......as_
-00001230: 706f 7369 7872 2300 0000 724e 0000 00da  posixr#...rN....
+00001230: 706f 7369 7872 2300 0000 7250 0000 00da  posixr#...rP....
 00001240: 0661 7070 656e 64da 0a73 7562 7072 6f63  .append..subproc
 00001250: 6573 73da 0550 6f70 656e da10 4445 5441  ess..Popen..DETA
 00001260: 4348 4544 5f50 524f 4345 5353 da18 4352  CHED_PROCESS..CR
 00001270: 4541 5445 5f4e 4557 5f50 524f 4345 5353  EATE_NEW_PROCESS
-00001280: 5f47 524f 5550 da03 7069 6472 4f00 0000  _GROUP..pidrO...
-00001290: 2908 722d 0000 0072 4a00 0000 da03 7573  ).r-...rJ.....us
+00001280: 5f47 524f 5550 da03 7069 6472 5100 0000  _GROUP..pidrQ...
+00001290: 2908 722d 0000 0072 4b00 0000 da03 7573  ).r-...rK.....us
 000012a0: 655a 0e6e 6f74 6562 6f6f 6b5f 7061 7468  eZ.notebook_path
-000012b0: 73da 0570 6174 6873 7210 0000 0072 4d00  s..pathsr....rM.
+000012b0: 73da 0570 6174 6873 7210 0000 0072 4f00  s..pathsr....rO.
 000012c0: 0000 da07 7072 6f63 6573 7372 0900 0000  ....processr....
 000012d0: 7209 0000 0072 0a00 0000 da0b 6f70 656e  r....r......open
-000012e0: 5f73 6572 7665 728e 0000 0073 3200 0000  _server....s2...
+000012e0: 5f73 6572 7665 7290 0000 0073 3200 0000  _server....s2...
 000012f0: 0009 1e01 0801 0801 0801 2401 1e01 0802  ..........$.....
 00001300: 0401 0a02 0801 0401 0201 0201 0201 0201  ................
 00001310: 0201 0201 0201 06f8 060a 1801 0801 0c01  ................
-00001320: 0e01 726d 0000 0063 0200 0000 0000 0000  ..rm...c........
+00001320: 0e01 726f 0000 0063 0200 0000 0000 0000  ..ro...c........
 00001330: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
 00001340: 7346 0000 0074 007c 0183 017d 0274 017c  sF...t.|...}.t.|
 00001350: 0064 0183 028f 207d 037c 03a0 0264 02a0  .d.... }.|...d..
 00001360: 037c 02a1 01a1 0101 0057 0064 0004 0004  .|.......W.d....
 00001370: 0083 0301 006e 1031 0073 3830 0001 0001  .....n.1.s80....
 00001380: 0001 0059 0001 0064 0053 0029 034e 7229  ...Y...d.S.).Nr)
-00001390: 0000 00da 0120 2904 724e 0000 0072 2a00  ..... ).rN...r*.
+00001390: 0000 00da 0120 2904 7250 0000 0072 2a00  ..... ).rP...r*.
 000013a0: 0000 da05 7772 6974 6572 1100 0000 2904  ....writer....).
-000013b0: 7210 0000 0072 4a00 0000 724d 0000 005a  r....rJ...rM...Z
+000013b0: 7210 0000 0072 4b00 0000 724f 0000 005a  r....rK...rO...Z
 000013c0: 0862 6174 5f66 696c 6572 0900 0000 7209  .bat_filer....r.
 000013d0: 0000 0072 0a00 0000 da17 6372 6561 7465  ...r......create
 000013e0: 5f63 6f6d 6d61 6e64 5f62 6174 5f66 696c  _command_bat_fil
-000013f0: 65b4 0000 0073 0600 0000 0001 0802 0c01  e....s..........
-00001400: 7270 0000 0063 0100 0000 0000 0000 0000  rp...c..........
+000013f0: 65b6 0000 0073 0600 0000 0001 0802 0c01  e....s..........
+00001400: 7272 0000 0063 0100 0000 0000 0000 0000  rr...c..........
 00001410: 0000 0a00 0000 0800 0000 4300 0000 731a  ..........C...s.
 00001420: 0100 0074 006a 0164 0119 007d 017c 0164  ...t.j.d...}.|.d
 00001430: 0217 007d 0264 037d 037c 0044 005d 207d  ...}.d.}.|.D.] }
 00001440: 047c 04a0 0264 0464 05a1 027d 047c 0364  .|...d.d...}.|.d
 00001450: 067c 049b 0064 079d 0317 007d 0371 1a64  .|...d.....}.q.d
 00001460: 087c 039b 0064 099d 037d 0574 006a 03a0  .|...d...}.t.j..
 00001470: 047c 02a1 0173 8474 0564 0a64 0b64 0c8d  .|...s.t.d.d.d..
@@ -347,47 +347,47 @@
 000015a0: 6970 7974 686f 6e5f 636f 6e66 6967 2e70  ipython_config.p
 000015b0: 797a 0a69 6d70 6f72 7420 7379 73fa 015c  yz.import sys..\
 000015c0: 7220 0000 007a 153b 2073 7973 2e70 6174  r ...z.; sys.pat
 000015d0: 682e 696e 7365 7274 2830 2c22 7a02 2229  h.insert(0,"z.")
 000015e0: 7a25 632e 496e 7465 7261 6374 6976 6553  z%c.InteractiveS
 000015f0: 6865 6c6c 4170 702e 6578 6563 5f6c 696e  hellApp.exec_lin
 00001600: 6573 203d 205b 277a 0227 5dda 0475 7365  es = ['z.']..use
-00001610: 7254 2901 724b 0000 00e9 0100 0000 7a0f  rT).rK........z.
+00001610: 7254 2901 724c 0000 00e9 0100 0000 7a0f  rT).rL........z.
 00001620: 2070 726f 6669 6c65 2063 7265 6174 6572   profile creater
-00001630: 5f00 0000 7a17 4372 6561 7469 6e67 2070  _...z.Creating p
+00001630: 6100 0000 7a17 4372 6561 7469 6e67 2070  a...z.Creating p
 00001640: 726f 6669 6c65 2077 6974 683a 2046 da01  rofile with: F..
 00001650: 724e 7a07 4164 6469 6e67 3ada 0161 da01  rNz.Adding:..a..
-00001660: 0a29 0b72 0f00 0000 7260 0000 0072 4500  .).r....r`...rE.
-00001670: 0000 7210 0000 0072 3900 0000 724e 0000  ..r....r9...rN..
-00001680: 0072 6500 0000 724f 0000 0072 2300 0000  .re...rO...r#...
-00001690: 722a 0000 0072 6f00 0000 290a 5a14 6578  r*...ro...).Z.ex
+00001660: 0a29 0b72 0f00 0000 7262 0000 0072 4600  .).r....rb...rF.
+00001670: 0000 7210 0000 0072 3a00 0000 7250 0000  ..r....r:...rP..
+00001680: 0072 6700 0000 7251 0000 0072 2300 0000  .rg...rQ...r#...
+00001690: 722a 0000 0072 7100 0000 290a 5a14 6578  r*...rq...).Z.ex
 000016a0: 7472 615f 6e6f 7465 626f 6f6b 5f70 6174  tra_notebook_pat
 000016b0: 6873 5a11 7573 6572 5f70 726f 6669 6c65  hsZ.user_profile
 000016c0: 5f70 6174 685a 1469 7079 7468 6f6e 5f70  _pathZ.ipython_p
 000016d0: 726f 6669 6c65 5f70 6174 685a 0f6e 625f  rofile_pathZ.nb_
 000016e0: 7061 7468 5f63 6f6d 6d61 6e64 7210 0000  path_commandr...
-000016f0: 005a 096e 625f 7374 7269 6e67 724d 0000  .Z.nb_stringrM..
-00001700: 0072 3900 0000 5a0c 7072 6f66 696c 655f  .r9...Z.profile_
-00001710: 636f 6465 7251 0000 0072 0900 0000 7209  coderQ...r....r.
+000016f0: 005a 096e 625f 7374 7269 6e67 724f 0000  .Z.nb_stringrO..
+00001700: 0072 3a00 0000 5a0c 7072 6f66 696c 655f  .r:...Z.profile_
+00001710: 636f 6465 7253 0000 0072 0900 0000 7209  coderS...r....r.
 00001720: 0000 0072 0a00 0000 da12 6164 645f 6e6f  ...r......add_no
-00001730: 7465 626f 6f6b 5f70 6174 6873 bc00 0000  tebook_paths....
+00001730: 7465 626f 6f6b 5f70 6174 6873 be00 0000  tebook_paths....
 00001740: 732c 0000 0000 040a 0108 0204 0108 010c  s,..............
 00001750: 0112 010c 020c 020c 010c 020e 010a 0804  ................
 00001760: 010c 0108 0108 0104 0124 0206 010a 010c  .........$......
-00001770: 0172 7800 0000 2902 7249 0000 0046 2901  .rx...).rI...F).
-00001780: 7249 0000 0029 1cda 075f 5f64 6f63 5f5f  rI...)...__doc__
-00001790: 722b 0000 0072 0f00 0000 723b 0000 0072  r+...r....r;...r
-000017a0: 1200 0000 7243 0000 0072 6500 0000 7234  ....rC...re...r4
-000017b0: 0000 0072 0c00 0000 7203 0000 0072 6800  ...r....r....rh.
-000017c0: 0000 7267 0000 0072 3a00 0000 da08 5f5f  ..rg...r:.....__
+00001770: 0172 7a00 0000 2902 724a 0000 0046 2901  .rz...).rJ...F).
+00001780: 724a 0000 0029 1cda 075f 5f64 6f63 5f5f  rJ...)...__doc__
+00001790: 722b 0000 0072 0f00 0000 723c 0000 0072  r+...r....r<...r
+000017a0: 1200 0000 7244 0000 0072 6700 0000 7235  ....rD...rg...r5
+000017b0: 0000 0072 0c00 0000 7203 0000 0072 6a00  ...r....r....rj.
+000017c0: 0000 7269 0000 0072 3b00 0000 da08 5f5f  ..ri...r;.....__
 000017d0: 6669 6c65 5f5f da06 7061 7265 6e74 da08  file__..parent..
 000017e0: 6162 736f 6c75 7465 5a12 4e4f 5445 424f  absoluteZ.NOTEBO
 000017f0: 4f4b 5f44 4952 4543 544f 5259 7205 0000  OK_DIRECTORYr...
 00001800: 0072 2700 0000 7230 0000 0072 3200 0000  .r'...r0...r2...
-00001810: 723f 0000 0072 4700 0000 7248 0000 0072  r?...rG...rH...r
-00001820: 4e00 0000 726d 0000 0072 7000 0000 7278  N...rm...rp...rx
+00001810: 7240 0000 0072 4800 0000 7249 0000 0072  r@...rH...rI...r
+00001820: 5000 0000 726f 0000 0072 7200 0000 727a  P...ro...rr...rz
 00001830: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
 00001840: 0000 720a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001850: 3e03 0000 0073 2e00 0000 0408 0801 0801  >....s..........
+00001850: 3e03 0000 0073 2e00 0000 0409 0801 0801  >....s..........
 00001860: 0801 0801 0801 0801 0801 0801 0c02 0401  ................
-00001870: 0402 1403 0e0f 0c10 0805 0805 0823 0808  .............#..
+00001870: 0403 1403 0e0f 0c10 0805 0805 0823 0808  .............#..
 00001880: 0808 0a17 1226 0a08                      .....&..
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/notebook_setup.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/notebook_setup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/notebooks/run.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/notebooks/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 Created on Fri Sep 24 13:55:39 2021
 
 @author: chris.kerklaan
 
 Opens a jupyter notebook based on nbopen using the command line
 
 """
+
 import json
 import os
 import pathlib
 import shutil
 import site
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
 
 CREATE_NEW_PROCESS_GROUP = 0x00000200
 DETACHED_PROCESS = 0x00000008
 
+# TODO variable also in constants.py
 NOTEBOOK_DIRECTORY = str(pathlib.Path(__file__).parent.absolute())
 
 
 class TempCopy:
     def __init__(self, original_path):
         self.original_path = Path(original_path)
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/queries.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,19 +192,19 @@
 geometry_check_query_base = f"""\
     SELECT *
     FROM (
         SELECT {{table}}.{id_col},
         '{{table}}' as table_name,
         {{table}}.{conn_node_start_id_col},
         {{table}}.{conn_node_end_id_col},
-        {f_aswkt}({f_transform}({{table}}.{geo_col}, {{projection}})) as {df_geo_col},
-        {f_aswkt}({f_transform}({f_pointn}({{table}}.{geo_col}, 1), {{projection}})) as {a_geo_start_coord},
-        {f_aswkt}({f_transform}({f_pointn}({{table}}.{geo_col}, {f_numpoints}({{table}}.{geo_col})), {{projection}})) as {a_geo_end_coord},
-        {f_aswkt}({f_transform}(connection_nodes_start.{geo_col}, {{projection}})) as {a_geo_start_node},
-        {f_aswkt}({f_transform}(connection_nodes_end.{geo_col}, {{projection}})) as {a_geo_end_node}
+        {f_aswkt}({{table}}.{geo_col}) as {df_geo_col},
+        {f_aswkt}({f_pointn}({{table}}.{geo_col}, 1)) as {a_geo_start_coord},
+        {f_aswkt}({f_pointn}({{table}}.{geo_col}, {f_numpoints}({{table}}.{geo_col}))) as {a_geo_end_coord},
+        {f_aswkt}(connection_nodes_start.{geo_col}) as {a_geo_start_node},
+        {f_aswkt}(connection_nodes_end.{geo_col}) as {a_geo_end_node}
         FROM
         {{table}}
         LEFT JOIN
         {connection_nodes_layer} as {a_geo_conn_nodes_end}
         ON
         connection_nodes_end.{id_col} IS {{table}}.{conn_node_end_id_col}
         LEFT JOIN
@@ -493,13 +493,13 @@
 
 controlled_structures_query = construct_controlled_structures_query()
 
 
 def construct_geometry_query(table_names, dst_crs=DEF_TRGT_CRS):
     queries_lst = []
     for table in table_names:
-        queries_lst.append(geometry_check_query_base.format(table=table, projection=dst_crs))
+        queries_lst.append(geometry_check_query_base.format(table=table))
     query = "\nUNION ALL\n".join(queries_lst)
     return query
 
 
 geometry_check_query = construct_geometry_query(table_names=[channels_layer, culvert_layer])
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/utils/queries_general_checks.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/utils/queries_general_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
     surface_id_col,
     surface_layer,
     surface_map_layer,
     weir_layer,
     width_col,
 )
 
-# Error messages
+# Error/warning/info messages
 msg_height_not_used_for_shape = "WARNING: cross section definition height not used for shape type 1"
 msg_uneven_width_height = "ERROR: multiple height and width entries must have the same count"
-msg_impervious_not_in_map = "ERROR: impervious surface is not in mapping table"
+msg_impervious_not_in_map = "WARNING: impervious surface is not in mapping table"
 msg_impervious_map_refers_to_none = "ERROR: impervious surface map refers to non-existent node"
-msg_surface_not_in_mapping = "ERROR: surface is not in mapping table"
-msg_impervious_surface_map_not_in_impervious = "ERROR: impervious surface map is not in impervious surface layer"
-msg_conn_node_without_imp_surface = "ERROR: connection node without impervious surface"
+msg_surface_not_in_mapping = "WARNING: surface is not in mapping table"
+msg_impervious_surface_map_not_in_impervious = "WARNING: impervious surface map is not in impervious surface layer"
+msg_conn_node_without_imp_surface = "WARNING: connection node without impervious surface"
 msg_channel_without_cross_loc = "ERROR: channel without cross section location"
 msg_cross_sec_loc_without_def = "ERROR: cross section location without definition"
 msg_culvert_without_def = "ERROR: culvert without cross section definition"
 msg_weir_without_def = "ERROR: weir without cross section definition"
 msg_orifice_without_def = "ERROR: orifice without cross section definition"
 msg_manhole_without_conn_node = "ERROR: manhole without connection node"
 msg_one_d_boundary_cond_without_conn = "WARNING: 1d boundary without connection node"
@@ -71,15 +71,15 @@
 )
 msg_orifice_strt_end_not_same_init_waterlvl = (
     "'WARNING: initial water level at start and end node are not equal ' " "|| {} || ', ' || {}"
 )
 msg_culvert_strt_end_not_same_init_waterlvl = (
     "'WARNING: Initial waterlevel at start en end node not equal' || {} || " "', ' || {}"
 )
-msg_imp_surface_perc = "ERROR: percentage = 100 and should be 14.4 or 11.5"
+msg_imp_surface_perc = "WARNING: percentage = 100 and should be 14.4 or 11.5"
 msg_control_table_too_many_chars = "ERROR: action_table has more than 1000 characters (model will crash)"
 
 
 def constr_in_clause(innotin, sel=False, frm=False, where=None):
     """
         constr_in_clause(
             innotin (string: either 'IN' or 'NOT IN')
@@ -239,15 +239,15 @@
     ######################################################################################
     "impervious_surface_map_refers_to_inv_imp_surf": construct_sel_from_where_query(
         where="{} " + constr_in_clause(innotin="NOT IN", sel=True, frm=True)
     ).format(
         construct_query_head(impervious_surface_map_layer, msg_impervious_surface_map_not_in_impervious),
         impervious_surface_map_layer,
         f"{impervious_surface_map_layer}.{id_col}",
-        impervious_surface_id_col,
+        id_col,
         impervious_surface_layer,
     ),
     ######################################################################################
     "conn_node_without_imp_surface": construct_sel_from_where_query(
         where="{}"
         + constr_in_clause(
             "IN",
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/api_settings.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/api_settings.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/bank_levels.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/bank_levels.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/database_aliases.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/database_aliases.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/database_variables.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/database_variables.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/model_state.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/model_state.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/one_d_two_d.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/one_d_two_d.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,8 +35,7 @@
 one_d_two_d = "1d2d"
 two_d = "2d"
 start_rain_sfx = "_start_rain"
 end_rain_sfx = "_end_rain"
 twelve_hr_after_rain_sfx = "_12_hours_after_rain"
 max_sfx = "_max"
 suffixes_list = [start_rain_sfx, end_rain_sfx, twelve_hr_after_rain_sfx, max_sfx]
-pump_line = "pump_line"
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/sqlite.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/sqlite.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools/variables/zero_d_one_d.py` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools/variables/zero_d_one_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools.egg-info/PKG-INFO` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 Metadata-Version: 2.1
 Name: hhnk-threedi-tools
-Version: 2023.4
+Version: 2024.1
 Summary: HHNK watersystemen analysis tools
 Home-page: https://github.com/threedi/hhnk-threedi-tools
 Author: Wietse van Gerwen, Laure Ravier
 Author-email: w.vangerwen@hhnk.nl
 Maintainer: Wietse van Gerwen
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/threedi/hhnk-threedi-tools/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-
-UNKNOWN
-
```

### Comparing `hhnk-threedi-tools-2023.4/hhnk_threedi_tools.egg-info/SOURCES.txt` & `hhnk_threedi_tools-2024.1/hhnk_threedi_tools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 hhnk_threedi_tools.egg-info/PKG-INFO
 hhnk_threedi_tools.egg-info/SOURCES.txt
 hhnk_threedi_tools.egg-info/dependency_links.txt
 hhnk_threedi_tools.egg-info/top_level.txt
 hhnk_threedi_tools/core/__init__.py
 hhnk_threedi_tools/core/folder_helpers.py
 hhnk_threedi_tools/core/folders.py
+hhnk_threedi_tools/core/folders_modelbuilder.py
 hhnk_threedi_tools/core/api/__init__.py
 hhnk_threedi_tools/core/api/calculation.py
 hhnk_threedi_tools/core/api/calculation_gui_class.py
 hhnk_threedi_tools/core/api/download_functions.py
 hhnk_threedi_tools/core/api/download_gui_class.py
 hhnk_threedi_tools/core/checks/__init__.py
 hhnk_threedi_tools/core/checks/bank_levels.py
@@ -282,17 +283,20 @@
 hhnk_threedi_tools/variables/model_state.py
 hhnk_threedi_tools/variables/one_d_two_d.py
 hhnk_threedi_tools/variables/sqlite.py
 hhnk_threedi_tools/variables/weirs.py
 hhnk_threedi_tools/variables/zero_d_one_d.py
 tests/test_bank_level_check.py
 tests/test_calculation_gui.py
+tests/test_create_schematisation_rasters.py
 tests/test_folder_structures.py
 tests/test_klimaatsommen_prep.py
+tests/test_layer_structure.py
 tests/test_modelsplitter.py
+tests/test_netcdf_to_gridgpkg.py
 tests/test_one_d_two_d.py
 tests/test_result_rasters.py
 tests/test_schema_migration.py
 tests/test_sqlite.py
 tests/test_zero_d_one_d.py
 tests/notebooks/__init__.py
 tests/notebooks/notebook_setup.py
```

### Comparing `hhnk-threedi-tools-2023.4/setup.py` & `hhnk_threedi_tools-2024.1/setup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/tests/notebooks/notebook_setup.py` & `hhnk_threedi_tools-2024.1/tests/notebooks/notebook_setup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/tests/notebooks/rtest_lizardapi.py` & `hhnk_threedi_tools-2024.1/tests/notebooks/rtest_lizardapi.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/tests/notebooks/rtest_notebooks.py` & `hhnk_threedi_tools-2024.1/tests/notebooks/rtest_notebooks.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/tests/notebooks/rtest_upload_schema.py` & `hhnk_threedi_tools-2024.1/tests/notebooks/rtest_upload_schema.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.4/tests/test_bank_level_check.py` & `hhnk_threedi_tools-2024.1/tests/test_bank_level_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # %%
 """
 Note: the curent tests are only ran to check if the functions work.
 They still must be checked qualitatively
 
 """
-# First-party imports
+import time
 from pathlib import Path
 
-# Local imports
-from hhnk_threedi_tools.core.folders import Folders
-from hhnk_threedi_tools.core.checks.bank_levels import BankLevelTest
-
 import pandas as pd
-# pd.options.mode.chained_assignment = 'raise' #catch SettingWithCopyWarning
 
+# pd.options.mode.chained_assignment = 'raise' #catch SettingWithCopyWarning
 import pytest
+
+from hhnk_threedi_tools.core.checks.bank_levels import BankLevelTest
+from hhnk_threedi_tools.core.folders import Folders
 from tests.config import FOLDER_TEST
-import time
 
 
-class TestBankLevel():
-    
+class TestBankLevel:
     @pytest.fixture(scope="class")
     def bl_test(self):
         bl = BankLevelTest(FOLDER_TEST)
         bl.import_data()
         return bl
-    
 
     def test_import_information_object(self, bl_test):
         """tests if the import of information works, if the correct amount is imported"""
 
         # look at counts
         assert all(bl_test.imports["manholes"].count() == 0)  # no manholes
         assert bl_test.imports["fixeddrainage"].count()["id"] == 32
@@ -39,89 +35,78 @@
         assert bl_test.imports["conn_nodes"].count()["conn_node_id"] == 72
         assert bl_test.imports["channels"].count()["channel_id"] == 49
         assert bl_test.imports["cross_loc"].count()["cross_loc_id"] == 96
         assert bl_test.imports["levee_lines"].count()["levee_id"] == 54
 
         # look at random info
         assert bl_test.imports["fixeddrainage"]["peil_id"][0] == "46442"
-        assert (
-            bl_test.imports["fixeddrainage_lines"]["streefpeil_bwn2"][1].values[0] == -0.85
-        )
+        assert bl_test.imports["fixeddrainage_lines"]["streefpeil_bwn2"][1].values[0] == -0.85
         assert bl_test.imports["lines_1d2d"]["storage_area"][423] == 20.5620565088836
         assert bl_test.imports["conn_nodes"]["conn_node_id"][15] == 15
         assert bl_test.imports["channels"]["initial_waterlevel"][487] == -0.55
         assert bl_test.imports["cross_loc"]["reference_level"][282] == -0.94
         assert bl_test.imports["levee_lines"]["levee_height"][54] == 0.159
 
-
     def test_levee_intersections(self, bl_test):
         """tests if levee intersections can be done"""
         bl_test.line_intersections()
         assert bl_test.line_intersects["levee_id"][425] == 16
 
-
     def test_divergent_waterlevel_nodes(self, bl_test):
         bl_test.divergent_waterlevel_nodes()
 
         assert bl_test.diverging_wl_nodes["type"][0] == "node_in_wrong_fixeddrainage_area"
 
-
     def test_manhole_information(self, bl_test):
-
         bl_test.divergent_waterlevel_nodes()
         bl_test.line_intersections()
         bl_test.manhole_information()
 
         assert bl_test.manholes_info["type"][9] == "node_in_wrong_fixeddrainage_area"
 
-
     def test_flowlines_1d2d(self, bl_test):
-
         bl_test.line_intersections()
         bl_test.flowlines_1d2d()
 
         assert bl_test.all_1d2d_flowlines["type"][99] == "1d2d_crosses_levee"
 
-
     def test_manholes_to_add_to_model(self, bl_test):
         bl_test.divergent_waterlevel_nodes()
         bl_test.line_intersections()
         bl_test.manhole_information()
         bl_test.manholes_to_add_to_model()
 
         assert bl_test.new_manholes_df["connection_node_id"][0] == 44
 
-
     def test_generate_cross_section_locations(self, bl_test):
         bl_test.line_intersections()
         bl_test.generate_cross_section_locations()
 
         assert bl_test.cross_loc_new_filtered["bank_level_source"][0] == "initial+10cm"
         assert bl_test.cross_loc_new["bank_level_diff"][82] == -1.66
 
-
     def test_generate_channels(self, bl_test):
         bl_test.line_intersections()
         bl_test.flowlines_1d2d()
         bl_test.generate_cross_section_locations()
         bl_test.generate_channels()
 
         assert bl_test.new_channels["initial_waterlevel"][48] == -0.85
 
-
     def test_results(self, bl_test):
         bl_test.run()
         results = bl_test.results
 
         assert results["line_intersects"].count()["node_id"] == 9
 
 
 # %%
 if __name__ == "__main__":
     import inspect
+
     selftest = TestBankLevel()
     bl_test = selftest.bl_test()
-    #Run all testfunctions
+    # Run all testfunctions
     for i in dir(selftest):
-        if i.startswith('test_') and hasattr(inspect.getattr_static(selftest,i), '__call__'):
+        if i.startswith("test_") and hasattr(inspect.getattr_static(selftest, i), "__call__"):
             print(i)
-            getattr(selftest, i)(bl_test)    
+            getattr(selftest, i)(bl_test)
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_calculation_gui.py` & `hhnk_threedi_tools-2024.1/tests/test_calculation_gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 # %%
 import shutil
 from pathlib import Path
-import pytest
 
 import hhnk_research_tools as hrt
-from hhnk_threedi_tools.core.folders import Folders
+import pytest
+
 from hhnk_threedi_tools.core.api.calculation import SimulationData
+from hhnk_threedi_tools.core.folders import Folders
 from tests.config import FOLDER_TEST, PATH_NEW_FOLDER
-     
+
 
 def test_simulationdata():
-    simdata = SimulationData(sqlite_path=FOLDER_TEST.model.schema_base.database.base, 
-                                    sim_name="test_simdata", 
-                                    sim_duration=900, 
-                                    rain_data=[{}],
-                                    threedi_api = None,
-                                    model_id = None)
+    simdata = SimulationData(
+        sqlite_path=FOLDER_TEST.model.schema_base.database.base,
+        sim_name="test_simdata",
+        sim_duration=900,
+        rain_data=[{}],
+        threedi_api=None,
+        model_id=None,
+    )
 
-    #Numerical settings
+    # Numerical settings
     numerical_settings = simdata.numerical_settings
     assert numerical_settings["use_nested_newton"] == 1
 
-    #Physical settings
+    # Physical settings
     physical_settings = simdata.physical_settings
     assert physical_settings["use_advection_1d"] == 1
 
-    #Timestep settings
+    # Timestep settings
     time_step_settings = simdata.time_step_settings
     assert time_step_settings["time_step"] == 15
-    
-    #Boundary data
+
+    # Boundary data
     boundaries = simdata.boundaries
     assert boundaries == []
 
-    #Aggregation settings
+    # Aggregation settings
     aggregation = simdata.aggregation
     assert len(aggregation) == 11
 
 
 # %%
 if __name__ == "__main__":
     from threedi_api_client import ThreediApi
+
     from hhnk_threedi_tools.utils.notebooks.notebook_setup import setup_notebook
+
     notebook_data = setup_notebook()
 
-    #Test if iniwlvl works. Needs api key so not on pytests (yet)
+    # Test if iniwlvl works. Needs api key so not on pytests (yet)
     api_keys = hrt.read_api_file(notebook_data["api_keys_path"])
     config = {
         "THREEDI_API_HOST": "https://api.3di.live",
         "THREEDI_API_PERSONAL_API_TOKEN": api_keys["threedi"],
     }
     threedi_api = ThreediApi(config=config)
     model_id = 58400
     FOLDER_TEST.model.set_modelsplitter_paths()
-    simdata = SimulationData(sqlite_path=FOLDER_TEST.model.schema_1d2d_glg.database.path, 
-                            sim_name="test_simdata", 
-                            sim_duration=900, 
-                            rain_data=[{}],
-                            threedi_api = threedi_api,
-                            model_id = model_id)
-
+    simdata = SimulationData(
+        sqlite_path=FOLDER_TEST.model.schema_1d2d_glg.database.path,
+        sim_name="test_simdata",
+        sim_duration=900,
+        rain_data=[{}],
+        threedi_api=threedi_api,
+        model_id=model_id,
+    )
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_folder_structures.py` & `hhnk_threedi_tools-2024.1/tests/test_folder_structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 # %%
 import shutil
 from pathlib import Path
-from hhnk_threedi_tools.core.folders import Folders
 
+from hhnk_threedi_tools.core.folders import Folders
 
 SUB_FOLDERS = ["01_source_data", "02_schematisation", "03_3di_results", "04_test_results"]
 
-from tests.config import FOLDER_TEST, PATH_TEST_MODEL, \
-                        FOLDER_NEW, PATH_NEW_FOLDER
+from tests.config import FOLDER_NEW, FOLDER_TEST, PATH_NEW_FOLDER, PATH_TEST_MODEL
 
-class TestFolder:
 
+class TestFolder:
     def test_create_project(self):
         """tests if a new project folders are created"""
         # create a project without creating sub-dirs
         new_folder = Folders(PATH_NEW_FOLDER, create=False)
-        assert not Path(PATH_NEW_FOLDER).exists()    # check sub-dirs empty
+        assert not Path(PATH_NEW_FOLDER).exists()  # check sub-dirs empty
         new_folder = Folders(PATH_NEW_FOLDER, create=True)
 
         # check if SUB_FOLDERS exist and contain a readme.txt
         for i in SUB_FOLDERS:
             assert PATH_NEW_FOLDER.joinpath(i).exists(), f"No folder: {i}"
             assert PATH_NEW_FOLDER.joinpath(i, "read_me.txt").exists(), f"No readme in {i}"
 
-
     def test_to_file_dict(self):
         """tests if a base path dictionary can be generated"""
         files_dict = FOLDER_NEW.to_file_dict()
         assert files_dict["0d1d_results_dir"] == str(PATH_NEW_FOLDER / "03_3di_results" / "0d1d_results")
 
-
     def test_create_revision(self):
         """tests if a new revision folder can be made"""
         if FOLDER_NEW.threedi_results.zero_d_one_d["new"].exists():
             shutil.rmtree(FOLDER_NEW.threedi_results.zero_d_one_d["new"].base)
 
         FOLDER_NEW.threedi_results.zero_d_one_d["new"].create()
 
         assert FOLDER_NEW.threedi_results.zero_d_one_d["new"].exists() is True
 
-        
     def test_find_dem(self):
         dem = FOLDER_TEST.full_path(r"02_schematisation/00_basis/rasters/dem_hoekje.tif")
-        assert Path(FOLDER_TEST.model.schema_base.rasters.dem.path) == Path(
-            dem.path
-        )
-
+        assert Path(FOLDER_TEST.model.schema_base.rasters.dem.path) == Path(dem.path)
 
     def test_find_threediresult(self):
-        assert FOLDER_TEST.threedi_results.zero_d_one_d[0].base == FOLDER_TEST.threedi_results.zero_d_one_d["BWN bwn_test #7 0d1d_test"].base
+        assert (
+            FOLDER_TEST.threedi_results.zero_d_one_d[0].base
+            == FOLDER_TEST.threedi_results.zero_d_one_d["BWN bwn_test #7 0d1d_test"].base
+        )
+
     # TODO .find() is weg.
     # def test_find_threedi_sources(self):
     #     results_path = TEST_DIRECTORY / r"model_test/03_3di_results/0d1d_results/BWN bwn_test #7 0d1d_test"
     #     folder = Folders(MODEL_FOLDER)
     #     results = folder.threedi_results.find(revision_path=results_path)
     #     assert Path(results["nc_file"]) == Path(
     #         results_path / "results_3di.nc"
@@ -62,15 +59,16 @@
         batch_fd = FOLDER_NEW.threedi_results.batch["test"]
         assert hasattr(batch_fd.downloads, "blok_ghg_T1000")
 
 
 # %%
 if __name__ == "__main__":
     import inspect
+
     selftest = TestFolder()
-    #Run all testfunctions
+    # Run all testfunctions
     for i in dir(selftest):
-        if i.startswith('test_') and hasattr(inspect.getattr_static(selftest,i), '__call__'):
+        if i.startswith("test_") and hasattr(inspect.getattr_static(selftest, i), "__call__"):
             print(i)
             getattr(selftest, i)()
 # %%
-#FOLDER_NEW.to_file_dict()
+# FOLDER_NEW.to_file_dict()
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_klimaatsommen_prep.py` & `hhnk_threedi_tools-2024.1/tests/test_klimaatsommen_prep.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 # %%
 # First-party imports
-import pandas as pd
 import shutil
+
+import hhnk_research_tools as hrt
+import pandas as pd
 import pytest
 
 # Local imports
-from hhnk_threedi_tools.core.climate_scenarios.klimaatsommen_prep import KlimaatsommenPrep
-from hhnk_threedi_tools.core.folders import Folders
+from hhnk_threedi_tools.core.climate_scenarios.klimaatsommen_prep import (
+    KlimaatsommenPrep,
+)
 from hhnk_threedi_tools.core.folder_helpers import ClimateResult
-import hhnk_research_tools as hrt
-
-
+from hhnk_threedi_tools.core.folders import Folders
 from tests.config import FOLDER_TEST, TEMP_DIR, TEST_DIRECTORY
 
+
 def test_klimaatsommenprep_verify():
     """Raises because not all 18 scenarios downloaded"""
     with pytest.raises(Exception):
-        klimaatsommenprep = KlimaatsommenPrep(folder=FOLDER_TEST,
+        klimaatsommenprep = KlimaatsommenPrep(
+            folder=FOLDER_TEST,
             batch_name="batch_test",
-            cfg_file = 'cfg_lizard.cfg',
-            landuse_file = FOLDER_TEST.model.schema_base.rasters.landuse,
-            verify=True
+            cfg_file="cfg_lizard.cfg",
+            landuse_file=FOLDER_TEST.model.schema_base.rasters.landuse,
+            verify=True,
         )
 
+
 def test_klimaatsommenprep():
-    klimaatsommenprep = KlimaatsommenPrep(folder=FOLDER_TEST,
+    """Test creation of gpkg and rasters"""
+    # %%
+    klimaatsommenprep = KlimaatsommenPrep(
+        folder=FOLDER_TEST,
         batch_name="batch_test",
-        cfg_file = 'cfg_lizard.cfg',
-        landuse_file = FOLDER_TEST.model.schema_base.rasters.landuse,
-        verify=False
+        cfg_file="cfg_lizard.cfg",
+        landuse_file=FOLDER_TEST.model.schema_base.rasters.landuse,
+        verify=False,
     )
-    
-    #Rebase the batch_fd so it will always create all output.
-    batch_test = TEMP_DIR/f"batch_test_{hrt.get_uuid()}"
+
+    # Rebase the batch_fd so it will always create all output.
+    batch_test = TEMP_DIR / f"batch_test_{hrt.get_uuid()}"
     batch_test = ClimateResult(batch_test, create=True)
-    shutil.copytree(src=klimaatsommenprep.batch_fd.downloads.piek_glg_T10.netcdf.path,
-                    dst=batch_test.downloads.piek_glg_T10.netcdf.path)
+    shutil.copytree(
+        src=klimaatsommenprep.batch_fd.downloads.piek_glg_T10.netcdf.path,
+        dst=batch_test.downloads.piek_glg_T10.netcdf.path,
+    )
     klimaatsommenprep.batch_fd = batch_test
-    
-    #Run test
+
+    # Run test
     klimaatsommenprep.run(overwrite=True, testing=True)
 
-    #check results
+    # check results
     for raster_type in ["depth_max", "damage_total"]:
         scenario_metadata = pd.read_csv(klimaatsommenprep.info_file[raster_type].path, sep=";")
-        assertion_metadata = pd.read_csv(TEST_DIRECTORY/fr"test_klimaatsommen/{raster_type}_info_expected.csv", sep=";")
-        # scenario_metadata = damage_data.drop(['Unnamed: 0'], axis=1)
-        # damage_data.set_index(['file name'], inplace = True)
-
-        pd.testing.assert_frame_equal(scenario_metadata, assertion_metadata)
+        assertion_metadata = pd.read_csv(
+            TEST_DIRECTORY / rf"test_klimaatsommen/{raster_type}_info_expected.csv", sep=";"
+        )
+        # we ignore the order of the columns (check_like=True)
+        pd.testing.assert_frame_equal(scenario_metadata, assertion_metadata, check_like=True)
 
 
 # %%
 if __name__ == "__main__":
     test_klimaatsommenprep()
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_modelsplitter.py` & `hhnk_threedi_tools-2024.1/tests/test_modelsplitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 # %%
 import shutil
 from pathlib import Path
-import pytest
 
 import hhnk_research_tools as hrt
+import pytest
+
 from hhnk_threedi_tools.core.folders import Folders
 from hhnk_threedi_tools.core.schematisation.model_splitter import ModelSchematisations
 from tests.config import FOLDER_TEST, PATH_NEW_FOLDER
 
 
-
-class TestModelSplitter():
-    
+class TestModelSplitter:
     @pytest.fixture(scope="class")
     def splitter(self):
-
         FOLDER_NEW = Folders(PATH_NEW_FOLDER, create=True)
-        shutil.copytree(FOLDER_TEST.model.schema_base.base, 
-                        FOLDER_NEW.model.schema_base.base, 
-                        dirs_exist_ok=True)
+        shutil.copytree(FOLDER_TEST.model.schema_base.base, FOLDER_NEW.model.schema_base.base, dirs_exist_ok=True)
         shutil.copy(FOLDER_TEST.model.settings.base, FOLDER_NEW.model.settings.base)
         shutil.copy(FOLDER_TEST.model.settings_default.base, FOLDER_NEW.model.settings_default.base)
         shutil.copy(FOLDER_TEST.model.model_sql.base, FOLDER_NEW.model.model_sql.base)
         spl = ModelSchematisations(folder=FOLDER_NEW)
         return spl
-    
 
     def test_create_schematisation(self, splitter):
         """tests if the import of information works, if the correct amount is imported"""
         splitter.create_schematisation(name="0d1d_test")
         splitter.create_schematisation(name="1d2d_glg")
 
         assert splitter.folder.model.schema_1d2d_glg.rasters.initial_wlvl_2d.exists()
 
-
     def test_create_local_sqlite_revision(self, splitter):
         local_rev_str = splitter.get_latest_local_revision_str()
         assert local_rev_str.startswith("no previous local") == True
 
-        #Create revision
+        # Create revision
         splitter.create_local_sqlite_revision("testrevision")
 
         local_rev_str = splitter.get_latest_local_revision_str()
         assert "testrevision" in local_rev_str
 
-
     def test_query(self, splitter):
         splitter.create_schematisation(name="basis_errors")
         database = splitter.folder.model.schema_basis_errors.database
 
-        cross_loc_df=database.read_table("v2_cross_section_location")
+        cross_loc_df = database.read_table("v2_cross_section_location")
         assert 99999 in cross_loc_df["id"].values
 
 
-
-
 # %%
-if __name__=="__main__":
+if __name__ == "__main__":
     selftest = TestModelSplitter()
     splitter = selftest.splitter()
 
     selftest.test_create_local_sqlite_revision(splitter)
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_one_d_two_d.py` & `hhnk_threedi_tools-2024.1/tests/test_one_d_two_d.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,55 @@
 # %%
-# -*- coding: utf-8 -*-
-"""
-Functional testing for oneDtwoD object
-"""
-# First-party imports
-import os
-import pathlib
+"""Functional testing for oneDtwoD object"""
+import geopandas as gpd
 import pytest
 
-# Local imports
 from hhnk_threedi_tools.core.checks.one_d_two_d import OneDTwoDTest
-from hhnk_threedi_tools.core.folders import Folders
+from tests.config import FOLDER_NEW, FOLDER_TEST
 
 # Globals
 REVISION = "BWN bwn_test #6 1d2d_test"
 
-from tests.config import FOLDER_TEST, FOLDER_NEW
-
 
 class TestOneDTwoD:
-    #Remove previous output
+    # Remove previous output.
     FOLDER_TEST.output.one_d_two_d.unlink_contents(rmdirs=True)
 
     @pytest.fixture(scope="class")
     def check_1d2d(self):
-        check_1d2d= OneDTwoDTest(folder=FOLDER_TEST, revision=REVISION)
+        check_1d2d = OneDTwoDTest(folder=FOLDER_TEST, revision=REVISION)
         check_1d2d.output_fd.create(parents=True)
         return check_1d2d
-    
 
     def test_run_flowline_stats(self, check_1d2d):
-        """test of de hydraulische testen werken"""
+        """Test of de hydraulische testen werken"""
         output = check_1d2d.run_flowline_stats()
 
         assert output["pump_capacity_m3_s"][1094] == 0.00116666666666667
 
-
-    def test_run_node_stats(self, check_1d2d):
-        output = check_1d2d.run_node_stats()
-
-        assert round(output["minimal_dem"][1], 3) == 1.54
-
-
-    def test_run_depth_at_timesteps_test(self, check_1d2d):
-        """test of de 0d1d test werkt"""
+    def test_run_depth_at_timesteps(self, check_1d2d):
+        """Test of de 0d1d test werkt"""
+        output_fd = check_1d2d.folder.output.one_d_two_d[check_1d2d.revision]
 
         check_1d2d.run_wlvl_depth_at_timesteps(overwrite=True)
 
-        assert "waterdiepte_T15.tif" in [i.name for i in check_1d2d.fenv.output.one_d_two_d[check_1d2d.revision].content]
-        assert check_1d2d.fenv.output.one_d_two_d[check_1d2d.revision].waterdiepte_T1.shape == [787, 242]
-        assert check_1d2d.fenv.output.one_d_two_d[check_1d2d.revision].waterdiepte_T15.sum() == 1576.087158203125
+        grid_gdf = gpd.read_file(output_fd.grid_nodes_2d.path)
+        assert grid_gdf.loc[0, "wlvl_corr_15h"] == 0.7591500282287598
+        output_fd.waterdiepte_T15.exists()
+
+        assert output_fd.waterdiepte_T1.shape == [787, 242]
+        assert output_fd.waterdiepte_T15.sum() == 1588.228515625
 
 
 # %%
 if __name__ == "__main__":
     import inspect
+
     self = TestOneDTwoD()
     check_1d2d = self.check_1d2d()
 
+    # %%
     # Run all testfunctions
     for i in dir(self):
-        if i.startswith('test_') and hasattr(inspect.getattr_static(self,i), '__call__'):
+        if i.startswith("test_") and hasattr(inspect.getattr_static(self, i), "__call__"):
             print(i)
-            getattr(self, i)(check_1d2d)  
-# %%
+            getattr(self, i)(check_1d2d)
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_result_rasters.py` & `hhnk_threedi_tools-2024.1/tests/test_result_rasters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 # %%
-# First-party imports
 import geopandas as gpd
-
-
-# Local imports
 import hhnk_research_tools as hrt
-from hhnk_threedi_tools.core.result_rasters.calculate_raster import BaseCalculatorGPKG
-# from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import BankLevelTest
 
-import pandas as pd
 # pd.options.mode.chained_assignment = 'raise' #catch SettingWithCopyWarning
-
 import pytest
-from tests.config import FOLDER_TEST, TEST_DIRECTORY, TEMP_DIR
 
-TEST_RESULT_DIR = TEST_DIRECTORY/r"test_result_rasters"
+from hhnk_threedi_tools.core.result_rasters.calculate_raster import BaseCalculatorGPKG
+from tests.config import FOLDER_TEST, TEMP_DIR, TEST_DIRECTORY
+
+TEST_RESULT_DIR = TEST_DIRECTORY / r"test_result_rasters"
 
 
 class TestBaseCalculatorGPKG:
     @pytest.fixture(scope="class")
     def grid_gdf(self):
-        return gpd.read_file(TEST_RESULT_DIR/"grid_corr_tiny.gpkg", driver="GPKG")
+        return gpd.read_file(TEST_RESULT_DIR / "grid_corr_tiny.gpkg", driver="GPKG")
 
     @pytest.fixture(scope="class")
     def basecalc(self, grid_gdf):
-        calculator_kwargs = {"dem_path":TEST_RESULT_DIR/"dem_tiny.tif",
-                    "grid_gdf":grid_gdf, 
-                    "wlvl_column":"wlvl_max_replaced"}
+        calculator_kwargs = {
+            "dem_path": TEST_RESULT_DIR / "dem_tiny.tif",
+            "grid_gdf": grid_gdf,
+            "wlvl_column": "wlvl_max_replaced",
+        }
         with BaseCalculatorGPKG(**calculator_kwargs) as basecalc:
             return basecalc
-      
 
     def test_wlvl(self, basecalc):
         output_file = hrt.Folder(TEMP_DIR).full_path(f"wlvl_corr_{hrt.get_uuid()}.tif")
-        basecalc.run(output_file=output_file.path,  
-                        mode="MODE_WLVL",
-                        overwrite=True)
-        
+        basecalc.run(output_file=output_file.path, mode="MODE_WLVL", overwrite=True)
+
         assert output_file.sum() == 43.918495178222656
 
     def test_wdepth(self, basecalc):
         output_file = hrt.Folder(TEMP_DIR).full_path(f"wdepth_corr_{hrt.get_uuid()}.tif")
-        basecalc.run(output_file=output_file.path,  
-                    mode="MODE_WDEPTH",
-                    overwrite=True)
+        basecalc.run(output_file=output_file.path, mode="MODE_WDEPTH", overwrite=True)
         assert output_file.sum() == 5.868329048156738
-    
+
 
 # %%
 if __name__ == "__main__":
     import inspect
+
     selftest = TestBaseCalculatorGPKG()
     basecalc = selftest.basecalc(selftest.grid_gdf())
     # self = selftest.bl_test
-    #Run all testfunctions
+    # Run all testfunctions
     for i in dir(selftest):
-        if i.startswith('test_') and hasattr(inspect.getattr_static(selftest,i), '__call__'):
+        if i.startswith("test_") and hasattr(inspect.getattr_static(selftest, i), "__call__"):
             print(i)
-            getattr(selftest, i)(basecalc)    
+            getattr(selftest, i)(basecalc)
 # %%
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_schema_migration.py` & `hhnk_threedi_tools-2024.1/tests/test_schema_migration.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
  # %%
 # First-party imports
 import shutil
 
+import hhnk_research_tools as hrt
+
 # Local imports
 from hhnk_threedi_tools.core.schematisation.migrate import MigrateSchema
-
-
-import hhnk_research_tools as hrt
 from tests.config import FOLDER_TEST, TEMP_DIR
 
+
 def test_schema_migration():
     """test if an old sqlite can be migrated to the latest schema version"""
     #Make a copy, the migration is done on the same database.
     database_old = FOLDER_TEST.full_path("bwn_test_v216.sqlite")
     database_new = hrt.Folder(TEMP_DIR).full_path(f"migrated_sqlite_{hrt.get_uuid()}.sqlite")
 
     try:
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_sqlite.py` & `hhnk_threedi_tools-2024.1/tests/test_sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,143 +1,130 @@
-# %% 
+# %%
 # First-party imports
 import inspect
-
-# Local imports
-from hhnk_threedi_tools.core.checks.sqlite.sqlite_main import SqliteCheck
-
 import shutil
 from pathlib import Path
-import pytest
 
 import hhnk_research_tools as hrt
+import pytest
+
+# Local imports
+from hhnk_threedi_tools.core.checks.sqlite.sqlite_main import SqliteCheck
 from hhnk_threedi_tools.core.folders import Folders
 from hhnk_threedi_tools.core.schematisation.model_splitter import ModelSchematisations
 from tests.config import FOLDER_TEST, PATH_NEW_FOLDER
 
+
 class TestSqlite:
     FOLDER_TEST.output.sqlite_tests.unlink_contents()
 
     sqlite_check = SqliteCheck(folder=FOLDER_TEST)
     sqlite_check.output_fd.create(parents=True)
-    
+
     @pytest.fixture(scope="class")
     def folder_new(self):
-        """Copy folder structure and sqlite and then run splitter so we 
-        get the correct sqlite (with errors) to run tests on."""
+        """Copy folder structure and sqlite and then run splitter so we
+        get the correct sqlite (with errors) to run tests on.
+        """
         FOLDER_NEW = Folders(PATH_NEW_FOLDER, create=True)
-        shutil.copytree(FOLDER_TEST.model.schema_base.path, 
-                        FOLDER_NEW.model.schema_base.path, 
-                        dirs_exist_ok=True)
+        shutil.copytree(FOLDER_TEST.model.schema_base.path, FOLDER_NEW.model.schema_base.path, dirs_exist_ok=True)
         shutil.copy(FOLDER_TEST.model.settings.path, FOLDER_NEW.model.settings.path)
         shutil.copy(FOLDER_TEST.model.settings_default.path, FOLDER_NEW.model.settings_default.path)
         shutil.copy(FOLDER_TEST.model.model_sql.path, FOLDER_NEW.model.model_sql.path)
         # self.folder=FOLDER_TEST
         spl = ModelSchematisations(folder=FOLDER_NEW)
-        spl.create_schematisation(name='basis_errors')
-        
+        spl.create_schematisation(name="basis_errors")
+
         return FOLDER_NEW
-    
-    def test_run_controlled_structures(self):       
+
+    def test_run_controlled_structures(self):
         self.sqlite_check.run_controlled_structures()
 
         output_file = self.sqlite_check.output_fd.gestuurde_kunstwerken
         assert output_file.exists()
 
         output_df = output_file.load()
         assert output_df["hdb_kruin_max"][0] == -0.25
 
-
     def test_run_dem_max_value(self):
         output = self.sqlite_check.run_dem_max_value()
         assert "voldoet aan de norm" in output
 
-
-    def test_run_dewatering_depth(self):           
+    def test_run_dewatering_depth(self):
         self.sqlite_check.run_dewatering_depth()
         assert self.sqlite_check.output_fd.drooglegging.exists()
 
-        assert self.sqlite_check.output_fd.drooglegging.statistics(approve_ok=False
-                    ) == {'min': -0.76, 
-                          'max': 10004.290039, 
-                          'mean': 2.167882, 
-                          'std': 91.391436}
-
+        assert self.sqlite_check.output_fd.drooglegging.statistics(approve_ok=False) == {
+            "min": -0.76,
+            "max": 10004.290039,
+            "mean": 2.167882,
+            "std": 91.391436,
+        }
 
     def test_run_model_checks(self):
         output = self.sqlite_check.run_model_checks()
         assert "node without initial waterlevel" in output.set_index("id").loc[482, "error"]
 
-
     def test_run_geometry(self):
         """TODO empty check"""
         output = self.sqlite_check.run_geometry_checks()
         assert output.empty
 
-
     def test_run_imp_surface_area(self):
         output = self.sqlite_check.run_imp_surface_area()
         assert "61 ha" in output
 
-
     def test_run_isolated_channels(self):
         output = self.sqlite_check.run_isolated_channels()
         assert output[0]["length_in_meters"][10] == 168.45
 
-
     def test_run_used_profiles(self):
         output = self.sqlite_check.run_used_profiles()
         assert output["width_at_wlvl"][0] == 2
 
-
     def test_run_cross_section_duplicates(self, folder_new):
-        database= folder_new.model.schema_basis_errors.database
+        database = folder_new.model.schema_basis_errors.database
         output = self.sqlite_check.run_cross_section_duplicates(database=database)
         assert output["cross_loc_id"].to_list() == [282, 99999]
 
-
     def test_run_cross_section_no_vertex(self, folder_new):
-        database= folder_new.model.schema_basis_errors.database
+        database = folder_new.model.schema_basis_errors.database
         output = self.sqlite_check.run_cross_section_no_vertex(database=database)
         assert output["cross_loc_id"].to_list() == [320]
         assert output["distance_to_vertex"].to_list() == [1.0]
 
-
     def test_create_grid_from_sqlite(self, folder_new):
         self.sqlite_check.create_grid_from_sqlite(output_folder=folder_new.output.sqlite_tests.path)
         assert folder_new.output.sqlite_tests.full_path("cells.gpkg").exists()
 
     def test_run_struct_channel_bed_level(self):
         """TODO empty check"""
         output = self.sqlite_check.run_struct_channel_bed_level()
         assert output.empty
 
-
     def test_run_watersurface_area(self):
         output = self.sqlite_check.run_watersurface_area()
         assert output[0]["area_diff"][0] == -20
 
-
     def test_run_weir_flood_level(self):
         output = self.sqlite_check.run_weir_floor_level()
         assert output[0]["proposed_reference_level"][1] == -1.26
 
 
-
 # %%
 if __name__ == "__main__":
-    import hhnk_research_tools as hrt
     import geopandas as gpd
+    import hhnk_research_tools as hrt
     import numpy as np
 
     self = TestSqlite()
     # self = selftest.sqlite_check
 
     # # Run all testfunctions
     # for i in dir(selftest):
     #     if i.startswith('test_') and hasattr(inspect.getattr_static(selftest,i), '__call__'):
     #         print(i)
     #         getattr(selftest, i)()
     folder_new = self.folder_new()
     # self.test_run_cross_section_duplicates(folder_new=folder_new)
     # self.test_run_cross_section_no_vertex(folder_new=folder_new)
-    self.test_create_grid_from_sqlite(folder_new)
+    self.test_run_geometry()
```

### Comparing `hhnk-threedi-tools-2023.4/tests/test_zero_d_one_d.py` & `hhnk_threedi_tools-2024.1/tests/test_zero_d_one_d.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,28 +12,25 @@
     test_0d1d = ZeroDOneDTest.from_path(PATH_TEST_MODEL)
 
     def test_run_zero_d_one_d_test(self):
         """test of de 0d1d test werkt"""
         self.test_0d1d.run()
         assert self.test_0d1d.results["lvl_end"].count() == 157
 
-
     def test_run_hydraulic_test(self):
         """test of de hydraulische testen werken"""
         self.test_0d1d.run_hydraulic()
         assert self.test_0d1d.hydraulic_results["channels"]["code"].count() == 134
 
 
 # %%
 if __name__ == "__main__":
     import inspect
+
     selftest = TestZeroDOneD()
     self = selftest.test_0d1d
-    #Run all testfunctions
+    # Run all testfunctions
     for i in dir(selftest):
-        if i.startswith('test_') and hasattr(inspect.getattr_static(selftest,i), '__call__'):
+        if i.startswith("test_") and hasattr(inspect.getattr_static(selftest, i), "__call__"):
             print(i)
-            getattr(selftest, i)()    
+            getattr(selftest, i)()
 # %%
-
-
-
```

