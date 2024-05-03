# Comparing `tmp/clfutils4r-1.0.2.tar.gz` & `tmp/clfutils4r-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clfutils4r-1.0.2.tar", last modified: Fri Apr 19 05:07:34 2024, max compression
+gzip compressed data, was "clfutils4r-1.0.3.tar", last modified: Fri May  3 20:49:30 2024, max compression
```

## Comparing `clfutils4r-1.0.2.tar` & `clfutils4r-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:07:34.977118 clfutils4r-1.0.2/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-1.0.2/LICENSE
--rw-r--r--   0 rgura001 (52843) rgura001 (52843)     7046 2024-04-19 05:07:34.973118 clfutils4r-1.0.2/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6402 2024-04-13 06:08:41.000000 clfutils4r-1.0.2/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2024-04-19 05:05:50.000000 clfutils4r-1.0.2/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-04-19 05:07:34.977118 clfutils4r-1.0.2/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:54:18.000000 clfutils4r-1.0.2/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:07:34.973118 clfutils4r-1.0.2/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:07:34.973118 clfutils4r-1.0.2/src/clfutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-1.0.2/src/clfutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    27610 2024-04-17 11:25:32.000000 clfutils4r-1.0.2/src/clfutils4r/eval_classification.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    22088 2024-04-19 04:31:39.000000 clfutils4r-1.0.2/src/clfutils4r/gridsearch_classification.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    10883 2024-04-13 04:18:23.000000 clfutils4r-1.0.2/src/clfutils4r/pretty_cm.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:07:34.973118 clfutils4r-1.0.2/src/clfutils4r.egg-info/
--rw-r--r--   0 rgura001 (52843) rgura001 (52843)     7046 2024-04-19 05:07:34.000000 clfutils4r-1.0.2/src/clfutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      330 2024-04-19 05:07:34.000000 clfutils4r-1.0.2/src/clfutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-04-19 05:07:34.000000 clfutils4r-1.0.2/src/clfutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2024-04-19 05:07:34.000000 clfutils4r-1.0.2/src/clfutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-05-03 20:49:30.627626 clfutils4r-1.0.3/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-1.0.3/LICENSE
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     7046 2024-05-03 20:49:30.627626 clfutils4r-1.0.3/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6402 2024-05-03 19:27:50.000000 clfutils4r-1.0.3/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2024-05-03 20:49:04.000000 clfutils4r-1.0.3/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-05-03 20:49:30.627626 clfutils4r-1.0.3/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:54:18.000000 clfutils4r-1.0.3/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-05-03 20:49:30.627626 clfutils4r-1.0.3/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-05-03 20:49:30.627626 clfutils4r-1.0.3/src/clfutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-1.0.3/src/clfutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    27602 2024-05-03 20:47:57.000000 clfutils4r-1.0.3/src/clfutils4r/eval_classification.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    22088 2024-04-19 04:31:39.000000 clfutils4r-1.0.3/src/clfutils4r/gridsearch_classification.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    10883 2024-04-13 04:18:23.000000 clfutils4r-1.0.3/src/clfutils4r/pretty_cm.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-05-03 20:49:30.627626 clfutils4r-1.0.3/src/clfutils4r.egg-info/
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     7046 2024-05-03 20:49:30.000000 clfutils4r-1.0.3/src/clfutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      330 2024-05-03 20:49:30.000000 clfutils4r-1.0.3/src/clfutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-05-03 20:49:30.000000 clfutils4r-1.0.3/src/clfutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2024-05-03 20:49:30.000000 clfutils4r-1.0.3/src/clfutils4r.egg-info/top_level.txt
```

### Comparing `clfutils4r-1.0.2/LICENSE` & `clfutils4r-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.2/PKG-INFO` & `clfutils4r-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clfutils4r-1.0.2/README.md` & `clfutils4r-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.2/pyproject.toml` & `clfutils4r-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clfutils4r"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn and scikit-plot utilities for classification."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers=[
```

### Comparing `clfutils4r-1.0.2/setup.py` & `clfutils4r-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.2/src/clfutils4r/eval_classification.py` & `clfutils4r-1.0.3/src/clfutils4r/eval_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from sklearn.model_selection import StratifiedKFold
 from sklearn.metrics import accuracy_score, average_precision_score, precision_score, recall_score, f1_score, roc_auc_score
 from sklearn.metrics import confusion_matrix, auc, classification_report, roc_curve, precision_recall_curve
 from sklearn.manifold import TSNE
 
 import scikitplot
 print(f"scikitplot version: {scikitplot.__version__}")
-import pretty_cm # type: ignore
+from . import pretty_cm
 
 import shap
 
 dpi=300
 
 @deprecated
 def print_metrics(y_test=None, y_pred=None, threshold = 0.5):
```

### Comparing `clfutils4r-1.0.2/src/clfutils4r/gridsearch_classification.py` & `clfutils4r-1.0.3/src/clfutils4r/gridsearch_classification.py`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.2/src/clfutils4r/pretty_cm.py` & `clfutils4r-1.0.3/src/clfutils4r/pretty_cm.py`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.2/src/clfutils4r.egg-info/PKG-INFO` & `clfutils4r-1.0.3/src/clfutils4r.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

