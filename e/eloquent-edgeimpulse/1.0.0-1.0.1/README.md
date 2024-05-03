# Comparing `tmp/eloquent_edgeimpulse-1.0.0.tar.gz` & `tmp/eloquent_edgeimpulse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eloquent_edgeimpulse-1.0.0.tar", last modified: Fri Mar  1 10:45:19 2024, max compression
+gzip compressed data, was "eloquent_edgeimpulse-1.0.1.tar", last modified: Fri May  3 16:15:03 2024, max compression
```

## Comparing `eloquent_edgeimpulse-1.0.0.tar` & `eloquent_edgeimpulse-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2024-03-01 10:45:19.915949 eloquent_edgeimpulse-1.0.0/
--rw-r--r--   0 simone     (501) staff       (20)     1071 2024-03-01 10:35:32.000000 eloquent_edgeimpulse-1.0.0/LICENSE
--rw-r--r--   0 simone     (501) staff       (20)      321 2024-03-01 10:45:19.915594 eloquent_edgeimpulse-1.0.0/PKG-INFO
--rw-r--r--   0 simone     (501) staff       (20)      943 2024-03-01 10:35:13.000000 eloquent_edgeimpulse-1.0.0/README.md
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2024-03-01 10:45:19.912690 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/
--rw-r--r--   0 simone     (501) staff       (20)       43 2024-03-01 10:15:55.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/__init__.py
--rw-r--r--   0 simone     (501) staff       (20)     2842 2024-03-01 10:33:22.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/fomo.py
--rw-r--r--   0 simone     (501) staff       (20)     5130 2024-03-01 10:10:55.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/image.py
--rw-r--r--   0 simone     (501) staff       (20)     3494 2024-03-01 10:10:53.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/runner.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2024-03-01 10:45:19.915068 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse.egg-info/
--rw-r--r--   0 simone     (501) staff       (20)      321 2024-03-01 10:45:19.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse.egg-info/PKG-INFO
--rw-r--r--   0 simone     (501) staff       (20)      368 2024-03-01 10:45:19.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse.egg-info/SOURCES.txt
--rw-r--r--   0 simone     (501) staff       (20)        1 2024-03-01 10:45:19.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse.egg-info/dependency_links.txt
--rw-r--r--   0 simone     (501) staff       (20)        6 2024-03-01 10:45:19.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse.egg-info/requires.txt
--rw-r--r--   0 simone     (501) staff       (20)       21 2024-03-01 10:45:19.000000 eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse.egg-info/top_level.txt
--rw-r--r--   0 simone     (501) staff       (20)       38 2024-03-01 10:45:19.916131 eloquent_edgeimpulse-1.0.0/setup.cfg
--rw-r--r--   0 simone     (501) staff       (20)      449 2024-03-01 10:45:15.000000 eloquent_edgeimpulse-1.0.0/setup.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2024-05-03 16:15:03.189904 eloquent_edgeimpulse-1.0.1/
+-rw-r--r--   0 simone     (501) staff       (20)     1071 2024-03-01 10:35:32.000000 eloquent_edgeimpulse-1.0.1/LICENSE
+-rw-r--r--   0 simone     (501) staff       (20)      321 2024-05-03 16:15:03.189231 eloquent_edgeimpulse-1.0.1/PKG-INFO
+-rw-r--r--   0 simone     (501) staff       (20)     1017 2024-03-05 11:52:02.000000 eloquent_edgeimpulse-1.0.1/README.md
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2024-05-03 16:15:03.185586 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/
+-rw-r--r--   0 simone     (501) staff       (20)       43 2024-03-01 10:15:55.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/__init__.py
+-rw-r--r--   0 simone     (501) staff       (20)     2848 2024-05-03 16:10:43.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/fomo.py
+-rw-r--r--   0 simone     (501) staff       (20)     5130 2024-03-01 10:10:55.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/image.py
+-rw-r--r--   0 simone     (501) staff       (20)     3494 2024-03-01 10:10:53.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/runner.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2024-05-03 16:15:03.188494 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse.egg-info/
+-rw-r--r--   0 simone     (501) staff       (20)      321 2024-05-03 16:15:03.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse.egg-info/PKG-INFO
+-rw-r--r--   0 simone     (501) staff       (20)      368 2024-05-03 16:15:03.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse.egg-info/SOURCES.txt
+-rw-r--r--   0 simone     (501) staff       (20)        1 2024-05-03 16:15:03.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse.egg-info/dependency_links.txt
+-rw-r--r--   0 simone     (501) staff       (20)        6 2024-05-03 16:15:03.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse.egg-info/requires.txt
+-rw-r--r--   0 simone     (501) staff       (20)       21 2024-05-03 16:15:03.000000 eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse.egg-info/top_level.txt
+-rw-r--r--   0 simone     (501) staff       (20)       38 2024-05-03 16:15:03.190141 eloquent_edgeimpulse-1.0.1/setup.cfg
+-rw-r--r--   0 simone     (501) staff       (20)      449 2024-05-03 16:15:02.000000 eloquent_edgeimpulse-1.0.1/setup.py
```

### Comparing `eloquent_edgeimpulse-1.0.0/LICENSE` & `eloquent_edgeimpulse-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eloquent_edgeimpulse-1.0.0/README.md` & `eloquent_edgeimpulse-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 ## Setup
 
 To run EI models from Python, you have to deploy a `.eim`
 file in the Deployment section by selecting either `Linux` or `macOS`
 and make it executable.
 
+Then, install from pip.
+
+```bash
+pip install -U eloquent_edgeimpulse
+```
+
 
 ## FOMO object detection
 
 To run FOMO, you will need a sample image and a way to load it
 (either `PIL` or `scikit-image` or `opencv`)
```

### Comparing `eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/fomo.py` & `eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/fomo.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         assert height == self.height, f'image height *must* be {self.height}'
 
         # convert from float [0, 1] to int [0, 255]
         if image.min() >= 0 and image.max() <= 1:
             image = (image * 255).astype(int)
 
         # convert 2D image to 3D image (RGB)
-        if len(image) == 2 or image.shape[2] == 1:
+        if len(image.shape) == 2 or image.shape[2] == 1:
             gray = image.reshape(image.shape[:2])
             image = np.dstack((gray, gray, gray))
 
         # convert 3D uint8 to 1D uint24
         def to_uint24(pixel):
             return (pixel[0] << 16) | (pixel[1] << 8) | pixel[2]
```

### Comparing `eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/image.py` & `eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/image.py`

 * *Files identical despite different names*

### Comparing `eloquent_edgeimpulse-1.0.0/eloquent_edgeimpulse/runner.py` & `eloquent_edgeimpulse-1.0.1/eloquent_edgeimpulse/runner.py`

 * *Files identical despite different names*

