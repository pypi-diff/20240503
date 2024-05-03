# Comparing `tmp/sliderule-4.3.2.tar.gz` & `tmp/sliderule-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-4.3.2.tar", last modified: Thu Apr  4 20:23:45 2024, max compression
+gzip compressed data, was "sliderule-4.4.0.tar", last modified: Fri May  3 12:28:50 2024, max compression
```

## Comparing `sliderule-4.3.2.tar` & `sliderule-4.4.0.tar`

### file list

```diff
@@ -1,58 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.794572 sliderule-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-04 20:23:36.000000 sliderule-4.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 20:23:36.000000 sliderule-4.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 20:23:45.794572 sliderule-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-04 20:23:36.000000 sliderule-4.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 20:23:36.000000 sliderule-4.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:23:45.794572 sliderule-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-04 20:23:36.000000 sliderule-4.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.786572 sliderule-4.3.2/sliderule/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/bathy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    36904 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16231 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)    36298 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (127)    38833 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (127)   118505 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)    50316 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/swot.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.794572 sliderule-4.3.2/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.790572 sliderule-4.3.2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/bathy_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_3dep_DEM_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/container_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/lpdaac_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/opendata_worldcover.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 20:23:36.000000 sliderule-4.3.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:28:50.008638 sliderule-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-03 12:28:40.000000 sliderule-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 12:28:40.000000 sliderule-4.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-03 12:28:50.008638 sliderule-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-03 12:28:40.000000 sliderule-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 12:28:40.000000 sliderule-4.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:28:50.008638 sliderule-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-03 12:28:40.000000 sliderule-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:28:50.004638 sliderule-4.4.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/bathy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37126 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16112 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35981 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45195 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125451 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52074 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/swot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-03 12:28:40.000000 sliderule-4.4.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:28:50.008638 sliderule-4.4.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-03 12:28:49.000000 sliderule-4.4.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-03 12:28:49.000000 sliderule-4.4.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:28:49.000000 sliderule-4.4.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 12:28:49.000000 sliderule-4.4.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 12:28:49.000000 sliderule-4.4.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:28:50.008638 sliderule-4.4.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/bathy_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/i2_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/lpdaac_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/opendata_worldcover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 12:28:40.000000 sliderule-4.4.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 12:28:40.000000 sliderule-4.4.0/version.txt
```

### Comparing `sliderule-4.3.2/LICENSE` & `sliderule-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/PKG-INFO` & `sliderule-4.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 4.3.2
+Version: 4.4.0
 Summary: Python client for interacting with sliderule server
-Home-page: https://github.com/ICESat2-SlideRule/sliderule/
+Home-page: https://github.com/SlideRuleEarth/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sliderule-4.3.2/README.md` & `sliderule-4.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 }
 
 # make request
 rsps = icesat2.atl06p(parms, "icesat2")
 print(f"{rsps}")
 ```
 
-More extensive examples in the form of Jupyter Notebooks can be found in the [examples](https://github.com/ICESat2-SlideRule/sliderule-python/tree/main/examples) folder of the [sliderule-python](https://github.com/ICESat2-SlideRule/sliderule-python) repository.
+More extensive examples in the form of Jupyter Notebooks can be found in the [examples](https://github.com/SlideRuleEarth/sliderule-python/tree/main/examples) folder of the [sliderule-python](https://github.com/SlideRuleEarth/sliderule-python) repository.
 
 ## III. Reference and User's Guide
 
 Please see our [documentation](https://slideruleearth.io/rtd/) page for reference and user's guide material.
```

### Comparing `sliderule-4.3.2/setup.py` & `sliderule-4.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 scripts=[os.path.join('utils',f) for f in os.listdir('utils') if f.endswith('.py')]
 
 setup(
     name='sliderule',
     author='SlideRule Developers',
     description='Python client for interacting with sliderule server',
     long_description_content_type="text/markdown",
-    url='https://github.com/ICESat2-SlideRule/sliderule/',
+    url='https://github.com/SlideRuleEarth/sliderule/',
     license='BSD 3-Clause',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Physics',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
```

### Comparing `sliderule-4.3.2/sliderule/container.py` & `sliderule-4.4.0/sliderule/bathy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,40 @@
-# Copyright (c) 2021, University of Washington
+# Copyright (c) 2023, University of Texas
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
 #
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 #    this list of conditions and the following disclaimer in the documentation
 #    and/or other materials provided with the distribution.
 #
-# 3. Neither the name of the University of Washington nor the names of its
+# 3. Neither the name of the University of Texas nor the names of its
 #    contributors may be used to endorse or promote products derived from this
 #    software without specific prior written permission.
 #
-# THIS SOFTWARE IS PROVIDED BY THE UNIVERSITY OF WASHINGTON AND CONTRIBUTORS
+# THIS SOFTWARE IS PROVIDED BY THE UNIVERSITY OF TEXAS AND CONTRIBUTORS
 # “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
 # TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-# PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE UNIVERSITY OF WASHINGTON OR
+# PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE UNIVERSITY OF TEXAS OR
 # CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import time
-import logging
-import sliderule
-from sliderule import logger
-
-###############################################################################
-# GLOBALS
-###############################################################################
-
-# profiling times for each major function
-profiles = {}
-
-###############################################################################
-# LOCAL FUNCTIONS
-###############################################################################
+from sliderule import sliderule, icesat2
 
 ###############################################################################
 # APIs
 ###############################################################################
 
-
 #
-#  Execute Container
+#  ATL24 Gold Standard
 #
-def execute (parm):
-    '''
-    Executes a containerized application using SlideRule
-
-    Parameters
-    ----------
-    parms:      dict
-                parameters used to configure container runtime environment
-
-    Returns
-    -------
-    str
-        json response
-    '''
-    tstart = time.perf_counter()
-    rsps = sliderule.source("cre", {"parms": parm})
-    profiles[execute.__name__] = time.perf_counter() - tstart
-    return rsps
+def atl24g(parm, callbacks={}, resources=None, keep_id=False, height_key=None):
+    return icesat2.atl24gp(parm, resources=[resource])
```

### Comparing `sliderule-4.3.2/sliderule/earthdata.py` & `sliderule-4.4.0/sliderule/earthdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,18 @@
 
 # default maximum number of resources to process in one request
 DEFAULT_MAX_REQUESTED_RESOURCES = 300
 max_requested_resources = DEFAULT_MAX_REQUESTED_RESOURCES
 
 # best effort match of datasets to providers and versions for earthdata
 DATASETS = {
-    "ATL03":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": [] },
+    "ATL03":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "ATL06":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "ATL08":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "ATL09":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI01_B":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI02_A":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI02_B":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".tiff"],  "collections": []},
     "GEDI_L3_LandSurface_Metrics_V2_1952":                 {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI_L4A_AGB_Density_V2_1_2056":                      {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI_L4B_Gridded_Biomass_2017":                       {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".tiff"],  "collections": []},
     "HLS":                                                 {"provider": "LPCLOUD",     "version": None,   "api": "stac",  "formats": [".tiff"],  "collections": ["HLSS30.v2.0", "HLSL30.v2.0"]},
@@ -86,14 +87,15 @@
     "swot-sim-ecco-llc4320": "SWOT_SIMULATED_L2_KARIN_SSH_ECCO_LLC4320_CALVAL_V1",
     "swot-sim-glorys": "SWOT_SIMULATED_L2_KARIN_SSH_GLORYS_CALVAL_V1",
     "usgs3dep-1meter-dem": "Digital Elevation Model (DEM) 1 meter",
     "landsat-hls": "HLS",
     "icesat2": "ATL03",
     "icesat2-atl06": "ATL06",
     "icesat2-atl08": "ATL08",
+    "icesat2-atl09": "ATL09",
     "atlas-local": "ATL03",
     "nsidc-s3": "ATL03"
 }
 
 # upper limit on resources returned from CMR query per request
 CMR_PAGE_SIZE = 2000
 
@@ -732,14 +734,15 @@
         if time_start != None:
             rqst["start"] = time_start
             rqst["stop"] = time_end
 
         # Make request
         rsps = context.get(url, params=rqst)
         rsps.raise_for_status()
+        print(rsps.content)
         data = json.loads(rsps.content)
         items += data['items']
         if len(items) == data['total']:
             break
 
     # Create GeoJSON
     geojson = {
```

### Comparing `sliderule-4.3.2/sliderule/gedi.py` & `sliderule-4.4.0/sliderule/gedi.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,17 +153,14 @@
         tstart = time.perf_counter()
 
         # Default the Asset
         rqst_parm = parm.copy()
         if "asset" not in rqst_parm:
             rqst_parm["asset"] = asset
 
-        # Get List of Resources from CMR (if not supplied)
-        resources = earthdata.search(rqst_parm, resources)
-
         # Build GEDI Request
         rqst = {
             "resources": resources,
             "parms": rqst_parm
         }
 
         # Make API Processing Request
```

### Comparing `sliderule-4.3.2/sliderule/h5.py` & `sliderule-4.4.0/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/sliderule/icesat2.py` & `sliderule-4.4.0/sliderule/icesat2.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 CNF_POSSIBLE_TEP = -2
 CNF_NOT_CONSIDERED = -1
 CNF_BACKGROUND = 0
 CNF_WITHIN_10M = 1
 CNF_SURFACE_LOW = 2
 CNF_SURFACE_MEDIUM = 3
 CNF_SURFACE_HIGH = 4
+SRT_DYNAMIC = -1
 SRT_LAND = 0
 SRT_OCEAN = 1
 SRT_SEA_ICE = 2
 SRT_LAND_ICE = 3
 SRT_INLAND_WATER = 4
 MAX_COORDS_IN_POLYGON = 16384
 GT1L = 10
@@ -267,17 +268,14 @@
 def __build_request(parm, resources, default_asset='icesat2'):
 
     # Default the Asset
     rqst_parm = parm.copy()
     if "asset" not in rqst_parm:
         rqst_parm["asset"] = default_asset
 
-    # Get List of Resources
-    resources = earthdata.search(rqst_parm, resources)
-
     # Build Request
     return {
         "resources": resources,
         "parms": rqst_parm
     }
 
 
@@ -755,24 +753,22 @@
                     ATL03 HDF5 filename
 
     Returns
     -------
     GeoDataFrame
         ATL03 extents (see `Photon Segments </web/rtd/user_guide/ICESat-2.html#segmented-photon-data>`_)
     '''
-    return atl03sp(parm, resources=[resource])
+    return atl24gp(parm, resources=[resource])
 
 #
-#  Parallel  Gold Standard
+#  Parallel ATL24 Gold Standard
 #
 def atl24gp(parm, callbacks={}, resources=None, keep_id=False, height_key=None):
     '''
-    Performs ATL24 gold standard generation in parallel on ATL03 data. Unlike the `atl03s <#atl03s>`_ function,
-    this function does not take a resource as a parameter; instead it is expected that the **parm** argument includes a polygon which
-    is used to fetch all available resources from the CMR system automatically.
+    Performs ATL24 gold standard generation in parallel on ATL03 data.
 
     Parameters
     ----------
         parms:          dict
                         parameters used to configure ATL03 subsetting (see `Parameters </web/rtd/user_guide/ICESat-2.html#parameters>`_)
         callbacks:      dictionary
                         a callback function that is called for each result record
```

### Comparing `sliderule-4.3.2/sliderule/io.py` & `sliderule-4.4.0/sliderule/io.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,24 +27,29 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import sys
 import json
 import warnings
 import datetime
-import geopandas
 import numpy as np
-from sliderule import logger
+from sliderule import logger, SLIDERULE_EPSG
 
 # imports with warnings if not present
 try:
     import scipy.io
 except ModuleNotFoundError as e:
     sys.stderr.write("Warning: missing packages, some functions will throw an exception if called. (%s)\n" % (str(e)))
 try:
+    import geopandas
+    from geopandas.io.arrow import _geopandas_to_arrow
+    from geopandas._compat import import_optional_dependency
+except ModuleNotFoundError as e:
+    sys.stderr.write("Warning: missing packages, some functions will throw an exception if called. (%s)\n" % (str(e)))  
+try:
     import h5py
 except ModuleNotFoundError as e:
     sys.stderr.write("Warning: missing packages, some functions will throw an exception if called. (%s)\n" % (str(e)))
 
 # attributes for ATL06-SR and ATL03 variables
 def get_attributes(**kwargs):
     # set default keyword arguments
@@ -333,14 +338,33 @@
 
 # determine if polygon winding is counter-clockwise
 def winding(x,y):
     npts = len(x)
     wind = np.sum([(x[i+1] - x[i])*(y[i+1] + y[i]) for i in range(npts - 1)])
     return wind
 
+# geodesic area of a polygon in square kilometers
+def area(lon, lat, a=6378.1370):
+    assert len(lon) == len(lat), "Longitude and Latitude arrays must be the same length"
+    assert len(lon) > 2, "Need at least 3 points to calculate area"
+    # factor for converting to radians
+    dtr = np.pi/180.0
+    # initialize area
+    area = 0.0
+    npts = len(lon)
+    # for each point in the polygon
+    for i in range(npts):
+        # wrap coordinates
+        ii = (i + 1) % npts
+        # calculate geodesic area in square kilometers
+        area += (a**2)*(lon[ii]*dtr - lon[i]*dtr) * \
+            (2.0 + np.sin(lat[i]*dtr) + np.sin(lat[ii]*dtr))/2.0
+    # return absolute value of area
+    return np.abs(area).squeeze()
+
 # fix longitudes to be -180:180
 def wrap_longitudes(lon):
     phi = np.arctan2(np.sin(lon*np.pi/180.0),np.cos(lon*np.pi/180.0))
     # convert phi from radians to degrees
     return phi*180.0/np.pi
 
 # convert coordinates to a sliderule region
@@ -357,42 +381,46 @@
         x[i] = p['lon']
         y[i] = p['lat']
     return (x,y)
 
 # convert geodataframe vector object to a list of sliderule regions
 def from_geodataframe(gdf):
     # verify that geodataframe is in latitude/longitude
-    geodataframe = gdf.to_crs(epsg=4326)
+    geodataframe = gdf.to_crs(SLIDERULE_EPSG)
     # create a list of regions
     regions = []
     # for each region
     for geometry in geodataframe.geometry:
         regions.append([{'lon':ln,'lat':lt} for ln,lt in geometry.exterior.coords])
     # return the list of regions
     return regions
 
 # output request parameters to JSON
 def to_json(filename, **kwargs):
     # set default keyword arguments
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
+    # import optional dependencies
+    pyproj = import_optional_dependency(
+        "pyproj", extra="pyproj is required for CRS conversion."
+    )
     # add each parameter as an attribute
     SRparams = ['H_min_win', 'atl08_class', 'atl03_quality', 'ats', 'cnf',
         'cnt', 'len', 'maxi', 'res', 'sigma_r_max', 'srt', 'yapc']
     output = {}
     # for each adjustable sliderule parameter
     for p in SRparams:
         # try to convert the parameter if available
         try:
             output[p] = attributes_encoder(kwargs['parameters'][p])
         except:
             pass
     # save CRS to JSON
-    crs = geopandas.tools.crs.CRS.from_string(kwargs['crs'])
+    crs = pyproj.CRS.from_string(kwargs['crs'])
     output['crs'] = crs.to_string()
     # save each region following GeoJSON specification
     output['type'] = 'FeatureCollection'
     output['features'] = []
     for i,poly in enumerate(kwargs['regions']):
         lon, lat = from_region(poly)
         lon = attributes_encoder(lon)
@@ -433,20 +461,123 @@
         # for each coordinate set in the feature
         for coords in feature['geometry']['coordinates']:
             # append to sliderule regions
             regions.append([{'lon':ln,'lat':lt} for ln,lt in coords])
     # return the sliderule parameters and regions
     return (parms, regions)
 
+def to_parquet(gdf, filename, **kwargs):
+    # set default keyword arguments
+    kwargs.setdefault('index',None)
+    kwargs.setdefault('compression','snappy')
+    kwargs.setdefault('schema_version',None)
+    kwargs.setdefault('parameters',dict())
+    kwargs.setdefault('regions',[])
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
+    # import optional dependencies
+    pyproj = import_optional_dependency(
+        "pyproj", extra="pyproj is required for CRS conversion."
+    )
+    parquet = import_optional_dependency(
+        "pyarrow.parquet", extra="pyarrow is required for Parquet support."
+    )
+    # output metadata
+    output = {}
+    # for each adjustable sliderule parameter
+    [kwargs['parameters'].pop(p) for p in ['poly']]
+    for p,val in kwargs['parameters'].items():
+        # try to convert the parameter if available
+        try:
+            output[p] = attributes_encoder(val)
+        except:
+            pass
+    # save CRS to JSON
+    crs = pyproj.CRS.from_string(kwargs['crs'])
+    output['crs'] = crs.to_string()
+    # save each region following GeoJSON specification
+    output['type'] = 'FeatureCollection'
+    output['features'] = []
+    for i,poly in enumerate(kwargs['regions']):
+        lon, lat = from_region(poly)
+        lon = attributes_encoder(lon)
+        lat = attributes_encoder(lat)
+        geometry=dict(type="polygon", coordinates=[])
+        geometry['coordinates'].append([[ln,lt] for ln,lt in zip(lon,lat)])
+        output['features'].append(dict(type="Feature", geometry=geometry))
+    # dump the attributes to encoded JSON-format
+    sliderule_metadata = json.dumps(output).encode('utf-8') 
+    # convert geodataframe to arrow table
+    table = _geopandas_to_arrow(gdf,
+        index=kwargs['index'],
+        schema_version=kwargs['schema_version']
+    )
+    # store sliderule specific file-level metadata
+    metadata = table.schema.metadata
+    metadata.update({b"sliderule": sliderule_metadata})
+    # replace schema metadata with updated
+    table = table.replace_schema_metadata(metadata)
+    # write arrow table to parquet file
+    parquet.write_table(table, filename,
+        compression=kwargs['compression']
+    )
+
+def from_parquet(filename, **kwargs):
+    # set default keyword arguments
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
+    kwargs.setdefault('return_parameters',False)
+    kwargs.setdefault('return_regions',False)
+    # import optional dependencies
+    parquet = import_optional_dependency(
+        "pyarrow.parquet", extra="pyarrow is required for Parquet support."
+    )
+    # read arrow table from parquet file
+    # and convert to coordinate reference system
+    gdf = geopandas.read_parquet(filename).to_crs(kwargs['crs'])
+    # if not returning the query parameters or polygon
+    if not (kwargs['return_parameters'] or kwargs['return_regions']):
+        # return geodataframe
+        return gdf
+    # create tuple with returns
+    output = (gdf,)
+    # get parquet file metadata
+    metadata = parquet.read_metadata(filename).metadata
+    # validate sliderule metadata
+    if b'sliderule' not in metadata.keys():
+        logger.error("No sliderule metadata found in Parquet file")
+        return output
+    # decode sliderule metadata from JSON
+    parms = json.loads(metadata[b'sliderule'].decode('utf-8'))
+    # create a list of regions
+    regions = []
+    # for each feature in the JSON file
+    for feature in parms.pop('features'):
+        # for each coordinate set in the feature
+        for coords in feature['geometry']['coordinates']:
+            # append to sliderule regions
+            regions.append([{'lon':ln,'lat':lt} for ln,lt in coords])
+    # if returning the parameters
+    if kwargs['return_parameters']:
+        # add parameters to output tuple
+        [parms.pop(v) for v in ('version','commit','type')]
+        output += (parms,)
+    # if returning the regions
+    if kwargs['return_regions']:
+        # add regions to output tuple
+        output += (regions,)
+    # return the combined tuple
+    return output
+
 # output geodataframe to netCDF (version 3)
 def to_nc(gdf, filename, **kwargs):
+    # add warning that function is deprecated
+    logger.critical(f"Deprecated. Will be removed in a future release")
     # set default keyword arguments
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
     kwargs.setdefault('units','seconds since 2018-01-01T00:00:00')
     # get output attributes
     attributes = get_attributes()
     # open netCDF3 file object (64-bit offset format)
     fileID = scipy.io.netcdf.netcdf_file(filename, 'w', version=2)
@@ -488,15 +619,15 @@
     fileID.reference = attributes['reference']
     fileID.date_created = attributes['date_created']
     fileID.date_type = attributes['date_type']
     fileID.time_type = attributes['time_type']
     # save geodataframe coordinate system
     fileID.crs = kwargs['crs']
     # add geospatial attributes
-    if (kwargs['crs'] == 'EPSG:4326'):
+    if kwargs['crs'] in ('EPSG:4326', SLIDERULE_EPSG):
         fileID.geospatial_lat_units = \
             attributes['geospatial_lat_units']
         fileID.geospatial_lon_units = \
             attributes['geospatial_lon_units']
         fileID.geospatial_ellipsoid = \
             attributes['geospatial_ellipsoid']
     # add each parameter as an attribute
@@ -531,16 +662,18 @@
     logger.info(list(fileID.variables.keys()))
     # Closing the netCDF file
     fileID.close()
     warnings.filterwarnings("default")
 
 # input geodataframe from netCDF (version 3)
 def from_nc(filename, **kwargs):
+    # add warning that function is deprecated
+    logger.critical(f"Deprecated. Will be removed in a future release")
     # set default crs
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
     kwargs.setdefault('index_key','time')
     kwargs.setdefault('return_parameters',False)
     kwargs.setdefault('return_regions',False)
     # open netCDF3 file object (64-bit offset format)
     fileID = scipy.io.netcdf.netcdf_file(filename, 'r', version=2)
@@ -627,15 +760,15 @@
 
 # output geodataframe to HDF5
 def to_hdf(gdf, filename, **kwargs):
     # set default keyword arguments
     kwargs.setdefault('driver','pytables')
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
     kwargs.setdefault('units','seconds since 2018-01-01T00:00:00')
     # get output attributes
     attributes = get_attributes()
     # convert geodataframe to pandas dataframe
     df = geopandas.pd.DataFrame(gdf.drop(columns='geometry'))
@@ -654,31 +787,33 @@
     elif (kwargs['driver'].lower() == 'h5py'):
         kwargs.pop('driver')
         # write dataframe to HDF5
         write_h5py(df, filename, attributes, **kwargs)
 
 # write pandas dataframe to pytables HDF5
 def write_pytables(df, filename, attributes, **kwargs):
+    # add warning that function is deprecated
+    logger.critical(f"Deprecated. Will be removed in a future release")
     # set default keyword arguments
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     # write data to a pytables HDF5 file
     df.to_hdf(filename, 'sliderule_segments', format="table", mode="w")
     # add file attributes
     fileID = geopandas.pd.HDFStore(filename, mode='a')
     fileID.root._v_attrs.TITLE = attributes['title']
     fileID.root._v_attrs.reference = attributes['reference']
     fileID.root._v_attrs.date_created = attributes['date_created']
     fileID.root._v_attrs.date_type = attributes['date_type']
     fileID.root._v_attrs.time_type = attributes['time_type']
     # set coordinate reference system as attribute
     fileID.root._v_attrs.crs = kwargs['crs']
     # add geospatial attributes
-    if (kwargs['crs'] == 'EPSG:4326'):
+    if kwargs['crs'] in ('EPSG:4326', SLIDERULE_EPSG):
         fileID.root._v_attrs.geospatial_lat_units = \
             attributes['geospatial_lat_units']
         fileID.root._v_attrs.geospatial_lon_units = \
             attributes['geospatial_lon_units']
         fileID.root._v_attrs.geospatial_ellipsoid = \
             attributes['geospatial_ellipsoid']
     # add each parameter as an attribute
@@ -712,18 +847,20 @@
     logger.info(filename)
     logger.info(fileID.get_storer('sliderule_segments').non_index_axes[0][1])
     # Closing the HDF5 file
     fileID.close()
 
 # write pandas dataframe to h5py HDF5
 def write_h5py(df, filename, attributes, **kwargs):
+    # add warning that function is deprecated
+    logger.critical(f"Deprecated. Will be removed in a future release")
     # set default keyword arguments
     kwargs.setdefault('parameters',None)
     kwargs.setdefault('regions',[])
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     kwargs.setdefault('units','seconds since 2018-01-01T00:00:00')
     # open HDF5 file object
     fileID = h5py.File(filename, mode='w')
     # create HDF5 records
     h5 = {}
     # create output delta time variable
     key = 'delta_time'
@@ -751,15 +888,15 @@
     fileID.attrs['reference'] = attributes['reference']
     fileID.attrs['date_created'] = attributes['date_created']
     fileID.attrs['date_type'] = attributes['date_type']
     fileID.attrs['time_type'] = attributes['time_type']
     # set coordinate reference system as attribute
     fileID.attrs['crs'] = kwargs['crs']
     # add geospatial attributes
-    if (kwargs['crs'] == 'EPSG:4326'):
+    if kwargs['crs'] in ('EPSG:4326', SLIDERULE_EPSG):
         fileID.attrs['geospatial_lat_units'] = \
             attributes['geospatial_lat_units']
         fileID.attrs['geospatial_lon_units'] = \
             attributes['geospatial_lon_units']
         fileID.attrs['geospatial_ellipsoid'] = \
             attributes['geospatial_ellipsoid']
     # add each parameter as an attribute
@@ -795,15 +932,15 @@
     # Closing the HDF5 file
     fileID.close()
 
 # input geodataframe from HDF5
 def from_hdf(filename, **kwargs):
     # set default keyword arguments
     kwargs.setdefault('driver','pytables')
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
     kwargs.setdefault('return_parameters',False)
     kwargs.setdefault('return_regions',False)
     if (kwargs['driver'].lower() == 'pytables'):
         kwargs.pop('driver')
         # return GeoDataFrame from pytables
@@ -811,16 +948,18 @@
     elif (kwargs['driver'].lower() == 'h5py'):
         kwargs.pop('driver')
         # return GeoDataFrame from h5py
         return read_h5py(filename, **kwargs)
 
 # read pandas dataframe from pytables HDF5
 def read_pytables(filename, **kwargs):
+    # add warning that function is deprecated
+    logger.critical(f"Deprecated. Will be removed in a future release")
     # set default crs
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
     kwargs.setdefault('return_parameters',False)
     kwargs.setdefault('return_regions',False)
     # open pytables HDF5 to read pandas dataframe
     df = geopandas.pd.read_hdf(filename, **kwargs)
     # generate geometry column
@@ -879,16 +1018,18 @@
         # add regions to output tuple
         output += (regions,)
     # return the combined tuple
     return output
 
 # read pandas dataframe from h5py HDF5
 def read_h5py(filename, **kwargs):
+    # add warning that function is deprecated
+    logger.critical(f"Deprecated. Will be removed in a future release")
     # set default crs
-    kwargs.setdefault('crs','EPSG:4326')
+    kwargs.setdefault('crs',SLIDERULE_EPSG)
     kwargs.setdefault('lon_key','longitude')
     kwargs.setdefault('lat_key','latitude')
     kwargs.setdefault('index_key','time')
     kwargs.setdefault('return_parameters',False)
     kwargs.setdefault('return_regions',False)
     # open HDF5 file object
     fileID = h5py.File(filename, mode='r')
@@ -963,19 +1104,27 @@
     if kwargs['return_regions']:
         # add regions to output tuple
         output += (regions,)
     # return the combined tuple
     return output
 
 # output formats wrapper
-def to_file(gdf, filename, format='hdf', **kwargs):
+def to_file(gdf, filename, format='parquet', **kwargs):
     if format.lower() in ('hdf','hdf5','h5'):
         to_hdf(gdf, filename, **kwargs)
     elif format.lower() in ('netcdf','nc'):
         to_nc(gdf, filename, **kwargs)
+    elif format.lower() in ('geojson','csv','shp'):
+        gdf.to_file(filename, **kwargs)
+    elif format.lower() in ('geoparquet','parquet'):
+        to_parquet(gdf, filename, **kwargs)
 
 # input formats wrapper
-def from_file(filename, format='hdf', **kwargs):
+def from_file(filename, format='parquet', **kwargs):
     if format.lower() in ('hdf','hdf5','h5'):
         return from_hdf(filename, **kwargs)
-    elif format.lower() in ('netcdf','nc'):
+    elif format.lower() in ('netcdf','netcdf4','nc'):
         return from_nc(filename, **kwargs)
+    elif format.lower() in ('geojson','csv','shp'):
+        return geopandas.from_file(filename, **kwargs)
+    elif format.lower() in ('geoparquet','parquet'):
+        return from_parquet(filename, **kwargs)
```

### Comparing `sliderule-4.3.2/sliderule/ipxapi.py` & `sliderule-4.4.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/sliderule/ipysliderule.py` & `sliderule-4.4.0/sliderule/ipysliderule.py`

 * *Files 3% similar despite different names*

```diff
@@ -516,16 +516,15 @@
                 "South: Polar Stereographic South (EPSG:3031)"),
             disabled=False,
             style=self.style,
         )
 
         # dropdown menu for selecting variable to draw on map
         variable_list = ['h_mean', 'h_sigma', 'dh_fit_dx', 'dh_fit_dy',
-            'rms_misfit', 'w_surface_window_final', 'delta_time',
-            'cycle', 'rgt']
+            'rms_misfit', 'w_surface_window_final', 'cycle', 'rgt']
         self.variable = ipywidgets.Dropdown(
             options=variable_list,
             value='h_mean',
             description='Variable:',
             description_tooltip="Variable: variable to display on leaflet map",
             disabled=False,
             style=self.style,
@@ -655,14 +654,24 @@
             description_tooltip="Track: Ground Track to plot",
             disabled=False
         )
 
         # watch plot kind widgets for changes
         self.plot_kind.observe(self.set_plot_kind)
 
+        # selection for output file format
+        format_options = ["GeoJSON","csv","geoparquet","netCDF","HDF5"]
+        self.file_format = ipywidgets.Dropdown(
+            options=format_options,
+            value="geoparquet",
+            description="Format:",
+            description_tooltip="Format: Output file format",
+            disabled=False
+        )
+
         # button and label for output file selection
         self.file = copy.copy(self.atl06_filename)
         self.savebutton = ipywidgets.Button(
             description="Save As"
         )
         self.savelabel = ipywidgets.Text(
             value=self.file,
@@ -997,20 +1006,24 @@
     def saveas_file(self, b):
         """function for file save
         """
         IPython.display.clear_output()
         root = tkinter.Tk()
         root.withdraw()
         root.call('wm', 'attributes', '.', '-topmost', True)
-        filetypes = (("HDF5 file", "*.h5"),
+        filetypes = (
+            ("geoparquet file", "*.parquet"),
+            ("GeoJSON file", "*.geojson"),
+            ("csv file", "*.csv"),
             ("netCDF file", "*.nc"),
+            ("HDF5 file", "*.h5"),
             ("All Files", "*.*"))
         b.files = tkinter.filedialog.asksaveasfilename(
             initialfile=self.file,
-            defaultextension='h5',
+            defaultextension='parquet',
             filetypes=filetypes)
         self.savelabel.value = b.files
         self.file = b.files
         return self
 
     def set_savefile(self, sender):
         """return filename from saveas function
@@ -1020,16 +1033,20 @@
     def select_file(self, b):
         """function for file selection
         """
         IPython.display.clear_output()
         root = tkinter.Tk()
         root.withdraw()
         root.call('wm', 'attributes', '.', '-topmost', True)
-        filetypes = (("HDF5 file", "*.h5"),
+        filetypes = (
+            ("geoparquet file", "*.parquet"),
+            ("GeoJSON file", "*.geojson"),
+            ("csv file", "*.csv"),
             ("netCDF file", "*.nc"),
+            ("HDF5 file", "*.h5"),
             ("All Files", "*.*"))
         b.files = tkinter.filedialog.askopenfilename(
             defaultextension='h5',
             filetypes=filetypes,
             multiple=False)
         self.loadlabel.value = b.files
         self.file = b.files
@@ -1037,62 +1054,97 @@
 
     def set_loadfile(self, sender):
         """return filename from file select function
         """
         self.file = self.loadlabel.value
 
     @property
-    def atl03_filename(self):
+    def atl03_filename(self) -> str:
         """default input and output file string for ATL03 requests
         """
         # get sliderule submission time
         now = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
-        args = (now, self.release.value)
-        return "ATL03-SR_{0}_{1}.h5".format(*args)
+        args = (now, self.release.value, self.suffix)
+        return "ATL03-SR_{0}_{1}.{2}".format(*args)
 
     @property
-    def atl06_filename(self):
+    def atl06_filename(self) -> str:
         """default input and output file string for ATL06 requests
         """
         # get sliderule submission time
         now = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
-        args = (now, self.release.value)
-        return "ATL06-SR_{0}_{1}.h5".format(*args)
+        args = (now, self.release.value, self.suffix)
+        return "ATL06-SR_{0}_{1}.{2}".format(*args)
 
     @property
-    def atl08_filename(self):
+    def atl08_filename(self) -> str:
         """default input and output file string for ATL08 requests
         """
         # get sliderule submission time
         now = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
-        args = (now, self.release.value)
-        return "ATL08-SR_{0}_{1}.h5".format(*args)
+        args = (now, self.release.value, self.suffix)
+        return "ATL08-SR_{0}_{1}.{2}".format(*args)
 
     @property
-    def format(self):
+    def format(self) -> str:
         """return the file format from file string
         """
-        hdf = ('h5','hdf5','hdf')
-        netcdf = ('nc','netcdf','nc3')
-        if self.file.endswith(hdf):
-            return 'hdf'
-        elif self.file.endswith(netcdf):
-            return 'netcdf'
-        else:
-            return ''
+        types = {}
+        types['hdf'] = ('h5','hdf5','hdf')
+        types['netcdf'] = ('nc','netcdf','nc3')
+        types['csv'] = ('csv','txt')
+        types['geojson'] = ('geojson','json')
+        types['parquet'] = ('geoparquet','parquet','pq')
+        for key, val in types.items():
+            if self.file.endswith(val):
+                return key
+        # return empty string if no match
+        return ''
+        
+    @property
+    def suffix(self) -> str:
+        """return the file suffix
+        """
+        SUFFIX = {
+            "GeoJSON":"geojson",
+            "csv":"csv",
+            "geoparquet":"parquet",
+            "netCDF":"nc",
+            "HDF5":"h5"
+        }
+        try:
+            return SUFFIX[self.file_format.value]
+        except KeyError:
+            return ""
 
     @property
-    def _r(self):
+    def mime_type(self) -> str:
+        """return the internet media type of the file format
+        """
+        MIME = {
+            "GeoJSON":"text/json",
+            "csv":"text/csv",
+            "geoparquet":"application/vnd.apache.parquet",
+            "netCDF":"application/x-netcdf",
+            "HDF5":"application/x-hdf5"
+        }
+        try:
+            return MIME[self.file_format.value]
+        except KeyError:
+            return ""
+
+    @property
+    def _r(self) -> str:
         """return string for reversed Matplotlib colormaps
         """
         cmap_reverse_flag = '_r' if self.reverse.value else ''
         return cmap_reverse_flag
 
     @property
-    def colormap(self):
+    def colormap(self) -> str:
         """return string for Matplotlib colormaps
         """
         return self.cmap.value + self._r
 
     # click handler for individual photons
     def atl03_click_handler(self, feature):
         """handler for leaflet map clicks
@@ -1881,60 +1933,67 @@
             providers[provider_name] = Bunch(
                 {i: xyzservices.lib.TileProvider(provider[i]) for i in provider.keys()}
             )
     return providers
 
 # create traitlets of basemap providers
 basemaps = _load_dict(providers)
+# set default map dimensions
+_default_layout = ipywidgets.Layout(width='100%', height='600px')
+_default_max_area = 500e3
 
 # draw ipyleaflet map
 class leaflet:
     def __init__(self, projection, **kwargs):
         # set default keyword arguments
         kwargs.setdefault('map',None)
+        kwargs.setdefault('layout', _default_layout)
         kwargs.setdefault('prefer_canvas', False)
         kwargs.setdefault('attribution', False)
         kwargs.setdefault('zoom_control', False)
         kwargs.setdefault('scale_control', False)
         kwargs.setdefault('full_screen_control', False)
         kwargs.setdefault('cursor_control', True)
         kwargs.setdefault('layer_control', True)
         kwargs.setdefault('color', 'green')
         # create basemap in projection
         if (projection == 'Global'):
-            kwargs.setdefault('center', (39,-108))
-            kwargs.setdefault('zoom', 9)
+            kwargs.setdefault('center', (40,-100))
+            kwargs.setdefault('zoom', 4)
             self.map = ipyleaflet.Map(center=kwargs['center'],
                 zoom=kwargs['zoom'], max_zoom=15, world_copy_jump=True,
                 prefer_canvas=kwargs['prefer_canvas'],
                 attribution_control=kwargs['attribution'],
-                basemap=ipyleaflet.basemaps.Esri.WorldTopoMap)
+                basemap=ipyleaflet.basemaps.Esri.WorldTopoMap,
+                layout=kwargs['layout'])
             self.crs = 'EPSG:3857'
         elif (projection == 'North'):
             kwargs.setdefault('center', (90,0))
             kwargs.setdefault('zoom', 5)
             self.map = ipyleaflet.Map(center=kwargs['center'],
                 zoom=kwargs['zoom'], max_zoom=24,
                 prefer_canvas=kwargs['prefer_canvas'],
                 attribution_control=kwargs['attribution'],
                 basemap=basemaps.Esri.ArcticOceanBase,
-                crs=projections.EPSG5936.ESRIBasemap)
+                crs=projections.EPSG5936.ESRIBasemap,
+                layout=kwargs['layout'])
             # add arctic ocean reference basemap
             reference = basemaps.Esri.ArcticOceanReference
             self.map.add(ipyleaflet.basemap_to_tiles(reference))
             self.crs = 'EPSG:5936'
         elif (projection == 'South'):
             kwargs.setdefault('center', (-90,0))
-            kwargs.setdefault('zoom', 2)
+            kwargs.setdefault('zoom', 3)
             self.map = ipyleaflet.Map(center=kwargs['center'],
                 zoom=kwargs['zoom'], max_zoom=9,
                 prefer_canvas=kwargs['prefer_canvas'],
                 attribution_control=kwargs['attribution'],
                 basemap=basemaps.Esri.AntarcticBasemap,
-                crs=projections.EPSG3031.ESRIBasemap)
+                crs=projections.EPSG3031.ESRIBasemap,
+                layout=kwargs['layout'])
             self.crs = 'EPSG:3031'
         else:
             # use a predefined ipyleaflet map
             assert kwargs['map'], 'Leaflet map needs to be defined'
             self.map = kwargs['map']
             self.crs = self.map.crs['name']
         # add control for full screen
@@ -1969,15 +2028,15 @@
         # add control for drawing polygons or bounding boxes
         draw_control = ipyleaflet.DrawControl(polyline={},circlemarker={},
             edit=False)
         shapeOptions = {'color':kwargs['color'],'fill_color':kwargs['color']}
         draw_control.rectangle = dict(shapeOptions=shapeOptions,
             metric=['km','m'])
         draw_control.polygon = dict(shapeOptions=shapeOptions,
-            allowIntersection=False,showArea=True,metric=['km','m'])
+            allowIntersection=False, showArea=True, metric=['km','m'])
         # create regions
         self.regions = []
         draw_control.on_draw(self.handle_draw)
         self.map.add(draw_control)
         # initialize data and colorbars
         self.geojson = None
         self.tooltip = None
@@ -2143,26 +2202,33 @@
         if (kwargs.get('type') == 'mousemove'):
             lat,lon = kwargs.get('coordinates')
             lon = sliderule.io.wrap_longitudes(lon)
             self.cursor.value = u"""Latitude: {d[0]:8.4f}\u00B0,
                 Longitude: {d[1]:8.4f}\u00B0""".format(d=[lat,lon])
 
     # keep track of rectangles and polygons drawn on map
-    def handle_draw(self, obj, action, geo_json):
+    def handle_draw(self, obj, action, geo_json, **kwargs):
         """callback for handling draw events and interactively
         creating SlideRule region objects
         """
+        kwargs.setdefault('check_valid', True)
+        kwargs.setdefault('maximum_area', _default_max_area)
         lon,lat = np.transpose(geo_json['geometry']['coordinates'])
         lon = sliderule.io.wrap_longitudes(lon)
         cx,cy = sliderule.io.centroid(lon,lat)
         wind = sliderule.io.winding(lon,lat)
         # set winding to counter-clockwise
         if (wind > 0):
             lon = lon[::-1]
             lat = lat[::-1]
+        # calculate area of region
+        area = sliderule.io.area(lon,lat)
+        if kwargs['check_valid'] and (area > kwargs['maximum_area']):
+            logger.warning(f"Region is too large: {area:0.0f} km^2")
+            return
         # create sliderule region from list
         region = sliderule.io.to_region(lon,lat)
         # append coordinates to list
         if (action == 'created'):
             self.regions.append(region)
         elif (action == 'deleted'):
             self.regions.remove(region)
@@ -2206,15 +2272,15 @@
         kwargs.setdefault('norm', None)
         kwargs.setdefault('radius', 1.0)
         kwargs.setdefault('fillOpacity', 0.5)
         kwargs.setdefault('weight', 3.0)
         kwargs.setdefault('stride', None)
         kwargs.setdefault('max_plot_points', 10000)
         kwargs.setdefault('tooltip', True)
-        kwargs.setdefault('fields', self.default_atl06_fields())
+        kwargs.setdefault('fields', [])
         kwargs.setdefault('colorbar', True)
         kwargs.setdefault('position', 'topright')
         # add warning that function is deprecated
         logger.critical(f"Deprecated. Will be removed in a future release")
         # remove any prior instances of a data layer
         if self.geojson is not None:
             self.map.remove(self.geojson)
@@ -2373,68 +2439,33 @@
         output = ipywidgets.Image(value=png.getvalue(), format='png')
         self.colorbar = ipyleaflet.WidgetControl(widget=output,
             transparent_bg=True, position=kwargs['position'])
         # add colorbar
         self.map.add(self.colorbar)
         plt.close()
 
-    @staticmethod
-    def default_atl03_fields():
-        """List of ATL03 tooltip fields
-        """
-        return ['atl03_cnf', 'atl08_class', 'cycle', 'height',
-            'pair', 'rgt', 'segment_id', 'track', 'yapc_score']
-
-    @staticmethod
-    def default_atl06_fields():
-        """List of ATL06-SR tooltip fields
-        """
-        return ['cycle', 'dh_fit_dx', 'gt', 'h_mean',
-            'h_sigma', 'rgt', 'rms_misfit', 'w_surface_window_final']
-
-    @staticmethod
-    def default_atl08_fields():
-        """List of ATL08-SR tooltip fields
-        """
-        return ['canopy_openness', 'cycle', 'gt', 'h_canopy',
-            'h_min_canopy', 'h_mean_canopy',
-            'h_max_canopy', 'h_te_median', 'rgt']
-
-    @staticmethod
-    def default_mosaic_fields(**kwargs):
-        kwargs.setdefault('with_flags', False)
-        kwargs.setdefault('zonal_stats', False)
-        """List of mosaic tooltip fields
-        """
-        columns = ['time','value']
-        if kwargs['with_flags']:
-            columns += ['flags']
-        if kwargs['zonal_stats']:
-            columns += ['count','min','max','mean','median','stdev','mad']
-        return [f'mosaic.{c}' for c in columns]
-
 @gpd.pd.api.extensions.register_dataframe_accessor("leaflet")
 class LeafletMap:
     """A geopandas GeoDataFrame extension for interactive map plotting,
     based on ipyleaflet
     """
 
     def __init__(self, gdf):
         # initialize map
         self.map = None
         self.crs = None
         # initialize geodataframe
         self._gdf = gdf
         # initialize data and colorbars
-        self.geojson = None
-        self.tooltip = None
-        self.tooltip_width = None
-        self.tooltip_height = None
-        self.fields = []
-        self.colorbar = None
+        self._geojson = None
+        self._tooltip = None
+        self._tooltip_width = None
+        self._tooltip_height = None
+        self._fields = []
+        self._colorbar = None
         # initialize hover control
         self.hover_control = None
         # initialize selected feature
         self.selected_callback = None
 
     # add geodataframe data to leaflet map
     def GeoData(self, m, **kwargs):
@@ -2474,79 +2505,82 @@
         kwargs.setdefault('fields', [])
         kwargs.setdefault('colorbar', True)
         kwargs.setdefault('position', 'topright')
         # set map and map coordinate reference system
         self.map = m
         self.crs = m.crs['name']
         # remove any prior instances of a data layer
-        if self.geojson is not None:
-            self.map.remove(self.geojson)
+        if self._geojson is not None:
+            self.map.remove(self._geojson)
         if kwargs['stride'] is not None:
             stride = np.copy(kwargs['stride'])
         elif (self._gdf.shape[0] > kwargs['max_plot_points']):
             stride = int(self._gdf.shape[0]//kwargs['max_plot_points'])
         else:
             stride = 1
         # sliced geodataframe for plotting
-        geodataframe = self._gdf[slice(None,None,stride)]
+        self._gdf_selected = self._gdf[slice(None,None,stride)]
         self.column_name = copy.copy(kwargs['column_name'])
-        geodataframe['data'] = geodataframe[self.column_name]
-        # set colorbar limits to 2-98 percentile
-        # if not using a defined plot range
-        clim = geodataframe['data'].quantile((0.02, 0.98)).values
-        if kwargs['vmin'] is None:
-            vmin = clim[0]
-        else:
-            vmin = np.copy(kwargs['vmin'])
-        if kwargs['vmax'] is None:
-            vmax = clim[-1]
-        else:
-            vmax = np.copy(kwargs['vmax'])
+        self._gdf_selected['data'] = self._gdf_selected[self.column_name]
+        # get the normalization bounds
+        self.get_norm_bounds(**kwargs)
         # create matplotlib normalization
         if kwargs['norm'] is None:
-            norm = colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
+            self.norm = colors.Normalize(vmin=self.vmin, vmax=self.vmax, clip=True)
         else:
-            norm = copy.copy(kwargs['norm'])
+            self.norm = copy.copy(kwargs['norm'])
         # normalize data to be within vmin and vmax
-        normalized = norm(geodataframe['data'])
+        normalized = self.norm(self._gdf_selected['data'])
+        # get colormap
+        self.cmap = copy.copy(cm.get_cmap(kwargs['cmap']))
         # create HEX colors for each point in the dataframe
-        geodataframe["color"] = np.apply_along_axis(colors.to_hex, 1,
-            cm.get_cmap(kwargs['cmap'], 256)(normalized))
+        self._gdf_selected["color"] = np.apply_along_axis(colors.to_hex, 1,
+            cm.get_cmap(self.cmap.name, 256)(normalized))
         # leaflet map point style
-        point_style = {key:kwargs[key] for key in ['radius','fillOpacity','weight']}
+        self._point_style = {
+            key:kwargs[key] for key in ['radius','fillOpacity','weight']
+        }
         # convert to GeoJSON object
-        self.geojson = ipyleaflet.GeoJSON(data=geodataframe.__geo_interface__,
-            point_style=point_style, style_callback=self.style_callback)
+        self._geojson = ipyleaflet.GeoJSON(
+            data=self._gdf_selected.__geo_interface__,
+            point_style=self._point_style,
+            style_callback=self.style_callback
+        )
         # add GeoJSON object to map
-        self.map.add(self.geojson)
+        self.map.add(self._geojson)
         # fields for tooltip views
         if kwargs['fields'] is None:
-            self.fields = geodataframe.columns.drop(
-                [geodataframe.geometry.name, "data", "color"])
+            self._fields = self._gdf_selected.columns.drop(
+                [self._gdf_selected.geometry.name, "data", "color"])
         else:
-            self.fields = copy.copy(kwargs['fields'])
+            self._fields = copy.copy(kwargs['fields'])
         # add hover tooltips
         if kwargs['tooltip']:
-            self.tooltip = ipywidgets.HTML()
-            self.tooltip.layout.margin = "0px 20px 20px 20px"
-            self.tooltip.layout.visibility = 'hidden'
-            self.tooltip_height = kwargs['tooltip_height']
-            self.tooltip_width = kwargs['tooltip_width']
+            self._tooltip = ipywidgets.HTML()
+            self._tooltip.layout.margin = "0px 20px 20px 20px"
+            self._tooltip.layout.visibility = 'hidden'
+            self._tooltip_height = kwargs['tooltip_height']
+            self._tooltip_width = kwargs['tooltip_width']
             # create widget for hover tooltips
             self.hover_control = ipyleaflet.WidgetControl(
-                widget=self.tooltip,
+                widget=self._tooltip,
                 position='bottomright')
-            self.geojson.on_hover(self.handle_hover)
-            self.geojson.on_msg(self.handle_mouseout)
-            self.geojson.on_click(self.handle_click)
+            self._geojson.on_hover(self.handle_hover)
+            self._geojson.on_msg(self.handle_mouseout)
+            self._geojson.on_click(self.handle_click)
         # add colorbar
-        if kwargs['colorbar']:
-            self.add_colorbar(column_name=self.column_name,
-                cmap=kwargs['cmap'], norm=norm,
-                position=kwargs['position'])
+        self.colorbar = kwargs['colorbar']
+        self.colorbar_position = kwargs['position']
+        if self.colorbar:
+            self.add_colorbar(
+                column_name=self.column_name,
+                cmap=self.cmap,
+                norm=self.norm,
+                position=self.colorbar_position
+            )
 
     # functional call for setting colors of each point
     def style_callback(self, feature):
         """callback for setting marker colors
         """
         return {
             "fillColor": feature["properties"]["color"],
@@ -2554,31 +2588,31 @@
         }
 
     # functional calls for hover events
     def handle_hover(self, feature, **kwargs):
         """callback for creating hover tooltips
         """
         # combine html strings for hover tooltip
-        self.tooltip.value = '<b>{0}:</b> {1}<br>'.format('id',feature['id'])
-        self.tooltip.value += '<br>'.join(['<b>{0}:</b> {1}'.format(field,
-            feature["properties"][field]) for field in self.fields])
-        self.tooltip.layout.width = self.tooltip_width
-        self.tooltip.layout.height = self.tooltip_height
-        self.tooltip.layout.visibility = 'visible'
+        self._tooltip.value = '<b>{0}:</b> {1}<br>'.format('id',feature['id'])
+        self._tooltip.value += '<br>'.join(['<b>{0}:</b> {1}'.format(field,
+            feature["properties"][field]) for field in self._fields])
+        self._tooltip.layout.width = self._tooltip_width
+        self._tooltip.layout.height = self._tooltip_height
+        self._tooltip.layout.visibility = 'visible'
         self.map.add(self.hover_control)
 
     def handle_mouseout(self, _, content, buffers):
         """callback for removing hover tooltips upon mouseout
         """
         event_type = content.get('type', '')
         if event_type == 'mouseout':
-            self.tooltip.value = ''
-            self.tooltip.layout.width = "0px"
-            self.tooltip.layout.height = "0px"
-            self.tooltip.layout.visibility = 'hidden'
+            self._tooltip.value = ''
+            self._tooltip.layout.width = "0px"
+            self._tooltip.layout.height = "0px"
+            self._tooltip.layout.visibility = 'hidden'
             self.map.remove(self.hover_control)
 
     # functional calls for click events
     def handle_click(self, feature, **kwargs):
         """callback for handling mouse clicks
         """
         if self.selected_callback != None:
@@ -2589,21 +2623,21 @@
         """
         self.selected_callback = callback
 
     def handle_region(self, action, **kwargs):
         """callback for handling region deletions
         """
         # remove any prior instances of a data layer
-        if (action == 'deleted') and self.geojson is not None:
-            self.remove(self.geojson)
-            self.geojson = None
+        if (action == 'deleted') and self._geojson is not None:
+            self.remove(self._geojson)
+            self._geojson = None
         # remove any prior instances of a colorbar
-        if (action == 'deleted') and self.colorbar is not None:
-            self.remove(self.colorbar)
-            self.colorbar = None
+        if (action == 'deleted') and self._colorbar is not None:
+            self.remove(self._colorbar)
+            self._colorbar = None
 
     # remove map layers
     def remove(self, layer):
         """wrapper function for removing layers from leaflet maps
         """
         # try to remove layer from map
         try:
@@ -2615,14 +2649,129 @@
             logger.info(f"Control {layer} already removed from map")
             pass
         except Exception as e:
             logger.critical(f"Could not remove layer {layer}")
             logger.error(traceback.format_exc())
             pass
 
+    def get_norm_bounds(self, **kwargs):
+        # set default keyword arguments
+        kwargs.setdefault('vmin', None)
+        kwargs.setdefault('vmax', None)
+        # set colorbar limits to 2-98 percentile
+        # if not using a defined plot range
+        clim = self._gdf_selected['data'].quantile((0.02, 0.98)).values
+        # set minimum for normalization
+        fmin = np.finfo(np.float64).min
+        if (kwargs['vmin'] is None) or np.isclose(kwargs['vmin'], fmin):
+            self.vmin = clim[0]
+            self._dynamic = True
+        else:
+            self.vmin = np.copy(kwargs['vmin'])
+            self._dynamic = False
+        # set maximum for normalization
+        fmax = np.finfo(np.float64).max
+        if (kwargs['vmax'] is None) or np.isclose(kwargs['vmax'], fmax):
+            self.vmax = clim[-1]
+            self._dynamic = True
+        else:
+            self.vmax = np.copy(kwargs['vmax'])
+            self._dynamic = False
+
+    def redraw(self, *args, **kwargs):
+        """
+        Redraw the GeoJSON on the map
+        """
+        # normalize data to be within vmin and vmax
+        normalized = self.norm(self._gdf_selected['data'])
+        # create HEX colors for each point in the dataframe
+        self._gdf_selected["color"] = np.apply_along_axis(colors.to_hex, 1,
+            cm.get_cmap(self.cmap.name, 256)(normalized))
+        # update data within GeoJSON object
+        self._geojson.data = self._gdf_selected.__geo_interface__
+
+    def redraw_colorbar(self, *args, **kwargs):
+        """
+        Redraw the colorbar on the map
+        """
+        try:
+            if self.colorbar:
+                self.add_colorbar(
+                    column_name=self.column_name,
+                    cmap=self.cmap,
+                    norm=self.norm,
+                    position=self.colorbar_position
+                )
+        except Exception as exc:
+            pass
+
+    # observe changes in widget parameters
+    def set_observables(self, widget, **kwargs):
+        """observe changes in widget parameters
+        """
+        # set default keyword arguments
+        # to map widget changes to functions
+        kwargs.setdefault('variable', [self.set_column_name])
+        kwargs.setdefault('cmap', [self.set_colormap])
+        kwargs.setdefault('reverse', [self.set_colormap])
+        # connect each widget with a set function
+        for key, val in kwargs.items():
+            # try to retrieve the functional
+            try:
+                observable = getattr(widget, key)
+            except AttributeError as exc:
+                continue
+            # assert that observable is an ipywidgets object
+            assert isinstance(observable, ipywidgets.widgets.widget.Widget)
+            assert hasattr(observable, 'observe')
+            # for each functional to map
+            for i, functional in enumerate(val):
+                # try to connect the widget to the functional
+                try:
+                    observable.observe(functional)
+                except (AttributeError, NameError, ValueError) as exc:
+                    pass
+
+    def set_column_name(self, sender):
+        """update the dataframe variable for a new selected column
+        """
+        # only update variable if a new final
+        if isinstance(sender['new'], str):
+            self.column_name = sender['new']
+        else:
+            return
+        # reduce to variable
+        self._gdf_selected['data'] = self._gdf_selected[self.column_name]
+        # check if dynamic normalization is enabled
+        if self._dynamic:
+            self.get_norm_bounds()
+            self.norm.vmin = self.vmin
+            self.norm.vmax = self.vmax
+        # try to redraw the selected dataset
+        self.redraw()
+        self.redraw_colorbar()
+
+    def set_colormap(self, sender):
+        """update the colormap for the selected variable
+        """
+        # only update colormap if a new final
+        if isinstance(sender['new'], str):
+            cmap_name = self.cmap.name
+            cmap_reverse_flag = '_r' if cmap_name.endswith('_r') else ''
+            self.cmap = cm.get_cmap(sender['new'] + cmap_reverse_flag)
+        elif isinstance(sender['new'], bool):
+            cmap_name = self.cmap.name.strip('_r')
+            cmap_reverse_flag = '_r' if sender['new'] else ''
+            self.cmap = cm.get_cmap(cmap_name + cmap_reverse_flag)
+        else:
+            return
+        # try to redraw the selected dataset
+        self.redraw()
+        self.redraw_colorbar()
+
     # add colorbar widget to leaflet map
     def add_colorbar(self, **kwargs):
         """Creates colorbars on leaflet maps
 
         Parameters
         ----------
         column_name : str, GeoDataFrame column to plot
@@ -2634,43 +2783,82 @@
         width : float, width of colorbar
         height : float, height of colorbar
         """
         kwargs.setdefault('column_name', 'h_mean')
         kwargs.setdefault('cmap', 'viridis')
         kwargs.setdefault('norm', None)
         kwargs.setdefault('alpha', 1.0)
-        kwargs.setdefault('orientation', 'horizontal')
+        kwargs.setdefault('orientation', 'vertical')
         kwargs.setdefault('position', 'topright')
-        kwargs.setdefault('width', 6.0)
-        kwargs.setdefault('height', 0.4)
+        kwargs.setdefault('width', 0.2)
+        kwargs.setdefault('height', 3.0)
         # remove any prior instances of a colorbar
-        if self.colorbar is not None:
-            self.map.remove(self.colorbar)
-        # colormap for colorbar
-        cmap = cm.get_cmap(kwargs['cmap'])
+        if self._colorbar is not None:
+            self.map.remove(self._colorbar)
         # create matplotlib colorbar
         _, ax = plt.subplots(figsize=(kwargs['width'], kwargs['height']))
-        cbar = matplotlib.colorbar.ColorbarBase(ax, cmap=cmap,
-            norm=kwargs['norm'], alpha=kwargs['alpha'],
+        cbar = matplotlib.colorbar.ColorbarBase(ax,
+            cmap=kwargs['cmap'],
+            norm=kwargs['norm'],
+            alpha=kwargs['alpha'],
             orientation=kwargs['orientation'],
-            label=kwargs['column_name'])
+            label=kwargs['column_name']
+        )
         cbar.solids.set_rasterized(True)
         cbar.ax.tick_params(which='both', width=1, direction='in')
         # save colorbar to in-memory png object
         png = io.BytesIO()
         plt.savefig(png, bbox_inches='tight', format='png')
         png.seek(0)
         # create output widget
         output = ipywidgets.Image(value=png.getvalue(), format='png')
-        self.colorbar = ipyleaflet.WidgetControl(widget=output,
-            transparent_bg=True, position=kwargs['position'])
+        self._colorbar = ipyleaflet.WidgetControl(
+            widget=output,
+            transparent_bg=True,
+            position=kwargs['position']
+        )
         # add colorbar
-        self.map.add(self.colorbar)
+        self.map.add(self._colorbar)
         plt.close()
 
+    @staticmethod
+    def default_atl03_fields():
+        """List of ATL03 tooltip fields
+        """
+        return ['atl03_cnf', 'atl08_class', 'cycle', 'height',
+            'pair', 'rgt', 'segment_id', 'track', 'yapc_score']
+
+    @staticmethod
+    def default_atl06_fields():
+        """List of ATL06-SR tooltip fields
+        """
+        return ['cycle', 'dh_fit_dx', 'gt', 'h_mean',
+            'h_sigma', 'rgt', 'rms_misfit', 'w_surface_window_final']
+
+    @staticmethod
+    def default_atl08_fields():
+        """List of ATL08-SR tooltip fields
+        """
+        return ['canopy_openness', 'cycle', 'gt', 'h_canopy',
+            'h_min_canopy', 'h_mean_canopy',
+            'h_max_canopy', 'h_te_median', 'rgt']
+
+    @staticmethod
+    def default_mosaic_fields(**kwargs):
+        kwargs.setdefault('with_flags', False)
+        kwargs.setdefault('zonal_stats', False)
+        """List of mosaic tooltip fields
+        """
+        columns = ['time','value']
+        if kwargs['with_flags']:
+            columns += ['flags']
+        if kwargs['zonal_stats']:
+            columns += ['count','min','max','mean','median','stdev','mad']
+        return [f'mosaic.{c}' for c in columns]
+
 @gpd.pd.api.extensions.register_dataframe_accessor("icesat2")
 class ICESat2:
     """A geopandas GeoDataFrame extension for plotting ICESat-2 transects
     """
 
     def __init__(self, gdf):
         # initialize geodataframe
```

### Comparing `sliderule-4.3.2/sliderule/raster.py` & `sliderule-4.4.0/sliderule/raster.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/sliderule/sliderule.py` & `sliderule-4.4.0/sliderule/sliderule.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import ctypes
 import time
 import logging
 import warnings
 import numpy
 import geopandas
 from shapely.geometry import Polygon
+from shapely.geometry.multipolygon import MultiPolygon
 from datetime import datetime
 from sliderule import version
 
 ###############################################################################
 # GLOBALS
 ###############################################################################
 
@@ -101,14 +102,23 @@
     0: logger.debug,
     1: logger.info,
     2: logger.warning,
     3: logger.error,
     4: logger.critical
 }
 
+exceptioncodes = {
+    "INFO": 0,
+    "ERROR": -1,
+    "TIMEOUT": -2,
+    "RESOURCE_DOES_NOT_EXIST": -3,
+    "EMPTY_SUBSET": -4,
+    "SIMPLIFY": -5
+}
+
 datatypes = {
     "TEXT":     0,
     "REAL":     1,
     "INTEGER":  2,
     "DYNAMIC":  3
 }
 
@@ -150,14 +160,17 @@
 
 class FatalError(RuntimeError):
     pass
 
 class TransientError(RuntimeError):
     pass
 
+class RetryRequest(RuntimeError):
+    pass
+
 ###############################################################################
 # UTILITIES
 ###############################################################################
 
 #
 # __StreamSource
 #
@@ -437,21 +450,23 @@
 # Default Record Processing
 ###############################################################################
 
 #
 #  __logeventrec
 #
 def __logeventrec(rec):
-    eventlogger[rec['level']]('%s' % (rec["attr"]))
+    eventlogger[rec['level']]('Log <%s, %d>: %s' % (rec["name"], rec["time"], rec["attr"]))
 
 #
 #  __exceptrec
 #
 def __exceptrec(rec):
-    if rec["code"] >= 0:
+    if rec["code"] == exceptioncodes["SIMPLIFY"]:
+        raise RetryRequest("cmr simplification requested")
+    elif rec["code"] < 0:
         eventlogger[rec["level"]]("Exception <%d>: %s", rec["code"], rec["text"])
     else:
         eventlogger[rec["level"]]("%s", rec["text"])
 
 #
 #  _arrowrec
 #
@@ -560,14 +575,17 @@
         if output["format"] == "parquet":
             if "as_geo" in output and not output["as_geo"]:
                 # Return Parquet File as DataFrame
                 return geopandas.pd.read_parquet(path)
             else:
                 # Return GeoParquet File as GeoDataFrame
                 return geopandas.read_parquet(path)
+        elif output["format"] == "feather":
+            # Return Feather File as DataFrame
+            return geopandas.pd.read_feather(path)
         elif output["format"] == "csv":
             # Return CSV File as DataFrame
             return geopandas.pd.read_csv(path)
         else:
             raise FatalError('unsupported output format: %s' % (output["format"]))
     else:
         # Return Parquet Filename
@@ -598,15 +616,15 @@
 def todataframe(columns, time_key="time", lon_key="longitude", lat_key="latitude", height_key=None, **kwargs):
 
     # Latch Start Time
     tstart = time.perf_counter()
 
     # Set Default Keyword Arguments
     kwargs['index_key'] = "time"
-    kwargs['crs'] = SLIDERULE_EPSG 
+    kwargs['crs'] = SLIDERULE_EPSG
 
     # Check Empty Columns
     if len(columns) <= 0:
         return emptyframe(**kwargs)
 
     # Generate Time Column
     columns['time'] = columns[time_key].astype('datetime64[ns]')
@@ -639,14 +657,46 @@
 
     # Update Profile
     profiles[todataframe.__name__] = time.perf_counter() - tstart
 
     # Return GeoDataFrame
     return gdf
 
+#
+# Simplify Polygon
+#
+def simplifypolygon(parm):
+    if "parms" not in parm:
+        return
+    
+    if "cmr" in parm["parms"]:
+        polygon = parm["parms"]["cmr"]["polygon"]
+    elif "poly" in parm["parms"]:
+        polygon = parm["parms"]["poly"]
+    else:
+        return
+
+    tolerance = 0.01
+    raw_multi_polygon = [[(tuple([(c['lon'], c['lat']) for c in polygon]), [])]]
+    shape = MultiPolygon(*raw_multi_polygon)
+    buffered_shape = shape.buffer(tolerance)
+    simplified_shape = buffered_shape.simplify(tolerance)
+    simplified_coords = list(simplified_shape.exterior.coords)
+
+    simplified_polygon = []
+    for coord in simplified_coords:
+        point = {"lon": coord[0], "lat": coord[1]}
+        simplified_polygon.insert(0, point)
+
+    if "cmr" not in parm["parms"]:
+        parm["parms"]["cmr"] = {}                    
+    parm["parms"]["cmr"]["polygon"] = simplified_polygon
+    
+    logger.warning('Using simplified polygon (for CMR request only!), {} points using tolerance of {}'.format(len(simplified_coords), tolerance))
+
 ###############################################################################
 # APIs
 ###############################################################################
 
 #
 #  Initialize
 #
@@ -731,27 +781,28 @@
         ...     "output": "GPS"
         ... }
         >>> rsps = sliderule.source("time", rqst)
         >>> print(rsps)
         {'time': 1300556199523.0, 'format': 'GPS'}
     '''
     global service_url, service_org
-    rqst = json.dumps(parm)
     rsps = {}
     headers = None
     # Build Callbacks
     for c in __callbacks:
         if c not in callbacks:
             callbacks[c] = __callbacks[c]
     # Attempt Request
     complete = False
     attempts = 3
     while not complete and attempts > 0:
         attempts -= 1
         try:
+            # Dump Parameters to Request JSON String
+            rqst = json.dumps(parm)
             # Construct Request URL and Authorization
             if service_org:
                 url = 'https://%s.%s%s/%s' % (service_org, service_url, path, api)
                 headers = buildauthheader()
             else:
                 url = 'http://%s%s/%s' % (service_url, path, api)
             # Perform Request
@@ -769,14 +820,17 @@
                 rsps = __parse_json(stream)
             elif format == 'application/octet-stream':
                 rsps = __parse_native(stream, callbacks)
             else:
                 raise FatalError('unsupported content type: %s' % (format))
             # Success
             complete = True
+        except RetryRequest as e:
+            logger.info("Retry requested by {}: {}".format(url, e))
+            simplifypolygon(parm)
         except requests.exceptions.SSLError as e:
             logger.debug("Exception in request to {}: {}".format(url, e))
             if not silence:
                 logger.error("Unable to verify SSL certificate for {} ...retrying request".format(url))
         except requests.ConnectionError as e:
             logger.debug("Exception in request to {}: {}".format(url, e))
             if not silence:
@@ -828,15 +882,15 @@
 #
 #  set_verbose
 #
 def set_verbose (enable, loglevel=logging.INFO):
     '''
     Sets up a console logger to print log messages to screen
 
-    If you want more control over the behavior of the log messages being captured, do not call this function but instead 
+    If you want more control over the behavior of the log messages being captured, do not call this function but instead
     create and configure a Python log handler of your own and attach it to `sliderule.logger`.
 
     Parameters
     ----------
         enable:     bool
                     True: creates console logger if it doesn't exist, False: destroys console logger if it does exist
 
@@ -1293,18 +1347,18 @@
     -------
     dict
         a list of longitudes and latitudes containing the region of interest that can be used for the **poly** and **raster** parameters in a processing request to SlideRule.
 
         region = {
 
             "gdf": <GeoDataFrame of region>
-            
-            "poly": [{"lat": <lat1>, "lon": <lon1> }, ...], 
-            
-            "raster": {"data": <geojson file as string>, 
+
+            "poly": [{"lat": <lat1>, "lon": <lon1> }, ...],
+
+            "raster": {"data": <geojson file as string>,
 
             "clusters": [[{"lat": <lat1>, "lon": <lon1>}, ...], [{"lat": <lat1>, "lon": <lon1>}, ...]] }
 
     Examples
     --------
     >>> import sliderule, json
     >>> region = sliderule.toregion("tests/data/grandmesa.geojson")
@@ -1342,15 +1396,15 @@
             "lon": -108.2878686387796,
             "lat": 38.89051431295789
         },
         {
             "lon": -108.20772968780051,
             "lat": 38.8232055291981
         }
-    ]    
+    ]
     '''
 
     tstart = time.perf_counter()
     tempfile = "temp.geojson"
 
     if isinstance(source, geopandas.GeoDataFrame):
         # user provided GeoDataFrame instead of a file
```

### Comparing `sliderule-4.3.2/sliderule/swot.py` & `sliderule-4.4.0/sliderule/swot.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,17 +126,14 @@
         tstart = time.perf_counter()
 
         # Default the Asset
         rqst_parm = parm.copy()
         if "asset" not in rqst_parm:
             rqst_parm["asset"] = "swot-sim-ecco-llc4320"
 
-        # Get List of Resources from CMR (if not supplied)
-        resources = earthdata.search(rqst_parm, resources)
-
         # Build GEDI Request
         rqst = {
             "resources": resources,
             "parms": rqst_parm
         }
 
         # Make API Processing Request
```

### Comparing `sliderule-4.3.2/sliderule.egg-info/PKG-INFO` & `sliderule-4.4.0/sliderule.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 4.3.2
+Version: 4.4.0
 Summary: Python client for interacting with sliderule server
-Home-page: https://github.com/ICESat2-SlideRule/sliderule/
+Home-page: https://github.com/SlideRuleEarth/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sliderule-4.3.2/utils/bathy_runner.py` & `sliderule-4.4.0/utils/bathy_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from sliderule import sliderule, icesat2
 import argparse
 import os
 
 # Command Line Arguments
 parser = argparse.ArgumentParser(description="""ATL24""")
-parser.add_argument('--output',         '-f',   type=str,               default="bathy.csv")
-parser.add_argument('--granule',        '-g',   type=str,               default="ATL03_20181223171641_13150101_006_02.h5")
-parser.add_argument('--aoi',            '-a',   type=str,               default="tests/data/bahia_de_jiguey.geojson")
+parser.add_argument('--granule',        '-g',   type=str,               default="ATL03_20190604044922_10220307_006_02.h5")
+parser.add_argument('--aoi',            '-a',   type=str,               default="tests/data/tarawa.geojson")
 parser.add_argument('--track',          '-t',   type=int,               default=1)
+parser.add_argument('--spots',          '-e',   type=int, nargs='+',    choices=range(1,7), default=[1,2,3,4,5,6])
 parser.add_argument('--domain',         '-d',   type=str,               default="slideruleearth.io")
 parser.add_argument('--organization',   '-o',   type=str,               default="bathy")
 parser.add_argument('--desired_nodes',  '-n',   type=int,               default=None)
 parser.add_argument('--time_to_live',   '-m',   type=int,               default=120)
+parser.add_argument('--timeout',        '-x',   type=int,               default=800)
 parser.add_argument('--verbose',        '-v',   action='store_true',    default=False)
 parser.add_argument('--loglvl',         '-l',   type=str,               default="INFO")
 parser.add_argument('--preserve',       '-p',   action='store_true',    default=False)
-parser.add_argument('--serverfile',     '-s',   type=str,               default="/tmp/bathyfile.csv")
+parser.add_argument('--serverfile',     '-s',   type=str,               default="/tmp/ATL24_20190604044922_10220307_006_02.h5")
+parser.add_argument('--return_inputs',  '-i',   action='store_true',    default=False)
+parser.add_argument('--send_to_client', '-c',   action='store_true',    default=False)
+parser.add_argument('--generate_ndwi',  '-w',   action='store_true',    default=False)
+parser.add_argument('--use_bathy_mask', '-b',   action='store_true',    default=False)
 args,_ = parser.parse_known_args()
 
 # Initialize Organization
 if args.organization == "None":
     args.organization = None
     args.desired_nodes = None
     args.time_to_live = None
@@ -29,33 +34,39 @@
 
 # Generate Region Polygon
 region = sliderule.toregion(args.aoi)
 
 # Set Parameters
 parms = { 
     "poly": region['poly'],
+    "srt": icesat2.SRT_DYNAMIC,
     "cnf": "atl03_not_considered",
     "pass_invalid": True,
-    "beam_file_prefix": "bathy",
-    "output": { 
+    "generate_ndwi": args.generate_ndwi,
+    "use_bathy_mask": args.use_bathy_mask,
+    "return_inputs": args.return_inputs,
+    "timeout": args.timeout,
+    "spots": args.spots,
+    "openoceans": {
+        "res_along_track": 10,
+        "res_z": 0.2,
+        "window_size": 11,
+        "range_z": [-50, 30],
+        "verbose": False,
+        "photon_bins": False,
+        "use_ndwi": args.generate_ndwi
+    }
+}
+if args.send_to_client:
+    parms["output"] = { 
         "path": args.serverfile, 
-        "format": "csv", 
-        "open_on_complete": True, 
+        "format": "hdf5", 
+        "open_on_complete": False, 
         "as_geo": False 
-    } 
-}
+    }
 
 # Make ATL24G Processing Request
 gdf = icesat2.atl24gp(parms, resources=[args.granule], keep_id=True)
 
-# Write to CSV Local File
-columns = [
-    "index_ph", "time", "geoid_corr_h", "latitude", "longitude", "x_ph", "y_ph", "x_atc", "y_atc", 
-    "sigma_along", "sigma_across", "ndwi", "yapc_score", "max_signal_conf", "quality_ph",
-    "region", "track", "pair", "sc_orient", "rgt", "cycle", "utm_zone", 
-    "background_rate", "solar_elevation", "wind_v", "pointing_angle", "extent_id" 
-]
-gdf.to_csv(args.output, index=False, columns=columns)
-
 # Clean Up Temporary Files
-if not args.preserve:
-    os.remove(args.serverfile)
+if args.send_to_client and not args.preserve:
+    os.remove(args.serverfile)
```

### Comparing `sliderule-4.3.2/utils/benchmark.py` & `sliderule-4.4.0/utils/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 # Imports
 import sliderule
 from sliderule import earthdata, h5, icesat2, gedi
 import argparse
-import logging
 import time
 import os
 
 # Command Line Arguments
 parser = argparse.ArgumentParser(description="""Subset granules""")
 parser.add_argument('--benchmarks',     '-b',   nargs='+', type=str,    default=[])
 parser.add_argument('--granule03',      '-p',   type=str,               default="ATL03_20181017222812_02950102_005_01.h5")
```

### Comparing `sliderule-4.3.2/utils/big_query.py` & `sliderule-4.4.0/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/create_geojson.py` & `sliderule-4.4.0/utils/create_geojson.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/extract_h5_dataset.py` & `sliderule-4.4.0/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/icepyx_region.py` & `sliderule-4.4.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/lpdaac_download.py` & `sliderule-4.4.0/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/monitor.py` & `sliderule-4.4.0/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/opendata_worldcover.py` & `sliderule-4.4.0/utils/opendata_worldcover.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/query_cmr.py` & `sliderule-4.4.0/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/query_elevations.py` & `sliderule-4.4.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/query_metrics.py` & `sliderule-4.4.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/query_photons.py` & `sliderule-4.4.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/query_stac.py` & `sliderule-4.4.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/query_version.py` & `sliderule-4.4.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/region_of_interest.py` & `sliderule-4.4.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/results_to_s3.py` & `sliderule-4.4.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/stac.py` & `sliderule-4.4.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/stream_events.py` & `sliderule-4.4.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/tail_events.py` & `sliderule-4.4.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.2/utils/utils.py` & `sliderule-4.4.0/utils/utils.py`

 * *Files identical despite different names*

