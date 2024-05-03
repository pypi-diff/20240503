# Comparing `tmp/spotflow_device-2.0.1-cp37-abi3-win_amd64.whl.zip` & `tmp/spotflow_device-2.0.2-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3365920 bytes, number of entries: 7
--rw-r--r--  4.6 unx      918 b- defN 24-Apr-30 07:28 spotflow_device-2.0.1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-30 07:28 spotflow_device-2.0.1.dist-info/WHEEL
--rw-r--r--  4.6 unx      143 b- defN 24-Apr-30 07:28 spotflow_device/__init__.py
--rw-r--r--  4.6 unx     2695 b- defN 24-Apr-30 07:28 spotflow_device/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-Apr-30 07:28 spotflow_device/py.typed
--rwxr-xr-x  4.6 unx  8174592 b- defN 24-Apr-30 07:28 spotflow_device/spotflow_device.pyd
--rw-r--r--  4.6 unx      570 b- defN 24-Apr-30 07:28 spotflow_device-2.0.1.dist-info/RECORD
-7 files, 8179012 bytes uncompressed, 3364908 bytes compressed:  58.9%
+Zip file size: 3360469 bytes, number of entries: 7
+-rw-r--r--  4.6 unx      918 b- defN 24-May-03 15:31 spotflow_device-2.0.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-03 15:31 spotflow_device-2.0.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx      143 b- defN 24-May-03 15:31 spotflow_device/__init__.py
+-rw-r--r--  4.6 unx     2695 b- defN 24-May-03 15:31 spotflow_device/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-03 15:31 spotflow_device/py.typed
+-rwxr-xr-x  4.6 unx  8112640 b- defN 24-May-03 15:31 spotflow_device/spotflow_device.pyd
+-rw-r--r--  4.6 unx      570 b- defN 24-May-03 15:31 spotflow_device-2.0.2.dist-info/RECORD
+7 files, 8117060 bytes uncompressed, 3359457 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: spotflow_device-2.0.1.dist-info/METADATA
+Filename: spotflow_device-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: spotflow_device-2.0.1.dist-info/WHEEL
+Filename: spotflow_device-2.0.2.dist-info/WHEEL
 Comment: 
 
 Filename: spotflow_device/__init__.py
 Comment: 
 
 Filename: spotflow_device/__init__.pyi
 Comment: 
 
 Filename: spotflow_device/py.typed
 Comment: 
 
 Filename: spotflow_device/spotflow_device.pyd
 Comment: 
 
-Filename: spotflow_device-2.0.1.dist-info/RECORD
+Filename: spotflow_device-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `spotflow_device-2.0.1.dist-info/METADATA` & `spotflow_device-2.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spotflow_device
-Version: 2.0.1
+Version: 2.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Device SDK for Spotflow IoT Platform
 Keywords: spotflow,iot,device,sdk
 Author-email: Spotflow <support@spotflow.io>
 Requires-Python: >=3.7
```

## Comparing `spotflow_device-2.0.1.dist-info/RECORD` & `spotflow_device-2.0.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-spotflow_device-2.0.1.dist-info/METADATA,sha256=QiLeyzkZnUhXelVQx3ekxP5c7TKtLA29CISQVYcVnGw,918
-spotflow_device-2.0.1.dist-info/WHEEL,sha256=2KdwICnFEHl2ghwQAXqeXd9gNxeAiTvogEqUIMDbYbo,94
+spotflow_device-2.0.2.dist-info/METADATA,sha256=aRkax5b-rdtRjm4Te_1CHjXa2o6cmZqyX-O6Mr0xWSc,918
+spotflow_device-2.0.2.dist-info/WHEEL,sha256=2KdwICnFEHl2ghwQAXqeXd9gNxeAiTvogEqUIMDbYbo,94
 spotflow_device/__init__.py,sha256=JfDnDKXS9NhCUjE-SCX9orPSkyDRS_iyfQXF4XMWs5o,143
 spotflow_device/__init__.pyi,sha256=yVJmQtUt_FpAOjQ7HgpT6lJtmdEDpUCdxRtQX5brnvQ,2695
 spotflow_device/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-spotflow_device/spotflow_device.pyd,sha256=07KLwAfGBPXp1EUm4J5pOeJPnCT_AHA55klpBsB0KKQ,8174592
-spotflow_device-2.0.1.dist-info/RECORD,,
+spotflow_device/spotflow_device.pyd,sha256=qaj0qrvvRGdAqhuGLK9vEfc_3RM1TuDo10QZtgJeV5M,8112640
+spotflow_device-2.0.2.dist-info/RECORD,,
```

