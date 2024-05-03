# Comparing `tmp/hippo_plot-0.0.4.tar.gz` & `tmp/hippo_plot-0.0.5.tar.gz`

## Comparing `hippo_plot-0.0.4.tar` & `hippo_plot-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,9 @@
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/.gitignore
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/README.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/__init__.py
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/cli.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/draw.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/io.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/hippo_plot/prep.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/.gitignore
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hippo_plot-0.0.5/PKG-INFO
```

### Comparing `hippo_plot-0.0.4/.gitignore` & `hippo_plot-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hippo_plot-0.0.4/pyproject.toml` & `hippo_plot-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hippo_plot"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Max Winokan", email = "max@winokan.com" },
 ]
 description = "Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 requires = []
@@ -18,14 +18,15 @@
 ]
 dependencies = [
     "mpytools >= 0.0.10",
     "plotly",
     "pandas",
     "dash",
     "rdkit",
+    "dash_dangerously_set_inner_html",
 ]
 [project.urls]
 "Homepage" = "https://hippo.winokan.com"
 "Bug Tracker" = "https://github.com/mwinokan/HIPPO_plot/issues"
 [tool.hatch.build]
 include = [
     "hippo_plot/*.py"
```

### Comparing `hippo_plot-0.0.4/PKG-INFO` & `hippo_plot-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: hippo_plot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs
 Project-URL: Homepage, https://hippo.winokan.com
 Project-URL: Bug Tracker, https://github.com/mwinokan/HIPPO_plot/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: dash
+Requires-Dist: dash-dangerously-set-inner-html
 Requires-Dist: mpytools>=0.0.10
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: rdkit
 Description-Content-Type: text/markdown
 
 # HIPPO_plot
```

