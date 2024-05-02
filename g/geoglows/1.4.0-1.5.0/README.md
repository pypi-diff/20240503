# Comparing `tmp/geoglows-1.4.0.tar.gz` & `tmp/geoglows-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.4.0.tar", last modified: Wed May  1 04:46:45 2024, max compression
+gzip compressed data, was "geoglows-1.5.0.tar", last modified: Thu May  2 23:49:10 2024, max compression
```

## Comparing `geoglows-1.4.0.tar` & `geoglows-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-01 04:46:41.000000 geoglows-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 04:46:41.000000 geoglows-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-01 04:46:45.913283 geoglows-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-01 04:46:41.000000 geoglows-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 04:46:41.000000 geoglows-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 04:46:45.917284 geoglows-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 04:46:41.000000 geoglows-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-02 23:49:02.000000 geoglows-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 23:49:02.000000 geoglows-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-02 23:49:10.469408 geoglows-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 23:49:02.000000 geoglows-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_download_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 23:49:02.000000 geoglows-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:49:10.469408 geoglows-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-02 23:49:02.000000 geoglows-1.5.0/setup.py
```

### Comparing `geoglows-1.4.0/LICENSE` & `geoglows-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/PKG-INFO` & `geoglows-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.4.0
+Version: 1.5.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.4.0/README.md` & `geoglows-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/_plots/__init__.py` & `geoglows-1.5.0/geoglows/_plots/__init__.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/_plots/format_tools.py` & `geoglows-1.5.0/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.5.0/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.5.0/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/_plots/plotly_helpers.py` & `geoglows-1.5.0/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.5.0/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/_plots/plots.py` & `geoglows-1.5.0/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/analyze.py` & `geoglows-1.5.0/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/bias.py` & `geoglows-1.5.0/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/streamflow.py` & `geoglows-1.5.0/geoglows/streamflow.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/streams.py` & `geoglows-1.5.0/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows/tables.py` & `geoglows-1.5.0/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.4.0/geoglows.egg-info/PKG-INFO` & `geoglows-1.5.0/geoglows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.4.0
+Version: 1.5.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.4.0/setup.py` & `geoglows-1.5.0/setup.py`

 * *Files identical despite different names*

