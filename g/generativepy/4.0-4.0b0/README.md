# Comparing `tmp/generativepy-4.0.tar.gz` & `tmp/generativepy-4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generativepy-4.0.tar", last modified: Fri May 12 21:42:09 2023, max compression
+gzip compressed data, was "generativepy-4.0b0.tar", last modified: Fri May 12 21:32:17 2023, max compression
```

## Comparing `generativepy-4.0.tar` & `generativepy-4.0b0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:42:09.752628 generativepy-4.0/
--rw-r--r--   0 martin    (1000) martin    (1000)     1071 2018-11-08 18:18:07.000000 generativepy-4.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     3317 2023-05-12 21:42:09.753628 generativepy-4.0/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     2890 2023-05-12 21:40:18.000000 generativepy-4.0/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:42:09.750628 generativepy-4.0/generativepy/
--rw-rw-r--   0 martin    (1000) martin    (1000)       22 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      813 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/analytics.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4314 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/bitmap.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)    15507 2023-01-22 21:34:18.000000 generativepy-4.0/generativepy/color.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5184 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/drawing.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3072 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/drawing3d.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4795 2022-08-29 20:05:50.000000 generativepy-4.0/generativepy/formulas.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    38910 2023-05-12 21:16:17.000000 generativepy-4.0/generativepy/geometry.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4087 2022-12-29 16:41:56.000000 generativepy-4.0/generativepy/geometry3d.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      746 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/gif.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)    17510 2023-04-27 17:12:01.000000 generativepy-4.0/generativepy/graph.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7759 2023-03-04 20:01:53.000000 generativepy-4.0/generativepy/math.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5847 2022-12-02 13:47:14.000000 generativepy-4.0/generativepy/movie.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5844 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/nparray.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1969 2023-03-04 18:09:14.000000 generativepy-4.0/generativepy/shape2d.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5015 2023-02-11 11:56:27.000000 generativepy-4.0/generativepy/table.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)     9272 2022-12-11 14:17:23.000000 generativepy-4.0/generativepy/tween.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1134 2021-12-19 11:40:04.000000 generativepy-4.0/generativepy/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:42:09.751628 generativepy-4.0/generativepy.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3317 2023-05-12 21:42:09.000000 generativepy-4.0/generativepy.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      846 2023-05-12 21:42:09.000000 generativepy-4.0/generativepy.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-12 21:42:09.000000 generativepy-4.0/generativepy.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       30 2023-05-12 21:42:09.000000 generativepy-4.0/generativepy.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-12 21:42:09.000000 generativepy-4.0/generativepy.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-05-12 21:42:09.753628 generativepy-4.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      744 2023-05-12 21:41:06.000000 generativepy-4.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:42:09.752628 generativepy-4.0/test/
--rw-rw-r--   0 martin    (1000) martin    (1000)    12818 2022-05-31 13:29:36.000000 generativepy-4.0/test/test_color.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      856 2022-08-29 20:05:08.000000 generativepy-4.0/test/test_formulas.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3491 2023-03-04 17:52:42.000000 generativepy-4.0/test/test_matrix.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2391 2023-03-04 20:01:14.000000 generativepy-4.0/test/test_points.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1541 2022-06-04 16:35:21.000000 generativepy-4.0/test/test_regular_polygon.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      992 2021-11-17 18:58:19.000000 generativepy-4.0/test/test_text.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2873 2022-01-09 14:53:02.000000 generativepy-4.0/test/test_transform.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    23498 2023-02-16 21:01:33.000000 generativepy-4.0/test/test_tween.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2208 2021-11-17 18:58:19.000000 generativepy-4.0/test/test_utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4264 2023-03-04 17:58:07.000000 generativepy-4.0/test/test_vector.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.658942 generativepy-4.0b0/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1071 2018-11-08 18:18:07.000000 generativepy-4.0b0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3363 2023-05-12 21:32:17.658942 generativepy-4.0b0/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     2934 2023-05-12 21:31:54.000000 generativepy-4.0b0/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.656942 generativepy-4.0b0/generativepy/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       22 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      813 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/analytics.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4314 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/bitmap.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)    15507 2023-01-22 21:34:18.000000 generativepy-4.0b0/generativepy/color.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5184 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/drawing.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3072 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/drawing3d.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4795 2022-08-29 20:05:50.000000 generativepy-4.0b0/generativepy/formulas.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    38910 2023-05-12 21:16:17.000000 generativepy-4.0b0/generativepy/geometry.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4087 2022-12-29 16:41:56.000000 generativepy-4.0b0/generativepy/geometry3d.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      746 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/gif.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)    17510 2023-04-27 17:12:01.000000 generativepy-4.0b0/generativepy/graph.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7759 2023-03-04 20:01:53.000000 generativepy-4.0b0/generativepy/math.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5847 2022-12-02 13:47:14.000000 generativepy-4.0b0/generativepy/movie.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5844 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/nparray.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1969 2023-03-04 18:09:14.000000 generativepy-4.0b0/generativepy/shape2d.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5015 2023-02-11 11:56:27.000000 generativepy-4.0b0/generativepy/table.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)     9272 2022-12-11 14:17:23.000000 generativepy-4.0b0/generativepy/tween.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1134 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.656942 generativepy-4.0b0/generativepy.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3363 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      846 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       30 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-05-12 21:32:17.659942 generativepy-4.0b0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      749 2023-05-12 21:22:36.000000 generativepy-4.0b0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.658942 generativepy-4.0b0/test/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12818 2022-05-31 13:29:36.000000 generativepy-4.0b0/test/test_color.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      856 2022-08-29 20:05:08.000000 generativepy-4.0b0/test/test_formulas.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3491 2023-03-04 17:52:42.000000 generativepy-4.0b0/test/test_matrix.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2391 2023-03-04 20:01:14.000000 generativepy-4.0b0/test/test_points.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1541 2022-06-04 16:35:21.000000 generativepy-4.0b0/test/test_regular_polygon.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      992 2021-11-17 18:58:19.000000 generativepy-4.0b0/test/test_text.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2873 2022-01-09 14:53:02.000000 generativepy-4.0b0/test/test_transform.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    23498 2023-02-16 21:01:33.000000 generativepy-4.0b0/test/test_tween.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2208 2021-11-17 18:58:19.000000 generativepy-4.0b0/test/test_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4264 2023-03-04 17:58:07.000000 generativepy-4.0b0/test/test_vector.py
```

### Comparing `generativepy-4.0/LICENSE` & `generativepy-4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/PKG-INFO` & `generativepy-4.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generativepy
-Version: 4.0
+Version: 4.0b0
 Summary: Generative art library
 Home-page: https://github.com/martinmcbride/generativepy
 Author: Martin McBride
 Author-email: mcbride.martin@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # generativepy
 
 Generative art and graphing library for creating images and animations.
 
-## Version 4.0 notes
+## Version 4.0 beta notes
 
-3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
+This is a beta version, mainly because 3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
 
 * Allow images to eb preloaded for `Image` objects, to avoid frequent file reloads when creating animations.
 * Add shapes2d module representing abstract shapes.
 * Add math module with 2D vector and matrix classes.
 * Add `ORANGE`, `CYAN` to `ArtisticColorScheme`.
 * Add table module for table layouts.
 * MINOR BREAKING CHANGE - Extra warning if some scenes don't have audio (behaviour change if not all audio present).
```

### Comparing `generativepy-4.0/README.md` & `generativepy-4.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # generativepy
 
 Generative art and graphing library for creating images and animations.
 
-## Version 4.0 notes
+## Version 4.0 beta notes
 
-3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
+This is a beta version, mainly because 3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
 
 * Allow images to eb preloaded for `Image` objects, to avoid frequent file reloads when creating animations.
 * Add shapes2d module representing abstract shapes.
 * Add math module with 2D vector and matrix classes.
 * Add `ORANGE`, `CYAN` to `ArtisticColorScheme`.
 * Add table module for table layouts.
 * MINOR BREAKING CHANGE - Extra warning if some scenes don't have audio (behaviour change if not all audio present).
```

### Comparing `generativepy-4.0/generativepy/analytics.py` & `generativepy-4.0b0/generativepy/analytics.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/bitmap.py` & `generativepy-4.0b0/generativepy/bitmap.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/color.py` & `generativepy-4.0b0/generativepy/color.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/drawing.py` & `generativepy-4.0b0/generativepy/drawing.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/drawing3d.py` & `generativepy-4.0b0/generativepy/drawing3d.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/formulas.py` & `generativepy-4.0b0/generativepy/formulas.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/geometry.py` & `generativepy-4.0b0/generativepy/geometry.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/geometry3d.py` & `generativepy-4.0b0/generativepy/geometry3d.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/gif.py` & `generativepy-4.0b0/generativepy/gif.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/graph.py` & `generativepy-4.0b0/generativepy/graph.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/math.py` & `generativepy-4.0b0/generativepy/math.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/movie.py` & `generativepy-4.0b0/generativepy/movie.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/nparray.py` & `generativepy-4.0b0/generativepy/nparray.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/shape2d.py` & `generativepy-4.0b0/generativepy/shape2d.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/table.py` & `generativepy-4.0b0/generativepy/table.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/tween.py` & `generativepy-4.0b0/generativepy/tween.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy/utils.py` & `generativepy-4.0b0/generativepy/utils.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/generativepy.egg-info/PKG-INFO` & `generativepy-4.0b0/generativepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generativepy
-Version: 4.0
+Version: 4.0b0
 Summary: Generative art library
 Home-page: https://github.com/martinmcbride/generativepy
 Author: Martin McBride
 Author-email: mcbride.martin@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # generativepy
 
 Generative art and graphing library for creating images and animations.
 
-## Version 4.0 notes
+## Version 4.0 beta notes
 
-3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
+This is a beta version, mainly because 3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
 
 * Allow images to eb preloaded for `Image` objects, to avoid frequent file reloads when creating animations.
 * Add shapes2d module representing abstract shapes.
 * Add math module with 2D vector and matrix classes.
 * Add `ORANGE`, `CYAN` to `ArtisticColorScheme`.
 * Add table module for table layouts.
 * MINOR BREAKING CHANGE - Extra warning if some scenes don't have audio (behaviour change if not all audio present).
```

### Comparing `generativepy-4.0/generativepy.egg-info/SOURCES.txt` & `generativepy-4.0b0/generativepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/setup.py` & `generativepy-4.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
  
 setup(name='generativepy',
-      version='4.0',
+      version='4.0 beta',
       url='https://github.com/martinmcbride/generativepy',
       license='MIT',
       author='Martin McBride',
       author_email='mcbride.martin@gmail.com',
       description='Generative art library',
       long_description=long_description,
       long_description_content_type="text/markdown",
```

### Comparing `generativepy-4.0/test/test_color.py` & `generativepy-4.0b0/test/test_color.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_formulas.py` & `generativepy-4.0b0/test/test_formulas.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_matrix.py` & `generativepy-4.0b0/test/test_matrix.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_points.py` & `generativepy-4.0b0/test/test_points.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_regular_polygon.py` & `generativepy-4.0b0/test/test_regular_polygon.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_text.py` & `generativepy-4.0b0/test/test_text.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_transform.py` & `generativepy-4.0b0/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_tween.py` & `generativepy-4.0b0/test/test_tween.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_utils.py` & `generativepy-4.0b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `generativepy-4.0/test/test_vector.py` & `generativepy-4.0b0/test/test_vector.py`

 * *Files identical despite different names*

