# Comparing `tmp/wellwiz-0.0.1.tar.gz` & `tmp/wellwiz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellwiz-0.0.1.tar", last modified: Wed May  1 04:58:34 2024, max compression
+gzip compressed data, was "wellwiz-0.0.2.tar", last modified: Fri May  3 10:36:21 2024, max compression
```

## Comparing `wellwiz-0.0.1.tar` & `wellwiz-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.597875 wellwiz-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.585875 wellwiz-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.589875 wellwiz-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.589875 wellwiz-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-01 04:58:22.000000 wellwiz-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 04:58:22.000000 wellwiz-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-01 04:58:22.000000 wellwiz-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-01 04:58:34.593875 wellwiz-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 04:58:22.000000 wellwiz-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.593875 wellwiz-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.593875 wellwiz-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.593875 wellwiz-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 04:58:22.000000 wellwiz-0.0.1/docs/wellwiz.md
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-01 04:58:22.000000 wellwiz-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-01 04:58:22.000000 wellwiz-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 04:58:22.000000 wellwiz-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-01 04:58:22.000000 wellwiz-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 04:58:34.597875 wellwiz-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.593875 wellwiz-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 04:58:22.000000 wellwiz-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-01 04:58:22.000000 wellwiz-0.0.1/tests/test_wellwiz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.593875 wellwiz-0.0.1/wellwiz/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-01 04:58:22.000000 wellwiz-0.0.1/wellwiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 04:58:22.000000 wellwiz-0.0.1/wellwiz/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 04:58:22.000000 wellwiz-0.0.1/wellwiz/wellwiz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:58:34.593875 wellwiz-0.0.1/wellwiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-01 04:58:34.000000 wellwiz-0.0.1/wellwiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-01 04:58:34.000000 wellwiz-0.0.1/wellwiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:58:34.000000 wellwiz-0.0.1/wellwiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 04:58:34.000000 wellwiz-0.0.1/wellwiz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 04:58:34.000000 wellwiz-0.0.1/wellwiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 04:58:34.000000 wellwiz-0.0.1/wellwiz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.373131 wellwiz-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.361131 wellwiz-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.361131 wellwiz-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.365131 wellwiz-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-03 10:36:10.000000 wellwiz-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 10:36:10.000000 wellwiz-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 10:36:10.000000 wellwiz-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-03 10:36:21.373131 wellwiz-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-03 10:36:10.000000 wellwiz-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.369131 wellwiz-0.0.2/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)  2053916 2024-05-03 10:36:10.000000 wellwiz-0.0.2/csv/Oil and Gas Well Permits.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-03 10:36:10.000000 wellwiz-0.0.2/csv/Oil&Gas.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.373131 wellwiz-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  2053916 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/Oil and Gas Well Permits.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.373131 wellwiz-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/examples/well.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.373131 wellwiz-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 10:36:10.000000 wellwiz-0.0.2/docs/wellwiz.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-03 10:36:10.000000 wellwiz-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-03 10:36:10.000000 wellwiz-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 10:36:10.000000 wellwiz-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 10:36:10.000000 wellwiz-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:36:21.373131 wellwiz-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.373131 wellwiz-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 10:36:10.000000 wellwiz-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-03 10:36:10.000000 wellwiz-0.0.2/tests/test_wellwiz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.373131 wellwiz-0.0.2/wellwiz/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 10:36:10.000000 wellwiz-0.0.2/wellwiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 10:36:10.000000 wellwiz-0.0.2/wellwiz/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-03 10:36:10.000000 wellwiz-0.0.2/wellwiz/wellwiz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:36:21.373131 wellwiz-0.0.2/wellwiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-03 10:36:21.000000 wellwiz-0.0.2/wellwiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-03 10:36:21.000000 wellwiz-0.0.2/wellwiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:36:21.000000 wellwiz-0.0.2/wellwiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 10:36:21.000000 wellwiz-0.0.2/wellwiz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 10:36:21.000000 wellwiz-0.0.2/wellwiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 10:36:21.000000 wellwiz-0.0.2/wellwiz.egg-info/top_level.txt
```

### Comparing `wellwiz-0.0.1/.github/workflows/docs-build.yml` & `wellwiz-0.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/.github/workflows/docs.yml` & `wellwiz-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/.github/workflows/installation.yml` & `wellwiz-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/.github/workflows/macos.yml` & `wellwiz-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/.github/workflows/pypi.yml` & `wellwiz-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/.github/workflows/ubuntu.yml` & `wellwiz-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/.github/workflows/windows.yml` & `wellwiz-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/.gitignore` & `wellwiz-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/LICENSE` & `wellwiz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/PKG-INFO` & `wellwiz-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellwiz
-Version: 0.0.1
+Version: 0.0.2
 Summary: A developing python package to gather information about the gas and oil wells and know the risk through a map visualization.
 Author-email: Shabiha Hossain <sabihahossain4105@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/OmiimO05/wellwiz
 Keywords: wellwiz
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: folium
+Requires-Dist: pandas
+Requires-Dist: pyshp
+Requires-Dist: geopandas
+Requires-Dist: localtileserver
+Requires-Dist: pylance
+Requires-Dist: panel
+Requires-Dist: geopy
 Provides-Extra: all
 Requires-Dist: wellwiz[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # wellwiz
 
@@ -31,12 +40,26 @@
 
 
 **A developing python package to gather information about the gas and oil wells and know the risk through a map visualization.**
 
 
 -   Free software: MIT License
 -   Documentation: https://OmiimO05.github.io/wellwiz
+
+![](https://i.gifer.com/GG4X.gif)
     
 
 ## Features
 
--   TODO
+-   To visualize the oil and gas wells in Knoxville, TN.
+-   To know their names and purpose.
+-   To identify the risk of fracking exposure.
+
+
+## Demo code
+For the demonstration you can visit- 
+[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmIImO05/netpanda/blob/main/docs/examples/example_code.ipynb)
+
+or you can also watch this video. 
+
+
+Thank you for interest!
```

### Comparing `wellwiz-0.0.1/docs/contributing.md` & `wellwiz-0.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/docs/installation.md` & `wellwiz-0.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `wellwiz-0.0.1/mkdocs.yml` & `wellwiz-0.0.2/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
               icon: material/toggle-switch
               name: Switch to light mode
     name: material
     icon:
         repo: fontawesome/brands/github
     # logo: assets/logo.png
     # favicon: assets/favicon.png
-    features:
+    features: To visualize the oil and gas wells in Knoxville, TN, To know their names and purpose and To identify the risk of fracking exposure.
         - navigation.instant
         - navigation.tracking
         - navigation.top
         - search.highlight
         - search.share
     custom_dir: "docs/overrides"
     font:
@@ -43,18 +43,18 @@
     - git-revision-date-localized:
           enable_creation_date: true
           type: timeago
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
-          execute: True
+          execute: false
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["*ignore.ipynb"]
+          execute_ignore: ["well.ipynb", "Oil and Gas Well Permits.csv", "Oil&Gas.csv"]
           
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -77,10 +77,11 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/OmiimO05/wellwiz/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/well.ipynb
     - API Reference:
           - wellwiz module: wellwiz.md
           - common module: common.md
```

### Comparing `wellwiz-0.0.1/pyproject.toml` & `wellwiz-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wellwiz"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "A developing python package to gather information about the gas and oil wells and know the risk through a map visualization."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `wellwiz-0.0.1/wellwiz.egg-info/PKG-INFO` & `wellwiz-0.0.2/wellwiz.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellwiz
-Version: 0.0.1
+Version: 0.0.2
 Summary: A developing python package to gather information about the gas and oil wells and know the risk through a map visualization.
 Author-email: Shabiha Hossain <sabihahossain4105@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/OmiimO05/wellwiz
 Keywords: wellwiz
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: folium
+Requires-Dist: pandas
+Requires-Dist: pyshp
+Requires-Dist: geopandas
+Requires-Dist: localtileserver
+Requires-Dist: pylance
+Requires-Dist: panel
+Requires-Dist: geopy
 Provides-Extra: all
 Requires-Dist: wellwiz[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # wellwiz
 
@@ -31,12 +40,26 @@
 
 
 **A developing python package to gather information about the gas and oil wells and know the risk through a map visualization.**
 
 
 -   Free software: MIT License
 -   Documentation: https://OmiimO05.github.io/wellwiz
+
+![](https://i.gifer.com/GG4X.gif)
     
 
 ## Features
 
--   TODO
+-   To visualize the oil and gas wells in Knoxville, TN.
+-   To know their names and purpose.
+-   To identify the risk of fracking exposure.
+
+
+## Demo code
+For the demonstration you can visit- 
+[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmIImO05/netpanda/blob/main/docs/examples/example_code.ipynb)
+
+or you can also watch this video. 
+
+
+Thank you for interest!
```

### Comparing `wellwiz-0.0.1/wellwiz.egg-info/SOURCES.txt` & `wellwiz-0.0.2/wellwiz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,27 @@
 .github/workflows/docs-build.yml
 .github/workflows/docs.yml
 .github/workflows/installation.yml
 .github/workflows/macos.yml
 .github/workflows/pypi.yml
 .github/workflows/ubuntu.yml
 .github/workflows/windows.yml
+csv/Oil and Gas Well Permits.csv
+csv/Oil&Gas.csv
+docs/Oil and Gas Well Permits.csv
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/usage.md
 docs/wellwiz.md
 docs/examples/intro.ipynb
+docs/examples/well.ipynb
 docs/overrides/main.html
 tests/__init__.py
 tests/test_wellwiz.py
 wellwiz/__init__.py
 wellwiz/common.py
 wellwiz/wellwiz.py
 wellwiz.egg-info/PKG-INFO
```

