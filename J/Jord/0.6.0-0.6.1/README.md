# Comparing `tmp/jord-0.6.0.tar.gz` & `tmp/jord-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jord-0.6.0.tar", last modified: Tue Apr 30 19:14:38 2024, max compression
+gzip compressed data, was "jord-0.6.1.tar", last modified: Fri May  3 12:20:07 2024, max compression
```

## Comparing `jord-0.6.0.tar` & `jord-0.6.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.475094 jord-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.447094 jord-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-30 19:14:34.000000 jord-0.6.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-30 19:14:34.000000 jord-0.6.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 19:14:34.000000 jord-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:34.000000 jord-0.6.0/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.467094 jord-0.6.0/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-30 19:14:38.000000 jord-0.6.0/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-30 19:14:38.000000 jord-0.6.0/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:14:38.000000 jord-0.6.0/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-30 19:14:38.000000 jord-0.6.0/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 19:14:38.000000 jord-0.6.0/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 19:14:34.000000 jord-0.6.0/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-30 19:14:34.000000 jord-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 19:14:34.000000 jord-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-30 19:14:38.475094 jord-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-30 19:14:34.000000 jord-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-30 19:14:34.000000 jord-0.6.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.447094 jord-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 19:14:34.000000 jord-0.6.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.447094 jord-0.6.0/jord/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 19:14:34.000000 jord-0.6.0/jord/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-30 19:14:34.000000 jord-0.6.0/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.447094 jord-0.6.0/jord/fiona_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:34.000000 jord-0.6.0/jord/fiona_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-30 19:14:34.000000 jord-0.6.0/jord/fiona_utilities/deserialise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.451094 jord-0.6.0/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/cloning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/drivers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/enums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/error_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-30 19:14:34.000000 jord-0.6.0/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.451094 jord-0.6.0/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geojson_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geojson_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.451094 jord-0.6.0/jord/geometric_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geometric_analysis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geometric_analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geometric_analysis/center_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geometric_analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geometric_analysis/intersections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geometric_analysis/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.451094 jord-0.6.0/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/geometry_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.455094 jord-0.6.0/jord/geopandas_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/serialisation/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/serialisation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/serialisation/well_known_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-04-30 19:14:34.000000 jord-0.6.0/jord/geopandas_utilities/serialisation/well_known_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.455094 jord-0.6.0/jord/networkx_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-30 19:14:34.000000 jord-0.6.0/jord/networkx_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-30 19:14:34.000000 jord-0.6.0/jord/networkx_utilities/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.455094 jord-0.6.0/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 19:14:34.000000 jord-0.6.0/jord/pillow_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-30 19:14:34.000000 jord-0.6.0/jord/pillow_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-30 19:14:34.000000 jord-0.6.0/jord/pillow_utilities/exif.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-30 19:14:34.000000 jord-0.6.0/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.459094 jord-0.6.0/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.459094 jord-0.6.0/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/configuration/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/configuration/plugin_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3263 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.459094 jord-0.6.0/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/conversion/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/conversion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      179 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/conversion/parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/data_provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/geo_interface_serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.459094 jord-0.6.0/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/copying.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/randomize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/helpers/timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16048 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/layer_creation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/layer_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.463094 jord-0.6.0/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/numpy_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/numpy_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/numpy_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/numpy_utilities/data_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/numpy_utilities/rasters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/styles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.463094 jord-0.6.0/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.463094 jord-0.6.0/jord/qlive_utilities/clients/
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/clients/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/clients/arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/clients/auto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/clients/batching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/pandas_procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.463094 jord-0.6.0/jord/qt_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qt_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-04-30 19:14:34.000000 jord-0.6.0/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.463094 jord-0.6.0/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 19:14:34.000000 jord-0.6.0/jord/rasterio_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-30 19:14:34.000000 jord-0.6.0/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.467094 jord-0.6.0/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/clamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27441 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/lines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/mirroring.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/points.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/polygons.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/projection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/rings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-30 19:14:34.000000 jord-0.6.0/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.467094 jord-0.6.0/jord/spatialite_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-30 19:14:34.000000 jord-0.6.0/jord/spatialite_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-30 19:14:34.000000 jord-0.6.0/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.467094 jord-0.6.0/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:34.000000 jord-0.6.0/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-30 19:14:34.000000 jord-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 19:14:34.000000 jord-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 19:14:38.475094 jord-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-30 19:14:34.000000 jord-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.467094 jord-0.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:14:38.467094 jord-0.6.0/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 19:14:34.000000 jord-0.6.0/tests/qgis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-30 19:14:34.000000 jord-0.6.0/tests/test_import.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-30 19:14:34.000000 jord-0.6.0/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.911470 jord-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-03 12:20:03.000000 jord-0.6.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-03 12:20:03.000000 jord-0.6.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 12:20:03.000000 jord-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:03.000000 jord-0.6.1/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 12:20:07.000000 jord-0.6.1/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 12:20:03.000000 jord-0.6.1/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-03 12:20:03.000000 jord-0.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-03 12:20:03.000000 jord-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-03 12:20:07.911470 jord-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 12:20:03.000000 jord-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-03 12:20:03.000000 jord-0.6.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-03 12:20:03.000000 jord-0.6.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/jord/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 12:20:04.000000 jord-0.6.1/jord/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-05-03 12:20:04.000000 jord-0.6.1/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.883470 jord-0.6.1/jord/fiona_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:04.000000 jord-0.6.1/jord/fiona_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-03 12:20:04.000000 jord-0.6.1/jord/fiona_utilities/deserialise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/cloning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/drivers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/error_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:20:04.000000 jord-0.6.1/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geojson_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geojson_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geometric_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/center_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/intersections.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geometric_analysis/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/geometry_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.887470 jord-0.6.1/jord/geopandas_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-05-03 12:20:04.000000 jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/networkx_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-03 12:20:04.000000 jord-0.6.1/jord/networkx_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-03 12:20:04.000000 jord-0.6.1/jord/networkx_utilities/construction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/exif.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-03 12:20:04.000000 jord-0.6.1/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.891470 jord-0.6.1/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/plugin_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3263 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.895470 jord-0.6.1/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/conversion/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/conversion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      179 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/conversion/parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/data_provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/geo_interface_serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.895470 jord-0.6.1/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/copying.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/randomize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/helpers/timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16113 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/layer_creation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/layer_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.895470 jord-0.6.1/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/data_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/numpy_utilities/rasters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/styles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/qlive_utilities/clients/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/batching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/pandas_procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/qt_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qt_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-05-03 12:20:04.000000 jord-0.6.1/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.899470 jord-0.6.1/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 12:20:04.000000 jord-0.6.1/jord/rasterio_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:20:04.000000 jord-0.6.1/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/clamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27441 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/lines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/mirroring.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/points.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/polygons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/projection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/rings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-05-03 12:20:04.000000 jord-0.6.1/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/jord/spatialite_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-03 12:20:04.000000 jord-0.6.1/jord/spatialite_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-05-03 12:20:04.000000 jord-0.6.1/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:04.000000 jord-0.6.1/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 12:20:04.000000 jord-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 12:20:04.000000 jord-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 12:20:07.911470 jord-0.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-05-03 12:20:04.000000 jord-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:07.903470 jord-0.6.1/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-03 12:20:04.000000 jord-0.6.1/tests/qgis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-05-03 12:20:04.000000 jord-0.6.1/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-05-03 12:20:04.000000 jord-0.6.1/tests/test_sanity.py
```

### Comparing `jord-0.6.0/.github/CODE_OF_CONDUCT.md` & `jord-0.6.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/.github/CONTRIBUTING.md` & `jord-0.6.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/Jord.egg-info/PKG-INFO` & `jord-0.6.1/Jord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -36,87 +36,87 @@
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
 Provides-Extra: samples
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: furo; extra == "docs"
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
 Provides-Extra: gdal
 Provides-Extra: tests
-Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 Provides-Extra: shapely
 Requires-Dist: shapely; extra == "shapely"
 Requires-Dist: pyproj; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: sorcery>=0.2.0; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
 Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: furo; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
-Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: warg>=1.1.6; extra == "dev"
 Requires-Dist: draugr>=1.0.9; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: sorcery>=0.2.0; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: mock; extra == "dev"
 Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
 Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
 Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: furo; extra == "dev"
 Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
 Requires-Dist: importlib-resources; extra == "legacy"
 Requires-Dist: importlib-metadata; extra == "legacy"
 Provides-Extra: setup
 Provides-Extra: all
-Requires-Dist: sorcery>=0.2.0; extra == "all"
-Requires-Dist: Pillow; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: PySide2; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
 Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: furo; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
 Requires-Dist: geopandas; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: Pillow; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
 Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
 Requires-Dist: networkx; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: furo; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
 Requires-Dist: importlib-resources; extra == "all"
 Requires-Dist: mock; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: fiona>=1.1.1; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: PySide2; extra == "all"
 Requires-Dist: pyproj; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: shapely; extra == "all"
 Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
-Requires-Dist: pyzmq>=1.1.1; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.6.0/Jord.egg-info/SOURCES.txt` & `jord-0.6.1/Jord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/Jord.egg-info/requires.txt` & `jord-0.6.1/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -4,72 +4,72 @@
 pyzmq>=1.1.1
 sorcery>=0.2.0
 sympy>=1.1.1
 tqdm>=1.1.1
 warg>=1.1.6
 
 [all]
-sorcery>=0.2.0
-Pillow
-pytest>=4.4.1
-PySide2
-twine>=1.13.0
-pytest>=4.3.0
+fiona>=1.1.1
 numpy>=1.20.0
-furo
-shapely
-sympy>=1.1.1
-tqdm>=1.1.1
 geopandas
+warg>=1.1.6
 draugr>=1.0.9
+sorcery>=0.2.0
 coveralls>=1.6.0
-pip>=22.1.2
+pytest>=4.3.0
+Pillow
+pytest-cov>=2.11.1
+twine>=1.13.0
 wheel>=0.33.0
+apppath>=1.0.2
+pip>=22.1.2
+sphinx>=4.0.1
+tqdm>=1.1.1
+importlib-metadata
 networkx
+sympy>=1.1.1
+pytest>=4.4.1
+black[jupyter]>=21.5b0
+furo
+pyzmq>=1.1.1
 importlib-resources
 mock
-apppath>=1.0.2
-fiona>=1.1.1
-sphinxcontrib-programoutput
+PySide2
 pyproj
-sphinx>=4.0.1
-black[jupyter]>=21.5b0
+sphinxcontrib-programoutput
+shapely
 pre-commit>=2.17.0
-warg>=1.1.6
-importlib-metadata
-pytest-cov>=2.11.1
-pyzmq>=1.1.1
 
 [dev]
-sorcery>=0.2.0
-pytest>=4.4.1
-twine>=1.13.0
-pytest>=4.3.0
 numpy>=1.20.0
-furo
-sympy>=1.1.1
-tqdm>=1.1.1
+warg>=1.1.6
 draugr>=1.0.9
 coveralls>=1.6.0
-pip>=22.1.2
+sorcery>=0.2.0
+pytest>=4.3.0
+pytest-cov>=2.11.1
+twine>=1.13.0
 wheel>=0.33.0
-mock
 apppath>=1.0.2
-sphinxcontrib-programoutput
+pip>=22.1.2
 sphinx>=4.0.1
+tqdm>=1.1.1
+sympy>=1.1.1
+pytest>=4.4.1
 black[jupyter]>=21.5b0
-pre-commit>=2.17.0
-warg>=1.1.6
-pytest-cov>=2.11.1
+furo
 pyzmq>=1.1.1
+mock
+sphinxcontrib-programoutput
+pre-commit>=2.17.0
 
 [docs]
-furo
 sphinxcontrib-programoutput
 sphinx>=4.0.1
+furo
 
 [extra]
 
 [fiona]
 fiona>=1.1.1
 
 [gdal]
@@ -98,9 +98,9 @@
 [setup]
 
 [shapely]
 shapely
 pyproj
 
 [tests]
-mock
 pytest>=4.4.1
+mock
```

### Comparing `jord-0.6.0/LICENSE.md` & `jord-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/PKG-INFO` & `jord-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -36,87 +36,87 @@
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
 Provides-Extra: samples
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: furo; extra == "docs"
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
 Provides-Extra: gdal
 Provides-Extra: tests
-Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 Provides-Extra: shapely
 Requires-Dist: shapely; extra == "shapely"
 Requires-Dist: pyproj; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: sorcery>=0.2.0; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
 Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: furo; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
-Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: warg>=1.1.6; extra == "dev"
 Requires-Dist: draugr>=1.0.9; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: sorcery>=0.2.0; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: mock; extra == "dev"
 Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
 Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
 Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: furo; extra == "dev"
 Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
 Requires-Dist: importlib-resources; extra == "legacy"
 Requires-Dist: importlib-metadata; extra == "legacy"
 Provides-Extra: setup
 Provides-Extra: all
-Requires-Dist: sorcery>=0.2.0; extra == "all"
-Requires-Dist: Pillow; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: PySide2; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
 Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: furo; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
 Requires-Dist: geopandas; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: Pillow; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
 Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
 Requires-Dist: networkx; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: furo; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
 Requires-Dist: importlib-resources; extra == "all"
 Requires-Dist: mock; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: fiona>=1.1.1; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: PySide2; extra == "all"
 Requires-Dist: pyproj; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: shapely; extra == "all"
 Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
-Requires-Dist: pyzmq>=1.1.1; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.6.0/README.md` & `jord-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/SECURITY.md` & `jord-0.6.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/__init__.py` & `jord-0.6.1/jord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 from warg import package_is_editable, clean_string, get_version
 
 __project__ = "Jord"
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Lindbjerg <chen@mapspeople.dk>
```

### Comparing `jord-0.6.0/jord/fiona_utilities/deserialise.py` & `jord-0.6.1/jord/fiona_utilities/deserialise.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/gdal_utilities/__init__.py` & `jord-0.6.1/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/gdal_utilities/cloning.py` & `jord-0.6.1/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/gdal_utilities/context.py` & `jord-0.6.1/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/gdal_utilities/conversion.py` & `jord-0.6.1/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/gdal_utilities/error_handling.py` & `jord-0.6.1/jord/gdal_utilities/error_handling.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/gdal_utilities/importing.py` & `jord-0.6.1/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/gdal_utilities/persistence.py` & `jord-0.6.1/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/geojson_utilities/geometry_types.py` & `jord-0.6.1/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/geometric_analysis/center_line.py` & `jord-0.6.1/jord/geometric_analysis/center_line.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/geometric_analysis/intersections.py` & `jord-0.6.1/jord/geometric_analysis/intersections.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/geopandas_utilities/geometry_filtering.py` & `jord-0.6.1/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/geopandas_utilities/serialisation/well_known_binary.py` & `jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/geopandas_utilities/serialisation/well_known_text.py` & `jord-0.6.1/jord/geopandas_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/networkx_utilities/construction.py` & `jord-0.6.1/jord/networkx_utilities/construction.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/__init__.py` & `jord-0.6.1/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/categorisation.py` & `jord-0.6.1/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/configuration/plugin_settings.py` & `jord-0.6.1/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/configuration/project_settings.py` & `jord-0.6.1/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/data_provider.py` & `jord-0.6.1/jord/qgis_utilities/data_provider.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/enums.py` & `jord-0.6.1/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/geo_interface_serialisation.py` & `jord-0.6.1/jord/qgis_utilities/geo_interface_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/geometry_types.py` & `jord-0.6.1/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/actions.py` & `jord-0.6.1/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/drawing.py` & `jord-0.6.1/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/environment.py` & `jord-0.6.1/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/groups.py` & `jord-0.6.1/jord/qgis_utilities/helpers/groups.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/logging.py` & `jord-0.6.1/jord/qgis_utilities/helpers/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,31 +61,31 @@
                 title=self.tag_name,
                 text=message,
                 level=level,
                 duration=(level + 1) * 3,
             )
 
 
-def add_logging_handler_once(logger, handler):
+def add_logging_handler_once(logger: logging.Logger, handler: logging.Handler) -> bool:
     """A helper to add a handler to a logger, ensuring there are no duplicates.
 
     :param logger: Logger that should have a handler added.
     :type logger: logging.logger
 
     :param handler: Handler instance to be added. It will not be added if an
         instance of that Handler subclass already exists.
     :type handler: logging.Handler
 
     :returns: True if the logging handler was added, otherwise False.
     :rtype: bool
     """
     class_name = handler.__class__.__name__
 
-    for handler in logger.handlers:
-        if handler.__class__.__name__ == class_name:
+    for handler_ in logger.handlers:
+        if handler_.__class__.__name__ == class_name:
             return False
 
     logger.addHandler(handler)
     return True
 
 
 def setup_logger(
```

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/models.py` & `jord-0.6.1/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/progress_bar.py` & `jord-0.6.1/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/randomize.py` & `jord-0.6.1/jord/qgis_utilities/helpers/randomize.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/sessions.py` & `jord-0.6.1/jord/qgis_utilities/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/signals.py` & `jord-0.6.1/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/helpers/timestamp.py` & `jord-0.6.1/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/layer_creation.py` & `jord-0.6.1/jord/qgis_utilities/layer_creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,17 @@
         ), f"{categorise_by_attribute} was not found in {fields}"
 
     if not geoms:
         logger.info("Found no geometries")
         return  # No geometry
 
     features = []
+    if not isinstance(geoms, Iterable):
+        geoms = [geoms]
+
     for geom in geoms:
         geom_type_ = json.loads(geom.asJson())["type"]
 
         assert geom_type_ is not None, f"could not read {geom_type_=} as json"
 
         if geom_type_ is None:
             raise Exception(f"Could not load {geom.asJson()} as json")
```

### Comparing `jord-0.6.0/jord/qgis_utilities/layer_serialisation.py` & `jord-0.6.1/jord/qgis_utilities/layer_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/numpy_utilities/conversion.py` & `jord-0.6.1/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/numpy_utilities/data_type.py` & `jord-0.6.1/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `jord-0.6.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/styles.py` & `jord-0.6.1/jord/qgis_utilities/styles.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qgis_utilities/styling.py` & `jord-0.6.1/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qlive_utilities/client.py` & `jord-0.6.1/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qlive_utilities/clients/auto.py` & `jord-0.6.1/jord/qlive_utilities/clients/auto.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qlive_utilities/procedures.py` & `jord-0.6.1/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qlive_utilities/serialisation.py` & `jord-0.6.1/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qlive_utilities/uri_utilities.py` & `jord-0.6.1/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/qt_utilities/enums.py` & `jord-0.6.1/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/__init__.py` & `jord-0.6.1/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/base.py` & `jord-0.6.1/jord/shapely_utilities/base.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/clamp.py` & `jord-0.6.1/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/geometry_types.py` & `jord-0.6.1/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/grouping.py` & `jord-0.6.1/jord/shapely_utilities/grouping.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/lines.py` & `jord-0.6.1/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/mirroring.py` & `jord-0.6.1/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/morphology.py` & `jord-0.6.1/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/points.py` & `jord-0.6.1/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/polygons.py` & `jord-0.6.1/jord/shapely_utilities/polygons.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/projection.py` & `jord-0.6.1/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/rings.py` & `jord-0.6.1/jord/shapely_utilities/rings.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/selection.py` & `jord-0.6.1/jord/shapely_utilities/selection.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/jord/shapely_utilities/transformation.py` & `jord-0.6.1/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/setup.py` & `jord-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `jord-0.6.0/tests/test_import.py` & `jord-0.6.1/tests/test_import.py`

 * *Files identical despite different names*

