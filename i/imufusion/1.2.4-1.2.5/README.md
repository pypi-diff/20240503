# Comparing `tmp/imufusion-1.2.4.tar.gz` & `tmp/imufusion-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imufusion-1.2.4.tar", last modified: Fri Mar  1 09:20:07 2024, max compression
+gzip compressed data, was "imufusion-1.2.5.tar", last modified: Fri May  3 10:19:57 2024, max compression
```

## Comparing `imufusion-1.2.4.tar` & `imufusion-1.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 09:20:07.010804 imufusion-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 09:20:07.006804 imufusion-1.2.4/Fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/Fusion.h
--rw-r--r--   0 runner    (1001) docker     (127)    20509 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionAhrs.c
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionAhrs.h
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionAxes.h
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionCalibration.h
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionCompass.c
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionCompass.h
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionConvention.h
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionOffset.c
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-01 09:19:52.000000 imufusion-1.2.4/Fusion/FusionOffset.h
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-01 09:19:52.000000 imufusion-1.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-01 09:19:52.000000 imufusion-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-01 09:20:07.010804 imufusion-1.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 09:20:07.002804 imufusion-1.2.4/Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 09:20:07.006804 imufusion-1.2.4/Python/Python-C-API/
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Ahrs.h
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Axes.h
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Compass.h
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Flags.h
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/InternalStates.h
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Offset.h
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/Settings.h
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-03-01 09:19:52.000000 imufusion-1.2.4/Python/Python-C-API/imufusion.c
--rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-03-01 09:19:52.000000 imufusion-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 09:20:07.006804 imufusion-1.2.4/imufusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-01 09:20:06.000000 imufusion-1.2.4/imufusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-01 09:20:06.000000 imufusion-1.2.4/imufusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 09:20:06.000000 imufusion-1.2.4/imufusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-01 09:20:06.000000 imufusion-1.2.4/imufusion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 09:20:07.010804 imufusion-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-01 09:19:52.000000 imufusion-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:19:57.814989 imufusion-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:19:57.810989 imufusion-1.2.5/Fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/Fusion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionAhrs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionAhrs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionAxes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionCalibration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionCompass.c
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionCompass.h
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionConvention.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionOffset.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-03 10:19:46.000000 imufusion-1.2.5/Fusion/FusionOffset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-03 10:19:46.000000 imufusion-1.2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 10:19:46.000000 imufusion-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 10:19:57.814989 imufusion-1.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:19:57.810989 imufusion-1.2.5/Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:19:57.814989 imufusion-1.2.5/Python/Python-C-API/
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Ahrs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Axes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Compass.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Flags.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/InternalStates.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Offset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-03 10:19:46.000000 imufusion-1.2.5/Python/Python-C-API/imufusion.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-05-03 10:19:46.000000 imufusion-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:19:57.814989 imufusion-1.2.5/imufusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 10:19:57.000000 imufusion-1.2.5/imufusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 10:19:57.000000 imufusion-1.2.5/imufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:19:57.000000 imufusion-1.2.5/imufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 10:19:57.000000 imufusion-1.2.5/imufusion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:19:57.814989 imufusion-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-03 10:19:46.000000 imufusion-1.2.5/setup.py
```

### Comparing `imufusion-1.2.4/Fusion/Fusion.h` & `imufusion-1.2.5/Fusion/Fusion.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionAhrs.c` & `imufusion-1.2.5/Fusion/FusionAhrs.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  */
 
 //------------------------------------------------------------------------------
 // Includes
 
 #include <float.h> // FLT_MAX
 #include "FusionAhrs.h"
-#include <math.h> // atan2f, cosf, powf, sinf
+#include <math.h> // atan2f, cosf, fabsf, powf, sinf
 
 //------------------------------------------------------------------------------
 // Definitions
 
 /**
  * @brief Initial gain used during the initialisation.
  */
@@ -113,15 +113,15 @@
 void FusionAhrsUpdate(FusionAhrs *const ahrs, const FusionVector gyroscope, const FusionVector accelerometer, const FusionVector magnetometer, const float deltaTime) {
 #define Q ahrs->quaternion.element
 
     // Store accelerometer
     ahrs->accelerometer = accelerometer;
 
     // Reinitialise if gyroscope range exceeded
-    if ((fabs(gyroscope.axis.x) > ahrs->settings.gyroscopeRange) || (fabs(gyroscope.axis.y) > ahrs->settings.gyroscopeRange) || (fabs(gyroscope.axis.z) > ahrs->settings.gyroscopeRange)) {
+    if ((fabsf(gyroscope.axis.x) > ahrs->settings.gyroscopeRange) || (fabsf(gyroscope.axis.y) > ahrs->settings.gyroscopeRange) || (fabsf(gyroscope.axis.z) > ahrs->settings.gyroscopeRange)) {
         const FusionQuaternion quaternion = ahrs->quaternion;
         FusionAhrsReset(ahrs);
         ahrs->quaternion = quaternion;
         ahrs->angularRateRecovery = true;
     }
 
     // Ramp down gain during initialisation
```

### Comparing `imufusion-1.2.4/Fusion/FusionAhrs.h` & `imufusion-1.2.5/Fusion/FusionAhrs.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionAxes.h` & `imufusion-1.2.5/Fusion/FusionAxes.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionCalibration.h` & `imufusion-1.2.5/Fusion/FusionCalibration.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionCompass.c` & `imufusion-1.2.5/Fusion/FusionCompass.c`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionCompass.h` & `imufusion-1.2.5/Fusion/FusionCompass.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionConvention.h` & `imufusion-1.2.5/Fusion/FusionConvention.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionMath.h` & `imufusion-1.2.5/Fusion/FusionMath.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Fusion/FusionOffset.c` & `imufusion-1.2.5/Fusion/FusionOffset.c`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
  * gyroscope offset.
  */
 
 //------------------------------------------------------------------------------
 // Includes
 
 #include "FusionOffset.h"
-#include <math.h> // fabs
+#include <math.h> // fabsf
 
 //------------------------------------------------------------------------------
 // Definitions
 
 /**
  * @brief Cutoff frequency in Hz.
  */
@@ -53,15 +53,15 @@
  */
 FusionVector FusionOffsetUpdate(FusionOffset *const offset, FusionVector gyroscope) {
 
     // Subtract offset from gyroscope measurement
     gyroscope = FusionVectorSubtract(gyroscope, offset->gyroscopeOffset);
 
     // Reset timer if gyroscope not stationary
-    if ((fabs(gyroscope.axis.x) > THRESHOLD) || (fabs(gyroscope.axis.y) > THRESHOLD) || (fabs(gyroscope.axis.z) > THRESHOLD)) {
+    if ((fabsf(gyroscope.axis.x) > THRESHOLD) || (fabsf(gyroscope.axis.y) > THRESHOLD) || (fabsf(gyroscope.axis.z) > THRESHOLD)) {
         offset->timer = 0;
         return gyroscope;
     }
 
     // Increment timer while gyroscope stationary
     if (offset->timer < offset->timeout) {
         offset->timer++;
```

### Comparing `imufusion-1.2.4/Fusion/FusionOffset.h` & `imufusion-1.2.5/Fusion/FusionOffset.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/LICENSE.md` & `imufusion-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Ahrs.h` & `imufusion-1.2.5/Python/Python-C-API/Ahrs.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Axes.h` & `imufusion-1.2.5/Python/Python-C-API/Axes.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Compass.h` & `imufusion-1.2.5/Python/Python-C-API/Compass.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Flags.h` & `imufusion-1.2.5/Python/Python-C-API/Flags.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Helpers.h` & `imufusion-1.2.5/Python/Python-C-API/Helpers.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/InternalStates.h` & `imufusion-1.2.5/Python/Python-C-API/InternalStates.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Offset.h` & `imufusion-1.2.5/Python/Python-C-API/Offset.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Quaternion.h` & `imufusion-1.2.5/Python/Python-C-API/Quaternion.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/Settings.h` & `imufusion-1.2.5/Python/Python-C-API/Settings.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/Python/Python-C-API/imufusion.c` & `imufusion-1.2.5/Python/Python-C-API/imufusion.c`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/README.md` & `imufusion-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/imufusion.egg-info/SOURCES.txt` & `imufusion-1.2.5/imufusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imufusion-1.2.4/setup.py` & `imufusion-1.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,21 +19,19 @@
                                       "Fusion/FusionCompass.c",
                                       "Fusion/FusionOffset.c"],
                         include_dirs=[numpy.get_include()],
                         define_macros=[("FUSION_USE_NORMAL_SQRT", None)],
                         libraries=(["m"] if "linux" in sys.platform else []))  # link math library for Linux
 
 setup(name="imufusion",
-      version="1.2.4",
+      version="1.2.5",
       description="Fusion Python package",
       long_description="See [github](" + github_url + ") for documentation and examples.",
       long_description_content_type='text/markdown',
       url=github_url,
       author="x-io Technologies Limited",
       author_email="info@x-io.co.uk",
       license="MIT",
-      classifiers=["Programming Language :: Python :: 3.8",
-                   "Programming Language :: Python :: 3.9",
-                   "Programming Language :: Python :: 3.10",
+      classifiers=["Programming Language :: Python :: 3.10",
                    "Programming Language :: Python :: 3.11",
                    "Programming Language :: Python :: 3.12"],  # versions shown by pyversions badge in README
       ext_modules=[ext_modules])
```

