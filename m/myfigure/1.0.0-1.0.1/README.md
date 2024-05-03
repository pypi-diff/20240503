# Comparing `tmp/myfigure-1.0.0.tar.gz` & `tmp/myfigure-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfigure-1.0.0.tar", last modified: Wed May  1 02:42:33 2024, max compression
+gzip compressed data, was "myfigure-1.0.1.tar", last modified: Fri May  3 20:34:36 2024, max compression
```

## Comparing `myfigure-1.0.0.tar` & `myfigure-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-05-01 02:42:33.497496 myfigure-1.0.0/
--rw-r--r--   0 matteo     (501) staff       (20)     1064 2024-04-13 02:45:51.000000 myfigure-1.0.0/LICENSE
--rw-r--r--   0 matteo     (501) staff       (20)     5574 2024-05-01 02:42:33.497306 myfigure-1.0.0/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)     4965 2024-05-01 02:34:32.000000 myfigure-1.0.0/README.md
--rwx------   0 matteo     (501) staff       (20)      653 2024-05-01 01:24:08.000000 myfigure-1.0.0/pyproject.toml
--rw-r--r--   0 matteo     (501) staff       (20)       38 2024-05-01 02:42:33.497538 myfigure-1.0.0/setup.cfg
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-05-01 02:42:33.494616 myfigure-1.0.0/src/
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-05-01 02:42:33.495475 myfigure-1.0.0/src/myfigure/
--rwx------   0 matteo     (501) staff       (20)        0 2024-04-06 03:49:57.000000 myfigure-1.0.0/src/myfigure/__init__.py
--rwx------   0 matteo     (501) staff       (20)    27569 2024-04-19 22:35:05.000000 myfigure-1.0.0/src/myfigure/myfigure.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-05-01 02:42:33.497081 myfigure-1.0.0/src/myfigure.egg-info/
--rw-r--r--   0 matteo     (501) staff       (20)     5574 2024-05-01 02:42:33.000000 myfigure-1.0.0/src/myfigure.egg-info/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)      284 2024-05-01 02:42:33.000000 myfigure-1.0.0/src/myfigure.egg-info/SOURCES.txt
--rw-r--r--   0 matteo     (501) staff       (20)        1 2024-05-01 02:42:33.000000 myfigure-1.0.0/src/myfigure.egg-info/dependency_links.txt
--rw-r--r--   0 matteo     (501) staff       (20)       79 2024-05-01 02:42:33.000000 myfigure-1.0.0/src/myfigure.egg-info/requires.txt
--rw-r--r--   0 matteo     (501) staff       (20)        9 2024-05-01 02:42:33.000000 myfigure-1.0.0/src/myfigure.egg-info/top_level.txt
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-05-01 02:42:33.496785 myfigure-1.0.0/tests/
--rw-r--r--   0 matteo     (501) staff       (20)     2924 2024-05-01 01:28:28.000000 myfigure-1.0.0/tests/test_myfigure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:34:36.681828 myfigure-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 20:34:31.000000 myfigure-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-03 20:34:36.681828 myfigure-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-03 20:34:31.000000 myfigure-1.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      694 2024-05-03 20:34:31.000000 myfigure-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:34:36.681828 myfigure-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:34:36.681828 myfigure-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:34:36.681828 myfigure-1.0.1/src/myfigure/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:34:31.000000 myfigure-1.0.1/src/myfigure/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27569 2024-05-03 20:34:31.000000 myfigure-1.0.1/src/myfigure/myfigure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:34:36.681828 myfigure-1.0.1/src/myfigure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-03 20:34:36.000000 myfigure-1.0.1/src/myfigure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-03 20:34:36.000000 myfigure-1.0.1/src/myfigure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:34:36.000000 myfigure-1.0.1/src/myfigure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 20:34:36.000000 myfigure-1.0.1/src/myfigure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 20:34:36.000000 myfigure-1.0.1/src/myfigure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:34:36.681828 myfigure-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-03 20:34:31.000000 myfigure-1.0.1/tests/test_myfigure.py
```

### Comparing `myfigure-1.0.0/LICENSE` & `myfigure-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myfigure-1.0.0/PKG-INFO` & `myfigure-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,15 @@
-Metadata-Version: 2.1
-Name: myfigure
-Version: 1.0.0
-Summary: a class for standardized accessible plots
-Author: Matteo Pecchi
-License: MIT
-Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.21.2
-Requires-Dist: pandas>=1.3.3
-Requires-Dist: matplotlib>=3.4.3
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: openpyxl
-Requires-Dist: pyarrow
-
 # MyFigure Module
 
 A class for standardized accessible scientific plots.
 
+[![Documentation Status](https://readthedocs.org/projects/myfigure/badge/?version=latest)](https://myfigure.readthedocs.io/en/latest/?badge=latest)
+
+[![Python CI](https://github.com/mpecchi/myfigure/actions/workflows/continuous_integration.yaml/badge.svg)](https://github.com/mpecchi/myfigure/actions/workflows/continuous_integration.yaml)
+    
 ## Overview
 MyFigure is a Python module tailored for creating and customizing sophisticated visualizations with Matplotlib and Seaborn. It offers an intuitive interface to streamline figure setup, axis configuration, and style management, making it ideal for both simple plots and complex graphical representations in publications and presentations.
 
 ## Features
 - **Seaborn and Matplotlib Integration**: Leverages the advanced styling and plotting capabilities of both Seaborn and Matplotlib to produce beautiful, scientific-grade figures.
 - **Default Keyword Arguments**: Supports easy customization and flexibility by allowing default configurations that can be overridden according to user needs.
 - **Broadcast Keyword Arguments**: Automatically broadcasts single values across multiple axes or applies unique values per axis, enhancing customization without additional code for each axis.
@@ -42,14 +26,18 @@
 
 ## Installation
 Install MyFigure using pip:
 ```bash
 pip install myfigure
 ```
 
+## Documentation
+
+Check out the [documentation](https://myfigure.readthedocs.io/).
+
 ## Examples 
 
 Examples are available in the ``examples`` folder.
 To run examples:
 1. Install ``myfigure`` in your Python environment
 2. Download or copy-paste the example code in your editor
 3. Run the code 
@@ -97,8 +85,8 @@
 mf_non_default = function_using_myfigure(
     x_lim=(0, 1), height=6, x_lab="a", y_lab="another_specific_label"
 ) # customized
 #
 mf = function_using_myfigure()
 mf.axs[0].plot([1], [1])  # something that was impossible inside the function
 mf.save_figure()
-```
+```
```

### Comparing `myfigure-1.0.0/pyproject.toml` & `myfigure-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "myfigure"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Matteo Pecchi"}
 ]
-description = "a class for standardized accessible plots"
+description = "standardized accessible plots"
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -21,12 +21,13 @@
     "matplotlib>=3.4.3",
     "seaborn>=0.11.2",
     "openpyxl",
     "pyarrow",
 ]
 
 [project.urls]
-Homepage = "https://github.com/mpecchi/tga_data_analysis"
+Homepage = "https://github.com/mpecchi/myfigure"
+Documentation = "https://myfigure.readthedocs.io/en/latest/"
 
 [tool.black]
 line-length = 100
```

### Comparing `myfigure-1.0.0/src/myfigure/myfigure.py` & `myfigure-1.0.1/src/myfigure/myfigure.py`

 * *Files identical despite different names*

### Comparing `myfigure-1.0.0/src/myfigure.egg-info/PKG-INFO` & `myfigure-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: myfigure
-Version: 1.0.0
-Summary: a class for standardized accessible plots
+Version: 1.0.1
+Summary: standardized accessible plots
 Author: Matteo Pecchi
 License: MIT
-Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
+Project-URL: Homepage, https://github.com/mpecchi/myfigure
+Project-URL: Documentation, https://myfigure.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.2
@@ -18,14 +19,18 @@
 Requires-Dist: openpyxl
 Requires-Dist: pyarrow
 
 # MyFigure Module
 
 A class for standardized accessible scientific plots.
 
+[![Documentation Status](https://readthedocs.org/projects/myfigure/badge/?version=latest)](https://myfigure.readthedocs.io/en/latest/?badge=latest)
+
+[![Python CI](https://github.com/mpecchi/myfigure/actions/workflows/continuous_integration.yaml/badge.svg)](https://github.com/mpecchi/myfigure/actions/workflows/continuous_integration.yaml)
+    
 ## Overview
 MyFigure is a Python module tailored for creating and customizing sophisticated visualizations with Matplotlib and Seaborn. It offers an intuitive interface to streamline figure setup, axis configuration, and style management, making it ideal for both simple plots and complex graphical representations in publications and presentations.
 
 ## Features
 - **Seaborn and Matplotlib Integration**: Leverages the advanced styling and plotting capabilities of both Seaborn and Matplotlib to produce beautiful, scientific-grade figures.
 - **Default Keyword Arguments**: Supports easy customization and flexibility by allowing default configurations that can be overridden according to user needs.
 - **Broadcast Keyword Arguments**: Automatically broadcasts single values across multiple axes or applies unique values per axis, enhancing customization without additional code for each axis.
@@ -42,14 +47,18 @@
 
 ## Installation
 Install MyFigure using pip:
 ```bash
 pip install myfigure
 ```
 
+## Documentation
+
+Check out the [documentation](https://myfigure.readthedocs.io/).
+
 ## Examples 
 
 Examples are available in the ``examples`` folder.
 To run examples:
 1. Install ``myfigure`` in your Python environment
 2. Download or copy-paste the example code in your editor
 3. Run the code
```

### Comparing `myfigure-1.0.0/tests/test_myfigure.py` & `myfigure-1.0.1/tests/test_myfigure.py`

 * *Files identical despite different names*

