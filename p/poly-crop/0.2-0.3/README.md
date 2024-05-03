# Comparing `tmp/poly_crop-0.2.tar.gz` & `tmp/poly_crop-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poly_crop-0.2.tar", last modified: Fri May  3 16:21:50 2024, max compression
+gzip compressed data, was "poly_crop-0.3.tar", last modified: Fri May  3 16:52:48 2024, max compression
```

## Comparing `poly_crop-0.2.tar` & `poly_crop-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 16:21:50.841179 poly_crop-0.2/
--rw-rw-rw-   0        0        0     1088 2024-05-02 13:07:22.000000 poly_crop-0.2/LICENSE
--rw-rw-rw-   0        0        0     1270 2024-05-03 16:21:50.839175 poly_crop-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1034 2024-05-03 16:21:19.000000 poly_crop-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 16:21:50.836179 poly_crop-0.2/poly_crop.egg-info/
--rw-rw-rw-   0        0        0     1270 2024-05-03 16:21:49.000000 poly_crop-0.2/poly_crop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-03 16:21:50.000000 poly_crop-0.2/poly_crop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 16:21:49.000000 poly_crop-0.2/poly_crop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-03 16:21:50.000000 poly_crop-0.2/poly_crop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 16:21:50.000000 poly_crop-0.2/poly_crop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 16:21:50.841179 poly_crop-0.2/setup.cfg
--rw-rw-rw-   0        0        0      442 2024-05-02 14:01:57.000000 poly_crop-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:52:48.238998 poly_crop-0.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-02 13:07:22.000000 poly_crop-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1270 2024-05-03 16:52:48.237993 poly_crop-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2024-05-03 16:21:19.000000 poly_crop-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 16:52:48.233998 poly_crop-0.3/poly_crop.egg-info/
+-rw-rw-rw-   0        0        0     1270 2024-05-03 16:52:47.000000 poly_crop-0.3/poly_crop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-03 16:52:47.000000 poly_crop-0.3/poly_crop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:52:47.000000 poly_crop-0.3/poly_crop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-03 16:52:47.000000 poly_crop-0.3/poly_crop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:52:47.000000 poly_crop-0.3/poly_crop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 16:52:48.239993 poly_crop-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      442 2024-05-03 16:51:30.000000 poly_crop-0.3/setup.py
```

### Comparing `poly_crop-0.2/LICENSE` & `poly_crop-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poly_crop-0.2/PKG-INFO` & `poly_crop-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poly_crop
-Version: 0.2
+Version: 0.3
 Summary: Python library for cropping polygons in images
 Author: Elias Jensen
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `poly_crop-0.2/README.md` & `poly_crop-0.3/README.md`

 * *Files identical despite different names*

### Comparing `poly_crop-0.2/poly_crop.egg-info/PKG-INFO` & `poly_crop-0.3/poly_crop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poly-crop
-Version: 0.2
+Version: 0.3
 Summary: Python library for cropping polygons in images
 Author: Elias Jensen
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

