# Comparing `tmp/pluma_analysis-0.5.0.tar.gz` & `tmp/pluma_analysis-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluma_analysis-0.5.0.tar", last modified: Thu May  2 09:16:39 2024, max compression
+gzip compressed data, was "pluma_analysis-0.6.0.tar", last modified: Fri May  3 12:58:14 2024, max compression
```

## Comparing `pluma_analysis-0.5.0.tar` & `pluma_analysis-0.6.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.566853 pluma_analysis-0.5.0/
--rw-rw-rw-   0        0        0       78 2024-01-04 11:17:02.000000 pluma_analysis-0.5.0/.gitignore
--rw-rw-rw-   0        0        0     1092 2022-11-21 15:02:54.000000 pluma_analysis-0.5.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-08-12 12:33:04.000000 pluma_analysis-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2554 2024-05-02 09:16:39.565854 pluma_analysis-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-05-02 08:57:11.000000 pluma_analysis-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.367099 pluma_analysis-0.5.0/pluma/
--rw-rw-rw-   0        0        0        0 2023-08-12 12:33:04.000000 pluma_analysis-0.5.0/pluma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.379641 pluma_analysis-0.5.0/pluma/export/
--rw-rw-rw-   0        0        0     2146 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/export/maps.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.383488 pluma_analysis-0.5.0/pluma/export/ogcapi/
--rw-rw-rw-   0        0        0     3254 2024-04-05 03:04:27.000000 pluma_analysis-0.5.0/pluma/export/ogcapi/features.py
--rw-rw-rw-   0        0        0     2465 2024-04-05 03:03:44.000000 pluma_analysis-0.5.0/pluma/export/ogcapi/records.py
--rw-rw-rw-   0        0        0     6426 2024-04-05 03:04:11.000000 pluma_analysis-0.5.0/pluma/export/streams.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.429244 pluma_analysis-0.5.0/pluma/io/
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.439538 pluma_analysis-0.5.0/pluma/io/_nepy/
--rw-rw-rw-   0        0        0    18315 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/_nepy/NedfReader.py
--rw-rw-rw-   0        0        0     2006 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/accelerometer.py
--rw-rw-rw-   0        0        0     4605 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/eeg.py
--rw-rw-rw-   0        0        0     3317 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/empatica.py
--rw-rw-rw-   0        0        0     3494 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/harp.py
--rw-rw-rw-   0        0        0     1442 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/microphone.py
--rw-rw-rw-   0        0        0     3777 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/path_helper.py
--rw-rw-rw-   0        0        0     6800 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/ubx.py
--rw-rw-rw-   0        0        0     1046 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/io/zeromq.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.445538 pluma_analysis-0.5.0/pluma/preprocessing/
--rw-rw-rw-   0        0        0     2107 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/preprocessing/ecg.py
--rw-rw-rw-   0        0        0     2401 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/preprocessing/resampling.py
--rw-rw-rw-   0        0        0      511 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/preprocessing/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.457545 pluma_analysis-0.5.0/pluma/schema/
--rw-rw-rw-   0        0        0    10132 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/schema/__init__.py
--rw-rw-rw-   0        0        0    11160 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/schema/outdoor.py
--rw-rw-rw-   0        0        0    12228 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/schema/vr.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.522901 pluma_analysis-0.5.0/pluma/stream/
--rw-rw-rw-   0        0        0     3016 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/stream/__init__.py
--rw-rw-rw-   0        0        0     1857 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/accelerometer.py
--rw-rw-rw-   0        0        0     1468 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/csv.py
--rw-rw-rw-   0        0        0     1733 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/eeg.py
--rw-rw-rw-   0        0        0      947 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/empatica.py
--rw-rw-rw-   0        0        0     6626 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/georeference.py
--rw-rw-rw-   0        0        0     2298 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/harp.py
--rw-rw-rw-   0        0        0     1097 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/microphone.py
--rw-rw-rw-   0        0        0     1578 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/siconversion.py
--rw-rw-rw-   0        0        0     3023 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/ubx.py
--rw-rw-rw-   0        0        0     6408 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/stream/zeromq.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.526452 pluma_analysis-0.5.0/pluma/sync/
--rw-rw-rw-   0        0        0     2049 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/sync/__init__.py
--rw-rw-rw-   0        0        0     7370 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/sync/ubx2harp.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.528452 pluma_analysis-0.5.0/pluma/templates/
--rw-rw-rw-   0        0        0     2980 2024-01-04 11:17:02.000000 pluma_analysis-0.5.0/pluma/templates/metadata_template.j2
-drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.563853 pluma_analysis-0.5.0/pluma_analysis.egg-info/
--rw-rw-rw-   0        0        0     2554 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1545 2024-05-02 08:55:22.000000 pluma_analysis-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 09:16:39.567855 pluma_analysis-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.129819 pluma_analysis-0.6.0/
+-rw-rw-rw-   0        0        0       78 2024-01-04 11:17:02.000000 pluma_analysis-0.6.0/.gitignore
+-rw-rw-rw-   0        0        0     1092 2022-11-21 15:02:54.000000 pluma_analysis-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-08-12 12:33:04.000000 pluma_analysis-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2554 2024-05-03 12:58:14.127819 pluma_analysis-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-03 12:56:42.000000 pluma_analysis-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.972980 pluma_analysis-0.6.0/pluma/
+-rw-rw-rw-   0        0        0        0 2023-08-12 12:33:04.000000 pluma_analysis-0.6.0/pluma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.975485 pluma_analysis-0.6.0/pluma/export/
+-rw-rw-rw-   0        0        0     2334 2024-05-03 12:20:23.000000 pluma_analysis-0.6.0/pluma/export/maps.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.979503 pluma_analysis-0.6.0/pluma/export/ogcapi/
+-rw-rw-rw-   0        0        0     2988 2024-05-03 12:33:39.000000 pluma_analysis-0.6.0/pluma/export/ogcapi/features.py
+-rw-rw-rw-   0        0        0     2465 2024-04-05 03:03:44.000000 pluma_analysis-0.6.0/pluma/export/ogcapi/records.py
+-rw-rw-rw-   0        0        0     6426 2024-04-05 03:04:11.000000 pluma_analysis-0.6.0/pluma/export/streams.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.998071 pluma_analysis-0.6.0/pluma/io/
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.002069 pluma_analysis-0.6.0/pluma/io/_nepy/
+-rw-rw-rw-   0        0        0    18315 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/_nepy/NedfReader.py
+-rw-rw-rw-   0        0        0     2006 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/accelerometer.py
+-rw-rw-rw-   0        0        0     4605 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/eeg.py
+-rw-rw-rw-   0        0        0     3317 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/empatica.py
+-rw-rw-rw-   0        0        0     3494 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/harp.py
+-rw-rw-rw-   0        0        0     1442 2024-05-03 12:22:48.000000 pluma_analysis-0.6.0/pluma/io/microphone.py
+-rw-rw-rw-   0        0        0     3777 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/path_helper.py
+-rw-rw-rw-   0        0        0     6800 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/ubx.py
+-rw-rw-rw-   0        0        0     1046 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/io/zeromq.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.013594 pluma_analysis-0.6.0/pluma/preprocessing/
+-rw-rw-rw-   0        0        0     2107 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/preprocessing/ecg.py
+-rw-rw-rw-   0        0        0     2401 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/preprocessing/resampling.py
+-rw-rw-rw-   0        0        0      511 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/preprocessing/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.039152 pluma_analysis-0.6.0/pluma/schema/
+-rw-rw-rw-   0        0        0    11227 2024-05-03 12:51:39.000000 pluma_analysis-0.6.0/pluma/schema/__init__.py
+-rw-rw-rw-   0        0        0    11160 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/schema/outdoor.py
+-rw-rw-rw-   0        0        0    12228 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/schema/vr.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.071719 pluma_analysis-0.6.0/pluma/stream/
+-rw-rw-rw-   0        0        0     3076 2024-05-03 11:22:24.000000 pluma_analysis-0.6.0/pluma/stream/__init__.py
+-rw-rw-rw-   0        0        0     1857 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/accelerometer.py
+-rw-rw-rw-   0        0        0     1468 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/csv.py
+-rw-rw-rw-   0        0        0     1733 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/eeg.py
+-rw-rw-rw-   0        0        0      947 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/empatica.py
+-rw-rw-rw-   0        0        0     6626 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/georeference.py
+-rw-rw-rw-   0        0        0     2298 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/harp.py
+-rw-rw-rw-   0        0        0     1097 2024-05-03 11:07:19.000000 pluma_analysis-0.6.0/pluma/stream/microphone.py
+-rw-rw-rw-   0        0        0     1578 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/siconversion.py
+-rw-rw-rw-   0        0        0     3023 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/ubx.py
+-rw-rw-rw-   0        0        0     6408 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/stream/zeromq.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.082241 pluma_analysis-0.6.0/pluma/sync/
+-rw-rw-rw-   0        0        0     2049 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/sync/__init__.py
+-rw-rw-rw-   0        0        0     1337 2024-05-02 13:12:29.000000 pluma_analysis-0.6.0/pluma/sync/plotting.py
+-rw-rw-rw-   0        0        0     6918 2024-05-03 00:07:30.000000 pluma_analysis-0.6.0/pluma/sync/ubx2harp.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.085240 pluma_analysis-0.6.0/pluma/templates/
+-rw-rw-rw-   0        0        0     2980 2024-01-04 11:17:02.000000 pluma_analysis-0.6.0/pluma/templates/metadata_template.j2
+drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.125810 pluma_analysis-0.6.0/pluma_analysis.egg-info/
+-rw-rw-rw-   0        0        0     2554 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1094 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1545 2024-05-02 08:55:22.000000 pluma_analysis-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 12:58:14.129819 pluma_analysis-0.6.0/setup.cfg
```

### Comparing `pluma_analysis-0.5.0/LICENSE` & `pluma_analysis-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/PKG-INFO` & `pluma_analysis-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluma-analysis
-Version: 0.5.0
+Version: 0.6.0
 Summary: A low-level interface to data collected with the pluma urban data acquisition system
 Author-email: Goncalo Lopes <g.lopes@neurogears.org>, Bruno Cruz <b.cruz@neurogears.org>, Andrew Erskine <a.erskine@neurogears.org>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/emotional-cities/pluma-analysis/issues
 Project-URL: Source Code, https://github.com/emotional-cities/pluma-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `pluma_analysis-0.5.0/README.md` & `pluma_analysis-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/export/maps.py` & `pluma_analysis-0.6.0/pluma/export/maps.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,36 +5,43 @@
 import pandas as pd
 import simplekml
 
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 
 def showmap(NavData,
+            fig=None,
+            ax=None,
             figsize=(20, 20),
             with_scaling=0.6,
-            to_aspect=(4/3),
+            to_aspect=None,
             tiles=tmb.tiles.build_OSM(),
             cmap='jet',
             markersize=15,
             colorscale_override=None,
-            **figkwargs):
+            **cbarkwargs):
 
     if 'Data' not in NavData.columns:
         raise ValueError(
             'NavData input must have a "Data" Column.\
                 See Stream.resample_temporospatial() for an example.')
 
-    fig, ax = plt.subplots(1, 1)
-    fig.set_size_inches(figsize)
+    if fig is None:
+        fig, ax = plt.subplots(1, 1)
+        fig.set_size_inches(figsize)
+    
     extent = tmb.Extent.from_lonlat(
         np.min(NavData['Longitude'].values),
         np.max(NavData['Longitude'].values),
         np.min(NavData['Latitude'].values),
         np.max(NavData['Latitude'].values))
-    extent = extent.to_aspect(to_aspect).with_scaling(with_scaling)
+    if to_aspect is not None:
+        extent = extent.to_aspect(to_aspect)
+    if with_scaling is not None:
+        extent = extent.with_scaling(with_scaling)
     ax.xaxis.set_visible(False)
     ax.yaxis.set_visible(False)
     ax.set_ylabel("Value")
     ax.set_xlabel("Time")
     plotter = tmb.Plotter(extent, tiles, width=600)
     plotter.plot(ax)
 
@@ -50,15 +57,15 @@
     im = ax.scatter(
         x, y,
         c=colorscale_override,
         s=markersize,
         cmap=cmap)
     divider = make_axes_locatable(ax)
     cax = divider.append_axes("right", size="5%", pad=0.05)
-    fig.colorbar(im, cax=cax)
+    fig.colorbar(im, cax=cax, **cbarkwargs)
     return fig
 
 
 def export_kml_line(df: pd.DataFrame,
                     output_path: str = "walk.kml",
                     **kwargs):
     kml = simplekml.Kml()
```

### Comparing `pluma_analysis-0.5.0/pluma/export/ogcapi/records.py` & `pluma_analysis-0.6.0/pluma/export/ogcapi/records.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/export/streams.py` & `pluma_analysis-0.6.0/pluma/export/streams.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/_nepy/NedfReader.py` & `pluma_analysis-0.6.0/pluma/io/_nepy/NedfReader.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/accelerometer.py` & `pluma_analysis-0.6.0/pluma/io/accelerometer.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/eeg.py` & `pluma_analysis-0.6.0/pluma/io/eeg.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/empatica.py` & `pluma_analysis-0.6.0/pluma/io/empatica.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/harp.py` & `pluma_analysis-0.6.0/pluma/io/harp.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/microphone.py` & `pluma_analysis-0.6.0/pluma/io/microphone.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/path_helper.py` & `pluma_analysis-0.6.0/pluma/io/path_helper.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/ubx.py` & `pluma_analysis-0.6.0/pluma/io/ubx.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/io/zeromq.py` & `pluma_analysis-0.6.0/pluma/io/zeromq.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/preprocessing/ecg.py` & `pluma_analysis-0.6.0/pluma/preprocessing/ecg.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/preprocessing/resampling.py` & `pluma_analysis-0.6.0/pluma/preprocessing/resampling.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/schema/__init__.py` & `pluma_analysis-0.6.0/pluma/schema/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 
 from dotmap import DotMap
 from typing import Union, Optional, Callable
 
 from pluma.schema.outdoor import build_schema
 
-from pluma.sync.ubx2harp import get_clockcalibration_ubx_to_harp_clock
+from pluma.sync.ubx2harp import SyncLookup, get_clockcalibration_model, get_clockcalibration_lookup
 from pluma.sync import ClockRefId
 
 from pluma.stream import StreamType, Stream
 
 from pluma.export import maps
 from pluma.export.ogcapi.features import convert_dataset_to_geoframe, export_dataset_to_geojson
 
@@ -42,15 +42,15 @@
         self.georeference = georeference
         self.schema = schema
         self.streams = None
         self.has_calibration = False
 
     def add_ubx_georeference(self,
                              ubxstream: UbxStream = None,
-                             event: str = "NAV-HPPOSLLH",
+                             event: str = _UBX_MSGIDS.NAV_HPPOSLLH,
                              calibrate_clock: bool = True,
                              strip=True):
         """_summary_
 
         Args:
             ubxstream (UbxStream, optional): UBX stream that will be used to automatically\
                 generate a valid NavData. Defaults to None.
@@ -79,43 +79,44 @@
         self.georeference.from_dataframe(navdata)
         if strip is True:
             self.georeference.strip()
         if calibrate_clock is True:
             self.georeference.clockreference.referenceid =\
                 ubxstream.clockreference.referenceid
 
-    def reload_streams(self,
-                       schema: Union[DotMap, Stream, None] = None,
-                       force_load: bool = False) -> None:
+    @staticmethod    
+    def _iter_schema_streams(schema: Union[DotMap, Stream, None] = None):
+        if isinstance(schema, Stream):
+            yield schema
+        elif isinstance(schema, DotMap):
+            for _stream in schema.values():
+                for _nested in Dataset._iter_schema_streams(_stream):
+                    yield _nested
+        else:
+            raise TypeError(f"Invalid type was found. Must be of \
+                            {Union[DotMap, Stream]}")
+
+    def reload_streams(self, force_load: bool = False) -> None:
         """Recursively loads, from disk , all available streams in the streams' schema
 
         Args:
             schema (Union[DotMap, Stream, None]): Target schema to reload. \
                 If None it will default to the Dataset.streams schema. Defaults to None.
             force_load (bool, optional): If True, it will attempt to load any stream found,\
                 ignoring the stream.autoload value. Defaults to False.
         Raises:
             TypeError: An error is raised if a not allowed type is passed.
         """
 
-        if schema is None:
-            schema = self.streams
-
-        if isinstance(schema, Stream):
+        for stream in self._iter_schema_streams(self.streams):
             if force_load is True:
-                schema.load()
+                stream.load()
             else:
-                if schema.autoload is True:
-                    schema.load()
-        elif isinstance(schema, DotMap):
-            for _stream in schema.values():
-                self.reload_streams(_stream, force_load=force_load)
-        else:
-            raise TypeError(f"Invalid type was found. Must be of \
-                            {Union[DotMap, Stream]}")
+                if stream.autoload is True:
+                    stream.load()
 
     @staticmethod
     def import_dataset(filename: Union[str, ComplexPath]) -> Dataset:
         path = ensure_complexpath(filename)
         with path.open('rb') as handle:
             return pickle.load(handle)
 
@@ -188,59 +189,85 @@
             root=root,
             parent_dataset=self,
             autoload=autoload)
 
     def calibrate_ubx_to_harp(self,
                               dt_error: float = 0.002,
                               plot_diagnosis: bool = False,
-                              r2_min_qc: float = 0.99):
+                              r2_min_qc: float = 0.99) -> SyncLookup:
         """Attempts to calibrate the ubx clock to harp clock using\
             the synchronization pulses as a reference.
 
         Args:
             dt_error (float, optional): Allowed error between the derivative\
                 of timestamps detected in the two streams. Defaults to 0.002 seconds.
             plot_diagnosis (bool, optional): If True plots the output of\
                 the syncing algorithm. Defaults to False.
             r2_min_qc (float, optional): Quality control parameter.
             If < r2_min_qc, an error will be raised, since it likely\
                 results from an automatic correction procedure. Defaults to 0.99.
         """
 
-        model = get_clockcalibration_ubx_to_harp_clock(
-                ubx_stream=self.streams.UBX,
-                harp_sync=self.streams.BioData.Set.data,
-                dt_error=dt_error,
-                r2_min_qc=r2_min_qc,
-                plot_diagnosis=plot_diagnosis)
+        sync_lookup = get_clockcalibration_lookup(
+            ubx_stream=self.streams.UBX,
+            harp_sync=self.streams.BioData.Set.data,
+            dt_error=dt_error,
+            plot_diagnosis=plot_diagnosis
+        )
+
+        model = get_clockcalibration_model(
+            sync_lookup=sync_lookup,
+            r2_min_qc=r2_min_qc
+        )
 
         self.streams.UBX.clockreference.set_conversion_model(
             model=model,
             reference_from=ClockRefId.HARP)
         self.has_calibration = True
+        return sync_lookup
 
     def showmap(self, **kwargs):
         """Overload to export.showmap that shows spatial information color-coded by time.
         """
         temp_df = self.georeference.spacetime.assign(Data=1)
         fig = maps.showmap(temp_df, **kwargs)
         return fig
 
-    def add_georeference_and_calibrate(self):
+    def add_georeference_and_calibrate(self, plot_diagnosis=True):
         if self.has_calibration is False:
-            self.calibrate_ubx_to_harp(plot_diagnosis=True, dt_error=1)
+            self.calibrate_ubx_to_harp(plot_diagnosis=plot_diagnosis, dt_error=1)
             self.add_ubx_georeference(event=_UBX_MSGIDS.NAV_HPPOSLLH,
                                     calibrate_clock=True)
             self.has_calibration = True
         else:
             raise AssertionError('Dataset is already been automatically calibrated.')
         
+    @staticmethod
+    def _offset_data_index(data, offset):
+        if isinstance(data, DotMap):
+            for frame in data.values():
+                Dataset._offset_data_index(frame, offset)
+        else:
+            data.index += offset - data.index[0]
+        
+    def reference_harp_to_ubx_time(self):
+        if self.has_calibration is False:
+            raise AssertionError('Dataset is not calibrated to UBX time.')
+
+        utc_offset = self.streams.UBX.positiondata['Time_UTC'][0]
+        Dataset._offset_data_index(self.georeference.spacetime, utc_offset)
+        Dataset._offset_data_index(self.georeference.time, utc_offset)
+        for stream in self._iter_schema_streams(self.streams):
+            if len(stream.data) == 0:
+                continue
+            if stream.clockreference.referenceid == ClockRefId.HARP:
+                Dataset._offset_data_index(stream.data, utc_offset)
+                stream.clockreference.referenceid = ClockRefId.GNSS
+        
     def to_geoframe(self,
-                    sampling_dt: datetime.timedelta = datetime.timedelta(seconds=1),
-                    rereference_to_ubx_time: bool = False):
-        return convert_dataset_to_geoframe(self, sampling_dt, rereference_to_ubx_time)
+                    sampling_dt: datetime.timedelta = datetime.timedelta(seconds=1)):
+        return convert_dataset_to_geoframe(self, sampling_dt)
 
     def to_geojson(self,
                    filename,
-                   sampling_dt: datetime.timedelta = datetime.timedelta(seconds=1),
-                   rereference_to_ubx_time: bool = False):
-        export_dataset_to_geojson(self, filename, sampling_dt, rereference_to_ubx_time)
+                   sampling_dt: datetime.timedelta = datetime.timedelta(seconds=1)):
+        export_dataset_to_geojson(self, filename, sampling_dt)
```

### Comparing `pluma_analysis-0.5.0/pluma/schema/outdoor.py` & `pluma_analysis-0.6.0/pluma/schema/outdoor.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/schema/vr.py` & `pluma_analysis-0.6.0/pluma/schema/vr.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/__init__.py` & `pluma_analysis-0.6.0/pluma/stream/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,26 +24,29 @@
 	"""Based class for all stream types
 	"""
 	def __init__(self,
               device: str,
               streamlabel: str,
               root: Union[str, ComplexPath] = '',
               data: any = None,
-              clockreference: ClockReference=ClockReference(referenceid=ClockRefId.NONE),
+              clockreference: ClockReference = None,
 			  parent_dataset=None,
 			  autoload: bool = True):
 		"""_summary_
 		Args:
 			device (str): Device label
 			streamlabel (str): Stream label
 			root (Union[str, ComplexPath], optional): Root path where the files of the stream are expected to be found. Defaults to ''.
 			data (any, optional): Data to initially populate the stream. Defaults to None.
    			autoload (bool, optional): If True, it will attempt to automatically load the data when instantiated. Defaults to True.
 		"""
 
+		if clockreference is None:
+			clockreference = ClockReference(referenceid=ClockRefId.NONE)
+
 		self.device = device
 		self.streamlabel = streamlabel
 		self._rootfolder = self.rootfolder = root
 		self.data = data
 		self.clockreference = clockreference
 		self.parent_dataset = parent_dataset
 		self.autoload = autoload
```

### Comparing `pluma_analysis-0.5.0/pluma/stream/accelerometer.py` & `pluma_analysis-0.6.0/pluma/stream/accelerometer.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/csv.py` & `pluma_analysis-0.6.0/pluma/stream/csv.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/eeg.py` & `pluma_analysis-0.6.0/pluma/stream/eeg.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/empatica.py` & `pluma_analysis-0.6.0/pluma/stream/empatica.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/georeference.py` & `pluma_analysis-0.6.0/pluma/stream/georeference.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/harp.py` & `pluma_analysis-0.6.0/pluma/stream/harp.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/microphone.py` & `pluma_analysis-0.6.0/pluma/stream/microphone.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 		Stream (_type_): _description_
 	"""
 	def __init__(self,
               data: np.array = np.empty(shape=(0, 2)),
               fs: float = None,
               channels: int = 2,
               si_conversion: SiUnitConversion = SiUnitConversion(),
-              clockreferenceid: ClockRefId = ClockRefId.HARP,
+              clockreferenceid: ClockRefId = ClockRefId.NONE,
               **kw):
 		super(MicrophoneStream, self).__init__(data=data, **kw)
 		self.streamtype = StreamType.MICROPHONE
 		self.fs = fs
 		self.channels = channels
 		self.si_conversion = si_conversion
 		self.clockreference.referenceid = clockreferenceid
```

### Comparing `pluma_analysis-0.5.0/pluma/stream/siconversion.py` & `pluma_analysis-0.6.0/pluma/stream/siconversion.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/ubx.py` & `pluma_analysis-0.6.0/pluma/stream/ubx.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/stream/zeromq.py` & `pluma_analysis-0.6.0/pluma/stream/zeromq.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/sync/__init__.py` & `pluma_analysis-0.6.0/pluma/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma/sync/ubx2harp.py` & `pluma_analysis-0.6.0/pluma/sync/ubx2harp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import numpy as np
-import matplotlib.pyplot as plt
-
-from matplotlib.ticker import MaxNLocator
-
+from dataclasses import dataclass
 from sklearn.linear_model import LinearRegression
 
 from pluma.stream.harp import HarpStream
 from pluma.stream.ubx import UbxStream, _UBX_MSGIDS, _UBX_CLASSES
 
-
 class SyncTimestamp:
     def __init__(self,
                  ts_array,
                  seconds_conversion=(lambda x: x)) -> None:
         self.raw_ts_array = ts_array
         self.ts_array = ts_array
         self.seconds_conversion_factor = seconds_conversion
@@ -75,14 +71,19 @@
 
     def __repr__(self) -> str:
         return str(self.ts_array)
 
     def __str__(self) -> str:
         return str(self.ts_array)
 
+@dataclass
+class SyncLookup:
+    ubx_ts: SyncTimestamp
+    harp_ts: SyncTimestamp
+    align_lookup: np.ndarray
 
 def align_ubx_to_harp(
         ubx_SyncTimestamp: SyncTimestamp,
         harp_SyncTimestamp: SyncTimestamp,
         dt_error: float = 0.002,
         plot_diagnosis: bool = False):
 
@@ -116,48 +117,28 @@
             ubx_ts.get_pair(pair)[-1],
             dt_error=dt_error,
             min_pair_index=min_pair_index)
         pulses_lookup[pair, :] = [pair, dyad[0]]
         min_pair_index = dyad[1]
 
     if plot_diagnosis is True:
-        plt.figure(figsize=(12, 8))
-        plt.subplot(211)
-        plt.plot(pulses_lookup[:, 0], pulses_lookup[:, 1], '.')
-        plt.xlabel('ubx_index')
-        plt.ylabel('Harp_index')
-        plt.title('Index correspondence between streams')
-
-        plt.subplot(212)
-
-        plt.scatter(
-            np.arange(len(ubx_ts.ts_array[pulses_lookup[:, 0]])-1),
-            np.diff(ubx_ts.ts_array[pulses_lookup[:, 0]]),
-            100, label="ubx")
-        plt.scatter(
-            np.arange(len(harp_ts.ts_array[pulses_lookup[:, 1]])-1),
-            np.diff(harp_ts.ts_array[pulses_lookup[:, 1]]),
-            label="HARP")
-
-        ax = plt.gca()
-        ax.xaxis.set_major_locator(MaxNLocator(integer=True))
-        plt.ylabel('$\Delta t$ (s)')
-        plt.xlabel('Trial number')
-        plt.legend()
-        plt.show()
+        import pluma.sync.plotting as plotting
+        plotting.plot_clockcalibration_diagnosis(
+            ubx_ts=ubx_ts,
+            harp_ts=harp_ts,
+            pulses_lookup=pulses_lookup)
 
     return pulses_lookup
 
-
-def get_clockcalibration_ubx_to_harp_clock(ubx_stream: UbxStream,
-                                           harp_sync: HarpStream,
-                                           dt_error: float = 0.002,
-                                           plot_diagnosis: bool = False,
-                                           r2_min_qc: float = 0.99) -> LinearRegression:
-
+def get_clockcalibration_lookup(
+        ubx_stream: UbxStream,
+        harp_sync: HarpStream,
+        dt_error: float = 0.002,
+        plot_diagnosis: bool = False) -> SyncLookup:
+    
     # Get the TIM_TM2 Message that timestamps the incoming TTL
     if not(ubx_stream.has_event(_UBX_MSGIDS.TIM_TM2)):
         raise KeyError(f"UbxStream does not contain \
             {_UBX_MSGIDS.TIM_TM2.value}\
                 event. Try to load it?")
 
     tim_tm2 = ubx_stream.data.TIM_TM2.copy()  # TTL
@@ -169,27 +150,35 @@
     risingEdgeEvents = tim_tm2["RisingEdge"].drop_duplicates(
         keep='first').values.astype(float)
 
     #  From Harp, get the second output channel
     harp_sync_out = harp_sync.copy()
     harp_sync_out = harp_sync_out[harp_sync_out["Value"].values & 3 > 0]
 
-    gps_ts = SyncTimestamp(risingEdgeEvents,
+    ubx_ts = SyncTimestamp(risingEdgeEvents,
                            seconds_conversion=lambda x: x*1e-3)
     harp_ts = SyncTimestamp(harp_sync_out.index.values,
                             seconds_conversion=lambda x: x /
                             np.timedelta64(1, 's'))
 
-    align_lookup = align_ubx_to_harp(gps_ts,
+    align_lookup = align_ubx_to_harp(ubx_ts,
                                      harp_ts,
                                      dt_error=dt_error,
                                      plot_diagnosis=plot_diagnosis)
+    return SyncLookup(ubx_ts, harp_ts, align_lookup)
+
+def get_clockcalibration_model(sync_lookup: SyncLookup,
+                               r2_min_qc: float = 0.99) -> LinearRegression:
+    
+    ubx_ts = sync_lookup.ubx_ts
+    harp_ts = sync_lookup.harp_ts
+    align_lookup = sync_lookup.align_lookup
 
     harp_ts_seconds = HarpStream.to_seconds(harp_ts.raw_ts_array)
-    x_gps_time = gps_ts.raw_ts_array[align_lookup[:, 0]].reshape(-1, 1)
+    x_gps_time = ubx_ts.raw_ts_array[align_lookup[:, 0]].reshape(-1, 1)
     y_harp_time = harp_ts_seconds[align_lookup[:, 1]]
     model = LinearRegression().fit(x_gps_time, y_harp_time)
     r2 = model.score(x_gps_time, y_harp_time)
     if r2 < r2_min_qc:
         raise AssertionError(
             f"The quality of the linear fit is lower than expected {r2}")
     else:
```

### Comparing `pluma_analysis-0.5.0/pluma/templates/metadata_template.j2` & `pluma_analysis-0.6.0/pluma/templates/metadata_template.j2`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.5.0/pluma_analysis.egg-info/PKG-INFO` & `pluma_analysis-0.6.0/pluma_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluma-analysis
-Version: 0.5.0
+Version: 0.6.0
 Summary: A low-level interface to data collected with the pluma urban data acquisition system
 Author-email: Goncalo Lopes <g.lopes@neurogears.org>, Bruno Cruz <b.cruz@neurogears.org>, Andrew Erskine <a.erskine@neurogears.org>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/emotional-cities/pluma-analysis/issues
 Project-URL: Source Code, https://github.com/emotional-cities/pluma-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `pluma_analysis-0.5.0/pluma_analysis.egg-info/SOURCES.txt` & `pluma_analysis-0.6.0/pluma_analysis.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 pluma/stream/georeference.py
 pluma/stream/harp.py
 pluma/stream/microphone.py
 pluma/stream/siconversion.py
 pluma/stream/ubx.py
 pluma/stream/zeromq.py
 pluma/sync/__init__.py
+pluma/sync/plotting.py
 pluma/sync/ubx2harp.py
 pluma/templates/metadata_template.j2
 pluma_analysis.egg-info/PKG-INFO
 pluma_analysis.egg-info/SOURCES.txt
 pluma_analysis.egg-info/dependency_links.txt
 pluma_analysis.egg-info/requires.txt
 pluma_analysis.egg-info/top_level.txt
```

### Comparing `pluma_analysis-0.5.0/pyproject.toml` & `pluma_analysis-0.6.0/pyproject.toml`

 * *Files identical despite different names*

