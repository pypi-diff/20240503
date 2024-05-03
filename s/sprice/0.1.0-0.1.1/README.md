# Comparing `tmp/sprice-0.1.0.tar.gz` & `tmp/sprice-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sprice-0.1.0.tar", last modified: Fri May  3 01:15:30 2024, max compression
+gzip compressed data, was "dist\sprice-0.1.1.tar", last modified: Fri May  3 03:12:40 2024, max compression
```

## Comparing `sprice-0.1.0.tar` & `sprice-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 01:15:30.760671 sprice-0.1.0/
--rw-rw-rw-   0        0        0       74 2024-05-02 02:58:05.000000 sprice-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8589 2024-05-03 01:15:30.759888 sprice-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7629 2024-05-03 01:06:50.000000 sprice-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 01:15:30.760874 sprice-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      671 2024-05-02 02:57:25.000000 sprice-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:15:30.691537 sprice-0.1.0/sprice/
--rw-rw-rw-   0        0        0        0 2024-05-02 02:55:28.000000 sprice-0.1.0/sprice/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-02 02:55:06.000000 sprice-0.1.0/sprice/core.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:15:30.751317 sprice-0.1.0/sprice/data/
--rw-rw-rw-   0        0        0  1157290 2024-05-02 01:55:06.000000 sprice-0.1.0/sprice/data/sprice_data_1.h5
--rw-rw-rw-   0        0        0  1164756 2024-05-02 01:53:50.000000 sprice-0.1.0/sprice/data/sprice_data_2.h5
-drwxrwxrwx   0        0        0        0 2024-05-03 01:15:30.726952 sprice-0.1.0/sprice.egg-info/
--rw-rw-rw-   0        0        0     8589 2024-05-03 01:15:30.000000 sprice-0.1.0/sprice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-05-03 01:15:30.000000 sprice-0.1.0/sprice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 01:15:30.000000 sprice-0.1.0/sprice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-03 01:15:30.000000 sprice-0.1.0/sprice.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 01:15:30.000000 sprice-0.1.0/sprice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 03:12:40.512063 sprice-0.1.1/
+-rw-rw-rw-   0        0        0       74 2024-05-02 02:58:05.000000 sprice-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8589 2024-05-03 03:12:40.509686 sprice-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7629 2024-05-03 01:06:50.000000 sprice-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 03:12:40.513163 sprice-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      791 2024-05-03 03:12:38.000000 sprice-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:12:40.436805 sprice-0.1.1/sprice/
+-rw-rw-rw-   0        0        0      512 2024-05-03 02:29:23.000000 sprice-0.1.1/sprice/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 02:55:06.000000 sprice-0.1.1/sprice/core.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:12:40.500341 sprice-0.1.1/sprice/data/
+-rw-rw-rw-   0        0        0  1157290 2024-05-02 01:55:06.000000 sprice-0.1.1/sprice/data/sprice_data_1.h5
+-rw-rw-rw-   0        0        0  1164756 2024-05-02 01:53:50.000000 sprice-0.1.1/sprice/data/sprice_data_2.h5
+drwxrwxrwx   0        0        0        0 2024-05-03 03:12:40.485143 sprice-0.1.1/sprice.egg-info/
+-rw-rw-rw-   0        0        0     8589 2024-05-03 03:12:40.000000 sprice-0.1.1/sprice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-05-03 03:12:40.000000 sprice-0.1.1/sprice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 03:12:40.000000 sprice-0.1.1/sprice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-03 03:12:40.000000 sprice-0.1.1/sprice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 03:12:40.000000 sprice-0.1.1/sprice.egg-info/top_level.txt
```

### Comparing `sprice-0.1.0/PKG-INFO` & `sprice-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprice
-Version: 0.1.0
+Version: 0.1.1
 Summary: Consumer price data package for Saudi Arabia
 Home-page: https://github.com/amjad-alt/sprice
 Author: Amjad Altuwayjiri
 Author-email: amjadibrahim1994@gmail.com
 License: UNKNOWN
 Description: 
         # Sprice - Consumer Price Data for Saudi Arabia
```

### Comparing `sprice-0.1.0/README.md` & `sprice-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sprice-0.1.0/setup.py` & `sprice-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sprice',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     # This tells setuptools to include files listed in MANIFEST.in
     include_package_data=True,
+    package_data={
+        # Include all .h5 files under the data directory
+        'sprice': ['data/*.h5'],
+    },
     install_requires=[
         'pandas',  # Add other dependencies needed for your package
         'h5py'
     ],
     description='Consumer price data package for Saudi Arabia',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `sprice-0.1.0/sprice/data/sprice_data_1.h5` & `sprice-0.1.1/sprice/data/sprice_data_1.h5`

 * *Files identical despite different names*

### Comparing `sprice-0.1.0/sprice/data/sprice_data_2.h5` & `sprice-0.1.1/sprice/data/sprice_data_2.h5`

 * *Files identical despite different names*

### Comparing `sprice-0.1.0/sprice.egg-info/PKG-INFO` & `sprice-0.1.1/sprice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprice
-Version: 0.1.0
+Version: 0.1.1
 Summary: Consumer price data package for Saudi Arabia
 Home-page: https://github.com/amjad-alt/sprice
 Author: Amjad Altuwayjiri
 Author-email: amjadibrahim1994@gmail.com
 License: UNKNOWN
 Description: 
         # Sprice - Consumer Price Data for Saudi Arabia
```

