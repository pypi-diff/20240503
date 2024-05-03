# Comparing `tmp/nutrical-0.0.1.tar.gz` & `tmp/nutrical-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutrical-0.0.1.tar", last modified: Fri May  3 01:48:53 2024, max compression
+gzip compressed data, was "nutrical-0.0.2.tar", last modified: Fri May  3 02:05:16 2024, max compression
```

## Comparing `nutrical-0.0.1.tar` & `nutrical-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 01:48:53.068913 nutrical-0.0.1/
--rw-rw-rw-   0        0        0     3132 2024-05-03 01:48:53.067194 nutrical-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2024-05-03 00:57:09.000000 nutrical-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 01:48:53.042732 nutrical-0.0.1/data/
--rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.1/data/TW_FDA_nutrition_items.csv
-drwxrwxrwx   0        0        0        0 2024-05-03 01:48:53.037586 nutrical-0.0.1/foodie/
--rw-rw-rw-   0        0        0       22 2024-05-03 00:35:00.000000 nutrical-0.0.1/foodie/__init__.py
--rw-rw-rw-   0        0        0     3955 2024-05-03 00:53:01.000000 nutrical-0.0.1/foodie/foodie.py
--rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.1/foodie/taiwan-fda.py
--rw-rw-rw-   0        0        0     1408 2024-05-03 00:52:10.000000 nutrical-0.0.1/foodie/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:48:53.063113 nutrical-0.0.1/nutrical.egg-info/
--rw-rw-rw-   0        0        0     3132 2024-05-03 01:48:52.000000 nutrical-0.0.1/nutrical.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-03 01:48:52.000000 nutrical-0.0.1/nutrical.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 01:48:52.000000 nutrical-0.0.1/nutrical.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 01:48:52.000000 nutrical-0.0.1/nutrical.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 01:48:52.000000 nutrical-0.0.1/nutrical.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 01:48:53.070895 nutrical-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      827 2024-05-03 01:48:48.000000 nutrical-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:48:53.065310 nutrical-0.0.1/test/
--rw-rw-rw-   0        0        0      954 2024-05-02 08:53:18.000000 nutrical-0.0.1/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:05:16.413337 nutrical-0.0.2/
+-rw-rw-rw-   0        0        0     3132 2024-05-03 02:05:16.410939 nutrical-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2024-05-03 00:57:09.000000 nutrical-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 02:05:16.400400 nutrical-0.0.2/data/
+-rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.2/data/TW_FDA_nutrition_items.csv
+drwxrwxrwx   0        0        0        0 2024-05-03 02:05:16.370548 nutrical-0.0.2/nutrical/
+-rw-rw-rw-   0        0        0       24 2024-05-03 01:55:26.000000 nutrical-0.0.2/nutrical/__init__.py
+-rw-rw-rw-   0        0        0     3955 2024-05-03 01:55:45.000000 nutrical-0.0.2/nutrical/nutrical.py
+-rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.2/nutrical/taiwan-fda.py
+-rw-rw-rw-   0        0        0     1408 2024-05-03 00:52:10.000000 nutrical-0.0.2/nutrical/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:05:16.396805 nutrical-0.0.2/nutrical.egg-info/
+-rw-rw-rw-   0        0        0     3132 2024-05-03 02:05:16.000000 nutrical-0.0.2/nutrical.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-03 02:05:16.000000 nutrical-0.0.2/nutrical.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 02:05:16.000000 nutrical-0.0.2/nutrical.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 02:05:16.000000 nutrical-0.0.2/nutrical.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 02:05:16.000000 nutrical-0.0.2/nutrical.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 02:05:16.413337 nutrical-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      915 2024-05-03 02:05:07.000000 nutrical-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:05:16.402858 nutrical-0.0.2/test/
+-rw-rw-rw-   0        0        0      954 2024-05-02 08:53:18.000000 nutrical-0.0.2/test/test.py
```

### Comparing `nutrical-0.0.1/PKG-INFO` & `nutrical-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutrical
-Version: 0.0.1
+Version: 0.0.2
 Summary: Nutrition calculation for recipes and ingredients
 Home-page: https://github.com/liao961120/nutrical
 Author: Yongfu Liao
 Author-email: liao961120@gmail.com
 License: UNKNOWN
 Description: Nutrition calculation for recipes and ingredients
         =================================================
```

### Comparing `nutrical-0.0.1/README.md` & `nutrical-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.1/data/TW_FDA_nutrition_items.csv` & `nutrical-0.0.2/data/TW_FDA_nutrition_items.csv`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.1/foodie/foodie.py` & `nutrical-0.0.2/nutrical/nutrical.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.1/foodie/utils.py` & `nutrical-0.0.2/nutrical/utils.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.1/nutrical.egg-info/PKG-INFO` & `nutrical-0.0.2/nutrical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutrical
-Version: 0.0.1
+Version: 0.0.2
 Summary: Nutrition calculation for recipes and ingredients
 Home-page: https://github.com/liao961120/nutrical
 Author: Yongfu Liao
 Author-email: liao961120@gmail.com
 License: UNKNOWN
 Description: Nutrition calculation for recipes and ingredients
         =================================================
```

### Comparing `nutrical-0.0.1/setup.py` & `nutrical-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+# Dynamic version
+with open("VERSION") as f:
+    version = f"0.0.{f.read().strip()}"
+
 setuptools.setup(
     name="nutrical", # Replace with your own username
-    version="0.0.1",
+    version=version,
     author="Yongfu Liao",
     author_email="liao961120@gmail.com",
     description="Nutrition calculation for recipes and ingredients",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liao961120/nutrical",
     # package_dir = {'': 'src'},
-    packages=['foodie'],
+    packages=['nutrical'],
     install_requires=[
         'Pint',
     ],
     package_data={
         "": ["../data/TW_FDA_nutrition_items.csv"],
     },
     classifiers=[
```

### Comparing `nutrical-0.0.1/test/test.py` & `nutrical-0.0.2/test/test.py`

 * *Files identical despite different names*

