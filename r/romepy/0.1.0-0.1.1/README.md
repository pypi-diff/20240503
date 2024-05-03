# Comparing `tmp/romepy-0.1.0.tar.gz` & `tmp/romepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romepy-0.1.0.tar", max compression
+gzip compressed data, was "romepy-0.1.1.tar", max compression
```

## Comparing `romepy-0.1.0.tar` & `romepy-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rwxr-xr-x   0        0        0     1070 2024-05-03 09:16:32.046348 romepy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1468 2024-05-03 09:47:53.792243 romepy-0.1.0/README.md
--rw-r--r--   0        0        0      665 2024-05-03 09:16:02.022466 romepy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 14:07:45.047069 romepy-0.1.0/rome/__init__.py
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 romepy-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2024-05-03 09:16:32.046348 romepy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1728 2024-05-03 10:14:59.118393 romepy-0.1.1/README.md
+-rw-r--r--   0        0        0      793 2024-05-03 10:14:15.218525 romepy-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0    15077 2024-05-03 10:15:17.642337 romepy-0.1.1/rome/ROME.py
+-rw-r--r--   0        0        0       11 2024-05-03 10:28:43.288407 romepy-0.1.1/rome/__init__.py
+-rw-r--r--   0        0        0     2612 1970-01-01 00:00:00.000000 romepy-0.1.1/PKG-INFO
```

### Comparing `romepy-0.1.0/LICENSE` & `romepy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `romepy-0.1.0/pyproject.toml` & `romepy-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [tool.poetry]
 name = "romepy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python implementation of the Robust Multi-Modal Density Estimator (ROME)"
 authors = ["Anna Meszaros <ana.mesaros@gmail.com>",
             "Julian F. Schumann <julian.frederik.schumann@gmail.com>"]
+
+maintainers = ["anna-meszaros <ana.mesaros@gmail.com>",
+               "julianschumann <julian.frederik.schumann@gmail.com>"]
+
 readme = "README.md"
 packages = [{include = "rome"}]
 
 license = "MIT"
 repository = "https://github.com/anna-meszaros/ROME"
 
 [tool.poetry.dependencies]
```

### Comparing `romepy-0.1.0/PKG-INFO` & `romepy-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: romepy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of the Robust Multi-Modal Density Estimator (ROME)
 Home-page: https://github.com/anna-meszaros/ROME
 License: MIT
 Author: Anna Meszaros
 Author-email: ana.mesaros@gmail.com
+Maintainer: anna-meszaros
+Maintainer-email: ana.mesaros@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,36 +23,44 @@
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # ROME
 This package implements the [Robust Multi-Modal Density Estimation](https://arxiv.org/abs/2401.10566). 
-This method is using clustering based on the OPTICS algortihm, using is to order sample points based on rechability analysis, based on which the clustering which maximizes the silhuette is selected.
-On each cluster, it then uses normalization and decorrelation, before fitting applying simple KDE to it.
+This method creates a probability density function using nonparametric methods.
+ROME clusters data based on the OPTICS algortihm, using it to order sample points based on rechability analysis.
+It then generates the clustering which maximizes the silhouette score.
+Each cluster is then decorrelated and normalized before applying kernel density estimation.
 
-ROME has shown itself to be superior when dealing with multi-modal and highly corrolated distributions.
+ROME has shown itself to be superior when dealing with multi-modal and highly correlated distributions, especially for
+high dimensions.
 
 ## Installation
-ROME can be installed using the simple "pip install romepy" command.
+ROME can be installed using:
+```
+pip install romepy
+```
 
 ## Usage
-Inside a script, ROME is loaded by the following command.
+Inside a script, ROME is loaded by the following command:
 ```
 from ROME import ROME
 
 rome = ROME()
 ```
 
 After initiliazing ROME, one can then call the typical functions most scikit-learn density estimators (KDE, GMM, etc.) have:
 ```
-rome = rome.fit(X, cluster=None)
-log_probs = rome.score_samples(X)
-X_new = rome.sample(num_samples = 10, random_state = 0)
+rome.fit(X, cluster=None) # fit distribution to data X
+log_probs = rome.score_samples(X) # obtain log_probs of data X according to fitted distribution
+X_new = rome.sample(num_samples = 10, random_state = 0) # generate new samples according to fitted distribution
 ```
 
-The main difference is the *cluster* parameter in the fit function. If it is not set to *None*, it can be used to skip the OPTICS based clustering and use a predifened clustering instead.
+The main difference is the *cluster* parameter in the *fit* function. If it is not set to *None*, it can be used to skip the OPTICS based clustering and use a predifened clustering instead.
 
 
 ## Changelog
+Version 0.1.1: Added all maintainers.
+
 Version 0.1.0: Initial upload of romepy.
```

