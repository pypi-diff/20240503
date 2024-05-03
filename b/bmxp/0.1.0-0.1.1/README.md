# Comparing `tmp/bmxp-0.1.0.tar.gz` & `tmp/bmxp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmxp-0.1.0.tar", last modified: Fri May  3 15:54:00 2024, max compression
+gzip compressed data, was "bmxp-0.1.1.tar", last modified: Fri May  3 16:06:39 2024, max compression
```

## Comparing `bmxp-0.1.0.tar` & `bmxp-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.089717 bmxp-0.1.0/
--rw-rw-rw-   0        0        0     1093 2022-09-27 19:05:11.000000 bmxp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      189 2023-01-09 17:26:29.000000 bmxp-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5478 2024-05-03 15:54:00.088707 bmxp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4810 2024-05-03 15:53:51.000000 bmxp-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.021101 bmxp-0.1.0/bmxp/
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.048101 bmxp-0.1.0/bmxp/blueshift/
--rw-rw-rw-   0        0        0    25428 2024-05-03 15:53:51.000000 bmxp-0.1.0/bmxp/blueshift/__init__.py
--rw-rw-rw-   0        0        0     2226 2024-04-29 17:37:08.000000 bmxp-0.1.0/bmxp/blueshift/blueshift_example.py
--rw-rw-rw-   0        0        0      227 2024-03-06 21:12:28.000000 bmxp-0.1.0/bmxp/blueshift/run_blueshift.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.054103 bmxp-0.1.0/bmxp/eclipse/
--rw-rw-rw-   0        0        0    49812 2024-05-03 15:53:51.000000 bmxp-0.1.0/bmxp/eclipse/__init__.py
--rw-rw-rw-   0        0        0     4367 2024-04-29 17:37:08.000000 bmxp-0.1.0/bmxp/eclipse/eclipse_example.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.063102 bmxp-0.1.0/bmxp/gravity/
--rw-rw-rw-   0        0        0    10337 2024-05-03 15:53:51.000000 bmxp-0.1.0/bmxp/gravity/__init__.py
--rw-rw-rw-   0        0        0     8807 2023-09-18 17:18:55.000000 bmxp-0.1.0/bmxp/gravity/correlation.c
--rw-rw-rw-   0        0        0    17408 2024-02-22 18:27:08.000000 bmxp-0.1.0/bmxp/gravity/correlation.dll
--rw-rw-rw-   0        0        0    16088 2024-03-06 21:23:01.000000 bmxp-0.1.0/bmxp/gravity/correlation.so
--rw-rw-rw-   0        0        0     3725 2023-01-31 21:44:10.000000 bmxp-0.1.0/bmxp/gravity/fallback.py
--rw-rw-rw-   0        0        0      558 2023-03-27 15:45:05.000000 bmxp-0.1.0/bmxp/gravity/gravity_example.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.041100 bmxp-0.1.0/bmxp.egg-info/
--rw-rw-rw-   0        0        0     5478 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1178 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2022-09-27 19:05:11.000000 bmxp-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 15:54:00.089717 bmxp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1289 2024-05-03 15:53:51.000000 bmxp-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.082891 bmxp-0.1.0/tests/
--rw-rw-rw-   0        0        0     8551 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/DCinfo1.csv
--rw-rw-rw-   0        0        0     9374 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/DCinfo2.csv
--rw-rw-rw-   0        0        0   177687 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/DCinput1.csv
--rw-rw-rw-   0        0        0   451309 2024-04-29 17:37:13.000000 bmxp-0.1.0/tests/DCinput2.csv
-drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.087975 bmxp-0.1.0/tests/__pycache__/
--rw-rw-rw-   0        0        0    46139 2024-04-30 18:17:48.000000 bmxp-0.1.0/tests/__pycache__/test_blueshift.cpython-311-pytest-7.4.0.pyc
--rw-rw-rw-   0        0        0    14842 2024-04-29 20:44:55.000000 bmxp-0.1.0/tests/__pycache__/test_blueshift.cpython-38-pytest-7.4.0.pyc
--rw-rw-rw-   0        0        0     1438 2024-04-29 20:44:39.000000 bmxp-0.1.0/tests/__pycache__/test_gravity.cpython-311-pytest-7.4.0.pyc
--rw-rw-rw-   0        0        0     1020 2024-04-29 20:44:55.000000 bmxp-0.1.0/tests/__pycache__/test_gravity.cpython-38-pytest-7.4.0.pyc
--rw-rw-rw-   0        0        0    58914 2024-05-02 16:46:35.000000 bmxp-0.1.0/tests/__pycache__/test_mseclipse.cpython-311-pytest-7.4.0.pyc
--rw-rw-rw-   0        0        0    18250 2024-04-29 20:44:56.000000 bmxp-0.1.0/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.4.0.pyc
--rw-rw-rw-   0        0        0  1376588 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/blueshift.pickle
--rw-rw-rw-   0        0        0    18988 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/example1.csv
--rw-rw-rw-   0        0        0      202 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/make_pickle.py
--rw-rw-rw-   0        0        0   118411 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/mseclipse.pickle
--rw-rw-rw-   0        0        0    13087 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/test1.csv
--rw-rw-rw-   0        0        0    12512 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/test2.csv
--rw-rw-rw-   0        0        0     1239 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/test3.csv
--rw-rw-rw-   0        0        0     8887 2024-05-03 15:53:51.000000 bmxp-0.1.0/tests/test_blueshift.py
--rw-rw-rw-   0        0        0    78529 2023-01-09 17:26:29.000000 bmxp-0.1.0/tests/test_gravity.csv
--rw-rw-rw-   0        0        0      606 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/test_gravity.py
--rw-rw-rw-   0        0        0    11452 2024-05-03 15:53:51.000000 bmxp-0.1.0/tests/test_mseclipse.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.639491 bmxp-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2022-09-27 19:05:11.000000 bmxp-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      189 2023-01-09 17:26:29.000000 bmxp-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5553 2024-05-03 16:06:39.638967 bmxp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4885 2024-05-03 16:06:26.000000 bmxp-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.601657 bmxp-0.1.1/bmxp/
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.613658 bmxp-0.1.1/bmxp/blueshift/
+-rw-rw-rw-   0        0        0    25428 2024-05-03 15:53:51.000000 bmxp-0.1.1/bmxp/blueshift/__init__.py
+-rw-rw-rw-   0        0        0     2226 2024-04-29 17:37:08.000000 bmxp-0.1.1/bmxp/blueshift/blueshift_example.py
+-rw-rw-rw-   0        0        0      227 2024-03-06 21:12:28.000000 bmxp-0.1.1/bmxp/blueshift/run_blueshift.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.614658 bmxp-0.1.1/bmxp/eclipse/
+-rw-rw-rw-   0        0        0    49812 2024-05-03 15:53:51.000000 bmxp-0.1.1/bmxp/eclipse/__init__.py
+-rw-rw-rw-   0        0        0     4367 2024-04-29 17:37:08.000000 bmxp-0.1.1/bmxp/eclipse/eclipse_example.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.619657 bmxp-0.1.1/bmxp/gravity/
+-rw-rw-rw-   0        0        0    10337 2024-05-03 15:53:51.000000 bmxp-0.1.1/bmxp/gravity/__init__.py
+-rw-rw-rw-   0        0        0     8807 2023-09-18 17:18:55.000000 bmxp-0.1.1/bmxp/gravity/correlation.c
+-rw-rw-rw-   0        0        0    17408 2024-02-22 18:27:08.000000 bmxp-0.1.1/bmxp/gravity/correlation.dll
+-rw-rw-rw-   0        0        0    16088 2024-03-06 21:23:01.000000 bmxp-0.1.1/bmxp/gravity/correlation.so
+-rw-rw-rw-   0        0        0     3725 2023-01-31 21:44:10.000000 bmxp-0.1.1/bmxp/gravity/fallback.py
+-rw-rw-rw-   0        0        0      558 2023-03-27 15:45:05.000000 bmxp-0.1.1/bmxp/gravity/gravity_example.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.611657 bmxp-0.1.1/bmxp.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-05-03 16:06:39.000000 bmxp-0.1.1/bmxp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1178 2024-05-03 16:06:39.000000 bmxp-0.1.1/bmxp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:06:39.000000 bmxp-0.1.1/bmxp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-03 16:06:39.000000 bmxp-0.1.1/bmxp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 16:06:39.000000 bmxp-0.1.1/bmxp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2022-09-27 19:05:11.000000 bmxp-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 16:06:39.639491 bmxp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1289 2024-05-03 16:06:26.000000 bmxp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.631658 bmxp-0.1.1/tests/
+-rw-rw-rw-   0        0        0     8551 2024-04-29 17:37:08.000000 bmxp-0.1.1/tests/DCinfo1.csv
+-rw-rw-rw-   0        0        0     9374 2024-04-29 17:37:08.000000 bmxp-0.1.1/tests/DCinfo2.csv
+-rw-rw-rw-   0        0        0   177687 2024-04-29 17:37:08.000000 bmxp-0.1.1/tests/DCinput1.csv
+-rw-rw-rw-   0        0        0   451309 2024-04-29 17:37:13.000000 bmxp-0.1.1/tests/DCinput2.csv
+drwxrwxrwx   0        0        0        0 2024-05-03 16:06:39.637895 bmxp-0.1.1/tests/__pycache__/
+-rw-rw-rw-   0        0        0    46139 2024-05-03 15:54:05.000000 bmxp-0.1.1/tests/__pycache__/test_blueshift.cpython-311-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0    14842 2024-04-29 20:44:55.000000 bmxp-0.1.1/tests/__pycache__/test_blueshift.cpython-38-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0     1438 2024-04-29 20:44:39.000000 bmxp-0.1.1/tests/__pycache__/test_gravity.cpython-311-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0     1020 2024-04-29 20:44:55.000000 bmxp-0.1.1/tests/__pycache__/test_gravity.cpython-38-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0    58930 2024-05-03 15:54:07.000000 bmxp-0.1.1/tests/__pycache__/test_mseclipse.cpython-311-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0    18250 2024-04-29 20:44:56.000000 bmxp-0.1.1/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0  1376588 2024-04-29 17:37:08.000000 bmxp-0.1.1/tests/blueshift.pickle
+-rw-rw-rw-   0        0        0    18988 2022-09-27 19:05:11.000000 bmxp-0.1.1/tests/example1.csv
+-rw-rw-rw-   0        0        0      202 2022-09-27 19:05:11.000000 bmxp-0.1.1/tests/make_pickle.py
+-rw-rw-rw-   0        0        0   118411 2022-09-27 19:05:11.000000 bmxp-0.1.1/tests/mseclipse.pickle
+-rw-rw-rw-   0        0        0    13087 2022-09-27 19:05:11.000000 bmxp-0.1.1/tests/test1.csv
+-rw-rw-rw-   0        0        0    12512 2022-09-27 19:05:11.000000 bmxp-0.1.1/tests/test2.csv
+-rw-rw-rw-   0        0        0     1239 2022-09-27 19:05:11.000000 bmxp-0.1.1/tests/test3.csv
+-rw-rw-rw-   0        0        0     8887 2024-05-03 15:53:51.000000 bmxp-0.1.1/tests/test_blueshift.py
+-rw-rw-rw-   0        0        0    78529 2023-01-09 17:26:29.000000 bmxp-0.1.1/tests/test_gravity.csv
+-rw-rw-rw-   0        0        0      606 2024-04-29 17:37:08.000000 bmxp-0.1.1/tests/test_gravity.py
+-rw-rw-rw-   0        0        0    11452 2024-05-03 15:53:51.000000 bmxp-0.1.1/tests/test_mseclipse.py
```

### Comparing `bmxp-0.1.0/LICENSE` & `bmxp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/PKG-INFO` & `bmxp-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmxp
-Version: 0.1.0
+Version: 0.1.1
 Summary: LCMS Processing tools used by the Metabolomics Platform at the Broad Institute.
 Home-page: https://github.com/broadinstitute/bmxp
 Author: Daniel S. Hitchcock
 Author-email: daniel.s.hitchcock@gmail.com
 License: MIT
 Keywords: LCMS,Alignment,Processing,Metabolomics,Clustering,Batch Correction,Drift Correction
 Classifier: License :: OSI Approved :: MIT License
@@ -21,17 +21,17 @@
 `pip install bmxp`
 
 Please cite:
 https://www.biorxiv.org/content/10.1101/2023.06.09.544417v1.full
 
 This is a collection of tools for processing our data, which powers our cloud processing workflow. Each tool is meant to be a standalone module that performs a step in our processing pipeline. They are written in Python and C, and designed to be perfomant and cloud-compatible.
 
-* [Eclipse](https://github.com/broadinstitute/bmxp/eclipse) - Align two or more same-method nontargeted LCMS datsets.
-* [Gravity](https://github.com/broadinstitute/bmxp/gravity) - Cluster redundant LCMS features based on RT and Correlation (And someday, XIC shape)
-* [Blueshift](https://github.com/broadinstitute/bmxp/blueshift) - Drift Correction via pooled technical replicates and internal standards
+* [Eclipse](https://github.com/broadinstitute/bmxp/blob/main/bmxp/eclipse/readme.md) - Align two or more same-method nontargeted LCMS datsets.
+* [Gravity](https://github.com/broadinstitute/bmxp/blob/main/bmxp/gravity/readme.md) - Cluster redundant LCMS features based on RT and Correlation (And someday, XIC shape)
+* [Blueshift](https://github.com/broadinstitute/bmxp/blob/main/bmxp/blueshift/readme.md) - Drift Correction via pooled technical replicates and internal standards
 
 In the future we will add:
 * Rawfilereader - Performant LCMS raw file reader (.mzml, .raw)
 * Formation - Format and Generate metrics for finalized datasets
 
 We expect users to be familiar with Python and already have an understanding of LCMS Metabolomics data processing and the specific steps they wish to accomplish.
```

### Comparing `bmxp-0.1.0/README.md` & `bmxp-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 `pip install bmxp`
 
 Please cite:
 https://www.biorxiv.org/content/10.1101/2023.06.09.544417v1.full
 
 This is a collection of tools for processing our data, which powers our cloud processing workflow. Each tool is meant to be a standalone module that performs a step in our processing pipeline. They are written in Python and C, and designed to be perfomant and cloud-compatible.
 
-* [Eclipse](https://github.com/broadinstitute/bmxp/eclipse) - Align two or more same-method nontargeted LCMS datsets.
-* [Gravity](https://github.com/broadinstitute/bmxp/gravity) - Cluster redundant LCMS features based on RT and Correlation (And someday, XIC shape)
-* [Blueshift](https://github.com/broadinstitute/bmxp/blueshift) - Drift Correction via pooled technical replicates and internal standards
+* [Eclipse](https://github.com/broadinstitute/bmxp/blob/main/bmxp/eclipse/readme.md) - Align two or more same-method nontargeted LCMS datsets.
+* [Gravity](https://github.com/broadinstitute/bmxp/blob/main/bmxp/gravity/readme.md) - Cluster redundant LCMS features based on RT and Correlation (And someday, XIC shape)
+* [Blueshift](https://github.com/broadinstitute/bmxp/blob/main/bmxp/blueshift/readme.md) - Drift Correction via pooled technical replicates and internal standards
 
 In the future we will add:
 * Rawfilereader - Performant LCMS raw file reader (.mzml, .raw)
 * Formation - Format and Generate metrics for finalized datasets
 
 We expect users to be familiar with Python and already have an understanding of LCMS Metabolomics data processing and the specific steps they wish to accomplish.
```

### Comparing `bmxp-0.1.0/bmxp/blueshift/__init__.py` & `bmxp-0.1.1/bmxp/blueshift/__init__.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/blueshift/blueshift_example.py` & `bmxp-0.1.1/bmxp/blueshift/blueshift_example.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/eclipse/__init__.py` & `bmxp-0.1.1/bmxp/eclipse/__init__.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/eclipse/eclipse_example.py` & `bmxp-0.1.1/bmxp/eclipse/eclipse_example.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/gravity/__init__.py` & `bmxp-0.1.1/bmxp/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/gravity/correlation.c` & `bmxp-0.1.1/bmxp/gravity/correlation.c`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/gravity/correlation.dll` & `bmxp-0.1.1/bmxp/gravity/correlation.dll`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/gravity/correlation.so` & `bmxp-0.1.1/bmxp/gravity/correlation.so`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/gravity/fallback.py` & `bmxp-0.1.1/bmxp/gravity/fallback.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp/gravity/gravity_example.py` & `bmxp-0.1.1/bmxp/gravity/gravity_example.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/bmxp.egg-info/PKG-INFO` & `bmxp-0.1.1/bmxp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmxp
-Version: 0.1.0
+Version: 0.1.1
 Summary: LCMS Processing tools used by the Metabolomics Platform at the Broad Institute.
 Home-page: https://github.com/broadinstitute/bmxp
 Author: Daniel S. Hitchcock
 Author-email: daniel.s.hitchcock@gmail.com
 License: MIT
 Keywords: LCMS,Alignment,Processing,Metabolomics,Clustering,Batch Correction,Drift Correction
 Classifier: License :: OSI Approved :: MIT License
@@ -21,17 +21,17 @@
 `pip install bmxp`
 
 Please cite:
 https://www.biorxiv.org/content/10.1101/2023.06.09.544417v1.full
 
 This is a collection of tools for processing our data, which powers our cloud processing workflow. Each tool is meant to be a standalone module that performs a step in our processing pipeline. They are written in Python and C, and designed to be perfomant and cloud-compatible.
 
-* [Eclipse](https://github.com/broadinstitute/bmxp/eclipse) - Align two or more same-method nontargeted LCMS datsets.
-* [Gravity](https://github.com/broadinstitute/bmxp/gravity) - Cluster redundant LCMS features based on RT and Correlation (And someday, XIC shape)
-* [Blueshift](https://github.com/broadinstitute/bmxp/blueshift) - Drift Correction via pooled technical replicates and internal standards
+* [Eclipse](https://github.com/broadinstitute/bmxp/blob/main/bmxp/eclipse/readme.md) - Align two or more same-method nontargeted LCMS datsets.
+* [Gravity](https://github.com/broadinstitute/bmxp/blob/main/bmxp/gravity/readme.md) - Cluster redundant LCMS features based on RT and Correlation (And someday, XIC shape)
+* [Blueshift](https://github.com/broadinstitute/bmxp/blob/main/bmxp/blueshift/readme.md) - Drift Correction via pooled technical replicates and internal standards
 
 In the future we will add:
 * Rawfilereader - Performant LCMS raw file reader (.mzml, .raw)
 * Formation - Format and Generate metrics for finalized datasets
 
 We expect users to be familiar with Python and already have an understanding of LCMS Metabolomics data processing and the specific steps they wish to accomplish.
```

### Comparing `bmxp-0.1.0/bmxp.egg-info/SOURCES.txt` & `bmxp-0.1.1/bmxp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/setup.py` & `bmxp-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(os.path.join(HERE, "requirements.txt"), encoding="utf-8") as f:
     REQUIREMENTS = f.read()
 
 module1 = Extension
 setup(
     name="bmxp",
     install_requires=REQUIREMENTS.split("\n"),
-    version="0.1.0",
+    version="0.1.1",
     description="LCMS Processing tools used by the Metabolomics Platform at the Broad"
     " Institute.",
     packages=find_namespace_packages(include=["bmxp.*"]),
     license="MIT",
     author="Daniel S. Hitchcock",
     author_email="daniel.s.hitchcock@gmail.com",
     long_description_content_type="text/markdown",
```

### Comparing `bmxp-0.1.0/tests/DCinfo1.csv` & `bmxp-0.1.1/tests/DCinfo1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/DCinfo2.csv` & `bmxp-0.1.1/tests/DCinfo2.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/DCinput1.csv` & `bmxp-0.1.1/tests/DCinput1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/DCinput2.csv` & `bmxp-0.1.1/tests/DCinput2.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/__pycache__/test_blueshift.cpython-311-pytest-7.4.0.pyc` & `bmxp-0.1.1/tests/__pycache__/test_blueshift.cpython-311-pytest-7.4.0.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xca353166 (Tue Apr 30 18:17:46 2024 UTC)
+moddate:  0x8f083566 (Fri May  3 15:53:51 2024 UTC)
 files sz: 8887
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `bmxp-0.1.0/tests/__pycache__/test_blueshift.cpython-38-pytest-7.4.0.pyc` & `bmxp-0.1.1/tests/__pycache__/test_blueshift.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/__pycache__/test_gravity.cpython-311-pytest-7.4.0.pyc` & `bmxp-0.1.1/tests/__pycache__/test_gravity.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/__pycache__/test_gravity.cpython-38-pytest-7.4.0.pyc` & `bmxp-0.1.1/tests/__pycache__/test_gravity.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/__pycache__/test_mseclipse.cpython-311-pytest-7.4.0.pyc` & `bmxp-0.1.1/tests/__pycache__/test_mseclipse.cpython-311-pytest-7.4.0.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x67c33366 (Thu May  2 16:46:31 2024 UTC)
-files sz: 11261
+moddate:  0x8f083566 (Fri May  3 15:53:51 2024 UTC)
+files sz: 11452
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x970064005a00640164026c015a02640164026c036d04630201006d055a
@@ -215,15 +215,15 @@
                526 MAKE_FUNCTION            0
                528 STORE_NAME              34 (test_dataset_selection)
    
    311         530 LOAD_CONST              19 (<code object test_schema, file "C:\Users\danie\PycharmProjects\bmxp\tests\test_mseclipse.py", line 311>)
                532 MAKE_FUNCTION            0
                534 STORE_NAME              35 (test_schema)
    
-   324         536 LOAD_CONST              20 (<code object test_instance_params, file "C:\Users\danie\PycharmProjects\bmxp\tests\test_mseclipse.py", line 324>)
+   330         536 LOAD_CONST              20 (<code object test_instance_params, file "C:\Users\danie\PycharmProjects\bmxp\tests\test_mseclipse.py", line 330>)
                538 MAKE_FUNCTION            0
                540 STORE_NAME              36 (test_instance_params)
                542 LOAD_CONST               2 (None)
                544 RETURN_VALUE
    consts
       '\nTests for MSEclipse\n'
       0
@@ -7630,36 +7630,41 @@
          
          314          90 LOAD_CONST               5 (('Compound_ID', 'RT', 'MZ', 'Intensity'))
                       92 BUILD_CONST_KEY_MAP      4
                       94 STORE_FAST               2 (schema_labels)
          
          321          96 LOAD_GLOBAL              3 (NULL + ms)
                      108 LOAD_ATTR                2 (MSAligner)
-                     118 LOAD_FAST                0 (dataframe_1)
+         
+         322         118 LOAD_FAST                0 (dataframe_1)
                      120 LOAD_METHOD              3 (rename)
                      142 LOAD_FAST                2 (schema_labels)
                      144 KW_NAMES                 6
                      146 PRECALL                  1
                      150 CALL                     1
-                     160 LOAD_FAST                1 (dataframe_2)
+         
+         323         160 LOAD_FAST                1 (dataframe_2)
                      162 LOAD_METHOD              3 (rename)
                      184 LOAD_FAST                2 (schema_labels)
                      186 KW_NAMES                 6
                      188 PRECALL                  1
                      192 CALL                     1
-                     202 LOAD_CONST               7 ('DS1')
+         
+         324         202 LOAD_CONST               7 ('DS1')
                      204 LOAD_CONST               8 ('DS2')
                      206 BUILD_LIST               2
-                     208 LOAD_FAST                2 (schema_labels)
-                     210 KW_NAMES                 9
+         
+         325         208 LOAD_FAST                2 (schema_labels)
+         
+         321         210 KW_NAMES                 9
                      212 PRECALL                  4
                      216 CALL                     4
                      226 STORE_FAST               3 (a)
          
-         322         228 LOAD_FAST                3 (a)
+         327         228 LOAD_FAST                3 (a)
                      230 LOAD_METHOD              4 (align)
                      252 PRECALL                  0
                      256 CALL                     0
                      266 POP_TOP
                      268 LOAD_CONST               0 (None)
                      270 RETURN_VALUE
          consts
@@ -7676,15 +7681,15 @@
          names      ('copy', 'ms', 'MSAligner', 'rename', 'align')
          varnames   ('dataframe_1', 'dataframe_2', 'schema_labels', 'a')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\danie\\PycharmProjects\\bmxp\\tests\\test_mseclipse.py'
          name       'test_schema'
          firstlineno 311
-         lnotab 0x02012801280202010201020102fc06078401
+         lnotab 0x02012801280202010201020102fc060716012a012a01060102fc1206
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x97006401640269017d037c00a000000000000000000000000000000000
@@ -7704,144 +7709,157 @@
             0001007405000000000000000000006a0300000000000000007c007c017c
             0267006404a2017c03ac05a6050000ab0500000000000000007d04640664
             0764089c027c045f0400000000000000007c04a009000000000000000000
             000000000000000000000064026409640a640b9c026901640c640d640e69
             01640f9c03a6010000ab01000000000000000001007c04a0080000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             0064005300
-         324           0 RESUME                   0
+         330           0 RESUME                   0
          
-         325           2 LOAD_CONST               1 ('RT')
+         331           2 LOAD_CONST               1 ('RT')
                        4 LOAD_CONST               2 ('rt (min)')
                        6 BUILD_MAP                1
                        8 STORE_FAST               3 (schema_labels)
          
-         326          10 LOAD_FAST                0 (dataframe_1)
+         332          10 LOAD_FAST                0 (dataframe_1)
                       12 LOAD_METHOD              0 (copy)
                       34 PRECALL                  0
                       38 CALL                     0
                       48 LOAD_METHOD              1 (rename)
                       70 LOAD_FAST                3 (schema_labels)
                       72 KW_NAMES                 3
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_FAST               0 (dataframe_1)
          
-         327          90 LOAD_FAST                1 (dataframe_2)
+         333          90 LOAD_FAST                1 (dataframe_2)
                       92 LOAD_METHOD              0 (copy)
                      114 PRECALL                  0
                      118 CALL                     0
                      128 LOAD_METHOD              1 (rename)
                      150 LOAD_FAST                3 (schema_labels)
                      152 KW_NAMES                 3
                      154 PRECALL                  1
                      158 CALL                     1
                      168 STORE_FAST               1 (dataframe_2)
          
-         328         170 LOAD_FAST                2 (dataframe_3)
+         334         170 LOAD_FAST                2 (dataframe_3)
                      172 LOAD_METHOD              0 (copy)
                      194 PRECALL                  0
                      198 CALL                     0
                      208 LOAD_METHOD              1 (rename)
                      230 LOAD_FAST                3 (schema_labels)
                      232 KW_NAMES                 3
                      234 PRECALL                  1
                      238 CALL                     1
                      248 STORE_FAST               2 (dataframe_3)
          
-         330         250 LOAD_GLOBAL              5 (NULL + ms)
+         336         250 LOAD_GLOBAL              5 (NULL + ms)
                      262 LOAD_ATTR                3 (MSAligner)
-                     272 LOAD_FAST                0 (dataframe_1)
-                     274 LOAD_FAST                1 (dataframe_2)
-                     276 LOAD_FAST                2 (dataframe_3)
-                     278 BUILD_LIST               0
+         
+         337         272 LOAD_FAST                0 (dataframe_1)
+         
+         338         274 LOAD_FAST                1 (dataframe_2)
+         
+         339         276 LOAD_FAST                2 (dataframe_3)
+         
+         340         278 BUILD_LIST               0
                      280 LOAD_CONST               4 (('DS1', 'DS2', 'DS3'))
                      282 LIST_EXTEND              1
-                     284 LOAD_FAST                3 (schema_labels)
-                     286 KW_NAMES                 5
+         
+         341         284 LOAD_FAST                3 (schema_labels)
+         
+         336         286 KW_NAMES                 5
                      288 PRECALL                  5
                      292 CALL                     5
                      302 STORE_FAST               4 (a)
          
-         331         304 LOAD_CONST               6 ('linear')
+         343         304 LOAD_CONST               6 ('linear')
                      306 LOAD_CONST               7 ('ppm')
                      308 LOAD_CONST               8 (('rt (min)', 'MZ'))
                      310 BUILD_CONST_KEY_MAP      2
                      312 LOAD_FAST                4 (a)
                      314 STORE_ATTR               4 (descriptors)
          
-         332         324 LOAD_CONST               9 (1.0)
+         344         324 LOAD_CONST               9 (1.0)
                      326 LOAD_CONST              10 (-1.0)
                      328 LOAD_CONST              11 (('upper', 'lower'))
                      330 BUILD_CONST_KEY_MAP      2
                      332 LOAD_FAST                4 (a)
                      334 LOAD_ATTR                5 (default_coarse_params)
                      344 LOAD_CONST               2 ('rt (min)')
                      346 STORE_SUBSCR
          
-         333         350 LOAD_CONST              12 (10)
+         345         350 LOAD_CONST              12 (10)
                      352 LOAD_FAST                4 (a)
                      354 STORE_ATTR               6 (default_cutoff)
          
-         334         364 LOAD_CONST              13 ('MZ')
+         346         364 LOAD_CONST              13 ('MZ')
                      366 LOAD_CONST              14 (6)
                      368 BUILD_MAP                1
                      370 LOAD_FAST                4 (a)
                      372 STORE_ATTR               7 (default_cutoffs)
          
-         335         382 LOAD_FAST                4 (a)
+         347         382 LOAD_FAST                4 (a)
                      384 LOAD_METHOD              8 (align)
                      406 PRECALL                  0
                      410 CALL                     0
                      420 POP_TOP
          
-         337         422 LOAD_GLOBAL              5 (NULL + ms)
+         349         422 LOAD_GLOBAL              5 (NULL + ms)
                      434 LOAD_ATTR                3 (MSAligner)
-                     444 LOAD_FAST                0 (dataframe_1)
-                     446 LOAD_FAST                1 (dataframe_2)
-                     448 LOAD_FAST                2 (dataframe_3)
-                     450 BUILD_LIST               0
+         
+         350         444 LOAD_FAST                0 (dataframe_1)
+         
+         351         446 LOAD_FAST                1 (dataframe_2)
+         
+         352         448 LOAD_FAST                2 (dataframe_3)
+         
+         353         450 BUILD_LIST               0
                      452 LOAD_CONST               4 (('DS1', 'DS2', 'DS3'))
                      454 LIST_EXTEND              1
-                     456 LOAD_FAST                3 (schema_labels)
-                     458 KW_NAMES                 5
+         
+         354         456 LOAD_FAST                3 (schema_labels)
+         
+         349         458 KW_NAMES                 5
                      460 PRECALL                  5
                      464 CALL                     5
                      474 STORE_FAST               4 (a)
          
-         338         476 LOAD_CONST               6 ('linear')
+         356         476 LOAD_CONST               6 ('linear')
                      478 LOAD_CONST               7 ('ppm')
                      480 LOAD_CONST               8 (('rt (min)', 'MZ'))
                      482 BUILD_CONST_KEY_MAP      2
                      484 LOAD_FAST                4 (a)
                      486 STORE_ATTR               4 (descriptors)
          
-         339         496 LOAD_FAST                4 (a)
+         357         496 LOAD_FAST                4 (a)
                      498 LOAD_METHOD              9 (set_instance_defaults)
          
-         340         520 LOAD_CONST               2 ('rt (min)')
+         359         520 LOAD_CONST               2 ('rt (min)')
                      522 LOAD_CONST               9 (1.0)
                      524 LOAD_CONST              10 (-1.0)
                      526 LOAD_CONST              11 (('upper', 'lower'))
                      528 BUILD_CONST_KEY_MAP      2
                      530 BUILD_MAP                1
          
-         341         532 LOAD_CONST              12 (10)
+         360         532 LOAD_CONST              12 (10)
          
-         342         534 LOAD_CONST              13 ('MZ')
+         361         534 LOAD_CONST              13 ('MZ')
                      536 LOAD_CONST              14 (6)
                      538 BUILD_MAP                1
          
-         339         540 LOAD_CONST              15 (('coarse_params', 'cutoff', 'cutoffs'))
+         358         540 LOAD_CONST              15 (('coarse_params', 'cutoff', 'cutoffs'))
                      542 BUILD_CONST_KEY_MAP      3
-                     544 PRECALL                  1
+         
+         357         544 PRECALL                  1
                      548 CALL                     1
                      558 POP_TOP
          
-         344         560 LOAD_FAST                4 (a)
+         364         560 LOAD_FAST                4 (a)
                      562 LOAD_METHOD              8 (align)
                      584 PRECALL                  0
                      588 CALL                     0
                      598 POP_TOP
                      600 LOAD_CONST               0 (None)
                      602 RETURN_VALUE
          consts
@@ -7863,23 +7881,24 @@
             ('coarse_params', 'cutoff', 'cutoffs')
          names      ('copy', 'rename', 'ms', 'MSAligner', 'descriptors', 'default_coarse_params', 'default_cutoff', 'default_cutoffs', 'align', 'set_instance_defaults')
          varnames   ('dataframe_1', 'dataframe_2', 'dataframe_3', 'schema_labels', 'a')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\danie\\PycharmProjects\\bmxp\\tests\\test_mseclipse.py'
          name       'test_instance_params'
-         firstlineno 324
+         firstlineno 330
          lnotab
-            0x02010801500150015002360114011a010e01120128023601140118010c
-            01020106fd1405
+            0x020108015001500150021601020102010201060102fb120714011a010e
+            01120128021601020102010201060102fb1207140118020c01020106fd04
+            ff1007
    names      ('__doc__', 'builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pathlib', 'Path', 'pickle', 'pytest', 'numpy', 'np', 'pandas', 'pd', 'bmxp.eclipse', 'eclipse', 'ms', 'fixture', 'filepath_1', 'filepath_2', 'filepath_3', 'dataframe_1', 'dataframe_2', 'dataframe_3', 'pickled_ms', 'test_initialize_add', 'test_add_dataset', 'test_alignment_methods', 'test_calc_score', 'mark', 'filterwarnings', 'test_calc_scalers', 'test_adding_intensity_column', 'test_dataset_selection', 'test_schema', 'test_instance_params')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\danie\\PycharmProjects\\bmxp\\tests\\test_mseclipse.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02020403260108010801080108010c031c0104ff0e0102071c0104
       ff0e0102071c0104ff0e0102071c0104ff0e0102071c0104ff0e0102071c
       0104ff0e0102071c0104ff0e01020b061b0618066e060e320104ff0e0102
-      0f060d0622060d
+      0f060d06220613
```

### Comparing `bmxp-0.1.0/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.4.0.pyc` & `bmxp-0.1.1/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/blueshift.pickle` & `bmxp-0.1.1/tests/blueshift.pickle`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/example1.csv` & `bmxp-0.1.1/tests/example1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/mseclipse.pickle` & `bmxp-0.1.1/tests/mseclipse.pickle`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/test1.csv` & `bmxp-0.1.1/tests/test1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/test2.csv` & `bmxp-0.1.1/tests/test2.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/test3.csv` & `bmxp-0.1.1/tests/test3.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/test_blueshift.py` & `bmxp-0.1.1/tests/test_blueshift.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/test_gravity.csv` & `bmxp-0.1.1/tests/test_gravity.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/test_gravity.py` & `bmxp-0.1.1/tests/test_gravity.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.1.0/tests/test_mseclipse.py` & `bmxp-0.1.1/tests/test_mseclipse.py`

 * *Files identical despite different names*

