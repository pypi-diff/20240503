# Comparing `tmp/smsfusion-0.2.0-py3-none-any.whl.zip` & `tmp/smsfusion-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26338 bytes, number of entries: 17
+Zip file size: 26740 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 smsfusion/__about__.py
 -rw-r--r--  2.0 unx      241 b- defN 20-Feb-02 00:00 smsfusion/__init__.py
 -rw-r--r--  2.0 unx     9220 b- defN 20-Feb-02 00:00 smsfusion/_ahrs.py
 -rw-r--r--  2.0 unx    33165 b- defN 20-Feb-02 00:00 smsfusion/_ins.py
 -rw-r--r--  2.0 unx     9280 b- defN 20-Feb-02 00:00 smsfusion/_transforms.py
 -rw-r--r--  2.0 unx     2226 b- defN 20-Feb-02 00:00 smsfusion/_vectorops.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 smsfusion/benchmark/__init__.py
 -rw-r--r--  2.0 unx    24303 b- defN 20-Feb-02 00:00 smsfusion/benchmark/_benchmark.py
--rw-r--r--  2.0 unx       59 b- defN 20-Feb-02 00:00 smsfusion/calibrate/__init__.py
--rw-r--r--  2.0 unx     1462 b- defN 20-Feb-02 00:00 smsfusion/calibrate/_calibrate.py
+-rw-r--r--  2.0 unx       83 b- defN 20-Feb-02 00:00 smsfusion/calibrate/__init__.py
+-rw-r--r--  2.0 unx     2772 b- defN 20-Feb-02 00:00 smsfusion/calibrate/_calibrate.py
 -rw-r--r--  2.0 unx      235 b- defN 20-Feb-02 00:00 smsfusion/noise/__init__.py
 -rw-r--r--  2.0 unx     2369 b- defN 20-Feb-02 00:00 smsfusion/noise/_allan.py
 -rw-r--r--  2.0 unx    15163 b- defN 20-Feb-02 00:00 smsfusion/noise/_noise.py
-?rw-r--r--  2.0 unx      705 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1064 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1377 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/RECORD
-17 files, 101467 bytes uncompressed, 24086 bytes compressed:  76.3%
+?rw-r--r--  2.0 unx      705 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1064 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1377 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/RECORD
+17 files, 102801 bytes uncompressed, 24488 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: smsfusion/noise/_allan.py
 Comment: 
 
 Filename: smsfusion/noise/_noise.py
 Comment: 
 
-Filename: smsfusion-0.2.0.dist-info/METADATA
+Filename: smsfusion-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: smsfusion-0.2.0.dist-info/WHEEL
+Filename: smsfusion-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: smsfusion-0.2.0.dist-info/licenses/LICENSE
+Filename: smsfusion-0.3.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: smsfusion-0.2.0.dist-info/RECORD
+Filename: smsfusion-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smsfusion/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0"
+__version__ = "0.3.0"
```

## smsfusion/calibrate/__init__.py

```diff
@@ -1,3 +1,3 @@
-from ._calibrate import calibrate
+from ._calibrate import calibrate, decompose
 
-__all__ = ["calibrate"]
+__all__ = ["calibrate", "decompose"]
```

## smsfusion/calibrate/_calibrate.py

```diff
@@ -1,42 +1,50 @@
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 
 
 def calibrate(
-    xyz_ref: ArrayLike, xyz: ArrayLike
+    xyz_ref: ArrayLike, xyz: ArrayLike, bias_alt: bool = False
 ) -> tuple[NDArray[np.float64], NDArray[np.float64]]:
     """
     Calculate the calibration values for 3-axis sensors.
 
     Parameters
     ----------
     xyz_ref : array-like, shape (N, 3)
         Reference values for the 3-axis sensors.
     xyz : array-like, shape (N, 3)
         Measured values from the 3-axis sensors.
-
+    bias_alt : bool, default False
+        If set to ``True``, the bias definition of the alternative calibration model
+        is returned. See Notes.
 
     Notes
     -----
     The calibration model is defined as::
 
-        xyz_ref = W_mat @ xyz + V_vec
+        xyz_ref = W @ xyz + bias
+
+    The alternative calibration model where biases are added first is defined as::
+
+        xyz_ref = W @ (xyz + bias)
+
+    The alternative model is enabled by setting ``bias_alt=True``.
 
     In total, 12 calibration parameters are needed. Accordingly, at least 4
     measurements (of 3 data points) are required to calibrate.
 
-
     Returns
     -------
     W : numpy.ndarray, shape (3, 3)
         Calibration matrix for the 3-axis sensors.
     bias : numpy.ndarray, shape (3,)
         Bias values for the 3-axis sensors.
     """
+
     xyz_ref = np.asarray_chkfinite(xyz_ref)
     xyz = np.asarray_chkfinite(xyz)
 
     if xyz_ref.shape != xyz.shape:
         raise ValueError("xyz_ref and xyz must have the same shape.")
     elif xyz_ref.shape[-1] != 3:
         raise ValueError("xyz_ref and xyz must have shape (N, 3).")
@@ -44,8 +52,48 @@
         raise ValueError("Too few measurements. Reqires at least 4 measurement points.")
 
     A_mat = np.column_stack((xyz, np.ones(len(xyz_ref))))
     x, *_ = np.linalg.lstsq(A_mat, xyz_ref, rcond=None)
 
     W = x[:3, :].T
     bias = x[3, :]
+
+    if bias_alt:
+        bias = np.linalg.inv(W) @ bias
     return W, bias
+
+
+def decompose(
+    W: ArrayLike,
+) -> tuple[NDArray[np.float64], NDArray[np.float64]]:
+    """
+    Polar decompose the calibration matrix into pure rotation and scaling.
+
+    The polar decomposition is defined as::
+
+        W = R @ S
+
+    where ``R`` is pure rotation and ``S`` is scaling.
+
+    Parameters
+    ----------
+    W : array-like, shape (3, 3)
+        Calibration matrix.
+
+    Returns
+    -------
+    R : numpy.ndarray, shape (3, 3)
+        Pure rotation associated with the calibration matrix.
+    S : numpy.ndarray, shape (3, 3)
+        Scaling associated with the calibration matrix.
+    """
+
+    W = np.asarray_chkfinite(W)
+
+    if W.shape != (3, 3):
+        raise ValueError("Invalid shape. W must have shape (3, 3).")
+
+    # Copied from scipy.linalg.polar
+    w, s, vh = np.linalg.svd(W, full_matrices=False)
+    R = w.dot(vh)
+    S = (vh.T.conj() * s).dot(vh)
+    return R, S
```

## Comparing `smsfusion-0.2.0.dist-info/METADATA` & `smsfusion-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smsfusion
-Version: 0.2.0
+Version: 0.3.0
 Summary: Sensor fusion algorithms and utilities for SMS Motion
 Project-URL: Homepage, https://github.com/4Subsea/smsfusion-python
 Project-URL: Bug Tracker, https://github.com/4Subsea/smsfusion-python/issues
 Author-email: 4Subsea <python@4subsea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `smsfusion-0.2.0.dist-info/licenses/LICENSE` & `smsfusion-0.3.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `smsfusion-0.2.0.dist-info/RECORD` & `smsfusion-0.3.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-smsfusion/__about__.py,sha256=Zn1KFblwuFHiDRdRAiRnDBRkbPttWh44jKa5zG2ov0E,22
+smsfusion/__about__.py,sha256=VrXpHDu3erkzwl_WXrqINBm9xWkcyUy53IQOj042dOs,22
 smsfusion/__init__.py,sha256=KuSQtN5M1mBXyaN3g5pFCZ-qNEz0cM88AJIC_MU9-I4,241
 smsfusion/_ahrs.py,sha256=ByD2KGv0HKODfBpBWeeAj6W0dTmkfQkIk4CZm1zD9g0,9220
 smsfusion/_ins.py,sha256=mccnRPXGTnIF3qGrGih37SbW7mD8AlVSLCst3bdH-kw,33165
 smsfusion/_transforms.py,sha256=S3vH3b7_tuohQLMStK6cLrffGm5mXTFj1TFvsoRtMJo,9280
 smsfusion/_vectorops.py,sha256=F6xDYgVMxU9Fo7xFQvKy7UnaBohpDBuFBHzUIjnmz-k,2226
 smsfusion/benchmark/__init__.py,sha256=m1daVGbSVG1MwgwQM28YJi1Sj1c0CdfPsxIEhPEOWoA,489
 smsfusion/benchmark/_benchmark.py,sha256=5j8Rr-mK5jxJDvNE3oBv5q-dhojVBGqQ8gUDt9H-tqc,24303
-smsfusion/calibrate/__init__.py,sha256=IcGWmSiklWxXoilbFyIwoohFjoDpU053wDLECYbk608,59
-smsfusion/calibrate/_calibrate.py,sha256=OFltx4jV8qbJkUw-N_KC1TOZt-FtGeWcXsq0w1n2wBg,1462
+smsfusion/calibrate/__init__.py,sha256=qZ37Ct8DLaxnF-xoagAixCzXD8VSNHe40Uv5jG7wJkk,83
+smsfusion/calibrate/_calibrate.py,sha256=pmD9TJQ8UYuBSm5sXfsF6FfHpjMV45gUYhd9XwwUnxM,2772
 smsfusion/noise/__init__.py,sha256=C5AIH5THPxkb2xmyoTo2eVBCuSFChdNdUGF639nBUus,235
 smsfusion/noise/_allan.py,sha256=JonvSQTviEPQfDEpZg9OWYEOl3sYzG5uB-afqrMV39s,2369
 smsfusion/noise/_noise.py,sha256=njKiHKAmD25FCyX0uBY1oQdTIeIWNPrk3SwPtY5qfFY,15163
-smsfusion-0.2.0.dist-info/METADATA,sha256=wN73YCryDi1re7-Z1yzXqJiY_QRVi1X69tT7zwXW4Mc,705
-smsfusion-0.2.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-smsfusion-0.2.0.dist-info/licenses/LICENSE,sha256=oEQkXxrh0POZZPEv5oYwkmLuh-USLG0uH2JiaThmjA0,1064
-smsfusion-0.2.0.dist-info/RECORD,,
+smsfusion-0.3.0.dist-info/METADATA,sha256=sR_hx6Km0TvPOV0aiCV56lMo99FSli33urGWwLZYjaQ,705
+smsfusion-0.3.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+smsfusion-0.3.0.dist-info/licenses/LICENSE,sha256=oEQkXxrh0POZZPEv5oYwkmLuh-USLG0uH2JiaThmjA0,1064
+smsfusion-0.3.0.dist-info/RECORD,,
```

