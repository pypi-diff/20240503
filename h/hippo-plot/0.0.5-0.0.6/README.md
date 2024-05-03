# Comparing `tmp/hippo_plot-0.0.5.tar.gz` & `tmp/hippo_plot-0.0.6.tar.gz`

## Comparing `hippo_plot-0.0.5.tar` & `hippo_plot-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/__init__.py
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/cli.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/draw.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/io.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/prep.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/.gitignore
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/README.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/hippo_plot/__init__.py
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/hippo_plot/cli.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/hippo_plot/draw.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/hippo_plot/io.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/hippo_plot/prep.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/.gitignore
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hippo_plot-0.0.6/PKG-INFO
```

### Comparing `hippo_plot-0.0.5/hippo_plot/cli.py` & `hippo_plot-0.0.6/hippo_plot/cli.py`

 * *Files identical despite different names*

### Comparing `hippo_plot-0.0.5/hippo_plot/prep.py` & `hippo_plot-0.0.6/hippo_plot/prep.py`

 * *Files identical despite different names*

### Comparing `hippo_plot-0.0.5/.gitignore` & `hippo_plot-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hippo_plot-0.0.5/pyproject.toml` & `hippo_plot-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hippo_plot"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Max Winokan", email = "max@winokan.com" },
 ]
 description = "Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 requires = []
@@ -28,8 +28,8 @@
 "Homepage" = "https://hippo.winokan.com"
 "Bug Tracker" = "https://github.com/mwinokan/HIPPO_plot/issues"
 [tool.hatch.build]
 include = [
     "hippo_plot/*.py"
 ]
 [project.scripts]
-hippo_plot = "hippo_plot.cli:main"
+hippo-plot = "hippo_plot.cli:main"
```

### Comparing `hippo_plot-0.0.5/PKG-INFO` & `hippo_plot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hippo_plot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs
 Project-URL: Homepage, https://hippo.winokan.com
 Project-URL: Bug Tracker, https://github.com/mwinokan/HIPPO_plot/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

