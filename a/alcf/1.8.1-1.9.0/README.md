# Comparing `tmp/alcf-1.8.1.tar.gz` & `tmp/alcf-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcf-1.8.1.tar", last modified: Fri Apr 26 20:22:33 2024, max compression
+gzip compressed data, was "alcf-1.9.0.tar", last modified: Fri May  3 16:29:07 2024, max compression
```

## Comparing `alcf-1.8.1.tar` & `alcf-1.9.0.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.757752 alcf-1.8.1/
--rw-r--r--   0 peter     (1000) peter     (1000)      239 2024-04-26 20:21:41.000000 alcf-1.8.1/.editorconfig
--rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-04-26 20:21:41.000000 alcf-1.8.1/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-04-26 20:21:41.000000 alcf-1.8.1/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-04-26 20:21:41.000000 alcf-1.8.1/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-26 20:22:33.757752 alcf-1.8.1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-04-26 20:21:41.000000 alcf-1.8.1/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.733752 alcf-1.8.1/alcf/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/algorithms/calibration/
--rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/calibration/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/calibration/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/algorithms/cloud_base_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/cloud_base_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      930 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/cloud_base_detection/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/algorithms/cloud_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/cloud_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1533 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/cloud_detection/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1871 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/couple.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/interp.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)      818 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/lidar_ratio.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/algorithms/noise_removal/
--rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/noise_removal/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/noise_removal/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1812 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/output_sample.py
--rw-r--r--   0 peter     (1000) peter     (1000)    11176 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1196 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/tsample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1365 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/algorithms/zsample.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/bin/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/bin/__init__.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)      319 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/bin/alcf.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      458 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4022 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/auto.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.737752 alcf-1.8.1/alcf/cmds/auto_cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/auto_cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/auto_cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2639 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/auto_cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/auto_cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/calibrate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/convert.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6399 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/download.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12355 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1430 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7307 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)    18510 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/plot.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6424 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/simulate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4947 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/cmds/stats.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.741752 alcf-1.8.1/alcf/download/
--rw-r--r--   0 peter     (1000) peter     (1000)       88 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/download/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2445 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/download/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2444 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/download/merra2.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.741752 alcf-1.8.1/alcf/fonts/
--rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/fonts/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/fonts/PublicSans-Bold.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/fonts/PublicSans-BoldItalic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/fonts/PublicSans-Italic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/fonts/PublicSans-Regular.otf
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.741752 alcf-1.8.1/alcf/lidars/
--rw-r--r--   0 peter     (1000) peter     (1000)     1426 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/blview.py
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/caliop.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1742 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/chm15k.py
--rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/cl31.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2278 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/cl51.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1865 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/cl61.py
--rw-r--r--   0 peter     (1000) peter     (1000)      985 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3545 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/mpl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2195 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/lidars/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6862 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/misc.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.741752 alcf-1.8.1/alcf/models/
--rw-r--r--   0 peter     (1000) peter     (1000)     2235 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4179 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/amps.py
--rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/cmip5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2674 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2521 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/icon.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1783 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/icon_intake_healpix.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2559 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/jra55.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1650 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/merra2.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1854 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/nzcsm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2939 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/nzesm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-26 20:21:41.000000 alcf-1.8.1/alcf/models/um.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.733752 alcf-1.8.1/alcf.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-26 20:22:33.000000 alcf-1.8.1/alcf.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     4676 2024-04-26 20:22:33.000000 alcf-1.8.1/alcf.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-26 20:22:33.000000 alcf-1.8.1/alcf.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-04-26 20:22:33.000000 alcf-1.8.1/alcf.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-26 20:22:33.000000 alcf-1.8.1/alcf.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)      204 2024-04-26 20:22:33.000000 alcf-1.8.1/alcf.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-04-26 20:22:33.000000 alcf-1.8.1/alcf.egg-info/top_level.txt
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-04-26 20:21:41.000000 alcf-1.8.1/build_doc
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.745752 alcf-1.8.1/cosp/
--rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/.editorconfig
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.745752 alcf-1.8.1/cosp/MISR_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/MISR_simulator/MISR_simulator.f
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.745752 alcf-1.8.1/cosp/MODIS_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/MODIS_simulator/modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/MODIS_simulator/test_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/Makefile.cmor1
--rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/Makefile.ibm
--rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/README.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/README_v1.4.1.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.749752 alcf-1.8.1/cosp/actsim/
--rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/actsim/lidar_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/actsim/lmd_ipsl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/actsim/mie_backscatter_1064.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/actsim/mie_backscatter_532.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/actsim/mie_backscatter_910.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.749752 alcf-1.8.1/cosp/cfmip2/
--rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_constants.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_defs.h
--rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_htfrtc.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_input_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_io.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_isccp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_lidar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_misr_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_output_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_rttov.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_rttov_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_types.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/cosp_utils.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.749752 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/
--rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/README
--rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/congvec.expected
--rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/congvec.f
--rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/icarus.f
--rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/input.data
--rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/input.data.halved
--rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
--rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/license
--rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/rcsid
--rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_congvec.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
--rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.749752 alcf-1.8.1/cosp/llnl/
--rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/llnl/cosp_radar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/llnl/llnl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/llnl/pf_to_mr.f
--rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/llnl/prec_scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/mac_info.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/predict_mom07.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.753752 alcf-1.8.1/cosp/quickbeam/
--rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/README
--rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/array_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/atmos_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/calc_Re.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/dsd.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/format_input.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/gases.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/load_hydrometeor_classes.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/load_mie_table.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/math_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/mrgrnk.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/optics_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/predict_psd07.f
--rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/radar_simulator.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/radar_simulator_init.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/radar_simulator_types.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/scale_LUTs_io.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/quickbeam/zeff.f90
--rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/replace_tabs.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/tests.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.753752 alcf-1.8.1/cosp/utils/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/utils/COSP_plots.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.8.1/cosp/utils/append_cf3hr_files.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-04-26 20:21:41.000000 alcf-1.8.1/download_cosp
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.753752 alcf-1.8.1/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     4583 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-auto.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2280 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-calibrate.1
--rw-r--r--   0 peter     (1000) peter     (1000)      811 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-compare.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2308 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-convert.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5120 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-download.1
--rw-r--r--   0 peter     (1000) peter     (1000)     7022 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-lidar.1
--rw-r--r--   0 peter     (1000) peter     (1000)     4811 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-model.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5666 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-plot.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1981 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-simulate.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3944 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1450 2024-04-26 20:21:41.000000 alcf-1.8.1/man/alcf.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-04-26 20:22:33.757752 alcf-1.8.1/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2261 2024-04-26 20:21:41.000000 alcf-1.8.1/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-26 20:22:33.753752 alcf-1.8.1/src/
--rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-04-26 20:21:41.000000 alcf-1.8.1/src/cosp_run.f03
--rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-04-26 20:21:41.000000 alcf-1.8.1/src/main.f03
--rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-04-26 20:21:41.000000 alcf-1.8.1/src/nc_utils.f03
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.198509 alcf-1.9.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      239 2024-05-03 16:23:18.000000 alcf-1.9.0/.editorconfig
+-rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-05-03 16:23:18.000000 alcf-1.9.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-05-03 16:23:18.000000 alcf-1.9.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-05-03 16:23:18.000000 alcf-1.9.0/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-05-03 16:29:07.198509 alcf-1.9.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-05-03 16:23:18.000000 alcf-1.9.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/
+-rw-r--r--   0 peter     (1000) peter     (1000)      109 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/
+-rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/calibration/
+-rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/calibration/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/calibration/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/cloud_base_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_base_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      930 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_base_detection/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/cloud_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1533 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_detection/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1871 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/couple.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/interp.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)      818 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/lidar_ratio.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/noise_removal/
+-rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/noise_removal/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/noise_removal/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1808 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/output_sample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    11260 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1192 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/tsample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1365 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/zsample.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/bin/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/bin/__init__.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      893 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/bin/alcf.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      458 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4022 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/cmds/auto_cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2639 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/calibrate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/convert.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6399 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/download.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12457 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1717 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7093 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    19067 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/plot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6987 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/simulate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4993 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/stats.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/download/
+-rw-r--r--   0 peter     (1000) peter     (1000)       88 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/download/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2445 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/download/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2444 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/download/merra2.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/fonts/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-Bold.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-BoldItalic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-Italic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-Regular.otf
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.182509 alcf-1.9.0/alcf/lidars/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1456 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2136 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/blview.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/caliop.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1697 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/chm15k.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/cl31.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2409 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/cl51.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1820 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/cl61.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3791 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/mpl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2150 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7005 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/misc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.182509 alcf-1.9.0/alcf/models/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2265 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4350 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/amps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/cmip5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2824 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2834 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/icon.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1814 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/icon_intake_healpix.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2881 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/jra55.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2213 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/merra2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1885 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/nzcsm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3063 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/nzesm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2443 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/um.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     4676 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)      204 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/top_level.txt
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-05-03 16:23:18.000000 alcf-1.9.0/build_doc
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/
+-rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/.editorconfig
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/MISR_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/MISR_simulator/MISR_simulator.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/MODIS_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/MODIS_simulator/modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/MODIS_simulator/test_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/Makefile.cmor1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/Makefile.ibm
+-rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/README.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/README_v1.4.1.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/actsim/
+-rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/lidar_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/lmd_ipsl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/mie_backscatter_1064.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/mie_backscatter_532.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/mie_backscatter_910.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.190509 alcf-1.9.0/cosp/cfmip2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_constants.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_defs.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_htfrtc.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_input_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_io.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_isccp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_lidar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_misr_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_output_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_rttov.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_rttov_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_types.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_utils.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.190509 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/README
+-rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/congvec.expected
+-rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/congvec.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/icarus.f
+-rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data
+-rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data.halved
+-rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/license
+-rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/rcsid
+-rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
+-rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.190509 alcf-1.9.0/cosp/llnl/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/cosp_radar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/llnl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/pf_to_mr.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/prec_scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/mac_info.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/predict_mom07.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.194509 alcf-1.9.0/cosp/quickbeam/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/README
+-rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/array_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/atmos_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/calc_Re.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/dsd.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/format_input.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/gases.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/load_hydrometeor_classes.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/load_mie_table.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/math_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/mrgrnk.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/optics_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/predict_psd07.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/radar_simulator.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/radar_simulator_init.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/radar_simulator_types.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/scale_LUTs_io.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/zeff.f90
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/replace_tabs.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/tests.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.194509 alcf-1.9.0/cosp/utils/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/utils/COSP_plots.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/utils/append_cf3hr_files.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-05-03 16:23:18.000000 alcf-1.9.0/download_cosp
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.194509 alcf-1.9.0/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4583 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-auto.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2280 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-calibrate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      811 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-compare.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2308 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-convert.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5120 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-download.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7022 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-lidar.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     4811 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-model.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5666 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-plot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1981 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-simulate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3944 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1450 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-05-03 16:29:07.198509 alcf-1.9.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2261 2024-05-03 16:23:18.000000 alcf-1.9.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.198509 alcf-1.9.0/src/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-05-03 16:23:18.000000 alcf-1.9.0/src/cosp_run.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-05-03 16:23:18.000000 alcf-1.9.0/src/main.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-05-03 16:23:18.000000 alcf-1.9.0/src/nc_utils.f03
```

### Comparing `alcf-1.8.1/LICENSE.md` & `alcf-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/Makefile` & `alcf-1.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/PKG-INFO` & `alcf-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.8.1
+Version: 1.9.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.8.1/README.md` & `alcf-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/algorithms/cloud_base_detection/default.py` & `alcf-1.9.0/alcf/algorithms/cloud_base_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/algorithms/cloud_detection/default.py` & `alcf-1.9.0/alcf/algorithms/cloud_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/algorithms/couple.py` & `alcf-1.9.0/alcf/algorithms/couple.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/algorithms/interp.pyx` & `alcf-1.9.0/alcf/algorithms/interp.pyx`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/algorithms/lidar_ratio.py` & `alcf-1.9.0/alcf/algorithms/lidar_ratio.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/algorithms/noise_removal/default.py` & `alcf-1.9.0/alcf/algorithms/noise_removal/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/algorithms/output_sample.py` & `alcf-1.9.0/alcf/algorithms/output_sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	n2 = int(output_sampling/tres)
 	time = d['time']
 	time_bnds = d['time_bnds']
 
 	time_half2 = np.linspace(t1, t2, n2 + 1)
 	time2 = 0.5*(time_half2[1:] + time_half2[:-1])
 
-	for var in ds.get_vars(d):
+	for var in ds.vars(d):
 		if 'time' not in d['.'][var]['.dims']:
 			continue
 		i = d['.'][var]['.dims'].index('time')
 		x = d[var]
 		size = x.shape
 		size2 = list(size)
 		size2[i] = n2
```

### Comparing `alcf-1.8.1/alcf/algorithms/stats.py` & `alcf-1.9.0/alcf/algorithms/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,28 +249,32 @@
 		state['backscatter_mol_avg'] += interp(
 			zhalf,
 			backscatter_mol_avg_tmp,
 			zhalf2
 		)
 
 def stats_reduce(state, bsd_z=None, **kwargs):
+	if not 'n' in state:
+		return {}
 	if len(state['cl'].shape) == 2:
 		for k in range(len(state['n'])):
+			if state['clt'][k] > 0:
+				state['cbh'][:,k] /= state['clt'][k]
 			if state['n'][k] > 0:
 				state['backscatter_hist'][:,:,k] /= state['n'][k]
 				state['cl'][:,k] /= state['n'][k]
-				state['cbh'][:,k] /= state['clt'][k]
 				state['clt'][k] /= state['n'][k]
 				state['backscatter_avg'][:,k] /= state['n'][k]
 				state['backscatter_mol_avg'][:,k] /= state['n'][k]
 	else:
+		if state['clt'] > 0:
+			state['cbh'] /= state['clt']
 		if state['n'] != 0:
 			state['backscatter_hist'] /= state['n']
 			state['cl'] /= state['n']
-			state['cbh'] /= state['clt']
 			state['clt'] /= state['n']
 			state['backscatter_avg'] /= state['n']
 			state['backscatter_mol_avg'] /= state['n']
 	state['backscatter_sd_hist'] /= state['n']
 	do = {
 		'cl': 100.*state['cl'],
 		'cbh': 100.*state['cbh'],
```

### Comparing `alcf-1.8.1/alcf/algorithms/tsample.py` & `alcf-1.9.0/alcf/algorithms/tsample.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		shape1 = list(d['backscatter_sd'].shape[1:])
 		d['backscatter_sd'] = np.sqrt(1./n*np.average(
 			d['backscatter_sd']**2,
 			axis=0,
 			weights=w,
 		))
 		d['backscatter_sd'] = d['backscatter_sd'].reshape([1] + shape1)
-	for var in ds.get_vars(d):
+	for var in ds.vars(d):
 		if var in ('time', 'time_bnds', 'backscatter_sd'):
 			continue
 		if 'time' not in d['.'][var]['.dims']:
 			continue
 		i = d['.'][var]['.dims'].index('time')
 		shape = list(d[var].shape)
 		d[var] = np.average(d[var], axis=i, weights=w)
```

### Comparing `alcf-1.8.1/alcf/algorithms/zsample.py` & `alcf-1.9.0/alcf/algorithms/zsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/auto.py` & `alcf-1.9.0/alcf/cmds/auto.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/auto_cmds/compare.py` & `alcf-1.9.0/alcf/cmds/auto_cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/auto_cmds/lidar.py` & `alcf-1.9.0/alcf/cmds/auto_cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/auto_cmds/model.py` & `alcf-1.9.0/alcf/cmds/auto_cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/calibrate.py` & `alcf-1.9.0/alcf/cmds/calibrate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/compare.py` & `alcf-1.9.0/alcf/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/convert.py` & `alcf-1.9.0/alcf/cmds/convert.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/download.py` & `alcf-1.9.0/alcf/cmds/download.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/cmds/lidar.py` & `alcf-1.9.0/alcf/cmds/lidar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-import logging
 import traceback
 import glob
+from warnings import warn
 import numpy as np
 import ds_format as ds
 import aquarius_time as aq
 from alcf.lidars import LIDARS
 from alcf.algorithms.calibration import CALIBRATION
 from alcf.algorithms.noise_removal import NOISE_REMOVAL
 from alcf.algorithms.cloud_detection import CLOUD_DETECTION
@@ -49,14 +49,15 @@
 	fix_cl_range=False,
 	cl_crit_range=6000,
 	lat=None,
 	lon=None,
 	r=False,
 	keep_vars=[],
 	align_output=True,
+	debug=False,
 	**options
 ):
 	"""
 alcf-lidar -- Process lidar data.
 ==========
 
 Synopsis
@@ -330,16 +331,17 @@
 				)
 				if d is None: continue
 				dd = process([d], state, **options)
 			except SystemExit:
 				raise
 			except SystemError:
 				raise
-			except:
-				logging.warning(traceback.format_exc())
+			except Exception as e:
+				if debug: warn('%s: %s' % (file_, traceback.format_exc()))
+				else: warn('%s: %s' % (file_, str(e)))
 		dd = process([None], state, **options)
 	else:
 		print('<- %s' % input_)
 		d = lidar.read(input_, VARIABLES,
 			altitude=altitude,
 			lon=lon,
 			lat=lat,
```

### Comparing `alcf-1.8.1/alcf/cmds/main.py` & `alcf-1.9.0/alcf/cmds/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import sys
 import re
+from alcf import __version__
 from alcf.cmds import CMDS
 
 def md_to_text(md):
 	text = md.strip()
 	text += '\n\nBug reporting\n-------------\n\nReport bugs to Peter Kuma (peter@peterkuma.net).\n'
 	return text
 
 def run(cmd=None, *args, **kwargs):
 	'''alcf -- Tool for processing of automatic lidar and ceilometer (ALC) data and intercomparison with atmospheric models.
 ====
 
 Synopsis
 --------
 
-    alcf <cmd> [<options>]
-    alcf <cmd> --help
+    alcf <cmd> [<options>] [<arguments>]
+    alcf [<cmd>] --help
+    alcf --version
 
 Arguments
 ---------
 
 - `cmd`: See Commands below.
-- `options`: Command options.
+- `arguments`: Command arguments. Use `alcf <cmd> --help` for more information.
+- `options`: Command options (see Options below).
 
 Commands
 --------
 
 - `auto`: Peform automatic processing of model or lidar data.
 - `calibrate`: Calibrate lidar backscatter.
 - `convert`: Convert input instrument or model data to the ALCF standard NetCDF.
@@ -35,17 +38,21 @@
 - `plot`: Plot lidar data.
 - `simulate`: Simulate lidar measurements from model data using COSP.
 - `stats`: Calculate cloud occurrence statistics.
 
 Options
 -------
 
-- `--help`: Print help for command.
 - `--debug`: Enable debugging information.
+- `--help`: Print general help or help for a command and exit.
+- `--version`: Print version and exit.
 '''
+	if 'version' in kwargs:
+		print(__version__)
+		return 0
 
 	if cmd is None:
 		sys.stderr.write(md_to_text(run.__doc__))
 		return 1
 
 	func = CMDS.get(cmd)
 	if func is None:
```

### Comparing `alcf-1.8.1/alcf/cmds/model.py` & `alcf-1.9.0/alcf/cmds/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 import sys
 import os
 import traceback
+from warnings import warn
 from concurrent.futures import ProcessPoolExecutor, as_completed
 import numpy as np
 import aquarius_time as aq
 import ds_format as ds
 from alcf.models import MODELS, META
 from alcf import misc
 
+REQ_VARS = [
+	'cl',
+	'cli',
+	'clw',
+	'lat',
+	'lon',
+	'orog',
+	'pfull',
+	'ps',
+	'ta',
+	'time',
+	'zfull',
+]
+
 def override_year_in_time(time, year):
 	try: len(time)
 	except:	return override_year_in_time(np.array([time]), year)[0]
 	date = aq.to_date(time)
 	y = date[1]
 	n = len(y)
 	if np.all(y == year):
@@ -46,32 +61,31 @@
 		warnings = []
 		d = model.read(input_, index, track_f, t1, t2,
 			warnings=warnings,
 			recursive=r,
 		)
 		for w in warnings:
 			if len(w) == 2:
-				print('Warning: %s' % w[0], file=sys.stderr)
-				if debug: print(w[1], file=sys.stderr)
-				else: print('Use --debug to print debugging information.', file=sys.stderr)
+				if debug: warn('%s\n%s' % (w[0], w[1]))
+				else: warn(w[0])
 			else:
-				print('Warning: %s' % w, file=sys.stderr)
-		if d is not None:
+				warn(w)
+		if d is not None and len(ds.vars(d)) > 0:
+			misc.require_vars(d, REQ_VARS)
 			if 'time_bnds' not in d and 'time' in d:
 				d['time_bnds'] = misc.time_bnds(d['time'], model.STEP, t1, t2)
 			for var in ['time', 'time_bnds']:
 				if 'time' in d:
 					d[var] = start + (d[var] - t1)
 			d['.'] = META
 			ds.write(output_filename, d)
 			print('-> %s' % output_filename)
 	except Exception as e:
-		print('Warning: %s' % str(e), file=sys.stderr)
-		if debug: print(traceback.format_exc(), file=sys.stderr)
-		else: print('Use --debug to print debugging information.', file=sys.stderr)
+		if debug: warn(traceback.format_exc())
+		else: warn(str(e))
 
 def run(type_, input_, output,
 	point=None,
 	time=None,
 	track=None,
 	track_gap=21600,
 	override_year=None,
@@ -173,12 +187,11 @@
 			if not misc.track_has_seg(d_track, t, t + 1):
 				continue
 			f = ex.submit(worker, type_, input_, index, output, d_track, t,
 				debug, r, override_year)
 			fs += [f]
 	for w in warnings:
 		if len(w) == 2:
-			print('Warning: %s' % w[0], file=sys.stderr)
-			if debug: print(w[1], file=sys.stderr)
-			else: print('Use --debug to print debugging information.', file=sys.stderr)
+			if debug: warn('%s\n%s' % (w[0], w[1]))
+			else: warn(w[0])
 		else:
-			print('Warning: %s' % w, file=sys.stderr)
+			warn(w)
```

### Comparing `alcf-1.8.1/alcf/cmds/plot.py` & `alcf-1.9.0/alcf/cmds/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
-import logging
+from warnings import warn
 import traceback
 import copy
 import numpy as np
 import datetime as dt
 import matplotlib as mpl
 mpl.use('Agg')
 import matplotlib.pyplot as plt
@@ -77,15 +77,16 @@
 	vlog=None,
 	zres=50,
 	zlim=None,
 	render='antialiased',
 	**opts
 ):
 	if plot_type == 'backscatter':
-		cmap = copy.copy(mpl.cm.get_cmap('viridis'))
+		misc.require_vars(d, ['time', 'zfull', 'backscatter', 'cloud_mask'])
+		cmap = copy.copy(mpl.colormaps.get_cmap('viridis'))
 		under = '#222222'
 		label = 'Att. vol. backscattering coef. (×10$^{-6}$ m$^{-1}$sr$^{-1}$)'
 		if vlim is None:
 			vlim = [0.1, 200]
 		if vlog is None:
 			vlog = True
 		if len(d['backscatter'].shape) == 3:
@@ -104,14 +105,15 @@
 			bmol = d['backscatter_mol']
 			mask = ~np.isnan(bmol)
 			b[mask] -= bmol[mask]
 		x = b*1e6
 		x[x <= 0.] = 0.5*vlim[0] # A value below the limit.
 		zfull = d['zfull']
 	elif plot_type in ('clw', 'cli', 'cl'):
+		misc.require_vars(d, ['time', 'zfull', plot_type])
 		cmap = copy.copy(mpl.cm.get_cmap({
 			'clw': 'Reds',
 			'cli': 'Blues',
 			'cl': 'Greys_r',
 		}[plot_type]))
 		under = {
 			'clw': 'white',
@@ -230,14 +232,15 @@
 			theme='dark'
 		)
 
 	if 'altitude' in d:
 		plt.plot(date2num(time_dt), d['altitude']*1e-3, color='red', lw=0.5)
 
 def plot_lr(d, subcolumn=0, **opts):
+	misc.require_vars(d, ['time', 'lr'])
 	lr = d['lr'][:,subcolumn] if d['lr'].ndim == 2 else d['lr'][:]
 	plt.plot(d['time'], lr, lw=0.7, color='#0087ed')
 	locator = AutoDateLocator()
 	plt.gca().xaxis.set_major_locator(locator)
 	plt.grid(lw=0.1, color='black')
 	def f(x, pos):
 		return aq.to_datetime(x).strftime('%d/%m\n%H:%M')
@@ -259,20 +262,22 @@
 	**kwargs
 ):
 	var = {
 		'cbh': 'cbh',
 		'cloud_occurrence': 'cl',
 	}[plot_type]
 	for i, d in enumerate(dd):
+		misc.require_vars(d, ['zfull'])
 		zfull = d['zfull']
 		x = d[var][:,subcolumn] \
 			if len(d[var].shape) == 2 \
 			else d[var]
 		label = (labels[i] if labels is not None else '')
 		if plot_type == 'cloud_occurrence':
+			misc.require_vars(d, ['clt'])
 			clt = d['clt'][subcolumn] \
 				if len(d['clt'].shape) == 1 \
 				else d['clt']
 			label += ' | CF: %d%%' % clt
 		plt.plot(x, 1e-3*zfull,
 			color=colors[i],
 			linestyle=(linestyle[i] if type(linestyle) is list else linestyle),
@@ -294,14 +299,16 @@
 	subcolumn=0,
 	xlim=None,
 	zlim=None,
 	vlim=None,
 	vlog=False,
 	**kwargs
 ):
+	misc.require_vars(d, ['backscatter_hist', 'backscatter_full', 'zfull'])
+
 	if vlim is None:
 		vlim = [
 			np.min(d['backscatter_hist'])*1e2,
 			np.max(d['backscatter_hist'])*1e2
 		]
 
 	if vlog is False:
@@ -313,15 +320,15 @@
 	if xlim is None:
 		xlim = [
 			(1.5*d['backscatter_full'][0] - 0.5*d['backscatter_full'][1])*1e6,
 			(1.5*d['backscatter_full'][-1] - 0.5*d['backscatter_full'][-2])*1e6,
 		]
 
 	under = '#222222'
-	cmap = copy.copy(mpl.cm.get_cmap('viridis'))
+	cmap = copy.copy(mpl.colormaps.get_cmap('viridis'))
 	cmap.set_under(under)
 	im = plt.imshow(
 		d['backscatter_hist'].T*1e2
 			if len(d['backscatter_hist'].shape) == 2
 			else d['backscatter_hist'][:,:,subcolumn].T*1e2,
 		origin='lower',
 		aspect='auto',
@@ -356,14 +363,15 @@
 	xlim=None,
 	zlim=None,
 	colors=COLORS,
 	linestyle=LINESTYLE,
 	**kwargs
 ):
 	for i, d in enumerate(dd):
+		misc.require_vars(d, ['backscatter_sd_full', 'backscatter_sd_hist'])
 		plt.plot(d['backscatter_sd_full']*1e6, d['backscatter_sd_hist'],
 			lw=1,
 			color=colors[i],
 			linestyle=(linestyle[i] if type(linestyle) is list else linestyle),
 			label=(labels[i] if labels is not None else None),
 		)
 	plt.gca().set_yscale('log')
@@ -640,25 +648,27 @@
 					try:
 						print('<- %s' % filename)
 						d = ds.read(filename, VARIABLES)
 					except SystemExit:
 						raise
 					except SystemError:
 						raise
-					except:
-						logging.warning(traceback.format_exc())
+					except Exception as e:
+						if debug: warn('%s: %s' % (file_, traceback.format_exc()))
+						else: warn('%s: %s' % (file_, str(e)))
 					try:
 						plot(plot_type, d, output_filename, **opts)
 						print('-> %s' % output_filename)
 					except SystemExit:
 						raise
 					except SystemError:
 						sys.exit(1)
-					except:
-						logging.warning(traceback.format_exc())
+					except Exception as e:
+						if debug: warn('%s: %s' % (file_, traceback.format_exc()))
+						else: warn('%s: %s' % (file_, str(e)))
 					finally:
 						plt.close()
 			else:
 				print('<- %s' % input1)
 				d = ds.read(input1, VARIABLES)
 				try:
 					plot(plot_type, d, output, **opts)
```

### Comparing `alcf-1.8.1/alcf/cmds/simulate.py` & `alcf-1.9.0/alcf/cmds/simulate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 import os
 import copy
 import tempfile
+from warnings import warn
 from string import Template
 import subprocess
+import ds_format as ds
+import alcf
+from alcf import misc
 from alcf.lidars import LIDARS
 
+VARS = [
+	'lon',
+	'lat',
+	'time',
+	'time_bnds',
+	'ps',
+	'orog',
+	'zfull',
+	'ta',
+	'pfull',
+	'clw',
+	'cli',
+	'cl',
+]
+
 CONFIG_TEMPLATE = """
 &config_nml
 	config%NPOINTS_IT=500,
 	config%NCOLUMNS=${ncolumns},
 	config%NLEVELS=${nlevels},
 	config%USE_VGRID=.true.,
 	config%NLR=40,
@@ -132,14 +151,15 @@
 		subprocess.call([program, config_filename, input_, output])
 	finally:
 		os.unlink(config_filename)
 
 def run(type_, input_, output,
 	ncolumns=10,
 	overlap='maximum-random',
+	debug=False,
 	**kwargs
 ):
 	'''
 alcf-simulate -- Simulate lidar measurements from model data using COSP.
 =============
 
 Synopsis
@@ -210,9 +230,20 @@
 		files = sorted(os.listdir(input_))
 		for file_ in files:
 			input_filename = os.path.join(input_, file_)
 			output_filename = os.path.join(output, file_)
 			if not os.path.isfile(input_filename):
 				continue
 			print('<- %s' % input_filename)
+			try:
+				d = ds.read(input_filename, VARS)
+				misc.require_vars(d, VARS)
+			except Exception as e:
+				if debug: warn('%s: %s' % (file_, traceback.format_exc()))
+				else: warn('%s: %s' % (file_, str(e)))
+				continue
 			cosp_alcf(config, input_filename, output_filename)
+			print('<- %s' % output_filename)
+			d = ds.read(output_filename)
+			d['.']['.'] = alcf.META
+			ds.write(output_filename, d)
 			print('-> %s' % output_filename)
```

### Comparing `alcf-1.8.1/alcf/cmds/stats.py` & `alcf-1.9.0/alcf/cmds/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import numpy as np
 import ds_format as ds
+import alcf
 from alcf.algorithms import interp
 from alcf.algorithms import stats
 from alcf.misc import parse_time
 
 VARIABLES = [
 	'cloud_mask',
 	'cbh',
@@ -127,8 +128,9 @@
 			dd = stats.stream([d], state, **options)
 	else:
 		d = ds.read(input_, VARIABLES)
 		print('<- %s' % input_)
 		dd = stats.stream([d], state, **options)
 	dd = stats.stream([None], state, **options)
 	print('-> %s' % output)
+	ds.attrs(dd[0], None, alcf.META)
 	ds.write(output, dd[0])
```

### Comparing `alcf-1.8.1/alcf/download/era5.py` & `alcf-1.9.0/alcf/download/era5.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/download/merra2.py` & `alcf-1.9.0/alcf/download/merra2.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/fonts/LICENSE.md` & `alcf-1.9.0/alcf/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/fonts/PublicSans-Bold.otf` & `alcf-1.9.0/alcf/fonts/PublicSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/fonts/PublicSans-BoldItalic.otf` & `alcf-1.9.0/alcf/fonts/PublicSans-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/fonts/PublicSans-Italic.otf` & `alcf-1.9.0/alcf/fonts/PublicSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/fonts/PublicSans-Regular.otf` & `alcf-1.9.0/alcf/fonts/PublicSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/alcf/lidars/__init__.py` & `alcf-1.9.0/alcf/lidars/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import alcf
+
 META = {
 	'time': {
 		'.dims': ['time'],
 		'long_name': 'time',
 		'standard_name': 'time',
 		'units': 'days since -4713-11-24 12:00 UTC',
 		'calendar': 'proleptic_gregorian',
@@ -38,14 +40,15 @@
 	},
 	'lat': {
 		'.dims': ['time'],
 		'long_name': 'instrument latitude',
 		'standard_name': 'latitude',
 		'units': 'degrees_north',
 	},
+	'.': alcf.META,
 }
 
 from . import chm15k
 from . import cl61
 from . import blview
 from . import cl51
 from . import cl31
```

### Comparing `alcf-1.8.1/alcf/lidars/blview.py` & `alcf-1.9.0/alcf/lidars/blview.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,38 +26,37 @@
 	lon=None,
 	lat=None,
 	tlim=None,
 	keep_vars=[],
 	**kwargs
 ):
 	sel = None
-	tres = None
 	if tlim is not None:
 		d = ds.read(filename, 'time')
+		misc.require_vars(d, ['time'])
 		d['time'] = d['time']/86400. + 2440587.5
-		tres = d['time'][1] - d['time'][0]
-		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		d['time_bnds'] = misc.time_bnds(d['time'])
 		mask = misc.time_mask(d['time_bnds'], tlim[0], tlim[1])
 		if np.sum(mask) == 0: return None
 		sel = { 'timeDim': mask }
 
 	dep_vars = misc.dep_vars(VARS, vars)
 	req_vars = dep_vars + DEFAULT_VARS + keep_vars
 	d = ds.read(filename, req_vars, sel=sel, full=True)
+	misc.require_vars(d, req_vars)
 	dx = {}
 	misc.populate_meta(dx, META, set(vars) & set(VARS))
 	n = ds.dim(d, 'timeDim')
 	m = ds.dim(d, 'range')
 	d['time'] = d['time']/86400. + 2440587.5
 	if 'time' in vars:
 		dx['time'] = d['time']
 	if 'time_bnds' in vars:
-		if tres is None: tres = d['time'][1] - d['time'][0]
 		args = [] if tlim is None else [tlim[0], tlim[1]]
-		dx['time_bnds'] = misc.time_bnds(d['time'], tres, *args)
+		dx['time_bnds'] = misc.time_bnds(d['time'], None, *args)
 	if 'altitude' in vars:
 		dx['altitude'] = d['altitude'][:,0].astype(np.float64).filled(np.nan)
 	if 'zfull' in vars:
 		range_ = d['range'].astype(np.float64).filled(np.nan)
 		dx['zfull'] = np.tile(range_, (n, 1))
 		dx['zfull'] = (dx['zfull'].T + dx['altitude']).T
 	if 'lon' in vars:
```

### Comparing `alcf-1.8.1/alcf/lidars/chm15k.py` & `alcf-1.9.0/alcf/lidars/chm15k.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,38 +26,37 @@
 	lon=None,
 	lat=None,
 	tlim=None,
 	keep_vars=[],
 	**kwargs
 ):
 	sel = None
-	tres = None
 	if tlim is not None:
 		d = ds.read(filename, 'time', jd=True)
-		tres = d['time'][1] - d['time'][0]
-		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		misc.require_vars(d, ['time'])
+		d['time_bnds'] = misc.time_bnds(d['time'])
 		mask = misc.time_mask(d['time_bnds'], tlim[0], tlim[1])
 		if np.sum(mask) == 0: return None
 		sel = {'time': mask}
 
 	dep_vars = misc.dep_vars(VARS, vars)
 	req_vars = dep_vars + DEFAULT_VARS + keep_vars
 	d = ds.read(filename, req_vars, jd=True, sel=sel, full=True)
+	misc.require_vars(d, req_vars)
 	dx = {}
 	misc.populate_meta(dx, META, set(vars) & set(VARS))
 	n = ds.dim(d, 'time')
 	m = ds.dim(d, 'range')
 	if altitude is None:
 		altitude = d['altitude']
 	if 'time' in vars:
 		dx['time'] = d['time']
 	if 'time_bnds' in vars:
-		if tres is None: tres = d['time'][1] - d['time'][0]
 		args = [] if tlim is None else [tlim[0], tlim[1]]
-		dx['time_bnds'] = misc.time_bnds(d['time'], tres, *args)
+		dx['time_bnds'] = misc.time_bnds(d['time'], None, *args)
 	if 'backscatter' in vars:
 		dx['backscatter'] = d['beta_raw']*1e-11*CALIBRATION_COEFF
 	if 'zfull' in vars:
 		zfull1 = d['range'] + altitude
 		dx['zfull'] = np.tile(zfull1, (n, 1))
 	if 'altitude' in vars:
 		dx['altitude'] = np.full(n, altitude, np.float64)
```

### Comparing `alcf-1.8.1/alcf/lidars/cl51.py` & `alcf-1.9.0/alcf/lidars/cl51.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,59 +10,64 @@
 SC_LR = 18.8 # sr. Stratocumulus lidar ratio (O'Connor et al., 2004).
 MAX_RANGE = 15400 # m
 
 VARS = {
 	'backscatter': ['backscatter'],
 }
 
-DEFAULT_VARS = [
-	'vertical_resolution',
-	'level',
-	'range',
+DEFAULT_VARS1 = [
 	'time',
 	'detection_status',
 ]
 
+DEFAULT_VARS2 = [
+	'vertical_resolution',
+	'range',
+	'level',
+]
+
 def read(filename, vars,
 	altitude=None,
 	lon=None,
 	lat=None,
 	calibration_coeff=CALIBRATION_COEFF,
 	fix_cl_range=False,
 	cl_crit_range=6000,
 	tlim=None,
 	keep_vars=[],
 	**kwargs
 ):
 	sel = None
-	tres = None
 	if tlim is not None:
 		d = ds.read(filename, 'time', jd=True)
-		tres = d['time'][1] - d['time'][0]
-		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		misc.require_vars(d, ['time'])
+		d['time_bnds'] = misc.time_bnds(d['time'])
 		mask = misc.time_mask(d['time_bnds'], tlim[0], tlim[1])
 		if np.sum(mask) == 0: return None
 		sel = {'time': mask}
 
 	dep_vars = misc.dep_vars(VARS, vars)
-	req_vars = dep_vars + DEFAULT_VARS + keep_vars
-	d = ds.read(filename, req_vars, jd=True, sel=sel, full=True)
+	req_vars = dep_vars + DEFAULT_VARS1 + keep_vars
+	vars_ = req_vars + DEFAULT_VARS2
+	d = ds.read(filename, vars_, jd=True, sel=sel, full=True)
+	misc.require_vars(d, req_vars)
 	dx = {}
 	misc.populate_meta(dx, META, set(vars) & set(VARS))
 	n = ds.dim(d, 'time')
 	if 'time' in vars:
 		dx['time'] = d['time']
 	if 'time_bnds' in vars:
-		if tres is None: tres = d['time'][1] - d['time'][0]
 		args = [] if tlim is None else [tlim[0], tlim[1]]
-		dx['time_bnds'] = misc.time_bnds(d['time'], tres, *args)
+		dx['time_bnds'] = misc.time_bnds(d['time'], None, *args)
 	if 'range' in d: # ARM CL51 format.
 		range_ = d['range']
-	else: # Generic CL51 format.
+	elif 'vertical_resolution' in d: # Generic CL51 format.
 		range_ = d['vertical_resolution'][0]*d['level']
+	else:
+		raise ValueError('Variable "range" or "level" and "vertical_resolution" is required')
 	if 'zfull' in vars:
 		zfull1 = range_
 		dx['zfull'] = np.tile(zfull1, (n, 1))
 		if altitude is not None:
 			dx['zfull'] += altitude
 	if 'backscatter' in vars:
 		factor = 1e-4 if (d['.']['backscatter']['units'] == '1/(sr*km*10000)') \
```

### Comparing `alcf-1.8.1/alcf/lidars/cl61.py` & `alcf-1.9.0/alcf/lidars/cl61.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,36 +26,35 @@
 	lon=None,
 	lat=None,
 	tlim=None,
 	keep_vars=[],
 	**kwargs
 ):
 	sel = None
-	tres = None
 	if tlim is not None:
 		d = ds.read(filename, 'time', jd=True)
-		tres = d['time'][1] - d['time'][0]
-		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		misc.require_vars(d, ['time'])
+		d['time_bnds'] = misc.time_bnds(d['time'])
 		mask = misc.time_mask(d['time_bnds'], tlim[0], tlim[1])
 		if np.sum(mask) == 0: return None
 		sel = {'time': mask}
 
 	dep_vars = misc.dep_vars(VARS, vars)
 	req_vars = dep_vars + DEFAULT_VARS + keep_vars
 	d = ds.read(filename, req_vars, sel=sel, full=True)
+	misc.require_vars(d, req_vars)
 	dx = {}
 	misc.populate_meta(dx, META, set(vars) & set(VARS))
 	n = ds.dim(d, 'profile')
 	d['time'] = d['time']/86400. + 2440587.5
 	if 'time' in vars:
 		dx['time'] = d['time']
 	if 'time_bnds' in vars:
-		if tres is None: tres = d['time'][1] - d['time'][0]
 		args = [] if tlim is None else [tlim[0], tlim[1]]
-		dx['time_bnds'] = misc.time_bnds(d['time'], tres, *args)
+		dx['time_bnds'] = misc.time_bnds(d['time'], None, *args)
 	if 'altitude' in vars:
 		if d['elevation'].ndim == 0:
 			dx['altitude'] = np.full(n, d['elevation'], np.float64)
 		else:
 			dx['altitude'] = d['elevation']
 	if 'zfull' in vars:
 		dx['zfull'] = np.tile(d['range'], (n, 1))
```

### Comparing `alcf-1.8.1/alcf/lidars/default.py` & `alcf-1.9.0/alcf/lidars/default.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,33 +4,38 @@
 from alcf.lidars import META
 
 WAVELENGTH = 1064 # nm
 CALIBRATION_COEFF = 1.0
 SURFACE_LIDAR = None
 SC_LR = None
 
-def read(filename, vars, altitude=None, lon=None, lat=None, time=None, **kwargs):
+def read(filename, vars,
+	altitude=None,
+	lon=None,
+	lat=None,
+	time=None,
+	keep_vars=[],
+	**kwargs
+):
 	sel = None
 	if time is not None:
 		d = ds.read(filename, 'time_bnds', jd=True)
 		mask = misc.time_mask(d['time_bnds'], time[0], time[1])
 		if np.sum(mask) == 0: return None
 		sel = {'time': mask}
 
 	d = ds.read(filename, vars, sel=sel)
 	n = d['backscatter'].shape[0]
-	d['altitude'] = d['altitude'] if altitude is None and 'altitude' in d else \
-		np.full(n, altitude, np.float64)
-	d['lon'] = d['lon'] if lon is None and 'lon' in d else \
-		np.full(n, lon, np.float64)
-	d['lat'] = d['lat'] if lat is None and 'lat' in d else \
-		np.full(n, lat, np.float64)
-	d['.']['altitude'] = META['altitude']
-	d['.']['lon'] = META['lon']
-	d['.']['lat'] = META['lat']
-	d['.'] = {
-		x: d['.'][x]
-		for x in vars
-		if x in d['.']
-	}
+	if 'altitude' in vars:
+		d['altitude'] = d['altitude'] \
+			if altitude is None and 'altitude' in d \
+			else np.full(n, altitude, np.float64)
+		d['.']['altitude'] = META['altitude']
+	if 'lon' in vars:
+		d['lon'] = d['lon'] if lon is None and 'lon' in d else \
+			np.full(n, lon, np.float64)
+		d['.']['lon'] = META['lon']
+	if 'lat' in vars:
+		d['lat'] = d['lat'] if lat is None and 'lat' in d else \
+			np.full(n, lat, np.float64)
+		d['.']['lat'] = META['lat']
 	return d
-
```

### Comparing `alcf-1.8.1/alcf/lidars/mpl.py` & `alcf-1.9.0/alcf/lidars/mpl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import ds_format as ds
 import datetime as dt
+import warnings
 from alcf import misc
 from alcf.lidars import META
 
 WAVELENGTH = 532 # nm
 CALIBRATION_COEFF = 0.375e-5
 SURFACE_LIDAR = True
 SC_LR = 16.0 # sr
@@ -76,22 +77,26 @@
 	keep_vars=[],
 	**kwargs
 ):
 	sel = None
 	tres = None
 	if tlim is not None:
 		d = ds.read(filename, TIME_VARS)
+		misc.require_vars(d, ['time'])
 		d['time'], d['time_bnds'], tres = convert_time(d)
 		mask = misc.time_mask(d['time_bnds'], tlim[0], tlim[1])
 		if np.sum(mask) == 0: return None
 		sel = {'time': mask}
 
 	dep_vars = misc.dep_vars(VARS, vars)
 	req_vars = dep_vars + DEFAULT_VARS + keep_vars
-	d = ds.read(filename, req_vars, sel=sel, full=True)
+	with warnings.catch_warnings():
+		warnings.filterwarnings('ignore', message='WARNING: valid_range not used since it\ncannot be safely cast to variable data type')
+		d = ds.read(filename, req_vars, sel=sel, full=True)
+	misc.require_vars(d, req_vars)
 	dx = {}
 	misc.populate_meta(dx, META, set(vars) & set(VARS))
 	n = ds.dim(d, 'time')
 	altitude = d['altitude'] if altitude is None else \
 		np.full(n, altitude, np.float64)
 	lon = d['longitude'] if lon is None else \
 		np.full(n, lon, np.float64)
```

### Comparing `alcf-1.8.1/alcf/lidars/mpl2nc.py` & `alcf-1.9.0/alcf/lidars/mpl2nc.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,43 +30,42 @@
 	lon=None,
 	lat=None,
 	tlim=None,
 	keep_vars=[],
 	**kwargs
 ):
 	sel = None
-	tres = None
 	if tlim is not None:
 		d = ds.read(filename, 'time', jd=True)
-		tres = d['time'][1] - d['time'][0]
-		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		misc.require_vars(d, ['time'])
+		d['time_bnds'] = misc.time_bnds(d['time'])
 		mask = misc.time_mask(d['time_bnds'], tlim[0], tlim[1])
 		if np.sum(mask) == 0: return None
 		sel = {'profile': mask}
 
 	dep_vars = misc.dep_vars(VARS, vars)
 	req_vars = dep_vars + DEFAULT_VARS + keep_vars
 	d = ds.read(filename, req_vars, jd=True, sel=sel, full=True)
+	misc.require_vars(d, req_vars)
 	mask = d['elevation_angle'] == 0.0
 	dx = {}
 	misc.populate_meta(dx, META, set(vars) & set(VARS))
 	n = ds.dim(d, 'profile')
 	m = ds.dim(d, 'range')
 	altitude = d['gps_altitude'] if altitude is None else \
 		np.full(n, altitude, np.float64)
 	lon = d['gps_longitude'] if lon is None else \
 		np.full(n, lon, np.float64)
 	lat = d['gps_latitude'] if lat is None else \
 		np.full(n, lat, np.float64)
 	if 'time' in vars:
 		dx['time'] = d['time']
 	if 'time_bnds' in vars:
-		if tres is None: tres = d['time'][1] - d['time'][0]
 		args = [] if tlim is None else [tlim[0], tlim[1]]
-		dx['time_bnds'] = misc.time_bnds(d['time'], tres, *args)
+		dx['time_bnds'] = misc.time_bnds(d['time'], None, *args)
 	if 'zfull' in vars:
 		dx['zfull'] = np.full((n, m), np.nan, np.float64)
 		for i in range(n):
 			range_ = 0.5*d['bin_time'][i]*d['c']*(np.arange(m) + 0.5)
 			dx['zfull'][i,:] = range_*np.sin(d['elevation_angle'][i]/180.0*np.pi)
 			dx['zfull'][i,:] += altitude[i]
 	if 'backscatter' in vars:
```

### Comparing `alcf-1.8.1/alcf/misc.py` & `alcf-1.9.0/alcf/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,20 @@
 def half(xfull):
 	xhalf = np.zeros(len(xfull) + 1, dtype=xfull.dtype)
 	xhalf[1:-1] = 0.5*(xfull[1:] + xfull[:-1])
 	xhalf[0] = 2.*xfull[0] - xfull[1]
 	xhalf[-1] = 2.*xfull[-1] - xfull[-2]
 	return xhalf
 
-def time_bnds(time, step, start=None, end=None):
+def time_bnds(time, step=None, start=None, end=None):
 	n = len(time)
+	if step is None:
+		if len(time) < 2:
+			raise ValueError('Too few profiles to determine temporal resolution')
+		step = time[1] - time[0]
 	bnds = np.full((n, 2), np.nan, time.dtype)
 	bnds[:,0] = time - step*0.5
 	bnds[:,1] = time + step*0.5
 	bnds[1:,0] = np.maximum(bnds[:-1,1], bnds[1:,0])
 	bnds[:-1,1] = np.minimum(bnds[1:,0], bnds[:-1,1])
 	if start is not None:
 		bnds[0,0] = max(bnds[0,0], start)
```

### Comparing `alcf-1.8.1/alcf/models/__init__.py` & `alcf-1.9.0/alcf/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import alcf
+
 META = {
 	'clw': {
 		'.dims': ['time', 'level'],
 		'long_name': 'mass fraction of cloud liquid water',
 		'standard_name': 'mass_fraction_of_cloud_liquid_water_in_air',
 		'units': '1',
 	},
@@ -69,14 +71,15 @@
 	},
 	'orog': {
 		'.dims': ['time'],
 		'long_name': 'surface altitude',
 		'standard_name': 'surface_altitude',
 		'units': 'm',
 	},
+	'.': alcf.META,
 }
 
 from . import amps
 #from . import cmip5
 from . import era5
 from . import jra55
 from . import merra2
```

### Comparing `alcf-1.8.1/alcf/models/amps.py` & `alcf-1.9.0/alcf/models/amps.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 	'CLWMR_GDS5_ISBL',
 	'ICMR_GDS5_ISBL',
 ]
 
 STEP = 3/24
 
 def index(dirname, warnings=[], recursive=False, njobs=1):
+	print('<- %s' % dirname)
 	return ds.readdir(dirname, ['XTIME'],
 		jd=True,
 		recursive=recursive,
 		warnings=warnings,
 		parallel=(njobs > 1),
 		njobs=njobs,
 		full=True,
@@ -54,15 +55,17 @@
 	time0 = aq.from_iso(time0.replace('_', 'T'))
 	if time < 2000000.:
 		time = time0 + time/(24*60)
 	if (time >= t1 - step*0.5) & (time < t2 + step*0.5):
 		lon0, lat0 = track(time)
 		if np.isnan(lon0) or np.isnan(lat0):
 			return
-		d = ds.read(d_index['filename'], variables=VARS_NC, sel={'Time': 0})
+		print('<- %s' % d_index['filename'])
+		d = ds.read(d_index['filename'], VARS_NC, sel={'Time': 0})
+		misc.require_vars(d, VARS_NC)
 		lon = np.where(d['XLONG'] < 0, 360 + d['XLONG'], d['XLONG'])
 		lat = d['XLAT']
 		l = np.argmin((lon - lon0)**2 + (lat - lat0)**2)
 		i, j = np.unravel_index(l, lon.shape)
 		clw = d['QCLOUD'][:,i,j]
 		cli = d['QICE'][:,i,j]
 		cl = np.full(len(clw), 100, dtype=np.float64)
@@ -104,15 +107,18 @@
 	dim1 = ds.dims(d_index, 'HGT_GDS5_ISBL')[0]
 	dim2 = ds.dims(d_index, 'CLWMR_GDS5_ISBL')[0]
 
 	if (time >= t1 - step*0.5) & (time < t2 + step*0.5):
 		lon0, lat0 = track(time)
 		if np.isnan(lon0) or np.isnan(lat0):
 			return
-		d = ds.read(d_index['filename'], variables=VARS_NCL + [dim1, dim2])
+		req_vars = VARS_NCL + [dim1, dim2]
+		print('<- %s' % d_index['filename'])
+		d = ds.read(d_index['filename'], req_vars)
+		misc.require_vars(d, req_vars)
 		lon = np.where(d['g5_lon_1'] < 0, 360 + d['g5_lon_1'], d['g5_lon_1'])
 		lat = d['g5_lat_0']
 		l = np.argmin((lon - lon0)**2 + (lat - lat0)**2)
 		i, j = np.unravel_index(l, lon.shape)
 		k1 = ds.dim(d, dim1)
 		k2 = ds.dim(d, dim2)
 		dk = k1 - k2
```

### Comparing `alcf-1.8.1/alcf/models/era5.py` & `alcf-1.9.0/alcf/models/era5.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import ds_format as ds
 import os
 import numpy as np
 from alcf.models import META
 from alcf import misc
 import aquarius_time as aq
 
+VARS_INDEX = ['time', 'latitude', 'longitude']
+
 VARS_PLEV = [
 	'time',
 	'clwc',
 	'ciwc',
 	'cc',
 	'latitude',
 	'longitude',
@@ -45,55 +47,59 @@
 }
 
 STEP = 1/24
 
 def read0(type_, dirname, track, t1, t2,
 	warnings=[], step=STEP, recursive=False):
 
+	print('<- %s' % dirname)
 	dd_idx = ds.readdir(dirname,
-		variables=['time', 'latitude', 'longitude'],
+		VARS_INDEX,
 		jd=True,
 		full=True,
 		warnings=warnings,
 		recursive=recursive,
 	)
 
-	vars = {
+	req_vars = {
 		'surf': VARS_SURF,
 		'plev': VARS_PLEV,
 	}[type_]
 
 	trans = {
 		'surf': TRANS_SURF,
 		'plev': TRANS_PLEV,
 	}[type_]
 
 	dd = []
 	for d_idx in dd_idx:
+		misc.require_vars(d_idx, VARS_INDEX)
 		time = d_idx['time']
 		lat = d_idx['latitude']
 		lon = d_idx['longitude']
 		lon = lon % 360
 		filename = d_idx['filename']
 
 		ii = np.nonzero(
 			(time >= t1 - step*0.5) &
 			(time < t2 + step*0.5)
 		)[0]
+		print('<- %s' % filename)
 		for i in ii:
 			t = time[i]
 			lon0, lat0 = track(time[i])
 			if np.isnan(lon0) or np.isnan(lat0):
 				continue
 			j = np.argmin(np.abs(lat - lat0))
 			k = np.argmin(np.abs(lon - lon0))
-			d = ds.read(filename, vars,
+			d = ds.read(filename, req_vars,
 				sel={'time': [i], 'latitude': j, 'longitude': k},
 				jd=True,
 			)
+			misc.require_vars(d, req_vars)
 			for a, b in trans.items():
 				if a in d.keys():
 					ds.rename(d, a, b)
 			d['lat'] = np.array([d['lat']])
 			d['lon'] = np.array([d['lon']])
 			d['lon'] = d['lon'] % 360
 			d['.']['lat']['.dims'] = ['time']
```

### Comparing `alcf-1.8.1/alcf/models/icon.py` & `alcf-1.9.0/alcf/models/icon.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,52 +13,59 @@
 	'ta',
 	'ps',
 ]
 
 STEP = 6/24
 
 def index(dirname, warnings=[], recursive=False, njobs=1):
+	print('<- %s' % dirname)
 	dd = ds.readdir(dirname,
 		variables=['time'],
 		jd=True,
 		full=True,
 		warnings=warnings,
 		recursive=recursive,
 		parallel=(njobs > 1),
 		njobs=njobs,
 	)
 
-	d_g = ds.read(os.path.join(dirname, 'vgrid.nc'), [
+	vgrid_filename = os.path.join(dirname, 'vgrid.nc')
+	print('<- %s' % vgrid_filename)
+	d_g = ds.read(vgrid_filename, [
 		'clon', 'clat'
 	], full=True)
+	misc.require_vars(d_g, ['clon', 'clat'])
 	d_g['clon'] *= 180/np.pi
 	d_g['clat'] *= 180/np.pi
 
 	return [dd, d_g]
 
 def read(dirname, index, track, t1, t2,
 	warnings=[], step=STEP, recursive=False):
 
 	vgrid_filename = os.path.join(dirname, 'vgrid.nc')
 	dd_out = []
 	dd_idx, d_g = index
 	ncells = ds.dim(d_g, 'ncells')
 	vgrid_cache = {}
 
+	print('<- %s' % vgrid_filename)
 	for var in VARS:
 		dd = []
 		for d_idx in dd_idx:
+			misc.require_vars(d_idx, ['time'])
 			if var not in d_idx['.']:
 				continue
 			time = d_idx['time']
 			filename = d_idx['filename']
 			ii = np.nonzero(
 				(time >= t1 - step*0.5) &
 				(time < t2 + step*0.5)
 			)[0]
+			print('<- %s' % filename)
 			for i in ii:
 				lon0, lat0 = track(time[i])
 				if np.isnan(lon0) or np.isnan(lat0):
 					continue
 				dist = misc.geo_distance(
 					np.full(ncells, lon0),
 					np.full(ncells, lat0),
@@ -71,24 +78,26 @@
 				if cell in vgrid_cache:
 					d_g2 = vgrid_cache[cell]
 				else:
 					d_g2 = ds.read(vgrid_filename, ['zg', 'zghalf'], sel={
 						'ncells': cell,
 						'height': ds.dim(d_g, 'height') - 1,
 					})
+					misc.require_vars(d_g2, ['zg', 'zghalf'])
 					vgrid_cache[cell] = d_g2
 
 				d = ds.read(filename, [var],
 					sel={
 						'time': [i],
 						'ncells': cell,
 						'cell': cell,
 					},
 					jd=True,
 				)
+				misc.require_vars(d, [var])
 				ds.rename_dim(d, 'height', 'level')
 				d['time'] = np.array([time[i]])
 				d['lat'] = np.array([d_g['clat'][cell]])
 				d['lon'] = np.array([d_g['clon'][cell]])
 				d['orog'] = np.array([d_g2['zghalf']])
 				d['zfull'] = d_g2['zg'][::-1]
 				d['zfull'] = d['zfull'].reshape((1, len(d['zfull'])))
```

### Comparing `alcf-1.8.1/alcf/models/icon_intake_healpix.py` & `alcf-1.9.0/alcf/models/icon_intake_healpix.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 		)
 		d = {}
 		d['time'] = t
 		d['lon'], d['lat'] = healpy.pix2ang(ids.crs.healpix_nside, j,
 			lonlat=True,
 			nest=nest
 		)
+		misc.require_vars(ids, VARS)
 		for var in VARS:
 			sel = {'cell': j}
 			if 'time' in ids[var].coords:
 				sel['time'] = i
 			x = np.array(ids[var].isel(**sel))
 			if var == 'phalf':
 				d['ps'] = x[-1]
```

### Comparing `alcf-1.8.1/alcf/models/jra55.py` & `alcf-1.9.0/alcf/models/jra55.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 	't',
 	'ciwc',
 	'clw',
 	'tcc',
 	'sp',
 ]
 
-VARS_AUX = [
-	'level',
+VARS_INDEX = ['time', 'latitude', 'longitude']
+
+VARS_AUX1 = [
 	'time',
 	'latitude',
 	'longitude',
 ]
 
+VARS_AUX2 = [
+	'level',
+]
+
 TRANS = {
 	'gh': 'zfull',
 	'latitude': 'lat',
 	'longitude': 'lon',
 	'level': 'pfull',
 	't': 'ta',
 	'ciwc': 'cli',
@@ -36,80 +41,86 @@
 }
 
 STEP = 6/24
 
 def read(dirname, index, track, t1, t2,
 	warnings=[], step=STEP, recursive=False):
 
-	d_ll = ds.read(os.path.join(dirname, 'LL125.nc'), [
-		'latitude',
-		'longitude',
-		'z'
-	])
+	req_vars = ['latitude', 'longitude', 'z']
+	ll_filename = os.path.join(dirname, 'LL125.nc')
+	print('<- %s' % ll_filename)
+	d_ll = ds.read(ll_filename, req_vars)
+	misc.require_vars(d_ll, req_vars)
 	lat_ll = d_ll['latitude']
 	lon_ll = d_ll['longitude']
 	orog_ll = d_ll['z'][0,:,:]/9.80665
 
-	dd_idx = ds.readdir(dirname,
-		variables=['time', 'latitude', 'longitude'],
+	print('<- %s' % dirname)
+	dd_idx = ds.readdir(dirname, VARS_INDEX,
 		jd=True,
 		full=True,
 		warnings=warnings,
 		recursive=recursive,
 	)
-	d_out = {}
+	do = {}
 	for var in VARS:
 		dd = []
 		var2 = TRANS[var]
 		for d_idx in dd_idx:
+			misc.require_vars(d_idx, VARS_INDEX)
 			if var not in d_idx['.']:
 				continue
 			time = d_idx['time']
 			lat = d_idx['latitude']
 			lon = d_idx['longitude']
 			filename = d_idx['filename']
 			ii = np.nonzero(
 				(time >= t1 - step*0.5) &
 				(time < t2 + step*0.5)
 			)[0]
+			print('<- %s' % filename)
 			for i in ii:
 				t = time[i]
 				lon0, lat0 = track(time[i])
 				if np.isnan(lon0) or np.isnan(lat0):
 					continue
 				j = np.argmin(np.abs(lat - lat0))
 				k = np.argmin(np.abs(lon - lon0))
 				j_ll = np.argmin(np.abs(lat_ll - lat0))
 				k_ll = np.argmin(np.abs(lon_ll - lon0))
-				d = ds.read(filename, VARS_AUX + [var],
+				req_vars = VARS_AUX1 + [var]
+				vars_ = req_vars + VARS_AUX2
+				d = ds.read(filename, vars_,
 					sel={
 						'time': [i],
 						'latitude': j,
 						'longitude': k,
 					},
 					jd=True,
 				)
+				misc.require_vars(d, req_vars)
 				for a, b in TRANS.items():
 					if a in d.keys():
 						ds.rename(d, a, b)
 				d['lat'] = np.array([d['lat']])
 				d['lon'] = np.array([d['lon']])
 				d['orog'] = np.array([orog_ll[j_ll,k_ll]])
 				d['.']['lat']['.dims'] = ['time']
 				d['.']['lon']['.dims'] = ['time']
 				d['.']['orog'] = {'.dims': ['time']}
-				if 'pfull' in ds.get_vars(d):
+				if 'pfull' in ds.vars(d):
 					d['pfull'] = d['pfull'].reshape([1, len(d['pfull'])])
 					d['.']['pfull']['.dims'] = ['time', 'pfull']
 					d['pfull'] = d['pfull'][:,::-1]
 					d[var2] = d[var2][:,::-1]
 					ds.select(d, {'pfull': np.arange(27)})
 				dd.append(d)
 		d = ds.op.merge(dd, 'time')
-		for var_aux in VARS_AUX:
-			if TRANS[var_aux] in ds.get_vars(d_out) \
-				and TRANS[var_aux] in ds.get_vars(d) \
-				and not np.all(d_out[TRANS[var_aux]] == d[TRANS[var_aux]]):
+		for var_aux in (VARS_AUX1 + VARS_AUX2):
+			if TRANS[var_aux] in ds.vars(do) \
+				and TRANS[var_aux] in ds.vars(d) \
+				and not np.all(do[TRANS[var_aux]] == d[TRANS[var_aux]]):
 				raise ValueError('%s: Field differs between input files' % TRANS[var_aux])
-		d_out.update(d)
-	d_out['pfull'] = d_out['pfull']*1e2
-	return d_out
+		do.update(d)
+	if 'pfull' in do:
+		do['pfull'] = do['pfull']*1e2
+	return do
```

### Comparing `alcf-1.8.1/alcf/models/merra2.py` & `alcf-1.9.0/alcf/models/nzcsm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,72 @@
 import ds_format as ds
 import os
 import numpy as np
 from alcf.models import META
 from alcf import misc
 
+VARS_INDEX = ['time0', 'latitude', 'longitude']
+
 VARS = [
-	'lon',
-	'lat',
-	'time',
-	'H',
-	'T',
-	'PL',
-	'PS',
-	'PHIS',
-	'QL',
-	'QI',
-	'CLOUD',
+	'hybridt32',
+	'latitude',
+	'longitude',
+	'model_press',
+	'model_qcf',
+	'model_qcl',
+	'theta_lev_temp',
+	'time0',
 ]
 
-STEP=3/24
+STEP = 2/24
 
 def read(dirname, index, track, t1, t2,
 	warnings=[], step=STEP, recursive=False):
 
-	dd_index = ds.readdir(dirname, variables=['time', 'lat', 'lon'], jd=True,
-		recursive=recursive)
+	print('<- %s' % dirname)
+	dd_index = ds.readdir(dirname, VARS_INDEX,
+		jd=True, recursive=recursive)
 	dd = []
 	for d_index in dd_index:
-		time = d_index['time']
-		lat = d_index['lat']
-		lon = d_index['lon']
+		misc.require_vars(d_index, VARS_INDEX)
+		time = d_index['time0']
+		lon = d_index['longitude']
 		lon = np.where(lon < 0., 360. + lon, lon)
+		lat = d_index['latitude']
 		filename = d_index['filename']
-		ii = np.nonzero(
-			(time >= t1 - step*0.5) &
-			(time < t2 + step*0.5)
-		)[0]
+		ii = np.where((time >= t1 - step*0.5) & (time <= t2 + step*0.5))[0]
+		print('<- %s' % filename)
 		for i in ii:
-			t = time[i]
 			lon0, lat0 = track(time[i])
 			if np.isnan(lon0) or np.isnan(lat0):
 				continue
-			j = np.argmin(np.abs(lat - lat0))
-			k = np.argmin(np.abs(lon - lon0))
-			d = ds.read(filename, variables=VARS,
-				sel={'time': i, 'lat': j, 'lon': k}
-			)
-			clw = d['QL'][::-1]
-			cli = d['QI'][::-1]
-			cl = d['CLOUD'][::-1]*100.
-			ps = d['PS']
-			orog = d['PHIS']/9.80665
-			pfull = d['PL'][::-1]
-			zfull = d['H'][::-1]
-			ta = d['T'][::-1]
-			nlev = len(clw)
-			newshape4 = (1, nlev)
+			l = np.argmin((lon - lon0)**2 + (lat - lat0)**2)
+			j, k = np.unravel_index(l, lon.shape)
+			d = ds.read(filename, VARS, sel={'time0': i, 'rlat': j, 'rlon': k})
+			misc.require_vars(d, VARS)
+			clw = d['model_qcl']
+			cli = d['model_qcf']
+			cl = 100.*np.ones(len(clw), dtype=np.float64)
+			ps = 2*d['model_press'][0] - d['model_press'][1]
+			orog = max(0., 2*d['hybridt32'][0] - d['hybridt32'][1])
+			pfull = d['model_press']
+			zfull = d['hybridt32']
+			ta = d['theta_lev_temp']
+			newshape4 = (1, len(clw))
 			newshape3 = (1,)
 			d_new = {
 				'clw': clw.reshape(newshape4),
 				'cli': cli.reshape(newshape4),
 				'ta': ta.reshape(newshape4),
 				'cl': cl.reshape(newshape4),
 				'pfull': pfull.reshape(newshape4),
 				'zfull': zfull.reshape(newshape4),
-				'ps': ps.reshape(newshape3),
-				'orog': orog.reshape(newshape3),
-				'lat': np.array([lat[j]]),
-				'lon': np.array([lon[k]]),
-				'time': np.array([t]),
+				'ps': [ps],
+				'orog': [orog],
+				'lon': np.array([lon[j,k]]),
+				'lat': np.array([lat[j,k]]),
+				'time': np.array([time[i]]),
 				'.': META,
 			}
 			dd.append(d_new)
 	d = ds.op.merge(dd, 'time')
 	return d
```

### Comparing `alcf-1.8.1/alcf/models/nzesm.py` & `alcf-1.9.0/alcf/models/nzesm.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,61 +2,67 @@
 import ds_format as ds
 import os
 import numpy as np
 from alcf.models import META
 from alcf import misc
 import aquarius_time as aq
 
-VARIABLES = [
+VARS = [
 	'air_pressure',
 	'air_temperature',
 	'mass_fraction_of_cloud_liquid_water_in_air',
 	'mass_fraction_of_cloud_ice_in_air',
 	'cloud_volume_fraction_in_atmosphere_layer',
 ]
 
+VARS_INDEX = ['time', 'latitude', 'longitude', 'level_height']
+
 TRANS = {
 	'air_pressure': 'pfull',
 	'air_temperature': 'ta',
 	'mass_fraction_of_cloud_liquid_water_in_air': 'clw',
 	'mass_fraction_of_cloud_ice_in_air': 'cli',
 	'cloud_volume_fraction_in_atmosphere_layer': 'cl',
 }
 
 STEP = 6/24
 
 def read(dirname, index, track, t1, t2, warnings=[], step=STEP):
+	print('<- %s' % dirname)
 	dd_index = ds.readdir(dirname,
-		variables=['time', 'latitude', 'longitude', 'level_height'],
+		VARS_INDEX,
 		jd=True,
 		full=True,
 		warnings=warnings,
 	)
 	d_var = {}
-	for var in VARIABLES:
+	for var in VARS:
 		dd = []
 		for d_index in dd_index:
 			if var not in d_index['.']:
 				continue
+			misc.require_vars(d_index, VARS_INDEX)
 			time = d_index['time']
 			time_half = misc.half(time)
 			lat = d_index['latitude']
 			lon = d_index['longitude']
 			level_height = d_index['level_height']
 			filename = d_index['filename']
 			ii = np.nonzero((time_half[1:] >= t1) & (time_half[:-1] < t2))[0]
+			print('<- %s' % filename)
 			for i in ii:
 				t = time[i]
 				lon0, lat0 = track(time[i])
 				if np.isnan(lon0) or np.isnan(lat0):
 					continue
 				j = np.argmin(np.abs(lat - lat0))
 				k = np.argmin(np.abs(lon - lon0))
-				d = ds.read(filename, variables=[var],
+				d = ds.read(filename, [var],
 					sel={'time': i, 'latitude': j, 'longitude': k})
+				misc.require_vars(d, [var])
 				d_new = {
 					'lat': np.array([lat[j]]),
 					'lon': np.array([lon[k]]),
 					'time': np.array([t]),
 					'level_height': np.array([level_height]),
 					'.': META,
 				}
```

### Comparing `alcf-1.8.1/alcf/models/um.py` & `alcf-1.9.0/alcf/models/um.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 	'STASH_m01s00i408',
 	'STASH_m01s00i409',
 	'STASH_m01s00i254',
 	'STASH_m01s00i012',
 	'STASH_m01s16i004',
 ]
 
+VARS_INDEX = ['TALLTS', 'latitude_t', 'longitude_t', 'DALLTH_zsea_theta']
+
 TRANS = {
 	'TALLTS': 'time',
 	'latitude_t': 'lat',
 	'longitude_t': 'lon',
 	'DALLTH_eta_theta': 'eta',
 	'STASH_m01s00i265': 'cl',
 	'STASH_m01s00i408': 'pfull',
@@ -33,53 +35,57 @@
 }
 
 STEP = 1/24
 
 def read(dirname, index, track, t1, t2,
 	warnings=[], step=STEP, recursive=False):
 
-	d_orog = ds.read(os.path.join(dirname, 'qrparm.orog.nc'), [
-		'latitude',
-		'longitude',
-		'surface_altitude',
-	])
+	req_vars = ['latitude', 'longitude', 'surface_altitude']
+	orog_filename = os.path.join(dirname, 'qrparm.orog.nc')
+	print('<- %s' % orog_filename)
+	d_orog = ds.read(orog_filename, req_vars)
+	misc.require_vars(d_orog, req_vars)
 
+	print('<- %s' % dirname)
 	dd_idx = ds.readdir(dirname,
-		variables=['TALLTS', 'latitude_t', 'longitude_t', 'DALLTH_zsea_theta'],
+		VARS_INDEX,
 		jd=True,
 		full=True,
 		warnings=warnings,
 		recursive=recursive,
 	)
 
 	dd = []
 	for d_idx in dd_idx:
-		if 'TALLTS' not in d_idx:
+		if d_idx['filename'] == orog_filename:
 			continue
+		misc.require_vars(d_idx, VARS_INDEX)
 
 		time = d_idx['TALLTS']
 		lat = d_idx['latitude_t']
 		lon = d_idx['longitude_t']
 		filename = d_idx['filename']
 
 		ii = np.nonzero(
 			(time >= t1 - step*0.5) &
 			(time < t2 + step*0.5)
 		)[0]
+		print('<- %s' % filename)
 		for i in ii:
 			t = time[i]
 			lon0, lat0 = track(time[i])
 			if np.isnan(lon0) or np.isnan(lat0):
 				continue
 			j = np.argmin(np.abs(lat - lat0))
 			k = np.argmin(np.abs(lon - lon0))
 			d = ds.read(filename, VARS,
 				sel={'TALLTS': [i], 'latitude_t': j, 'longitude_t': k},
 				jd=True,
 			)
+			misc.require_vars(d, VARS)
 			for a, b in TRANS.items():
 				if a in d.keys():
 					ds.rename(d, a, b)
 			d['lat'] = np.array([d['lat']])
 			d['lon'] = np.array([d['lon']])
 			d['.']['lat']['.dims'] = ['time']
 			d['.']['lon']['.dims'] = ['time']
```

### Comparing `alcf-1.8.1/alcf.egg-info/PKG-INFO` & `alcf-1.9.0/alcf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.8.1
+Version: 1.9.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.8.1/alcf.egg-info/SOURCES.txt` & `alcf-1.9.0/alcf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/build_doc` & `alcf-1.9.0/build_doc`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/MISR_simulator/MISR_simulator.f` & `alcf-1.9.0/cosp/MISR_simulator/MISR_simulator.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/MODIS_simulator/modis_simulator.F90` & `alcf-1.9.0/cosp/MODIS_simulator/modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/MODIS_simulator/test_modis_simulator.F90` & `alcf-1.9.0/cosp/MODIS_simulator/test_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/Makefile` & `alcf-1.9.0/cosp/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/Makefile.cmor1` & `alcf-1.9.0/cosp/Makefile.cmor1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/Makefile.ibm` & `alcf-1.9.0/cosp/Makefile.ibm`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/README.md` & `alcf-1.9.0/cosp/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/README.txt` & `alcf-1.9.0/cosp/README.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/actsim/lidar_simulator.F90` & `alcf-1.9.0/cosp/actsim/lidar_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/actsim/lmd_ipsl_stats.F90` & `alcf-1.9.0/cosp/actsim/lmd_ipsl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/actsim/mie_backscatter_1064.F90` & `alcf-1.9.0/cosp/actsim/mie_backscatter_1064.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/actsim/mie_backscatter_532.F90` & `alcf-1.9.0/cosp/actsim/mie_backscatter_532.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/actsim/mie_backscatter_910.F90` & `alcf-1.9.0/cosp/actsim/mie_backscatter_910.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt` & `alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt` & `alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt` & `alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt` & `alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt` & `alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt` & `alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp.F90` & `alcf-1.9.0/cosp/cosp.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_constants.F90` & `alcf-1.9.0/cosp/cosp_constants.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_defs.h` & `alcf-1.9.0/cosp/cosp_defs.h`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_htfrtc.F90` & `alcf-1.9.0/cosp/cosp_htfrtc.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_input_nl.txt` & `alcf-1.9.0/cosp/cosp_input_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_io.F90` & `alcf-1.9.0/cosp/cosp_io.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_isccp_simulator.F90` & `alcf-1.9.0/cosp/cosp_isccp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_lidar.F90` & `alcf-1.9.0/cosp/cosp_lidar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_misr_simulator.F90` & `alcf-1.9.0/cosp/cosp_misr_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_modis_simulator.F90` & `alcf-1.9.0/cosp/cosp_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_output_nl.txt` & `alcf-1.9.0/cosp/cosp_output_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_rttov.F90` & `alcf-1.9.0/cosp/cosp_rttov.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_rttov_simulator.F90` & `alcf-1.9.0/cosp/cosp_rttov_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_simulator.F90` & `alcf-1.9.0/cosp/cosp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_stats.F90` & `alcf-1.9.0/cosp/cosp_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_types.F90` & `alcf-1.9.0/cosp/cosp_types.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/cosp_utils.F90` & `alcf-1.9.0/cosp/cosp_utils.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/Makefile` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/README` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/README`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/congvec.f` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/icarus.f` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/icarus.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/input.data` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/input.data.halved` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data.halved`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/license` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/license`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/scops.f` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_congvec.f` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh` & `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/llnl/cosp_radar.F90` & `alcf-1.9.0/cosp/llnl/cosp_radar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/llnl/llnl_stats.F90` & `alcf-1.9.0/cosp/llnl/llnl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/llnl/pf_to_mr.f` & `alcf-1.9.0/cosp/llnl/pf_to_mr.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/llnl/prec_scops.f` & `alcf-1.9.0/cosp/llnl/prec_scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/mac_info.txt` & `alcf-1.9.0/cosp/mac_info.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/predict_mom07.F90` & `alcf-1.9.0/cosp/predict_mom07.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/README` & `alcf-1.9.0/cosp/quickbeam/README`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/array_lib.f90` & `alcf-1.9.0/cosp/quickbeam/array_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/atmos_lib.f90` & `alcf-1.9.0/cosp/quickbeam/atmos_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/calc_Re.f90` & `alcf-1.9.0/cosp/quickbeam/calc_Re.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/dsd.f90` & `alcf-1.9.0/cosp/quickbeam/dsd.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/format_input.f90` & `alcf-1.9.0/cosp/quickbeam/format_input.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/gases.f90` & `alcf-1.9.0/cosp/quickbeam/gases.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/load_hydrometeor_classes.f90` & `alcf-1.9.0/cosp/quickbeam/load_hydrometeor_classes.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/load_mie_table.f90` & `alcf-1.9.0/cosp/quickbeam/load_mie_table.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/math_lib.f90` & `alcf-1.9.0/cosp/quickbeam/math_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/mrgrnk.f90` & `alcf-1.9.0/cosp/quickbeam/mrgrnk.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/optics_lib.f90` & `alcf-1.9.0/cosp/quickbeam/optics_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/predict_psd07.f` & `alcf-1.9.0/cosp/quickbeam/predict_psd07.f`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/radar_simulator.f90` & `alcf-1.9.0/cosp/quickbeam/radar_simulator.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/radar_simulator_init.f90` & `alcf-1.9.0/cosp/quickbeam/radar_simulator_init.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/radar_simulator_types.f90` & `alcf-1.9.0/cosp/quickbeam/radar_simulator_types.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/scale_LUTs_io.f90` & `alcf-1.9.0/cosp/quickbeam/scale_LUTs_io.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/quickbeam/zeff.f90` & `alcf-1.9.0/cosp/quickbeam/zeff.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/utils/COSP_plots.py` & `alcf-1.9.0/cosp/utils/COSP_plots.py`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/cosp/utils/append_cf3hr_files.sh` & `alcf-1.9.0/cosp/utils/append_cf3hr_files.sh`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-auto.1` & `alcf-1.9.0/man/alcf-auto.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-calibrate.1` & `alcf-1.9.0/man/alcf-calibrate.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-compare.1` & `alcf-1.9.0/man/alcf-compare.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-convert.1` & `alcf-1.9.0/man/alcf-convert.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-download.1` & `alcf-1.9.0/man/alcf-download.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-lidar.1` & `alcf-1.9.0/man/alcf-lidar.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-model.1` & `alcf-1.9.0/man/alcf-model.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-plot.1` & `alcf-1.9.0/man/alcf-plot.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-simulate.1` & `alcf-1.9.0/man/alcf-simulate.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf-stats.1` & `alcf-1.9.0/man/alcf-stats.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/man/alcf.1` & `alcf-1.9.0/man/alcf.1`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/setup.py` & `alcf-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	def run(self):
 		subprocess.run('make', cwd='cosp', check=True)
 		subprocess.run('make', check=True)
 		build_py.run(self)
 
 setup(
 	name='alcf',
-	version='1.8.1',
+	version='1.9.0',
 	description='Automatic Lidar and Ceilometer Framework (ALCF)',
 	author='Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn',
 	author_email='peter@peterkuma.net',
 	license='MIT',
 	entry_points={
 		'console_scripts': 'alcf = alcf.bin.alcf:main_wrapper',
 	},
```

### Comparing `alcf-1.8.1/src/cosp_run.f03` & `alcf-1.9.0/src/cosp_run.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/src/main.f03` & `alcf-1.9.0/src/main.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.8.1/src/nc_utils.f03` & `alcf-1.9.0/src/nc_utils.f03`

 * *Files identical despite different names*

