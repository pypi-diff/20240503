# Comparing `tmp/poly-crop-0.1.tar.gz` & `tmp/poly_crop-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poly-crop-0.1.tar", last modified: Thu May  2 13:51:41 2024, max compression
+gzip compressed data, was "poly_crop-0.2.tar", last modified: Fri May  3 16:21:50 2024, max compression
```

## Comparing `poly-crop-0.1.tar` & `poly_crop-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 13:51:41.525317 poly-crop-0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-02 13:07:22.000000 poly-crop-0.1/LICENSE
--rw-rw-rw-   0        0        0     1237 2024-05-02 13:51:41.524322 poly-crop-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-02 13:31:30.000000 poly-crop-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 13:51:41.521323 poly-crop-0.1/poly_crop.egg-info/
--rw-rw-rw-   0        0        0     1237 2024-05-02 13:51:40.000000 poly-crop-0.1/poly_crop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-02 13:51:41.000000 poly-crop-0.1/poly_crop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 13:51:40.000000 poly-crop-0.1/poly_crop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-02 13:51:41.000000 poly-crop-0.1/poly_crop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 13:51:41.000000 poly-crop-0.1/poly_crop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 13:51:41.526494 poly-crop-0.1/setup.cfg
--rw-rw-rw-   0        0        0      439 2024-05-02 13:49:02.000000 poly-crop-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:21:50.841179 poly_crop-0.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-02 13:07:22.000000 poly_crop-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1270 2024-05-03 16:21:50.839175 poly_crop-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2024-05-03 16:21:19.000000 poly_crop-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 16:21:50.836179 poly_crop-0.2/poly_crop.egg-info/
+-rw-rw-rw-   0        0        0     1270 2024-05-03 16:21:49.000000 poly_crop-0.2/poly_crop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-03 16:21:50.000000 poly_crop-0.2/poly_crop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:21:49.000000 poly_crop-0.2/poly_crop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-03 16:21:50.000000 poly_crop-0.2/poly_crop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:21:50.000000 poly_crop-0.2/poly_crop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 16:21:50.841179 poly_crop-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      442 2024-05-02 14:01:57.000000 poly_crop-0.2/setup.py
```

### Comparing `poly-crop-0.1/LICENSE` & `poly_crop-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poly-crop-0.1/PKG-INFO` & `poly_crop-0.2/poly_crop.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: poly-crop
-Version: 0.1
+Version: 0.2
 Summary: Python library for cropping polygons in images
-Author: Your Name
+Author: Elias Jensen
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Crop
-Crop is a Python library for cropping polygons in images.
+# Poly_Crop
+poly_crop is a Python library for cropping polygons in images.
 
 ## Installation
-You can install Crop via pip:
+You can install poly_crop via pip:
 
 ```python
-pip install crop
+pip install poly_crop
 ```
 ## Usage
 ### Crop Function
 The `crop` function is used to crop a polygonal region from an image.
 
 ```python
-from crop import crop
+from poly_crop import crop
 
 # Example usage
 image_path = "path/to/your/image.jpg"
 image = cv2.imread(image_path)
 vertices = [(100, 100), (175, 50), (300, 100), (175, 150), (170, 100)]
 
 cropped_image = crop(image, vertices, resize=False)
 ```
 ### Preview Function
 The `preview` function is used to draw a preview of a polygonal region on an image.
 
 ```python
-from crop import preview
+from poly_crop import preview
 
 # Example usage
 image_path = "path/to/your/image.jpg"
 image = cv2.imread(image_path)
 vertices = [(100, 100), (175, 50), (300, 100), (175, 150), (170, 100)]
 
 preview_image = preview(image, vertices, colour=(255, 0, 0), width=2)
```

### Comparing `poly-crop-0.1/README.md` & `poly_crop-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# Crop
-Crop is a Python library for cropping polygons in images.
+# Poly_Crop
+poly_crop is a Python library for cropping polygons in images.
 
 ## Installation
-You can install Crop via pip:
+You can install poly_crop via pip:
 
 ```python
-pip install crop
+pip install poly_crop
 ```
 ## Usage
 ### Crop Function
 The `crop` function is used to crop a polygonal region from an image.
 
 ```python
-from crop import crop
+from poly_crop import crop
 
 # Example usage
 image_path = "path/to/your/image.jpg"
 image = cv2.imread(image_path)
 vertices = [(100, 100), (175, 50), (300, 100), (175, 150), (170, 100)]
 
 cropped_image = crop(image, vertices, resize=False)
 ```
 ### Preview Function
 The `preview` function is used to draw a preview of a polygonal region on an image.
 
 ```python
-from crop import preview
+from poly_crop import preview
 
 # Example usage
 image_path = "path/to/your/image.jpg"
 image = cv2.imread(image_path)
 vertices = [(100, 100), (175, 50), (300, 100), (175, 150), (170, 100)]
 
 preview_image = preview(image, vertices, colour=(255, 0, 0), width=2)
```

### Comparing `poly-crop-0.1/poly_crop.egg-info/PKG-INFO` & `poly_crop-0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
-Name: poly-crop
-Version: 0.1
+Name: poly_crop
+Version: 0.2
 Summary: Python library for cropping polygons in images
-Author: Your Name
+Author: Elias Jensen
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Crop
-Crop is a Python library for cropping polygons in images.
+# Poly_Crop
+poly_crop is a Python library for cropping polygons in images.
 
 ## Installation
-You can install Crop via pip:
+You can install poly_crop via pip:
 
 ```python
-pip install crop
+pip install poly_crop
 ```
 ## Usage
 ### Crop Function
 The `crop` function is used to crop a polygonal region from an image.
 
 ```python
-from crop import crop
+from poly_crop import crop
 
 # Example usage
 image_path = "path/to/your/image.jpg"
 image = cv2.imread(image_path)
 vertices = [(100, 100), (175, 50), (300, 100), (175, 150), (170, 100)]
 
 cropped_image = crop(image, vertices, resize=False)
 ```
 ### Preview Function
 The `preview` function is used to draw a preview of a polygonal region on an image.
 
 ```python
-from crop import preview
+from poly_crop import preview
 
 # Example usage
 image_path = "path/to/your/image.jpg"
 image = cv2.imread(image_path)
 vertices = [(100, 100), (175, 50), (300, 100), (175, 150), (170, 100)]
 
 preview_image = preview(image, vertices, colour=(255, 0, 0), width=2)
```

