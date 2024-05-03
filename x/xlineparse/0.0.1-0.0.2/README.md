# Comparing `tmp/xlineparse-0.0.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip` & `tmp/xlineparse-0.0.2-cp312-cp312-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 637235 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 14:44 xlineparse-0.0.1.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 14:44 xlineparse/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 14:44 xlineparse.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 14:44 xlineparse-0.0.1.dist-info/license_files/
--rw-r--r--  2.0 unx     2670 b- defN 24-May-03 14:44 xlineparse-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      690 b- defN 24-May-03 14:44 xlineparse-0.0.1.dist-info/RECORD
--rw-r--r--  2.0 unx       49 b- defN 24-May-03 14:44 xlineparse-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      212 b- defN 24-May-03 14:44 xlineparse-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx     1071 b- defN 24-May-03 14:44 xlineparse-0.0.1.dist-info/license_files/LICENSE
--rw-r--r--  2.0 unx        0 b- defN 24-May-03 14:44 xlineparse/py.typed
--rw-r--r--  2.0 unx     6585 b- defN 24-May-03 14:44 xlineparse/__init__.py
--rwxr-xr-x  2.0 unx  2309716 b- defN 24-May-03 14:44 xlineparse/xlineparse.cpython-312-i386-linux-gnu.so
-12 files, 2320993 bytes uncompressed, 635545 bytes compressed:  72.6%
+Zip file size: 478377 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 15:03 xlineparse/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 15:03 xlineparse-0.0.2.dist-info/
+-rwxr-xr-x  2.0 unx  1976976 b- defN 24-May-03 15:03 xlineparse/xlineparse.cpython-312-darwin.so
+-rw-r--r--  2.0 unx     6585 b- defN 24-May-03 15:03 xlineparse/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-03 15:03 xlineparse/py.typed
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 15:03 xlineparse-0.0.2.dist-info/license_files/
+-rw-r--r--  2.0 unx      682 b- defN 24-May-03 15:03 xlineparse-0.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx      104 b- defN 24-May-03 15:03 xlineparse-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-03 15:03 xlineparse-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     2670 b- defN 24-May-03 15:03 xlineparse-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-03 15:03 xlineparse-0.0.2.dist-info/license_files/LICENSE
+11 files, 1988137 bytes uncompressed, 476811 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
-Filename: xlineparse-0.0.1.dist-info/
-Comment: 
-
 Filename: xlineparse/
 Comment: 
 
-Filename: xlineparse.libs/
+Filename: xlineparse-0.0.2.dist-info/
 Comment: 
 
-Filename: xlineparse-0.0.1.dist-info/license_files/
+Filename: xlineparse/xlineparse.cpython-312-darwin.so
 Comment: 
 
-Filename: xlineparse-0.0.1.dist-info/METADATA
+Filename: xlineparse/__init__.py
 Comment: 
 
-Filename: xlineparse-0.0.1.dist-info/RECORD
+Filename: xlineparse/py.typed
 Comment: 
 
-Filename: xlineparse-0.0.1.dist-info/entry_points.txt
+Filename: xlineparse-0.0.2.dist-info/license_files/
 Comment: 
 
-Filename: xlineparse-0.0.1.dist-info/WHEEL
+Filename: xlineparse-0.0.2.dist-info/RECORD
 Comment: 
 
-Filename: xlineparse-0.0.1.dist-info/license_files/LICENSE
+Filename: xlineparse-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xlineparse/py.typed
+Filename: xlineparse-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: xlineparse/__init__.py
+Filename: xlineparse-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xlineparse/xlineparse.cpython-312-i386-linux-gnu.so
+Filename: xlineparse-0.0.2.dist-info/license_files/LICENSE
 Comment: 
 
 Zip file comment:
```

## Comparing `xlineparse-0.0.1.dist-info/METADATA` & `xlineparse-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xlineparse
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Python
 Requires-Dist: maturin ==1.4.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'dev'
 Requires-Dist: mypy ==1.6.* ; extra == 'dev'
 Requires-Dist: pip ==24.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'test'
 Provides-Extra: dev
```

## Comparing `xlineparse-0.0.1.dist-info/RECORD` & `xlineparse-0.0.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-xlineparse-0.0.1.dist-info/METADATA,sha256=bUPj6c1_GOkKkjU0Y2GdJ3OsFoBhMNdfX5OGs799Tcc,2670
-xlineparse-0.0.1.dist-info/RECORD,,
-xlineparse-0.0.1.dist-info/entry_points.txt,sha256=V5wyMr5vlGqrFnfZFcMHMIIEXq5C7DmJr8rizjOO_s8,49
-xlineparse-0.0.1.dist-info/WHEEL,sha256=Ae3Tfi6BqeCLKeRR5nIV4A0W4paDC7wSiuTKW2pKNx4,212
-xlineparse-0.0.1.dist-info/license_files/LICENSE,sha256=jpcl6JKJdeKotYCJv0d4vXrgrcA0qF9HpZFuHXLeAyE,1071
-xlineparse/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+xlineparse/xlineparse.cpython-312-darwin.so,sha256=4pNesKQgb-JsvY9Z_16CIuCUs_WJ1Wti_kZXCAK_y7Q,1976976
 xlineparse/__init__.py,sha256=0SDshbZ67xycznvGJGrdIIO4xnvS0fsf51dNTDku15E,6585
-xlineparse/xlineparse.cpython-312-i386-linux-gnu.so,sha256=Jm8rtfwrV0UoEcqgRLP-ryAFhnlFBQ0qcrM1ODznYxg,2309716
+xlineparse/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+xlineparse-0.0.2.dist-info/RECORD,,
+xlineparse-0.0.2.dist-info/WHEEL,sha256=thWVGQI-HQrMGqeZp3gcIE7HFmAcTYQ1tQTxzJgo3SI,104
+xlineparse-0.0.2.dist-info/entry_points.txt,sha256=V5wyMr5vlGqrFnfZFcMHMIIEXq5C7DmJr8rizjOO_s8,49
+xlineparse-0.0.2.dist-info/METADATA,sha256=zazADZHfgJ97ao3lbmHDBAENJQxZku5WFAhIURjRI_I,2670
+xlineparse-0.0.2.dist-info/license_files/LICENSE,sha256=jpcl6JKJdeKotYCJv0d4vXrgrcA0qF9HpZFuHXLeAyE,1071
```

## Comparing `xlineparse-0.0.1.dist-info/license_files/LICENSE` & `xlineparse-0.0.2.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

