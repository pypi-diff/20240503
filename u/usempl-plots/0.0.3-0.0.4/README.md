# Comparing `tmp/usempl-plots-0.0.3.tar.gz` & `tmp/usempl-plots-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usempl-plots-0.0.3.tar", last modified: Fri May  3 07:04:56 2024, max compression
+gzip compressed data, was "usempl-plots-0.0.4.tar", last modified: Fri May  3 07:28:08 2024, max compression
```

## Comparing `usempl-plots-0.0.3.tar` & `usempl-plots-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:56.219777 usempl-plots-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-03 07:04:56.219777 usempl-plots-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:04:56.219777 usempl-plots-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:56.219777 usempl-plots-0.0.3/usempl_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:56.219777 usempl-plots-0.0.3/usempl_plots/data/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/data/recession_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/data/usempl_2024-03-01.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/data/usempl_2024-03-01_streaks.csv
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/data/usempl_annual_1919-1938.csv
--rw-r--r--   0 runner    (1001) docker     (127)   105196 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/data/usempl_pk_2024-03-01.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/get_payems.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/tseries_payems.py
--rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/usempl_industry.py
--rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/usempl_npp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-05-03 07:04:51.000000 usempl-plots-0.0.3/usempl_plots/usempl_streaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:04:56.219777 usempl-plots-0.0.3/usempl_plots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-03 07:04:56.000000 usempl-plots-0.0.3/usempl_plots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-03 07:04:56.000000 usempl-plots-0.0.3/usempl_plots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:04:56.000000 usempl-plots-0.0.3/usempl_plots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 07:04:56.000000 usempl-plots-0.0.3/usempl_plots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 07:04:56.000000 usempl-plots-0.0.3/usempl_plots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/usempl_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/usempl_plots/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/recession_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_2024-03-01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_2024-03-01_streaks.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_annual_1919-1938.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   105196 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_pk_2024-03-01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/get_payems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/tseries_payems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/usempl_industry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/usempl_npp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/usempl_streaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/usempl_plots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/top_level.txt
```

### Comparing `usempl-plots-0.0.3/LICENSE` & `usempl-plots-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/PKG-INFO` & `usempl-plots-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: usempl-plots
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for creating plots of US employment and unemployment
 Home-page: https://github.com/OpenSourceEcon/usempl-plots
 Download-URL: https://github.com/OpenSourceEcon/usempl-plots
 Author: Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/OpenSourceEcon/usempl-plots/issues
 Keywords: Data analysis visualization tools US employment unemployment
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plots of US employment and unemployment
 
 | | |
 | --- | --- |
```

### Comparing `usempl-plots-0.0.3/README.md` & `usempl-plots-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/setup.py` & `usempl-plots-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,43 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="usempl-plots",
-    version="0.0.3",
+    version="0.0.4",
     author="Richard W. Evans",
     license="CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     description="Package for creating plots of US employment and unemployment",
     long_description=readme,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
         "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="Data analysis visualization tools US employment unemployment",
     url="https://github.com/OpenSourceEcon/usempl-plots",
     download_url="https://github.com/OpenSourceEcon/usempl-plots",
     project_urls={
         "Issue Tracker": "https://github.com/OpenSourceEcon/usempl-plots/issues",
     },
     packages=find_packages(),
     package_data={"usempl_plots": ["data/*"]},
     include_packages=True,
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     install_requires=[
         "numpy>=1.23.4",
         "scipy>=1.9.3",
         "pandas>=1.5.2",
         "pandas-datareader>=0.10.0",
         "bokeh>=3.0",
         "matplotlib",
```

### Comparing `usempl-plots-0.0.3/usempl_plots/data/recession_data.csv` & `usempl-plots-0.0.4/usempl_plots/data/recession_data.csv`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/data/usempl_2024-03-01.csv` & `usempl-plots-0.0.4/usempl_plots/data/usempl_2024-03-01.csv`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/data/usempl_2024-03-01_streaks.csv` & `usempl-plots-0.0.4/usempl_plots/data/usempl_2024-03-01_streaks.csv`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/data/usempl_pk_2024-03-01.csv` & `usempl-plots-0.0.4/usempl_plots/data/usempl_pk_2024-03-01.csv`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/get_payems.py` & `usempl-plots-0.0.4/usempl_plots/get_payems.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/tseries_payems.py` & `usempl-plots-0.0.4/usempl_plots/tseries_payems.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/usempl_industry.py` & `usempl-plots-0.0.4/usempl_plots/usempl_industry.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/usempl_npp.py` & `usempl-plots-0.0.4/usempl_plots/usempl_npp.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots/usempl_streaks.py` & `usempl-plots-0.0.4/usempl_plots/usempl_streaks.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.3/usempl_plots.egg-info/PKG-INFO` & `usempl-plots-0.0.4/usempl_plots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: usempl-plots
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for creating plots of US employment and unemployment
 Home-page: https://github.com/OpenSourceEcon/usempl-plots
 Download-URL: https://github.com/OpenSourceEcon/usempl-plots
 Author: Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/OpenSourceEcon/usempl-plots/issues
 Keywords: Data analysis visualization tools US employment unemployment
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plots of US employment and unemployment
 
 | | |
 | --- | --- |
```

### Comparing `usempl-plots-0.0.3/usempl_plots.egg-info/SOURCES.txt` & `usempl-plots-0.0.4/usempl_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

